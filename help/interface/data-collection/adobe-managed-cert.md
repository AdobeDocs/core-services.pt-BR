---
description: Saiba como configurar certificados seguros para usar com cookies primários do Adobe CX Enterprise.
solution: Experience Cloud,Analytics
title: Programa de certificado gerenciado pela Adobe
index: true
snippet: 'y'
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: e15abde5-8027-4aed-a0c1-8a6fc248db5e
autotag-review: '2026-09-09T20:12:24.943Z'
TQID: 'https://experienceleague.adobe.com/8CSBLQaw3KOByyxxCYr1By4gyAQsDIhiofOdAzn38dg'
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
    internal-label: CX Enterprise
  - id: e55547f1-a1ff-40c6-8978-026e40ab7fa4
    internal-label: Analytics
feature_v2:
  - id: b3f03848-ae12-48b2-8aab-cad18567eb32
    internal-label: Metrics
  - id: e9dbdbc5-3e52-40f0-a7bc-e18542967b7a
    internal-label: Implementations
  - id: fd307ce7-56f5-4ee3-af68-a7833ff6e85e
    internal-label: API
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
    internal-label: Administration
subfeature_v2:
  - id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
    internal-label: Support
  - id: c8add8f2-4250-4fd9-9cde-9707036c567d
    internal-label: Methods
  - id: d2311670-43bd-4c2e-bc98-1da2aaba9cef
    internal-label: Appmeasurement implementation
  - id: e992d880-33bc-4949-a648-aa7d410276cd
    internal-label: Validation
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
    internal-label: Measurement
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: d3cdead0-685a-4489-9250-4bb709942f66
    internal-label: Data collection
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 18fd590d6f0fd1800e3d5c62851453aa91d9db5f
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 2%
---
# Programa de certificado gerenciado pela Adobe

O programa de certificados gerenciados pela Adobe é o processo recomendado para configurar certificados primários necessários para uma implementação CNAME. O programa é totalmente automatizado depois de configurado. Ele renova certificados em tempo hábil para que não haja impacto na coleta de dados devido a certificados expirados. O programa é gratuito para os primeiros 100 CNAMEs.

O programa de certificado gerenciado pela Adobe não oferece suporte ao roteamento de coleta de dados por meio de uma rede de entrega de conteúdo (CDN). Se você usar um CDN, consulte [Rotear coleta de dados por meio de um CDN](cdn.md). As organizações que precisam gerenciar seus próprios certificados podem usar [certificados gerenciados pelo cliente](customer-managed-cert.md). Se você gerencia seus próprios certificados e deseja migrar para o programa de certificados gerenciados pela Adobe, entre em contato com o Atendimento ao cliente da Adobe.

## Implementação

Para implementar um novo certificado para a coleta de dados próprios, siga estas etapas:

