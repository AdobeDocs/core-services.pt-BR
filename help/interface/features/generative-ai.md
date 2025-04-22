---
title: IA em aplicativos da Experience Cloud
description: Saiba mais sobre IA gerativa e como os aplicativos do Experience Cloud usam o genAI e o Assistente de IA.
solution: Experience Cloud
feature: AI Assistant, Generative AI
topic: Administration
role: Admin
level: Intermediate
exl-id: bdc51956-82aa-4aae-b627-a2018f80b5f5
source-git-commit: aad561869cdfa7ddbc66b296d0a46c8f49f83d94
workflow-type: tm+mt
source-wordcount: '1313'
ht-degree: 4%

---

# IA em aplicativos da Experience Cloud

Esta página ajuda você a entender a IA gerativa e como usá-la em aplicativos do Experience Cloud. Saiba quais recursos do produto usam IA gerativa, o AI Assistant e se o Adobe Firefly é compatível.

## Sobre a IA gerativa e o Assistente de IA

A IA gerativa é um tipo de inteligência artificial que faz mais do que simplesmente responder a perguntas. Ele _cria_ conteúdo e _responde_ aos seus _prompts_ (perguntas e instruções).

* **Criar:** refere-se à capacidade da IA de gerar novo conteúdo (texto, imagens, música ou vídeos) do zero, com base em seu treinamento e prompts de entrada. Esta habilidade é o aspecto _gerativo_ da IA gerativa.

* **Responder:** refere-se à IA que fornece uma resposta ou reação a um prompt específico, normalmente com base em seu conhecimento ou em seus recursos de raciocínio.

Se você é novo no Experience Cloud, pode usar IA gerativa para obter conhecimento sobre o produto rapidamente. Como usuário experiente, você pode descobrir insights operacionais em segundos em vez de horas.

### Assistente de IA

O [Assistente de IA](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/landing) é uma ferramenta conversacional com suporte no Experience Platform e em aplicativos relacionados. Use-o para acelerar seus fluxos de trabalho, melhorar o conhecimento sobre o produto, solucionar problemas ou pesquisar informações. Em certos aplicativos, o Assistente de IA permite descobrir insights operacionais imediatamente.

