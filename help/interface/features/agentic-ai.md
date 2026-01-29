---
title: IA de agente em aplicativos do Experience Cloud
description: Saiba onde a IA de agente está disponível nos aplicativos da Experience Cloud.
solution: Experience Cloud
landing-page-name: ai
landing-page-breadcrumb-title: AI Documentation
topic: Artificial Intelligence
feature: Agentic AI, AI Tools
role: Admin, User
level: Intermediate
exl-id: c1a8f9a7-4752-4040-b5f0-dc775417f536
source-git-commit: 3ed72cfa1fd7a6559ac7dd7b31007798c228d53e
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 3%

---

# IA de agente no Adobe Experience Cloud

Atualizado em: **29 de janeiro de 2026**

Os agentes do Adobe Experience Platform usam o Experience Platform [Agent Orchestrator](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/home) para adicionar recursos baseados em agente aos aplicativos do Experience Cloud.

Esses agentes ajudam a automatizar tarefas, fornecer insights mais rapidamente e simplificar fluxos de trabalho. Como resultado, as equipes podem trabalhar com mais eficiência e obter mais valor do Experience Cloud.

O acesso aos agentes de IA no Experience Cloud está disponível no:

* [Aplicativos Experience Cloud existentes](#existing-apps)
* [Aplicativos Experience Cloud AI First](#ai-first-apps)

As seções a seguir descrevem essas duas maneiras de ativar a IA agêntica no Experience Cloud.

## Aplicativos Experience Cloud existentes {#existing-apps}

Em aplicativos existentes, você pode usar a linguagem natural para instruir os Adobe Experience Platform Agents por meio da interface conversacional do [Assistente de IA](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/home). O Assistente de IA está disponível nas exibições em tela cheia e no painel direito.

Os agentes podem ser ativados nos aplicativos Experience Cloud existentes para clientes em uma das seguintes categorias:

* Você adquiriu uma licença de Créditos de IA de agentes da Adobe Experience Platform
* Você está incluído em uma avaliação vinculada ao uso (créditos de IA limitados fornecidos)
* Você transacionou a SKU do Agent Orchestrator Promo (licença de avaliação limitada por tempo)

O uso de agentes de IA para executar _trabalhos de agente_ consome créditos de IA. Saiba mais sobre trabalhos de agentes e créditos de IA em _[Trabalhos de agentes e consumo de crédito de IA](/help/interface/features/ai-credit-consumption.md)_.

Os agentes de IA seguem a _sua_ entrada, supervisão e respeitam os controles de acesso no nível do produto. Você só pode executar tarefas ou acessar dados que estão autorizados a usar no produto Experience Cloud subjacente.

### Agentes de IA em aplicativos Experience Cloud existentes {#existing-apps-table}

A tabela a seguir lista os Experience Platform Agents disponíveis nos aplicativos Experience Cloud existentes.

| Nome do agente | Recursos | Aplicativos compatíveis |
|---|----------|----------|
| [Audience Agent](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/agents/audience) | Capacite suas equipes para criar, gerenciar e otimizar públicos-alvo usando solicitações de linguagem natural para facilitar, aumentar a eficiência e acelerar a comercialização. | <ul><li>Real-Time CDP (edições B2B, B2C e B2P)</li><li>Adobe Journey Optimizer (edições B2B e B2C)</li></ul> |
| **Agente do Supervisor de Conteúdo** | <ul><li>[Descoberta de Conteúdo](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/discovery/overview): acelere a criação e impulsione a descoberta com prompts simplificados em linguagem natural para localizar e exibir instantaneamente o conteúdo do Experience Manager em imagens, vídeos, documentos baseados em texto, fragmentos de conteúdo e formulários.</li><li>[Otimização de conteúdo](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/content-optimization/overview): simplifique a criação de variantes de conteúdo visual a partir de ativos de origem usando prompts de linguagem natural.</li><li>[Produção de experiência](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/production/overview): automatiza tarefas de alto esforço e alto volume na CMS. Esse agente transforma processos manuais e demorados em fluxos de trabalho rápidos assistidos por IA que mantêm cada experiência atualizada e consistente, ajudando sua empresa a atingir suas metas.</li></ul> | <ul><li>Adobe Experience Manager (Descoberta de Conteúdo)</li></ul><ul><li>Adobe Experience Manager com Dynamic Media com OpenAPI (otimização de conteúdo)</li></ul><ul><li>Adobe Experience Manager Cloud Services e Edge Delivery Services (produção da experiência) </li></ul> |
| [Data Insights Agent](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/cja-b2c-overview/data-analysis-ai) | Responde rapidamente a perguntas sobre seus dados. Ele cria visualizações relevantes no Analysis Workspace usando componentes da visualização de dados e seus dados reais. | <ul><li>Customer Journey Analytics (edições B2B e B2C)</li></ul> |
| **Brand Experience Agent** | [Suporte de Implantação](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/development/overview): ajuda desenvolvedores e administradores técnicos do AEM CS a solucionar falhas de etapa de compilação no pipeline da Cloud Manager, analisando a causa raiz e sugerindo correções. | <ul><li>Assistente de IA no AEM Cloud Service e no Adobe Managed Services</li></ul> |
| **Agente de governança de marca*** | [Governança da marca](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/governance/overview): proteja a integridade e a conformidade da marca aplicando políticas de segurança, normativas e de marca em toda a Experience Manager. Esse agente aplica a governança da marca para manter os padrões visuais e de mensagens. Ele usa permissões granulares para gerenciar alterações de acesso e conteúdo e incorpora o DRM para manter as restrições de licenciamento e uso. | <ul><li>Adobe Experience Manager Sites</li><li>Adobe Experience Manager Assets</li><li>Adobe Experience Manager Forms</li></ul> |
| [Journey Agent](https://experienceleague.adobe.com/pt-br/docs/experience-cloud-ai/experience-cloud-ai/agents/ajo-agent-analyze) | Permita que suas equipes criem, analisem e otimizem rapidamente as jornadas de clientes multitoque em escala. | <ul><li>Adobe Journey Optimizer (edições B2B e B2C)</li></ul> |
| [Agente de Suporte ao Produto](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/new-features/customer-support) | Solucione problemas de suporte sem sair dos workflows, crie tíquetes de suporte ao cliente e rastreie o progresso do caso usando o Assistente de IA. | <ul><li>Real-Time CDP (edições B2B, B2C e B2P)</li><li>Adobe Journey Optimizer (edições B2B e B2C)</li><li>Adobe Journey Optimizer B2B edition</li><li>Customer Journey Analytics</li><li>Adobe Experience Manager</li></ul> |

Asterisco (*): este agente está acessível aos clientes no programa Explorer. O Explorer Program é um programa exclusivo para convidados que fornece acesso antecipado aos recursos mais recentes da Adobe. Entre em contato com o seu representante de conta para obter mais informações.

## Aplicativos Experience Cloud AI First {#ai-first-apps}

Aplicativos de AI-first são construídos com Al gerativo ou agêntico no núcleo. Eles usam Al gerativo ou agêntico para tarefas-chave, e os recursos de agente já estão incluídos na licença de aplicativo Al-first. Dessa forma, eles não exigem a licença da Experience Platform Agent Orchestrator.

A tabela a seguir lista os Experience Platform Agents disponíveis como aplicativos Al-first. Eles são ativados pelo licenciamento desses aplicativos Al-first:

| Nome do agente | Recursos | Aplicativos compatíveis |
|---|----------|----------|
| [Agente de experimentação](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/content-experiment/experiment/experiment-accelerator-security) | Automatize, analise e sintetize insights para que você possa identificar rapidamente experiências de alto impacto e oportunidades de crescimento em um espaço de trabalho centralizado — tudo isso enquanto reduz os processos manuais. | <ul><li>AJO Experimentation Accelerator</li></ul> |
| [Agente de Otimização LLM](https://experienceleague.adobe.com/pt-br/docs/llm-optimizer/using/home) | Melhore a visibilidade, a precisão e a influência em ambientes de pesquisa orientados por IA, forneça insights sobre a presença da marca em respostas geradas por IA, ofereça recomendações de conteúdo prescritivas e automatize correções de otimização. | <ul><li>Adobe LLM Optimizer</li></ul> |
| [Site Optimization Agent](https://experienceleague.adobe.com/pt-br/docs/experience-manager-sites-optimizer/content/home) | Maximize o impacto nos negócios, detectando e implantando automaticamente as melhorias no site. Com o uso de IA gerativa e várias tecnologias de monitoramento, você pode aumentar a aquisição de tráfego do site, o engajamento e muito mais | <ul><li>AEM Sites Optimizer</li></ul> |
| [Product Advisor Agent](https://experienceleague.adobe.com/en/docs/brand-concierge/content/documentation/overview) | Impulsione a conversão e o engajamento por meio da descoberta inteligente de produtos com reconhecimento de contexto e adaptada às preferências e comportamentos individuais. | <ul><li>Adobe Brand Concierge</li></ul> |

## Mais ajuda sobre este tópico

* Página inicial da documentação do [AI no Experience Cloud](https://experienceleague.adobe.com/pt-br/docs/ai)
* [Visão geral dos agentes no AEM](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/overview)

[!BADGE Saiba mais sobre o Adobe for Business]{type=Informative url="https://business.adobe.com/products/experience-platform/agent-orchestrator.html" tooltip="Acesse Business.adobe.com"}