1. Baixe e preencha o [Formulário de solicitação de domínio próprio](cookies/assets/First_Party_Domain_Request_Form.xlsx)
1. Abra um tíquete no Atendimento ao cliente da Adobe solicitando a configuração da coleta de dados primários no programa de certificados gerenciados pela Adobe. Se sua organização tiver requisitos de residência ou conformidade de dados, especifique o [tipo de RDC](rdc.md) desejado em sua solicitação.
1. Ao receber o tíquete, o representante da Adobe fornece um registro CNAME. Esse registro deve ser configurado no servidor DNS da empresa para que a Adobe possa comprar o certificado em seu nome. Por exemplo, o nome de host `data.example.com` aponta para `hiodsibxvip01.data.adobedc.net`. Se sua organização usar registros de autorização de autoridade de certificação (CAA) de DNS, verifique se os registros de CAA permitem que a DigiCert emita certificados. Consulte [Manutenção e renovações](#renewals).
1. Quando o registro CNAME estiver em vigor nos servidores da organização, a Adobe trabalhará com a DigiCert para comprar e instalar um certificado nos servidores de coleta de dados da Adobe.
1. Se precisar de uma atualização para seu arquivo `robots.txt` quando hospedado pelo Adobe CNAME para fins próprios, entre em contato com o Atendimento ao Cliente com uma solicitação. Essa solicitação é relevante quando você deseja atualizar o arquivo `robots.txt` para impedir que o Google rastree seus subdomínios.

## Validar o encaminhamento do nome do host

Depois que o Adobe tiver instalado o certificado, você poderá usar um dos métodos a seguir para validar se ele está funcionando.

+++**Validação do navegador**

Você pode usar qualquer navegador para validar se um certificado está instalado corretamente. Digite seu CNAME com `_check` como o caminho para a barra de endereços. Por exemplo:

`data.example.com/_check`

Se tudo funcionar, o navegador mostrará `SUCCESS`. Se o certificado não estiver instalado corretamente, você receberá um aviso de segurança.

+++

+++**Linha de comando (`curl`)**

A maioria dos sistemas operacionais modernos já tem o [`curl`](https://curl.se) instalado.

Digite o seguinte na linha de comando:

```sh
curl data.example.com/_check
```

Se tudo funcionar corretamente, o console retornará `SUCCESS`.

>[!TIP]
>
>Você pode usar o sinalizador `-k` para desabilitar o aviso de segurança para ajudar na solução de problemas.

+++

+++**Linha de comando (`nslookup`)**

Digite o seguinte na linha de comando:

```sh
nslookup data.example.com
```

Se tudo funcionar corretamente, os servidores de coleta de dados da Adobe serão retornados:

```text
Server: hiodsibxvip01.corp.adobe.com
Address: 10.50.112.247

Name: example.com.ssl.d1.sc.omtrdc.net
Addresses: 63.140.37.126
    63.140.37.206
    63.140.36.51
    63.140.36.145
Aliases: data.example.com
```

+++

## Atualizar código de implementação

Para usar o novo nome de host CNAME, atualize a implementação do Adobe depois de validar que o certificado funciona corretamente. Consulte [Atualizar sua implementação](collection-domain.md#update-implementation).

## Manutenção e renovações {#renewals}

O Adobe renova o certificado automaticamente. Trinta dias antes da expiração do certificado, o Adobe verifica se o CNAME ainda é válido e está em uso, além de renovar o certificado em seu nome. Para manter as renovações funcionando, evite as seguintes alterações de DNS:

* **Remoção ou redirecionamento do registro CNAME**: se o registro CNAME for removido ou não apontar mais para o nome de host seguro do Adobe, o Adobe não poderá renovar o certificado. Essa condição inclui apontar o registro CNAME para uma rede de entrega de conteúdo (CDN). Se você planeja usar uma CDN, consulte [Mover uma implementação primária existente para uma CDN](cdn.md#migrate) antes de alterar seus registros DNS.
* **Adicionando registros CAA que não autorizam DigiCert**: as autoridades de certificação verificam os registros CAA (Autorização de Autoridade de Certificação) no nome de host e seus domínios pai. Se você usar registros CAA, inclua `digicert.com` como emissor autorizado. Por exemplo, `example.com. IN CAA 0 issue "digicert.com"`.
* **Restringindo a emissão de DigiCert para uma conta específica**: o recurso de bloqueio de domínio da DigiCert adiciona um parâmetro `account=` a um registro CAA, como `example.com. IN CAA 0 issue "digicert.com; account=<token>"`. Esse parâmetro restringe a emissão para a conta DigiCert da sua organização, mesmo se `digicert.com` estiver autorizado, o que impede a Adobe de obter um certificado. Se sua organização exigir o bloqueio de domínio DigiCert, use [certificados gerenciados pelo cliente](customer-managed-cert.md). Os bloqueios de domínio definidos no seu registrador de domínios, às vezes chamados de bloqueios de transferência, não estão relacionados e não afetam os certificados gerenciados pela Adobe.

>[!IMPORTANT]
>
>Se o seu registro CNAME não apontar mais para o nome de host seguro do Adobe, a entrada no sistema da Adobe será marcada para remoção sem comunicação adicional.

## Perguntas frequentes

+++Esse processo é seguro?

Sim. O programa de certificados gerenciados pela Adobe é mais seguro do que [certificados gerenciados pelo cliente](customer-managed-cert.md). Nenhum certificado ou chave privada é transferido para fora da Adobe e da autoridade de certificação emissora.

+++

+++Como a Adobe pode comprar um certificado para o nosso domínio?

O certificado só pode ser comprado quando você aponta o nome de host especificado para um nome de host da Adobe. Você delega esse nome de host à Adobe e permite que a Adobe compre o certificado em seu nome.

+++

+++Posso solicitar que o certificado seja revogado?

Sim. Como proprietário do domínio, você está autorizado a solicitar que o certificado seja revogado. Entre em contato com o Atendimento ao cliente da Adobe para iniciar esse processo.

+++

+++Que tipo de criptografia é usado?

A Adobe trabalha com a DigiCert para emitir um certificado SHA-2.

+++

+++Esse programa gera custo adicional?

A Adobe oferece esse programa a todos os clientes da Adobe CX Enterprise sem custo adicional para os primeiros 100 CNAMEs.

+++

+++Quais níveis de segurança de criptografia o Adobe oferece?

A Adobe oferece dois níveis de segurança de criptografia para atender às diversas necessidades de segurança do cliente na coleta de dados primários. Esses níveis determinam quais algoritmos de criptografia são compatíveis com conexões HTTPS com servidores do Adobe. A Adobe revisa e atualiza regularmente o conjunto de algoritmos compatíveis com base nas práticas atuais de segurança. Para alterar as configurações de segurança de criptografia, entre em contato com o Atendimento ao cliente.

* **Standard** requer TLS 1.2 ou mais recente e criptografia de pelo menos 128 bits. Ele foi projetado para fornecer a mais ampla compatibilidade de dispositivos, mantendo a criptografia segura.
* **High** requer TLS 1.2 ou mais recente e remove o suporte para cifras mais fracas. Ele foi projetado para clientes que desejam a criptografia mais forte. Os clientes lançados antes de 2015 normalmente não podem se conectar quando a segurança de criptografia está definida como **Alta**.

+++

+++Quais tipos de certificado HTTPS são compatíveis?

A Adobe aceita certificados RSA e ECC, e os clientes modernos aceitam ambos os tipos de certificados. Os certificados ECC exigem menos processamento no servidor e no cliente. Para certificados gerenciados pela Adobe, a Adobe fornece certificados RSA e ECC. Para [certificados gerenciados pelo cliente](customer-managed-cert.md), o RSA é obrigatório e o ECC é recomendado.

+++