As respostas do Experience League ao conhecimento do produto são verificáveis e citadas com links. Saiba mais sobre os tipos de [prompts baseados em objetivos](https://experienceleague.adobe.com/pt-br/docs/experience-platform/ai-assistant/home) para aproveitar ao máximo o Assistente de IA.

<!-- **Your data remains yours**

In AI Assistant, security is the priority:

* Customer data is not used to train language models.
* AI Assistant looks at only the documents that you tell it to. You are in control.
* Your people can use AI Assistant only on documents they can access.
* It's audit-ready: Responses are attributable to source documents.
* Enterprise controls are in place to manage who has AI access in the company. -->

## Aplicativos com recursos que oferecem suporte a IA

* [GenStudio para marketing de desempenho](#gspm)
* [Gerar variações no AEM Sites (Cloud Service)](#aem-sites)
* [Assistente de IA no Journey Optimizer](#journey-optimizer)
* [ADOBE JOURNEY OPTIMIZER PRIME e ULTIMATE](#ajo-prime-ultimate)
* [Journey Optimizer edição B2B](#ajo-b2b)
* [Assistente de IA no Journey Optimizer Prime e Ultimate](#ajo-prime-ultimate)
* [Assistente de IA no Journey Optimizer B2B edition](#ajo-b2b)
* [Assistente de IA no Campaign Managed Cloud Services](#campaign-cs)
* [Assistente de IA no Customer Journey Analytics](#cja)
* [Legendas inteligentes no Customer Journey Analytics](#cja-captions)
* [Assistente de IA no Real-Time CDP](#rtcdp)
* [Dynamic Chat no Marketo](#marketo)
* [Assistente de IA no Workfront](#workfront)

### GenStudio para marketing de desempenho {#gspm}

O [GenStudio for Performance Marketing](https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/home) é uma plataforma gerativa orientada por IA com recursos que podem transformar a forma como o conteúdo de marketing é criado, revisado, compartilhado e analisado.

Na página inicial [Criar](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview), você pode criar experiências com alto desempenho e sobre as marcas. Gerar conteúdo para:

* Emails
* Meta ads
* Anúncios do LinkedIn
* Exibir anúncios
* Banners

Você também pode treinar a GenStudio for Performance Marketing em sua marca usando exemplos, descrições de personas e produtos do cliente e diretrizes de marca. [Saiba mais...](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview)

**Compatível com o Adobe Firefly:** Planejado

### Gerar variações no Experience Manager Sites {#aem-sites}

[Gerar variações](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations) no AEM Sites usa a IA gerativa para criar variações de conteúdo com base em prompts. Estes prompts são fornecidos pela [Adobe](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#get-started) ou criados e gerenciados por [usuários](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#create-prompt).

Depois de criar variações, você pode usar o conteúdo em seu site e medir seu sucesso usando o recurso Experimentação no Edge Delivery Services.

### Campos de entrada e saída

Os campos de entrada incluem:

* Número de variações a serem geradas
* Audience Source
* Público-alvo
* Contexto adicional
* Solicitações orientadas pelo cliente

A saída é conteúdo gerado ou cópia de mercado.

Você também tem a opção de gerar imagens no Adobe Express usando os recursos de IA geradores do Firefly. [Saiba mais...](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#generate-image)

**Compatível com o Adobe Firefly:** Sim

## Assistente de IA no Journey Optimizer {#journey-optimizer}

No Journey Optimizer, o Assistente de IA pode ajudá-lo a obter conhecimento sobre o produto e insights operacionais.

**Conhecimento do produto:** o Assistente de IA consulta armazenamentos de dados da Adobe (como a documentação do produto Experience League) para o insight do produto. A saída é independente do cliente.

Exemplo:

* _Quantas atividades ativas posso ter em uma sandbox da Adobe Journey Optimizer?_

**Insights Operacionais (Beta)** - O Assistente de IA consulta um repositório de dados de insights operacionais específicos do cliente que contém dados operacionais centralizados sobre o Jornada, particionados pela sandbox do cliente. Esse recurso extrai metadados somente de objetos comerciais e não acessa dados na sandbox.

Exemplo de prompt:

* _Quantas Jornadas foram criadas nos últimos sete dias?_

A saída dos Insights operacionais depende dos metadados extraídos dos objetos comerciais do cliente. Essa saída é independente do cliente.

O _Jornada_ é o único objeto disponível para o Assistente de IA no Journey Optimizer, e os metadados são obtidos da sandbox atual. [Saiba mais...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant).

**Compatível com o Adobe Firefly:** Não

## Assistente de IA no Journey Optimizer Prime e Ultimate {#ajo-prime-ultimate}

O Journey Optimizer Prime e o Ultimate usam o [Assistente de IA para Acelerador de Conteúdo](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative) para oferecer sugestões de variação de conteúdo pró-ativo para texto e imagens.

Este recurso está disponível para [email](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-email), [notificações por push](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-push), [página da Web](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-web), [conteúdo](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-experimentation) e [SMS](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-sms) canais. Ele fornece geração de texto e imagem com base em prompt.

**Observação:** a saída do Acelerador de Conteúdo no AJO Prime e no Ultimate é indenizada.

**Compatível com o Adobe Firefly:** Sim

## Assistente de IA no Journey Optimizer B2B edition {#ajo-b2b}

O Journey Optimizer B2B edition usa o [Assistente de IA](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/ai-assistant/ai-assistant-overview) para ajudá-lo com o conhecimento do produto, com base nos prompts de conhecimento do produto.

**Conhecimento sobre o produto** - Consulta armazenamentos de dados da Adobe (como a documentação do produto da Experience League) para o insight do produto. Essa saída é independente do cliente.

* **Entrada:** Como faço para enviar um email em uma jornada de conta?

* **Saída:** o Conhecimento do Produto é extraído do Experience League (documentação pública). [Saiba mais...](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/ai-assistant/question-guidance)

**Compatível com o Adobe Firefly:** Não

## Assistente de IA no Campaign Managed Cloud Services {#campaign-cs}

O Campaign Managed Cloud Services usa o [Assistente de IA para Acelerador de Conteúdo](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-gs). Esse recurso permite gerar automaticamente conteúdo personalizado, envolvente e eficaz com base em seu objetivo de marketing, com conteúdo otimizado para estilos, layouts, tons e muito mais. Você pode usá-lo em canais como [email](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-content), [SMS](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-sms) e [push](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-push).

**Observação:** a saída do Acelerador de Conteúdo no Campaign Managed Cloud Services é indenizada.

**Compatível com o Adobe Firefly:** Sim

## Assistente de IA no Customer Journey Analytics {#cja}

O Customer Journey Analytics usa o [Assistente de IA](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/cja-b2c-overview/ai-assistant) para ajudar você a descobrir o conhecimento e os insights do produto no Experience League.

**Exemplo de prompt:** Como criar uma métrica calculada?

Novos usuários podem usá-lo para aprender conceitos sobre o Customer Journey Analytics e integrar-se a produtos e recursos com os quais você não está familiarizado.

Usuários experientes podem usar o AI Assistant para apresentar casos de uso mais avançados ou dicas e truques e executar tarefas em um ritmo rápido. Entenda conceitos, solucione problemas ou pesquise informações. [Saiba mais...](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant#knowledge)

**Compatível com o Adobe Firefly:** Não

## Legendas inteligentes no Customer Journey Analytics {#cja-captions}

As [Legendas inteligentes](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions) no Customer Journey Analytics fornecem insights de linguagem natural para as visualizações do Workspace usadas com mais frequência.

**Compatível com o Adobe Firefly:** Não

## Assistente de IA no Real-Time CDP {#rtcdp}

O Real-Time CDP usa o [Assistente de IA](https://experienceleague.adobe.com/pt-br/docs/experience-platform/ai-assistant/home) para ajudar você a descobrir o conhecimento e os insights do produto no Experience League. [Obtenha dicas](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/questions) sobre como fazer perguntas.

Ele também oferece insights operacionais (em beta). O Assistente de IA consulta um armazenamento de dados de insights operacionais específicos do cliente que contém dados operacionais centralizados, particionados pela sandbox da AEP do cliente. Ele extrai metadados somente de Atributos, Públicos-alvo, Fluxos de dados, Conjuntos de dados, Destinos, Esquemas e Fontes e não acessa dados na sandbox.

Por exemplo, para uma consulta sobre uma audiência, [!DNL AI Assistant] pode acessar o nome da audiência e outros metadados associados, mas não pode acessar os perfis dentro dessa audiência.

Por exemplo:

* Entrada: _Quantos conjuntos de dados eu tenho?_

* Resposta: a saída do Insights Operacionais depende dos metadados obtidos dos objetos de negócios do Cliente (Atributos, Públicos, Fluxos de dados, Conjuntos de dados, Destinos, Esquemas e Fontes) e inclui um link para uma página de interface do usuário específica contendo dados consultados.

Para obter mais exemplos, consulte as tabelas de entrada _Conhecimento do Produto_ e _Insights Operacionais_ no [Assistente de IA no Experience Platform](https://experienceleague.adobe.com/pt-br/docs/experience-platform/ai-assistant/home)

**Compatível com o Firefly:** Não

## Dynamic Chat no Marketo {#marketo}

Os recursos alimentados por IA gerativa no Adobe Dynamic Chat permitem otimizar a produtividade de seus agentes de vendas, obter insights sobre a intenção de visitante do site e responder às perguntas do visitante de maneira segura. Você pode pré-aprovar as perguntas, as respostas e o resumo da conversa. [Saiba mais...](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/overview)

**Compatível com o Firefly:** Não

## Assistente de IA no Workfront {#workfront}

O Assistente de IA no Workfront ajuda você a realizar seu trabalho oferecendo informações e sugestões no aplicativo. É possível:

* Obtenha resumos de alguns objetos, fornecendo uma exibição de alto nível da intenção ou dos detalhes do objeto.
* Faça perguntas e deixe [!DNL AI Assistant] encontrar respostas no Experience League.
* Obtenha fórmulas geradas com base em seus prompts. Você também pode resolver erros em suas expressões personalizadas inválidas em campos calculados.
* Localize projetos, tarefas e problemas.

[Saiba mais...](https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview)

**Compatível com o Firefly:** Não
