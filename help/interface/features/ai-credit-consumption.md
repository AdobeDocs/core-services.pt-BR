---
title: Trabalhos de agentes e consumo de crédito de IA
description: Saiba mais sobre tarefas de agente e taxas de consumo de crédito de IA em aplicativos do Experience Cloud.
solution: Experience Cloud
topic: Artificial Intelligence
feature: Agentic AI, AI Tools
role: Admin, User
level: Intermediate
source-git-commit: 7eb6c6e463102ca445093c69797619202202b35e
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 9%

---

# Trabalhos de agentes e consumo de crédito de IA

Saiba mais sobre trabalhos de IA agênica e consumo de crédito de IA em aplicativos do Experience Cloud. Para obter informações sobre como habilitar recursos de IA de agente em aplicativos Experience Cloud existentes, consulte [IA de agente no Experience Cloud](agentic-ai.md#existing-apps).

## Trabalhos do agente

Um _trabalho de agente_ é uma série de tarefas e ações que um Agente executa para atingir um resultado específico, conforme determinado pelas entradas do cliente.

Usando prompts de linguagem natural por meio do Assistente de IA, você pode solicitar que os agentes realizem tarefas específicas. Com base nessas entradas, a Agent Orchestrator coordena os agentes apropriados para executar cada etapa nos aplicativos relevantes do Experience Cloud.

## Créditos de IA

Um _crédito de IA_ é uma métrica baseada no uso que quantifica a execução de trabalhos do agente. Os créditos de IA não se aplicam a [aplicativos AI-first](/help/interface/features/agentic-ai.md).

## Consumo de crédito de IA

O uso do crédito de IA pode variar dependendo da complexidade e do valor do trabalho executado:

* Tarefas simples (geralmente de etapa única) consomem menos créditos
* Tarefas complexas (geralmente de várias etapas) consomem mais créditos
* Tarefas que envolvem raciocínio avançado, validação, coordenação de vários agentes ou integração consomem mais créditos

### Taxas de consumo de crédito de IA estimadas

| Agente | Trabalho | Aplicativos compatíveis | Créditos de IA estimados |
|------|-----|------------------------|----------------------|
| Audience Agent | Público-alvo/ideação de conta | <ul><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li></ul> | 50  |
| Audience Agent | Criação de contas/públicos-alvo com base no conhecimento | <ul><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li></ul> | 150 |
| Audience Agent | Gerenciamento de público-alvo/conta | <ul><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li></ul> | 25 |
| Audience Agent | Análise de público-alvo/conta | <ul><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li></ul> | 25 |
| Audience Agent | Ideação de grupo de compra | <ul><li>Adobe Journey Optimizer (B2B)</li></ul> | 25 |
| Data Insights Agent | Análise e visualização de dados | <ul><li>Customer Journey Analytics</li></ul> | 25 |
| Journey Agent | Jornada ideação | <ul><li>Adobe Journey Optimizer (B2B)</li></ul> | 25 |
| Journey Agent | Criação de jornada | <ul><li>Adobe Journey Optimizer (B2B, B2C)</li></ul> | 30 |
| Journey Agent | Análise de jornada | <ul><li>Adobe Journey Optimizer (B2B, B2C)</li></ul> | 50  |
| Journey Agent | Gerenciamento de jornadas | <ul><li>Adobe Journey Optimizer (B2B, B2C)</li></ul> | 25 |
| Agente de suporte ao produto | Solução de problemas com base no conhecimento | <ul><li>Vários aplicativos Experience Cloud</li></ul> | 0 |
| Agente de suporte ao produto | Criação e rastreamento de casos de suporte | <ul><li>Vários aplicativos Experience Cloud</li></ul> | 10 |
| Agente do Supervisor de Conteúdo | Descoberta de conteúdo | <ul><li>Serviços em nuvem Adobe Experience Manager</li></ul> | 5 |
| Agente do Supervisor de Conteúdo | Atualização e otimização de conteúdo | <ul><li>Serviços em nuvem Adobe Experience Manager</li></ul> | 10 |
| Brand Experience Agent | Suporte de implantação | <ul><li>Serviços em nuvem Adobe Experience Manager</li></ul> | 5 |
| Brand Experience Agent | Modernização do site | <ul><li>Serviços em nuvem Adobe Experience Manager</li></ul> | 100 |

>[!NOTE]
>
>O consumo real de crédito de IA pode variar dependendo do número de etapas executadas e iterações por etapa.

## Mais ajuda sobre este tópico

* [IA de agente no Experience Cloud](/help/interface/features/agentic-ai.md)
* [avaliação associada ao uso dos Adobe Experience Platform Agents](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/agents/trial)