---
description: Saiba mais sobre os requisitos e o que esperar ao atualizar para o Analytics Premium.
keywords: Atualização do Adobe Analytics Premium
solution: Experience Cloud
title: 'Atualização para o Analytics Premium e a Experience Cloud '
topic: Administração
uuid: 450a601c-d199-4e90-b525-19bd9f9576d2
feature: Admin Console
role: Administrator
level: Experienced
exl-id: 746d396d-9629-42db-8c55-07d2d24e4611
source-git-commit: ebefd433e96da422674e7ee71c8988d4011fed11
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 70%

---

# Atualização para o Analytics Premium e a Experience Cloud

Os administradores podem saber mais sobre os requisitos e o que esperar ao atualizar para o Analytics Premium e onde encontrar ajuda como administrador da Experience Cloud.

## Analytics Premium {#section_7F50AD7906544F899B844BE31D3BB507}

A atualização para o Adobe Analytics Premium oferece todos os recursos ou produtos disponíveis no Analytics Standard, inclusive o Data Warehouse, Ad Hoc Analysis, Report Builder e Data Connectors.

O Analytics Premium oferece:

* Acesso a 250 variáveis de conversão (eVars)
* [Análise de aplicativos móveis](https://experienceleague.adobe.com/docs/mobile-services/using/home.html?lang=en)
* Data Workbench (consulta de dados visuais; atribuição baseada em regras; análise entre canais)

>[!NOTE]
>
>Nenhuma migração é necessária durante a atualização, mas há algumas considerações a serem levadas em conta:
>
>* As eVars 76-250 e 100-250 (Padrão) estão visíveis nas Ferramentas administrativas, mas não estão habilitadas.
>* A Análise de colaboração é ativada pela Adobe. Ela não altera o local (ainda está disponível na página Detecção de anomalias), mas inicia automaticamente a análise de todos os pontos de dados.


## Analytics Premium completo {#section_BFAD815EDF364845A52B340B2FD5B64C}

No Analytics Premium completo, você obtém todos os recursos do [Analytics Premium](upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507), além das seguintes atualizações:

| Produto | Atualizações |
|--- |--- |
| Reports &amp; Analytics | <ul><li>[Análise de contribuição](https://experienceleague.adobe.com/docs/analytics/analyze/analysis-workspace/virtual-analyst/contribution-analysis/ca-tokens.html?lang=en)</li><li>[Atributos do cliente](attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1) (Até 200)</li></ul> |
| Data Workbench | <ul><li>Atribuição algorítmica</li><li>Espaços de trabalho pré-criados</li></ul> |
| Analytics Platform | [Live Stream](https://github.com/AdobeDocs/analytics-1.4-apis/blob/master/docs/live-stream-api/index.md) (dados brutos, painéis, acionadores) |

## Inteligência preditiva {#section_B407932C07A7476F83FB0275C3FB63DC}

Atualizar para Inteligência preditiva permite o [Analytics Premium](upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) e:

| Produto | Atualizações |
|---|---|
| Reports &amp; Analytics | [Análise de contribuição](https://experienceleague.adobe.com/docs/analytics/analyze/analysis-workspace/virtual-analyst/contribution-analysis/ca-tokens.html?lang=en) |
| Data Workbench | Espaços de trabalho pré-criados para qualificações de público-alvo e marketing preditivo |
| Plataforma do Analytics | Live Stream (painéis e acionadores) |

## Visão completa do cliente {#section_3B2AC245388248688067DC9A48957AFB}

Atualização para ofertas do Customer 360 no [Analytics Premium](upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) e:

| Produto | Atualizações |
|--- |--- |
| [Atributos do cliente](attributes.md) | Atributos do cliente (análise e compartilhamento de segmentos) |
| Data Workbench | <ul><li>Atributos derivados do cliente</li><li>Espaços de trabalho pré-criados para descoberta de públicos-alvo</li></ul> |
| Plataforma do Analytics | [Atributos do cliente](attributes.md) |

## Atribuição avançada {#section_9E4986A8389946CCAA7D003268343296}

A Atribuição avançada oferece acesso ao [Analytics Premium](upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) e também à Atribuição algorítmica no Data Workbench (25% do volume de chamadas do servidor).

## Requisitos do Data Workbench {#section_D959CA68D6DB42C38707F8E0CA3654CC}

Os usuários suportados podem solicitar que todas as licenças dos clientes sejam atualizadas para refletir o Premium ao enviar um email para a `dwb@adobe.com`. Essa atualização habilita recursos como Atribuição algorítmica.

A TechOps analisa seu compromisso contratual e determina a infraestrutura gerenciada adequada, aumentando ou reduzindo a capacidade e, em seguida, coordena com você, por meio do Gerente de conta ou consultoria, para implantar quaisquer alterações.

Qualquer software que estiver sendo executado no local deverá ser desativado. Este software inclui Sensores, o que significa que você deve garantir o rastreamento adequado por meio de tags [!DNL Analytics].

## Experience Cloud - Administrar usuários e produtos {#section_6471C54454024301B2E0B687F79F6738}

O Experience Cloud e os serviços principais estão disponíveis para usuários do Analytics Standard e Premium, se você tiver seguido a modernização de implementação descrita em [Introdução - ative as soluções para os serviços principais](core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C). (Esse processo ajuda a modernizar a implementação e permitirá que você se torne um administrador na Experience Cloud.)

Após associar-se à Experience Cloud, é possível fazer logon por meio da Experience Cloud em [!DNL experience.adobe.com] e começar a usar os principais serviços (inclusive os atributos do cliente, os públicos-alvo e a análise de aplicativos móveis).

### Administre usuários e grupos

O gerenciamento de usuários é executado no [Adobe Admin Console](https://helpx.adobe.com/br/enterprise/using/admin-console.html) (link do produto).

Você pode configurar um mapeamento 1:1 entre um grupo criado no Adobe Admin Console e um grupo de soluções (como o Adobe Analytics). Consequentemente, um novo usuário adicionado ao grupo de Admin Console mapeado tem uma conta de solução do Analytics criada automaticamente e vinculada à Adobe ID do usuário. (Os usuários existentes devem vincular manualmente as credenciais da conta da solução para acessar as soluções por meio do logon da Experience Cloud.)

>[!NOTE]
>
>Você pode mapear diversos grupos de solução para um grupo do Admin Console. No entanto, Adobe recomenda o mapeamento de 1:1. Mapear os grupos antecipadamente permite convidar, criar, permitir e adicionar vários usuários carregando um CSV.
