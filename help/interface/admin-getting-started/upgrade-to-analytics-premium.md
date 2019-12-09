---
description: Os administradores podem saber mais sobre os requisitos e o que esperar ao atualizar para o Analytics Premium e onde encontrar ajuda como administrador da Experience Cloud.
keywords: upgrading
seo-description: Os administradores podem saber mais sobre os requisitos e o que esperar ao atualizar para o Analytics Premium e onde encontrar ajuda como administrador da Experience Cloud.
seo-title: Atualização para o Analytics Premium e a Experience Cloud
solution: Experience Cloud
title: Atualização para o Analytics Premium e a Experience Cloud
topic: Premium
uuid: 450a601c-d199-4e90-b525-19bd9f9576d2
translation-type: tm+mt
source-git-commit: ae97db27349940a8df7ee2ba6678683f57585678

---


# Atualização para o Analytics Premium e a Experience Cloud

Os administradores podem saber mais sobre os requisitos e o que esperar ao atualizar para o Analytics Premium e onde encontrar ajuda como administrador da Experience Cloud.

## Analytics Premium {#section_7F50AD7906544F899B844BE31D3BB507}

A atualização para o Adobe Analytics Premium oferece todos os recursos ou produtos disponíveis no Analytics Standard, inclusive o Data Warehouse, Ad Hoc Analysis, Report Builder e Data Connectors. (Esses produtos foram vendidos separadamente para clientes que usam a solução de ponto, o SiteCatalyst.)

O Analytics Premium oferece:

* Acesso a 250 variáveis de conversão (eVars)
* [Análise de aplicativo móvel](https://docs.adobe.com/content/help/en/mobile-services/using/home.html)
* Data Workbench (consulta de dados visuais; atribuição baseada em regras; análise entre canais)

>[!NOTE]
>
>Não é necessário fazer nenhuma migração durante a atualização, mas é preciso fazer algumas considerações:
>
>* eVars 76-250 (SiteCatalyst) e 100-250 (Standard) estarão visíveis nas Ferramentas administrativas, mas ainda não estarão habilitadas.&gt;
>* A Análise de colaboração é ativada pela Adobe. A localização dela não será alterada (ainda está disponível na página de Detecção de anomalias), mas, agora, ela começará a analisar dados automaticamente em todos os pontos de dados.&gt;


## Analytics Premium completo {#section_BFAD815EDF364845A52B340B2FD5B64C}

No Analytics Premium completo, você terá todos os recursos do [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507), além das atualizações a seguir:

| Produto | Atualizações |
|--- |--- |
| Reports &amp; Analytics | <ul><li>[Análise de contribuição](https://docs.adobe.com/content/help/en/analytics/analyze/analysis-workspace/virtual-analyst/contribution-analysis/ca-tokens.html)</li><li>[Atributos do cliente](../attributes/attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1) (Até 200)</li></ul> |
| Data Workbench | <ul><li>Atribuição algorítmica</li><li>Espaços de trabalho pré-criados</li></ul> |
| Plataforma de análise | [Transmissão ao vivo](https://helpx.adobe.com/analytics/kb/getting-started-with-livestream-api.html) (dados brutos, painéis e acionadores) |

## Inteligência preditiva {#section_B407932C07A7476F83FB0275C3FB63DC}

Atualizar para Inteligência preditiva habilita o [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) e:

| Produto | Atualizações |
|---|---|
| Reports &amp; Analytics | [Análise de contribuição](https://docs.adobe.com/content/help/en/analytics/analyze/analysis-workspace/virtual-analyst/contribution-analysis/ca-tokens.html) |
| Data Workbench | Espaços de trabalho pré-criados para qualificações de público-alvo e marketing preditivo. |
| Plataforma de análise | Transmissão ao vivo (painéis e acionadores) |

## Visão completa do cliente {#section_3B2AC245388248688067DC9A48957AFB}

Atualizar para a visão completa do cliente oferece [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) e:

| Produto | Atualizações |
|--- |--- |
| [Atributos do cliente](../attributes/attributes.md) | Atributos do cliente (análise e compartilhamento de segmentos) |
| Data Workbench | <ul><li>Atributos derivados do cliente</li><li>Espaços de trabalho pré-criados para descoberta de público-alvo</li></ul> |
| Plataforma de análise | [Atributos do cliente](../attributes/attributes.md) |

## Atribuição avançada {#section_9E4986A8389946CCAA7D003268343296}

A atribuição avançada oferece acesso ao [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) e também à Atribuição algorítmica na Data Workbench (25% do volume de chamadas do servidor).

## Exigências da Data Workbench {#section_D959CA68D6DB42C38707F8E0CA3654CC}

Os usuários suportados podem solicitar que todas as licenças dos clientes sejam atualizadas para refletir o Premium ao enviar um email para a `dwb@adobe.com`. Isso permite recursos como a Atribuição algorítmica.

O TechOps verificará o compromisso do contrato e determinará a infraestrutura gerenciada adequada, aumentando ou reduzindo a capacidade e, então, vocês combinarão a implantação de quaisquer alterações por meio do Account Manager.

Qualquer software que estiver sendo executado no local deverá ser desativado. Isso inclui Sensores, o que significa que você precisará garantir o rastreamento adequado por meio de tags de Análise.

## Experience Cloud - Administrar usuários e produtos {#section_6471C54454024301B2E0B687F79F6738}

A Experience Cloud e os serviços principais estão disponíveis para usuários do Analytics Standard e Premium, desde que você tenha seguido a modernização de implementação descrita na [Introdução - ative as soluções para os serviços principais](../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C). (Esse processo ajuda a modernizar a implementação e permitirá que você se torne um administrador na Experience Cloud.)

Após associar-se à Experience Cloud, é possível fazer logon por meio da Experience Cloud em [!DNL experiencecloud.adobe.com] e começar a usar os principais serviços (inclusive os atributos do cliente, os públicos-alvo e a análise de aplicativos móveis).

### Administre usuários e grupos

O gerenciamento do usuário é executado no [Adobe Admin Console](https://helpx.adobe.com/enterprise/help/aedash.html) (link do produto).

Você pode configurar um mapeamento 1:1 entre um grupo criado no Adobe Admin Console e um grupo de soluções (como o Adobe Analytics). Consequentemente, um novo usuário incluído no grupo do Admin Console mapeado terá uma conta de solução de Análise automaticamente criada e vinculada à Adobe ID do usuário. (Os usuários atuais devem vincular manualmente as credenciais de conta da solução para acessar soluções pelo logon da Experience Cloud.)

>[!NOTE]
>
>Você pode mapear diversos grupos de solução para um grupo do Admin Console. No entanto, Adobe recomenda o mapeamento de 1:1. Mapear os grupos antecipadamente permite convidar, criar, permitir e incluir vários usuários ao fazer upload de um CSV.
