---
title: Rotear a coleta de dados por meio de um CDN
description: Saiba como configurar uma rede de entrega de conteúdo (CDN) para encaminhar solicitações de coleta de dados ao Adobe sem afetar a qualidade dos dados.
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
    internal-label: CX Enterprise
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: d3cdead0-685a-4489-9250-4bb709942f66
    internal-label: Data collection
source-git-commit: e1185eeafc809b036b10955880536db7a576ca0b
workflow-type: tm+mt
source-wordcount: '1421'
ht-degree: 0%
---
# Rotear a coleta de dados por meio de um CDN

Algumas organizações roteiam solicitações de coleta de dados por meio de sua rede de entrega de conteúdo (CDN) em vez de enviá-las diretamente para a Adobe. Motivos comuns incluem proteção de firewall de aplicativo da Web (WAF), políticas corporativas que exigem que todo o tráfego do site passe por um CDN e a capacidade de inspecionar o tráfego enviado ao Adobe. A CDN recebe solicitações em um nome de host de sua organização e as encaminha para um nome de host de coleção de dados da Adobe, chamado de origem.

>[!IMPORTANT]
>
>O Adobe não pode revisar ou validar a configuração do CDN. Sua organização e seu provedor de CDN são responsáveis por configurar o CDN corretamente. Para obter ajuda sobre como configurar o CDN, entre em contato com o provedor de CDN. CDNs configurados incorretamente podem resultar em perda de dados.

## Escolher um tipo de origem {#origin-type}

| | Origem de terceiros (recomendado) | Origem própria |
| --- | --- | --- |
| **Nome do host de origem** | Seu subdomínio de ID de locatário de `data.adobedc.net`, como `example.data.adobedc.net` | Seu nome de host próprio, como `data.example.com` |
| **Certificado em servidores Adobe** | Certificado da Adobe (`*.data.adobedc.net`) | [Certificado gerenciado pelo cliente](customer-managed-cert.md) |
| **Renovações de certificado** | Nenhuma ação necessária | Sua organização renova o certificado e o fornece à Adobe antes de cada expiração |
| **RDC [bloqueada por região](rdc.md)** | Incompatível | Suportado |
| **Quando usar** | Todas as implementações de CDN, a menos que sua organização exija uma origem primária | Sua política de segurança requer controle direto do certificado de origem ou sua organização requer um tipo de RDC bloqueado por região |

>[!NOTE]
>
>O [programa de certificado gerenciado pela Adobe](adobe-managed-cert.md) não dá suporte a implementações CDN. O Adobe não pode validar a propriedade do domínio ou renovar certificados para nomes de host que apontem para seu CDN. Use uma origem de terceiros ou uma origem própria com um [certificado gerenciado pelo cliente](customer-managed-cert.md).

## Requisitos para todas as implementações de CDN {#requirements}

As bibliotecas de coleção de dados do Adobe, como AppMeasurement e Web SDK, incluem tudo o que o Adobe precisa em cada solicitação. Configure sua CDN para encaminhar essas solicitações à Adobe sem alterá-las.

>[!IMPORTANT]
>
>Nunca altere o endpoint ou algo que determine para onde os dados vão, incluindo a ID do conjunto de relatórios (AppMeasurement) ou a ID de sequência de dados (Web SDK). Alterar esses valores causa perda de dados.

A configuração do CDN deve:

* Encaminhe o método de solicitação, o caminho do URL, a string de consulta e o corpo sem alterações.
* Deixe o cabeçalho `Host` inalterado.
* Deixe o domínio em que os cookies do Adobe estão definidos inalterado.
* Mantenha todos os cookies listados na [seção de cookies](cookies/overview.md) deste guia.
* Adicione o cabeçalho `X-Forwarded-For` que contém o endereço IP do visitante. O Adobe usa esse cabeçalho para geolocalização. Sem ele, os dados de geolocalização refletem a localização dos servidores da CDN em vez dos visitantes.
* Retorne as respostas da Adobe ao navegador sem alterações.

