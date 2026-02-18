---
title: Trabalhos de agentes e consumo de crédito de IA
description: Saiba mais sobre tarefas de agente e taxas de consumo de crédito de IA em aplicativos do Experience Cloud.
solution: Experience Cloud
topic: Artificial Intelligence
feature: Agentic AI, AI Tools
role: Admin, User
level: Intermediate
source-git-commit: bb6adf13bed37d4a885b5baec28199efade592e1
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 2%

---

# Trabalhos de agentes do Adobe Experience Platform e consumo de créditos de IA

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
| ------ |-----|------------------------|----------------------|----------------|
| Audience Agent | Público-alvo/ideação da conta | <ul><li>Real-Time CDP (edições B2B, B2C e B2P)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 50 | <ul><li>Mostre-me campos para compradores ricos</li><li>Localizar todos os campos relacionados às preferências do cliente</li></ul> |
| Audience Agent | Criação de conta/público-alvo com base no conhecimento | <ul><li>Real-Time CDP (edições B2B, B2C e B2P)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 150 | <ul><li>Criar um público-alvo composto por pessoas que vivem na Califórnia</li><li>Gerar um público-alvo de membros do VIP que gastaram mais de US$ 1.000 neste trimestre</li><li>Crie um público-alvo de usuários que compraram itens de roupas, mas não fizeram uma compra nos últimos 60 dias</li></ul> |
| Audience Agent | Gerenciamento de público-alvo/conta | <ul><li>Real-Time CDP (edições B2B, B2C e B2P)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 25 | <ul><li>Tenho públicos-alvo duplicados?</li><li>Mostre-me os 5 maiores públicos-alvo.</li><li>Mostre-me públicos que não estão ativados para nenhum destino</li><li>Listar todos os públicos-alvo usados em jornadas ativas</li></ul> |
| Audience Agent | Análise de público-alvo/conta | <ul><li>Real-Time CDP (edições B2B, B2C e B2P)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 25 | <ul><li>Quais públicos-alvo aumentaram de tamanho em mais de 20% na última semana?</li><li>Quanto mudou o público de &quot;Platina Leal&quot; em comparação com o valor de 30 dias atrás?</li><li>Qual é o meu público que cresce mais rápido?</li></ul> |
| Audience Agent | Ideação de grupo de compra | <ul><li>Adobe Journey Optimizer (B2B edition)</li></ul> | 25 | <ul><li>Quais contas estão mostrando a intenção para esses produtos?</li><li>Mostre-me as pessoas principais por intenção de produto para XYZ.</li><li>Quais grupos de compras têm mais de cinco membros?</li></ul> |
| Data Insights Agent | Análise e visualização de dados | <ul><li>Customer Journey Analytics (edições B2C e B2B)</li></ul> | 25 | <ul><li>Pedidos de tendência em julho</li><li>Mostrar receita por região.</li><li>Mostre pedidos por gênero, de março a junho.</li><li>Quais eram meus 10 principais SKUs por lucro em junho</li><li>Proporção de compras por mês do ano</li><li>Parte da receita por categoria de produto</li></ul> |
| Journey Agent | Jornada ideação | <ul><li>Adobe Journey Optimizer (B2B edition)</li></ul> | 25 | <ul><li>Criar uma jornada para contas de espaço em branco com intenção para minha solução, concentrando-se em pessoas envolvidas com conteúdo no site</li></ul> |
| Journey Agent | Criação de jornada | <ul><li>Adobe Journey Optimizer (edições B2B e B2C)</li></ul> | 30 | <ul><li>Gerar uma jornada para enviar um lembrete aos usuários que não concluíram a primeira compra nos últimos sete dias</li><li>Quando os usuários concluírem a primeira compra, enviem uma confirmação por SMS e uma explicação dos benefícios de acompanhamento por email após 3 dias</li></ul> |
| Journey Agent | Análise de jornada | <ul><li>Adobe Journey Optimizer (edições B2B e B2C)</li></ul> | 50 | <ul><li>Quero analisar o fallout por nó para a Campanha do jornada de 4 de julho.</li><li>Há conflitos de agendamento para a jornada X</li><li>Mostrar conflitos de sobreposição de público alvo para a jornada X</li></ul> |
| Journey Agent | Gerenciamento de jornadas | <ul><li>Adobe Journey Optimizer (edições B2B e B2C)</li></ul> | 25 | <ul><li>Quantas jornadas ao vivo eu tenho?</li><li>Liste todas as jornadas usando o público-alvo X.</li><li>Listar todas as jornadas atualmente no modo de teste</li></ul> |
| Agente de suporte ao produto | Solução de problemas com base no conhecimento | <ul><li>Real-Time CDP (edições B2B, B2C e B2P)</li><li>Adobe Journey Optimizer (edições B2C e B2B)</li><li>Customer Journey Analytics (edições B2C e B2B)</li></ul> | 0 | <ul><li>Por que minha contagem de perfis é diferente no Painel de uso de licenças e na página inicial do Experience Platform?</li><li>Quais são os motivos pelos quais uma jornada não é acionada?</li><li>Como o Adobe Experience Platform cria experiências em tempo real?</li><li>Como você configura e usa alertas no Adobe Experience Platform?</li><li>Qual é o limite médio de riqueza de perfil na Ativação do Adobe Experience Platform?</li></ul> |
| Agente de suporte ao produto | Criação e rastreamento de casos de suporte | <ul><li>Real-Time CDP (edições B2B, B2C e B2P)</li>Adobe Journey Optimizer (edições B2C e B2B)<li>Customer Journey Analytics (edições B2C e B2B)</li><li>Adobe Experience Manager</li></ul> | 10 | <ul><li>Criar um novo tíquete de suporte para meu trabalho de segmentação com falha</li><li>Qual é o status do ticket E-001772068?</li></ul> |
| Agente do Supervisor de Conteúdo | Descoberta de conteúdo | <ul><li>Serviços em nuvem Adobe Experience Manager</li></ul> | 5 | <ul><li>Mostrar fragmentos de conteúdo para criar a campanha de oferta WKND.</li><li>Localizar imagens PNG da embalagem do produto.</li><li>Mostrar imagens marcadas no Office na pasta WKND.</li><li>Há algum svgs na pasta WKND?</li><li>Mostre-me todos os formulários de solicitação de empréstimo.</li><li>Estou procurando formulários de integração de funcionários.</li></ul> |
| Agente do Supervisor de Conteúdo | <ul><li>Atualização de conteúdo</li><li>Otimização de conteúdo</li><li>Criação de Forms</li></ul> | <ul><li>Serviços em nuvem Adobe Experience Manager</li></ul> | 10 | <ul><li>Crie uma representação 2000px como JPEG com 80% de qualidade.</li><li>Crie uma representação para uma história do Instagram.</li><li>Sobreponha a imagem com gráficos com 30% de desconto sobre o banner promocional, colocando-a a 100px do centro.</li><li>Alterar a cor de fundo do PNG para #ff8932.</li></ul> |
| Brand Experience Agent | <ul><li>Suporte da experiência</li><li>Suporte de implantação</li></ul> | <ul><li>Serviços em nuvem Adobe Experience Manager</li></ul> | 5 | <ul><li>Solucionar problemas do pipeline que falhou</li><li>Listar meus pipelines com falha para o Programa principal.</li><li>Analise meu pipeline com falha chamado &quot;Pipeline de desenvolvimento&quot;.</li><li>Solução de problemas de execução de pipeline 1234567</li></ul> |
| Brand Experience Agent | Modernização do site | Serviços em nuvem Adobe Experience Manager | 100 | <ul><li>Migrar a página https://wknd-trendsetters.site</li></ul> |

>[!NOTE]
>
>O consumo real de crédito de IA pode variar dependendo do número de etapas executadas e iterações por etapa.

## Mais ajuda sobre este tópico

* [IA de agente no Experience Cloud](/help/interface/features/agentic-ai.md)
* [avaliação associada ao uso dos Adobe Experience Platform Agents](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/agents/trial)