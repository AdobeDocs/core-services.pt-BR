---
description: Os administradores podem saber mais sobre os requisitos e o que esperar ao atualizar para o Analytics Premium e onde encontrar ajuda como administrador da Experience Cloud.
keywords: Adobe Analytics Premium upgrade
solution: Adobe Experience Cloud
title: Como atualizar para o Analytics Premium e o Experience Cloud | Adobe Experience Cloud
topic: Premium
uuid: 450a601c-d199-4e90-b525-19bd9f9576d2
translation-type: tm+mt
source-git-commit: 4bea0c29afa580dc63b21535ce5c275cd649c9a5
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 97%

---


# Atualização para o Analytics Premium e a Experience Cloud

Os administradores podem saber mais sobre os requisitos e o que esperar ao atualizar para o Analytics Premium e onde encontrar ajuda como administrador da Experience Cloud.

## Analytics Premium {#section_7F50AD7906544F899B844BE31D3BB507}

A atualização para o Adobe Analytics Premium oferece todos os recursos ou produtos disponíveis no Analytics Standard, inclusive o Data Warehouse, Ad Hoc Analysis, Report Builder e Data Connectors. (Esses produtos foram vendidos separadamente para clientes que usam a solução de ponto, o SiteCatalyst.)

O Analytics Premium oferece:

* Acesso a 250 variáveis de conversão (eVars)
* [Análise de aplicativos móveis](https://docs.adobe.com/content/help/pt-BR/mobile-services/using/home.html)
* Data Workbench (consulta de dados visuais; atribuição baseada em regras; análise entre canais)

>[!NOTE]
>
>Nenhuma migração é necessária durante a atualização, mas há algumas considerações a serem levadas em conta:
>
>* As eVars 76-250 (SiteCatalyst) e 100-250 (Standard) estarão visíveis nas Ferramentas administrativas, mas ainda não estarão habilitadas.>
>* A Análise de colaboração é ativada pela Adobe. Ela não alterará o local (ainda está disponível na página Detecção de anomalias), mas agora será iniciada automaticamente ao analisar todos os pontos de dados.>


## Analytics Premium completo {#section_BFAD815EDF364845A52B340B2FD5B64C}

No Analytics Premium completo, você obtém todos os recursos do [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507), além das seguintes atualizações:

| Produto | Atualizações |
|--- |--- |
| Reports &amp; Analytics | <ul><li>[Análise de contribuição](https://docs.adobe.com/content/help/pt-BR/analytics/analyze/analysis-workspace/virtual-analyst/contribution-analysis/ca-tokens.html)</li><li>[Atributos do cliente](../attributes/attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1) (Até 200)</li></ul> |
| Data Workbench | <ul><li>Atribuição algorítmica</li><li>Espaços de trabalho pré-criados</li></ul> |
| Analytics Platform | [Live Stream](https://helpx.adobe.com/br/analytics/kb/getting-started-with-livestream-api.html) (dados brutos, painéis, acionadores) |

## Inteligência preditiva {#section_B407932C07A7476F83FB0275C3FB63DC}

Atualizar para Inteligência preditiva permite o [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) e:

| Produto | Atualizações |
|---|---|
| Reports &amp; Analytics | [Análise de contribuição](https://docs.adobe.com/content/help/pt-BR/analytics/analyze/analysis-workspace/virtual-analyst/contribution-analysis/ca-tokens.html) |
| Data Workbench | Espaços de trabalho pré-criados para qualificações de público-alvo e marketing preditivo |
| Analytics Platform | Live Stream (painéis e acionadores) |

## Visão completa do cliente {#section_3B2AC245388248688067DC9A48957AFB}

Atualização para ofertas do Customer 360 no [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) e:

| Produto | Atualizações |
|--- |--- |
| [Atributos do cliente](../attributes/attributes.md) | Atributos do cliente (análise e compartilhamento de segmentos) |
| Data Workbench | <ul><li>Atributos derivados do cliente</li><li>Espaços de trabalho pré-criados para descoberta de públicos-alvo</li></ul> |
| Analytics Platform | [Atributos do cliente](../attributes/attributes.md) |

## Atribuição avançada {#section_9E4986A8389946CCAA7D003268343296}

A Atribuição avançada oferece acesso ao [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) e também à Atribuição algorítmica no Data Workbench (25% do volume de chamadas do servidor).

## Requisitos do Data Workbench {#section_D959CA68D6DB42C38707F8E0CA3654CC}

Os usuários suportados podem solicitar que todas as licenças dos clientes sejam atualizadas para refletir o Premium ao enviar um email para a `dwb@adobe.com`. Isso habilita recursos como Atribuição algorítmica.

A TechOps verificará seu compromisso contratual e determinará a infraestrutura gerenciada adequada, aumentando ou reduzindo a capacidade e, então, eles coordenarão com você por meio do Gerente de conta ou consultoria para implantar quaisquer alterações.

Qualquer software que estiver sendo executado no local deverá ser desativado. Isso inclui Sensores, o que significa que você precisará garantir o rastreamento correto por meio de tags do Analytics.

## Experience Cloud - Administrar usuários e produtos {#section_6471C54454024301B2E0B687F79F6738}

A Experience Cloud e os serviços principais estão disponíveis para usuários do Analytics Standard e Premium, desde que você tenha seguido a modernização de implementação descrita na [Introdução - ative as soluções para os serviços principais](../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C). (Esse processo ajuda a modernizar a implementação e permitirá que você se torne um administrador na Experience Cloud.)

Após associar-se à Experience Cloud, é possível fazer logon por meio da Experience Cloud em [!DNL experiencecloud.adobe.com] e começar a usar os principais serviços (inclusive os atributos do cliente, os públicos-alvo e a análise de aplicativos móveis).

### Administre usuários e grupos

O gerenciamento de usuários é executado no [Adobe Admin Console](https://helpx.adobe.com/br/enterprise/help/aedash.html) (link do produto).

Você pode configurar um mapeamento 1:1 entre um grupo criado no Adobe Admin Console e um grupo de soluções (como o Adobe Analytics). Consequentemente, um novo usuário incluído no grupo do Admin Console mapeado terá uma conta de solução de Análise automaticamente criada e vinculada à Adobe ID do usuário. (Os usuários existentes devem vincular manualmente as credenciais da conta da solução para acessar as soluções por meio do logon da Experience Cloud.)

>[!NOTE]
>
>Você pode mapear diversos grupos de solução para um grupo do Admin Console. No entanto, Adobe recomenda o mapeamento de 1:1. Mapear os grupos antecipadamente permite convidar, criar, permitir e adicionar vários usuários carregando um CSV.