A configuração do CDN pode:

* Remova os cookies que a Adobe não usa, como cookies de outros sistemas do site. Cookies não relacionados adicionam sobrecarga a cada solicitação.
* Use os serviços de WAF, filtragem de bot ou remoção de dados pessoais, desde que eles não alterem nada listado acima. Teste esses serviços com um conjunto de relatórios de desenvolvimento ou sequência de dados antes de aplicá-los ao tráfego de produção. Uma filtragem excessivamente agressiva pode remover dados suficientes para tornar os relatórios inutilizáveis.

A configuração do CDN não deve:

* Armazenar em cache solicitações ou respostas de coleta de dados. Todas as solicitações devem chegar à Adobe.
* Aponte para um nome de host de origem que não existe.
* Aceite certificados expirados ou fixe um certificado específico da origem. A Adobe não oferece suporte à veiculação de certificados expirados e pode removê-los a qualquer momento.

## Configurar um CDN com uma origem de terceiros {#third-party-origin}

Uma origem de terceiros usa o próprio certificado da Adobe, portanto, sua organização não precisa manter um certificado nos servidores da Adobe.

1. Encontre a ID de locatário da sua organização. Consulte [Encontrar a ID do locatário](collection-domain.md#tenant-id).
1. Na configuração do CDN, defina o nome de host de origem para o subdomínio da ID de locatário de `data.adobedc.net`. Por exemplo, `example.data.adobedc.net`.
1. Ativar a SNI (Server Name Indication) para a origem. Defina o nome de host SNI como o nome de host de origem (por exemplo, `example.data.adobedc.net`), não o nome de host do seu site.
1. Configure sua CDN para atender aos [requisitos para todas as implementações de CDN](#requirements) acima.
1. Se o nome de host para o qual sua implementação envia dados for alterado, [atualize sua implementação](collection-domain.md#update-implementation). Se você mantiver o mesmo nome de host, nenhuma alteração de implementação será necessária.

>[!WARNING]
>
>Não defina sua origem como o nome de host fornecido pelo Adobe como seu destino CNAME, como `hiodsibxvip01.data.adobedc.net`. Esse nome de host está vinculado ao seu certificado próprio e pode parar de funcionar quando o certificado for removido.

As origens de terceiros sempre usam o [tipo de RDC](rdc.md) padrão, para que os dados possam ser coletados em qualquer local de coleta de dados da Adobe.

## Configurar um CDN com uma origem própria {#first-party-origin}

Use uma origem própria somente se sua organização exigir. Os motivos comuns incluem:

* Sua política de segurança requer controle direto do certificado de origem. Por exemplo, sua organização deve ser capaz de revogar o certificado por meio de sua própria autoridade de certificação.
* Sua organização requer um [tipo de RDC](rdc.md) bloqueado por região.

1. Entre em contato com o Atendimento ao cliente da Adobe para configurar um [certificado gerenciado pelo cliente](customer-managed-cert.md) para seu nome de host próprio, como `data.example.com`. Se sua organização exigir um tipo de RDC bloqueado por região, especifique-o em sua solicitação.
1. Na configuração do CDN, defina o nome de host de origem como o nome de host próprio.
1. Ativar a SNI (Server Name Indication) para a origem. Defina o nome de host SNI como o nome de host próprio e configure a CDN para esperar seu certificado próprio da origem.
1. Configure sua CDN para atender aos [requisitos para todas as implementações de CDN](#requirements) acima.
1. Se o nome de host para o qual sua implementação envia dados for alterado, [atualize sua implementação](collection-domain.md#update-implementation). Se você mantiver o mesmo nome de host, nenhuma alteração de implementação será necessária.

>[!IMPORTANT]
>
>Sua organização é responsável por renovar o certificado gerenciado pelo cliente e fornecê-lo ao Atendimento ao cliente da Adobe antes de expirar. Se o certificado nos servidores da Adobe expirar, seu CDN poderá rejeitar a conexão e descartar dados sem notificá-lo. Consulte [Renovar o certificado](customer-managed-cert.md#renewals).

## Mover uma implementação primária existente para um CDN {#migrate}

Se sua organização atualmente envia dados diretamente para um nome de host próprio com um certificado hospedado pela Adobe, use as seguintes etapas para migrar para um CDN:

1. Identifique cada implementação que envia dados para seu nome de host primário em todos os produtos da Adobe. Outros produtos, como Adobe Target ou Adobe Journey Optimizer, podem usar o mesmo nome de host, e um único certificado pode abranger muitos nomes de host.
1. Escolha um [tipo de origem](#origin-type). Se você escolher uma origem própria, entre em contato com o Atendimento ao cliente da Adobe para converter seu certificado em um [certificado gerenciado pelo cliente](customer-managed-cert.md) antes de expirar.
1. Configure seu CDN. Mantenha seu nome de host existente para que você não precise atualizar suas implementações.
1. Antes de o certificado expirar, aponte o nome do host para o CDN e alterne todas as implementações para usá-lo.
1. [Verifique seus dados](#check).
1. Se você escolher uma origem de terceiros, entre em contato com o Atendimento ao cliente da Adobe para marcar seu certificado próprio para remoção.

Depois que o nome de host aponta para o CDN, o Adobe não pode renovar o certificado próprio. Se qualquer implementação ainda depender do certificado quando expirar, os dados dessa implementação serão perdidos. Entrar em contato com o Atendimento ao cliente da Adobe permite que sua organização controle quando o certificado é removido.

## Verifique seus dados {#check}

O Adobe não pode validar a configuração do CDN. Depois de rotear a coleta de dados por meio da CDN, compare os dados antes e depois da alteração:

* Os dados continuam a chegar aos conjuntos de relatórios, fluxos de dados ou conjuntos de dados esperados no volume normal.
* Os relatórios de geolocalização mostram a localização de seus visitantes, não um pequeno número de cidades onde os servidores da CDN estão localizados.
* As contagens de visitantes únicos não aumentam inesperadamente.
* Nas ferramentas do desenvolvedor do seu navegador, as solicitações de coleta de dados para o seu nome de host foram bem-sucedidas e os cookies do Adobe estão definidos no mesmo domínio de antes.

## Erros comuns

Os seguintes problemas são conhecidos por causar problemas de qualidade de dados ou perda de dados. Esta lista não é exaustiva.

| Sintoma | Causa provável |
| --- | --- |
| Os dados param de chegar em um conjunto de relatórios ou fluxo de dados | O CDN altera o URL da solicitação ou o nome de host de origem não existe |
| Os dados param de chegar depois que um certificado expira | O CDN espera um certificado próprio da origem e esse certificado expirou |
| Os dados de geolocalização mostram apenas algumas cidades | A CDN não adiciona o cabeçalho `X-Forwarded-For` |
| As contagens de visitantes únicos aumentam inesperadamente | A CDN remove cookies do Adobe, altera o cabeçalho `Host` ou altera o domínio do cookie |
| Faltam muitos dados nos relatórios | A remoção de dados pessoais ou as regras do WAF removem muitas solicitações |

## Perguntas frequentes

+++Esta página se aplica a produtos diferentes do Adobe Analytics?

Sim. Esta página se aplica a todos os produtos da Adobe que usam a coleta de dados da Adobe, incluindo Customer Journey Analytics, Adobe Experience Platform, Adobe Target e Adobe Journey Optimizer.

+++

+++O Adobe pode rejeitar dados que não vêm por meio da minha CDN?

Não. No momento, a Adobe não oferece uma maneira de restringir a coleta de dados às solicitações do CDN.

+++

+++A Adobe pode fornecer ou validar uma configuração para meu CDN?

Não. As opções de configuração do CDN diferem entre os provedores e mudam ao longo do tempo. Entre em contato com seu provedor de CDN para obter ajuda sobre como configurar seu CDN e consulte [Verificar seus dados](#check) para saber como identificar problemas com sua configuração.

+++
