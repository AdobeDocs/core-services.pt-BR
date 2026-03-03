---
title: Trabalhos de agentes e consumo de crédito de IA
description: Saiba mais sobre tarefas de agente e taxas de consumo de crédito de IA em aplicativos do Experience Cloud.
solution: Experience Cloud
topic: Artificial Intelligence
feature: Agentic AI, AI Tools
role: Admin, User
level: Intermediate
source-git-commit: d9d9eb0b3bad1abd517e4c6b0bd5ecaa45a7930d
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 3%

---

# Trabalhos de agentes do Adobe Experience Platform e consumo de créditos de IA

Atualização: **quarta-feira, 3 de março de 2026**

Saiba mais sobre trabalhos de IA agênica e consumo de crédito de IA em aplicativos do Experience Cloud. Para obter informações sobre como habilitar recursos de IA de agente em aplicativos Experience Cloud existentes, consulte [IA de agente no Experience Cloud](agentic-ai.md#existing-apps).

## Trabalhos do agente

Um _trabalho de agente_ é uma série de tarefas e ações que um agente executa para atingir um resultado específico, conforme determinado pelas entradas do cliente.

Usando prompts de linguagem natural por meio do Assistente de IA, você pode solicitar que os agentes realizem tarefas específicas. Com base nessas entradas, a Agent Orchestrator coordena os agentes apropriados para executar cada etapa nos aplicativos relevantes do Experience Cloud.

## Créditos de IA

Um _crédito de IA_ é uma métrica baseada no uso que quantifica a execução de trabalhos do agente. Os créditos de IA não se aplicam a [aplicativos AI-first](/help/interface/features/agentic-ai.md).

## Consumo de crédito de IA

O uso do crédito de IA pode variar dependendo da complexidade e do valor do trabalho executado:

* Tarefas simples (geralmente de etapa única) consomem menos créditos
* Tarefas complexas (geralmente de várias etapas) consomem mais créditos
* Tarefas que envolvem raciocínio avançado, validação, coordenação de vários agentes ou integração consomem mais créditos

### Taxas de consumo de crédito de IA estimadas

| Agente | Trabalho | Aplicativos compatíveis | Créditos de IA estimados | Exemplos de prompts |
| ------ | ----- | ------------------------ | ----------------------- | ----------------- |
| Audience Agent | Público-alvo/ideação da conta | <ul><li>Real-Time CDP (edições B2B, B2C e B2P)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 50 | <ul><li>_Mostre-me campos para compradores ricos_</li><li>_Localizar todos os campos relacionados às preferências do cliente_</li></ul> |
| Audience Agent | Criação de conta/público-alvo com base no conhecimento | <ul><li>Real-Time CDP (edições B2B, B2C e B2P)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 150 | <ul><li>_Crie um público-alvo composto por pessoas que vivem na Califórnia_</li><li>_Gerar um público-alvo de membros do VIP que gastaram mais de US$ 1.000 neste trimestre_</li><li>_Crie um público-alvo de usuários que compraram itens de roupas, mas não fizeram uma compra nos últimos 60 dias_</li></ul> |
| Audience Agent | Gerenciamento de público-alvo/conta | <ul><li>Real-Time CDP (edições B2B, B2C e B2P)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 25 | <ul><li>_Tenho públicos-alvo duplicados?_</li><li>_Mostre-me os cinco maiores públicos-alvo._</li><li>_Mostre-me públicos que não estão ativados para nenhum destino_</li><li>_Listar todos os públicos-alvo usados em jornadas ao vivo_</li></ul> |
| Audience Agent | Análise de público-alvo/conta | <ul><li>Real-Time CDP (edições B2B, B2C e B2P)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 25 | <ul><li>_Quais públicos-alvo aumentaram de tamanho em mais de 20% na última semana?_</li><li>_Quanto o público-alvo &quot;Platina Fiel&quot; mudou em comparação ao valor de 30 dias atrás?_</li><li>_Qual é o meu público que cresce mais rápido?_</li></ul> |
| Audience Agent | Ideação de grupo de compra | <ul><li>Adobe Journey Optimizer (B2B edition)</li></ul> | 25 | <ul><li>_Quais contas estão mostrando a intenção para esses produtos?_</li><li>_Mostre-me as pessoas principais por intenção de produto para XYZ._</li><li>_Quais grupos de compras têm mais de 5 membros?_</li></ul> |
| Data Insights Agent | Análise e visualização de dados | <ul><li>Customer Journey Analytics (edições B2C e B2B)</li></ul> | 25 | <ul><li>_Pedidos de tendência em julho_</li><li>_Mostrar receita por região._</li><li>_Mostrar pedidos por gênero, de março a junho._</li><li>_Quais foram minhas 10 principais SKUs por lucro em junho_</li><li>_Proporção de compras por mês do ano_</li><li>_Cota de receita por categoria de produto_</li></ul> |
| Journey Agent | Jornada ideação | <ul><li>Adobe Journey Optimizer (B2B edition)</li></ul> | 25 | <ul><li>_Crie uma jornada para contas de espaço em branco com intenção para minha solução, focalizando pessoas envolvidas com conteúdo no site_</li></ul> |
| Journey Agent | Criação de jornada | <ul><li>Adobe Journey Optimizer (edições B2B e B2C)</li></ul> | 30 | <ul><li>_Gerar uma jornada para enviar um lembrete aos usuários que não concluíram sua primeira compra nos últimos 7 dias_</li><li>_Quando os usuários concluírem sua primeira compra, envie uma confirmação por SMS e uma explicação dos benefícios de acompanhamento por email após 3 dias_</li></ul> |
| Journey Agent | Análise de jornada | <ul><li>Adobe Journey Optimizer (edições B2B e B2C)</li></ul> | 50 | <ul><li>_Quero analisar o fallout por nó para a Campanha do jornada de 4 de julho._</li><li>_Há conflitos de agendamento para a jornada X_</li><li>_Mostrar conflitos de sobreposição de público alvo para a jornada X_</li></ul> |
| Journey Agent | Gerenciamento de jornadas | <ul><li>Adobe Journey Optimizer (edições B2B e B2C)</li></ul> | 25 | <ul><li>_Quantas jornadas ativas eu tenho?_</li><li>_Listar todas as jornadas usando o público X._</li><li>_Listar todas as jornadas atualmente no modo de teste_</li></ul> |
| Agente de suporte ao produto | Solução de problemas com base no conhecimento | <ul><li>Real-Time CDP (edições B2B, B2C e B2P)</li><li>Adobe Journey Optimizer (edições B2C e B2B)</li><li>Customer Journey Analytics (edições B2C e B2B)</li></ul> | 0 | <ul><li>_Por que minha contagem de perfis é diferente no Painel de Uso da Licença e na home page do Experience Platform?_</li><li>_Quais são os motivos para uma jornada não ser acionada?_</li><li>_Como o Adobe Experience Platform cria experiências em tempo real?_</li><li>_Como você configura e usa alertas no Adobe Experience Platform?_</li><li>_Qual é o limite de riqueza média de perfis na Ativação do Adobe Experience Platform?_</li></ul> |
| Agente de suporte ao produto | Criação e rastreamento de casos de suporte | <ul><li>Real-Time CDP (edições B2B, B2C e B2P)</li>Adobe Journey Optimizer (edições B2C e B2B)<li>Customer Journey Analytics (edições B2C e B2B)</li><li>Adobe Experience Manager</li></ul> | 10 | <ul><li>_Criar um novo tíquete de suporte para meu trabalho de segmentação com falha_</li><li>_Qual é o status do tíquete E-001772068?_</li></ul> |
| Agente do Supervisor de Conteúdo | Descoberta de conteúdo | <ul><li>Adobe Experience Manager Assets</li></ul> | 5 | <ul><li>_Mostrar fragmentos de conteúdo para criar a campanha de oferta WKND._</li><li>_Localizar imagens PNG da embalagem do produto._</li><li>_Mostrar imagens com marcas de formatação do Office na pasta WKND._</li><li>_Há svgs na pasta WKND?_</li><li>_Mostre-me todos os formulários de pedido de empréstimo._</li><li>_Estou procurando formulários de integração de funcionários._</li></ul> |
| Agente do Supervisor de Conteúdo | <ul><li>Otimização de conteúdo</li></ul> | <ul><li>Adobe Experience Manager Assets</li></ul> | 10 | <ul><li>_Crie uma representação 2000px como JPEG com 80% de qualidade._</li><li>_Criar uma representação para uma história do Instagram._</li><li>_Sobreponha a imagem com 30% de gráficos com desconto sobre o banner promocional, colocando-a a 100px do centro._</li><li>_Alterar cor de fundo do PNG para #ff8932._</li></ul> |
| Agente de governança de marca | <ul><li>Atualização de conteúdo</li><li>Criação de Forms</li><li>Solução de problemas de pipeline</li></ul> | <ul><li>Serviços em nuvem Adobe Experience Manager</li><li>Adobe Experience Manager Sites</li><li>Adobe Experience Manager Forms</li></ul> | 50 | <ul><li>_Solucionar problemas do meu pipeline com falha_</li><li>_Listar meus pipelines com falha para o Programa Principal._</li><li>_Analise meu pipeline com falha chamado &quot;Pipeline de Desenvolvimento&quot;._</li><li>_Solução de problemas de execução de pipeline 1234567_</li></ul> |
| Brand Experience Agent | Modernização do site | Serviços em nuvem Adobe Experience Manager | 100 | <ul><li>_Migrar a página`https://wknd-trendsetters.site`_</li></ul> |

>[!NOTE]
>
>O consumo real de crédito de IA pode variar dependendo do número de etapas executadas e iterações por etapa.

## Mais ajuda sobre este tópico

* [IA de agente no Experience Cloud](/help/interface/features/agentic-ai.md)
* [avaliação associada ao uso dos Adobe Experience Platform Agents](https://experienceleague.adobe.com/pt-br/docs/experience-cloud-ai/experience-cloud-ai/agents/trial)
