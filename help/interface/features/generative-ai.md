---
title: IA em aplicativos da Experience Cloud
description: Saiba como os aplicativos do Experience Cloud usam a IA gerativa e o Assistente de IA.
solution: Experience Cloud
feature: AI Assistant, Generative AI
topic: Administration
role: Admin
level: Intermediate
hide: false
hidefromtoc: true
index: n
exl-id: bdc51956-82aa-4aae-b627-a2018f80b5f5
source-git-commit: fb9d3c45beca38e1ca372b24565946bf1a1da839
workflow-type: tm+mt
source-wordcount: '1392'
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

## Aplicativos com recursos que oferecem suporte a IA

* [GenStudio para marketing de desempenho](#gspm)
* [Gerar variações no AEM Sites (Cloud Service)](#aem-sites)
* [Assistente de IA no Journey Optimizer](#journey-optimizer)
* [ADOBE JOURNEY OPTIMIZER PRIME e ULTIMATE](#ajo-prime-ultimate)
* [Journey Optimizer edição B2B](#ajo-b2b)

### GenStudio para marketing de desempenho {#gspm}

O [GenStudio for Performance Marketing](https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/home) é uma plataforma gerativa orientada por IA que permite criar, entregar e otimizar ativos da campanha. Seus recursos de IA gerativos transformam a forma como o conteúdo de marketing é criado, revisado, compartilhado e analisado.

O recurso _Criação de GenStudio for Performance Marketing_ (ou simplesmente _Criação_) permite que profissionais de marketing e equipes distribuídas criem experiências de alto desempenho sobre a marca. É possível gerar conteúdo para:

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

**Entrada:** Os campos de entrada incluem:

* Número de variações a serem geradas
* Audience Source
* Público-alvo
* Contexto adicional
* Solicitações orientadas pelo cliente

**Saída:** Conteúdo Gerado / Cópia de Mercado. Você também tem a opção de gerar imagens no Adobe Express usando os recursos de IA geradores do Firefly.

Consulte [Gerar imagem](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#generate-image) para saber mais.

**Compatível com o Adobe Firefly:** Sim

## Assistente de IA no Journey Optimizer {#journey-optimizer}

No Journey Optimizer, o Assistente de IA pode ajudá-lo a obter conhecimento sobre o produto e insights operacionais.

**Conhecimento do produto:** o Assistente de IA consulta armazenamentos de dados da Adobe (como a documentação do produto Experience League) para o insight do produto. A saída é independente do cliente.

Exemplo:

* _Quantas atividades ativas posso ter em uma sandbox da Adobe Journey Optimizer?_

**Insights Operacionais (Beta)** - Consulta um repositório de dados de insights operacionais específicos do cliente que contém dados operacionais centralizados sobre o Jornada, particionados pela sandbox do cliente. Esse recurso extrai metadados somente de objetos comerciais e não acessa dados na sandbox.

Exemplo de prompt:

* _Quantas Jornadas foram criadas nos últimos sete dias?_

A saída dos Insights operacionais depende dos metadados extraídos dos objetos comerciais do cliente. Essa saída é independente do cliente.

O _Jornada_ é o único objeto disponível para o Assistente de IA no Journey Optimizer, e os metadados são obtidos da sandbox atual. [Saiba mais...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant).

**Compatível com o Adobe Firefly:** Não

## JOURNEY OPTIMIZER PRIME e ULTIMATE {#ajo-prime-ultimate}

O Journey Optimizer Prime e o Ultimate usam o [Assistente de IA para Acelerador de Conteúdo](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative) para oferecer sugestões de variação de conteúdo pró-ativo para texto e imagens.

Este recurso está disponível para [email](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-email), [notificações por push](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-push), [página da Web](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-web), [conteúdo](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-experimentation) e [SMS](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-sms) canais. Ele fornece geração de texto e imagem com base em prompt.

**Observação:** a saída do Acelerador de Conteúdo no AJO Prime e no Ultimate é indenizada.

**Compatível com o Adobe Firefly:** Sim

## Assistente de IA no Journey Optimizer B2B edition {#ajo-b2b}

O Journey Optimizer B2B edition usa o [Assistente de IA](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant) para ajudá-lo com o conhecimento do produto, com base nos prompts de conhecimento do produto.

**Conhecimento sobre o produto** - Consulta armazenamentos de dados da Adobe (como a documentação do produto da Experience League) para o insight do produto. Essa saída é independente do cliente.

* **Entrada:** Como faço para enviar um email em uma jornada de conta?

* **Saída:** o Conhecimento do Produto é extraído do Experience League (documentação pública). [Saiba mais...](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant)

**Compatível com o Adobe Firefly:** Não

## Cloud Services gerenciados pelo Campaign

O Campaign Managed Cloud Services usa o [Assistente de IA para Acelerador de conteúdo](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-gs) para gerar automaticamente conteúdo personalizado, envolvente e eficaz com base no objetivo de marketing, com conteúdo otimizado para estilos, layouts, tom e muito mais em canais como email, SMS e push.

* **Email** - Gerar um email completo, somente texto ou somente imagem. [Saiba mais](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-content)

* **SMS** - Gerar somente SMS completo ou texto. [Saiba mais...](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-sms)

* **Push** - Criar mensagens atraentes e gerar conteúdo. [Saiba mais...](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-push)

**Observação:** a saída do Acelerador de Conteúdo no Campaign Managed Cloud Services é indenizada.

**Compatível com o Adobe Firefly:** Sim

## Customer Journey Analytics - Assistente de IA

O CJA usa o [Assistente de IA](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant) para ajudar você a descobrir o conhecimento e os insights do produto no Experience League.

**Exemplo de prompt:** Como criar uma métrica calculada?

Novos usuários podem usá-lo para aprender conceitos sobre o Customer Journey Analytics e integrar-se a produtos e recursos com os quais você não está familiarizado.

Usuários experientes podem usar o AI Assistant para apresentar casos de uso mais avançados ou dicas e truques e executar tarefas em um ritmo rápido. Entenda conceitos, solucione problemas ou pesquise informações. [Saiba mais...](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant#knowledge)

**Compatível com o Adobe Firefly:** Não

## Customer Journey Analytics - Legendas inteligentes

[Legendas inteligentes](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions) fornecem insights de linguagem natural para visualizações de linha em visualizações Workspace.

**Exemplo de entrada:** visualizações de linha. As legendas são geradas automaticamente com base nessas visualizações de linha quando você clica em **Legendas inteligentes**.

**Saída:** Legendas de linguagem natural geradas automaticamente.

**Compatível com o Adobe Firefly:** Não

## Real-Time CDP

O Real-Time CDP usa o [Assistente de IA](https://experienceleague.adobe.com/pt-br/docs/experience-platform/ai-assistant/home) para ajudar você a descobrir o conhecimento e os insights do produto no Experience League. Ele consulta um banco de dados e traduz os dados do banco de dados em uma resposta legível.

Há duas classes de perguntas disponíveis:

**Conhecimento sobre o produto** - Consulta armazenamentos de dados da Adobe (como a documentação do produto da Experience League) para o insight do produto. Essa saída é independente do cliente.

Por exemplo:

* _Como é calculada a riqueza do perfil?_

**Insights Operacionais (Beta)** - Consulta um repositório de dados de insights operacionais específicos do cliente que contém dados operacionais centralizados, particionados pela sandbox da AEP do cliente. Extrai metadados somente de Atributos, Públicos-alvo, Fluxos de dados, Conjuntos de dados, Destinos, Esquemas e Fontes, e não acessa dados na sandbox.

Por exemplo, para uma consulta sobre uma audiência, [!DNL AI Assistant] pode acessar o nome da audiência e outros metadados associados, mas não pode acessar os perfis dentro dessa audiência.

Por exemplo:

* Entrada: _Quantos conjuntos de dados eu tenho?_

* Resposta: _A saída dos Insights Operacionais depende dos metadados obtidos dos objetos comerciais do Cliente (Atributos, Públicos, Fluxos de Dados, Conjuntos de Dados, Destinos, Esquemas e Fontes) e inclui um link para uma página de interface do usuário específica contendo os dados consultados._

Para obter mais exemplos, consulte as tabelas de entrada _Conhecimento do Produto_ e _Insights Operacionais_ no [Assistente de IA no Experience Platform](https://experienceleague.adobe.com/pt-br/docs/experience-platform/ai-assistant/home)

**Compatível com o Firefly:** Não


## Marketo

O [Dynamic Chat](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview) cria conversas assistidas por IA com perguntas e respostas personalizadas e pré-aprovadas, bem como um resumo da conversa |<ul><li> **Gerar Perguntas** Forneça URLs das quais o conteúdo é extraído e usado para gerar perguntas/respostas. </li><li> **Resumo da Conversa:** gera um resumo de uma conversa de chat. </li></ul> [Saiba mais...](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/response-library)  | Não |

## Workfront

O [Assistente de IA](https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview) do Workfront ajuda você a realizar seu trabalho, oferecendo informações e sugestões no aplicativo em uma conversa em idioma natural. O AI Assistant oferece a seguinte funcionalidade: resume projetos/tarefas/problemas/documentos, fornece instruções ou informações de referência extraídas da documentação do Workfront no Experience League, gera ou refina fórmulas para campos personalizados calculados.  | <ul><li>**Resumir a Entrada do Projeto:** Resuma este projeto </li><li> **Resumir Saída do Projeto:** Retorna descrições breves da finalidade e do status do projeto, fornece exemplos de tarefas concluídas e ainda pendentes e fornece detalhes e observações adicionais.</li><li> **Gerar/Refinar Entrada de Fórmula:** &quot;Reescreva esta fórmula para remover o erro de expressão inválida.&quot; </li><li> **Gerar/Refinar Saída de Fórmula:** Fórmula gerada ou refinada. </li></ul>**Observação:** o AI Assistant pode levar alguns minutos para gerar a fórmula revisada, dependendo do tamanho e da complexidade da fórmula. | Não  |


<!-- ## Experience Cloud applications that use AI

Learn how Experience Cloud applications use generative AI or AI Assistant, and whether Adobe Firefly is supported. 

| Application | How Generative AI Is Used | Examples | Adobe Firefly? |
|----------|------------|-----------|----------------|
| GenStudio for Performance Marketing | [GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home) is a generative AI-driven platform. It infuses the content creation lifecycle with generative AI capabilities that transform how marketing content is created, reviewed, shared, and analyzed.<br>You can train GenStudio for Performance Marketing on your brand using examples, descriptions of customer personas and products, and brand guidelines. |_GenStudio for Performance Marketing Create_ lets you generate content for emails, Meta ads, LinkedIn ads, display ads, and banners. <br>**Inputs:** <ul><li>Use templates to start the content creation process. </li><li>Add parameters like Brands, Products, and Personas (guidelines) and Content (assets) to shape the generated experience. </li><li>Enter descriptive prompts that describe the context or experience you intend to generate. [Learn more...](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview)</li></ul> |Yes |
|Adobe Experience Manager Sites (Cloud Service)  | AEM Sites uses [Generate Variations](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations). <br>Generate Variations uses generative AI to create content variations based on prompts. These prompts are either provided by Adobe or created and managed by users. |After creating variations, you can use the content on your website and measure its success using the Experimentation functionality of Edge Delivery Services. <br>**Input:** Input fields include Number of Variations to generate; Audience Source / Audience Target; Additional Context, and customer-driven prompts. <ul><li>[Adobe prompt template](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#get-started) </li><li>[User generated prompt](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#create-prompt)</li></ul> **Output:** Generated Content / Market Copy. You also have the option to generate images in Adobe Express using the generative AI capabilities of Firefly. See [Generate Image](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#generate-image). | Yes|
| Adobe Journey Optimizer |Journey Optimizer uses [AI Assistant](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home) with two classes of questions:<ul><li>**Product knowledge** - Queries Adobe data stores (such as Experience League product documentation) for product insight. This output is customer agnostic. </li><li>**Operational Insights (Beta)** - queries a customer-specific operational insights data store that contains centralized operational data about Journeys, partitioned by the customer's sandbox. Pulls metadata only from business objects and does not access data within the sandbox.</li></ul>|<ul><li>**Product Knowledge Input:** How many live activities can I have in one Adobe Journey Optimizer sandbox?</li><li>**Product Knowledge Output:** Product Knowledge pulls from Experience League (public documentation). </li><li>**Operational Insights Input:** How many Journeys have been created in the last seven days? </li><li>**Operational Insights Output:** Operational Insights output depends on metadata pulled from customer's business objects. Journeys is the only object available in AJO, and metadata is pulled from the current sandbox. </li></ul> See [Work with the AI Assistant](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant) and [Field Readiness](https://fieldreadiness-adobe.highspot.com/items/6661f1c132683fd5e6a8adf4?lfrm=srp.1#11) | No |
| Journey Optimizer: _Prime_ and _Ultimate_  | [AI Assistant for Content Accelerator](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative) brings proactive content variation suggestions for text and images. It is available for email, push, web and SMS channels. This new capability provides prompt-based text and image generation. |<ul><li> **Email** - generate a full email, text only or image only. [Learn more...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-email) </li><li> **Push Notification** - Generate a full push notification, text only or image only. [Learn more...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-push) </li><li> **SMS** - Generate a full SMS, or text only. [Learn more](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-sms) </li><li> **Webpage** - Generate web page images or web page text. [Learn more...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-web) </li><li> **Content** - Generate content for various messaging campaigns. [Learn more...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-experimentation)</li></ul> **Note:** Output from Content Accelerator in AJO Prime and Ultimate is indemnified. | Yes   |
| Journey Optimizer B2B Edition  | Uses [AI Assistant](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant) with one class of questions: <br> **Product knowledge** - Queries Adobe data stores (such as Experience League product documentation) for product insight. This output is customer agnostic. | <ul><li>**Input:** How do I send an email in an account journey?</li><li>**Output:** Product Knowledge pulls from Experience League (public documentation). [Learn more...](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant)</li></ul>   | No   |
| Campaign Managed Cloud Services | [AI Assistant for Content Accelerator](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-gs) auto-generates personalized, engaging, and effective content based on the marketing objective with content optimized for brand outlined styles, layouts, tone, and more across channels like Email, SMS, Push. |<ul><li> **Email** - Generate a full email, text only or image only. [Learn more](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-content) </li><li> **SMS** - Generate full SMS or text only. [Learn more...](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-sms) </li><li> **Push** - Craft compelling messaging and generate content. [Learn more...](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-push) </li></ul> **Note:** Output from Content Accelerator in Campaign Managed Cloud Services is indemnified. | Yes  |
| Customer Journey Analytics   | CJA uses [AI Assistant](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant) to help you discover product knowledge and insights from Experience League. <br>For example, new users can use it to learn Customer Journey Analytics concepts and onboard yourself to products and features that you are unfamiliar with. <br>Experienced users can use AI Assistant to present more advanced use cases or tips and tricks and perform tasks at a fast pace. Understand concepts, troubleshoot problems, or search for information. [Learn more...](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant#knowledge) | <ul><li>**Product Knowledge Input:** How do I build a calculated metric? </li><li> **Product Knowledge Output:** Product Knowledge pulls from Experience League (public documentation). </li></ul> | No |
| Customer Journey Analytics    | [Intelligent Captions](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions) provides natural-language insights for line visualizations in Workspace visualizations.| <ul><li>**Input:** Line visualizations. Captions are auto-generated based on such line visualizations when you click **Intelligent captions**. </li><li> **Output:** Auto-generated natural-language captions.</li></ul>  | No             |
| Real-Time CDP |Uses [AI Assistant](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home) to help you discover product knowledge and insights from Experience League. It queries a database and translates data from the database into a human-readable answer. Two classes of questions: <br> **Product knowledge** - Queries Adobe data stores (such as Experience League product documentation) for product insight. This output is customer agnostic. <br> **Operational Insights (Beta)** - Queries a customer-specific operational insights data store that contains centralized operational data, partitioned by the customer's AEP sandbox. Pulls metadata only from Attributes, Audiences, Dataflows, Datasets, Destinations, Schemas, and Sources, and does not access data within the sandbox. <br>For example, for a query about an audience [!DNL AI Assistant] can access the name of the audience and other associated metadata but cannot access the profiles within that audience. | <ul><li>**Product Knowledge Input:** How is profile richness calculated? </li><li>**Product Knowledge Output:** Product Knowledge pulls from Experience League (public documentation). </li><li> **Operational Insights Input:** How many datasets do I have? </li><li> **Operational Insights Output:** Operational Insights output depends on metadata pulled from Customer's business objects (Attributes, Audiences, Dataflows, Datasets, Destinations, Schemas, and Sources), and includes a link to specific UI page containing queried data. </li></ul>For examples, see the _Product Knowledge_ and _Operational Insights_ input tables in [AI Assistant in Experience Platform](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home)  | No |
| Marketo  | [Dynamic Chat](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview) creates AI-assisted conversations with customized and pre-approved questions and answers, as well as conversation summary |<ul><li> **Generate Questions:** Provide URLs from which content is extracted and used to generate questions / responses. </li><li> **Conversation Summary:** Generates a summary of a chat conversation. </li></ul> [Learn more...](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/response-library)  | No |
| Workfront | [AI Assistant](https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview) in Workfront helps you accomplish your work by offering in-app information and suggestions in a natural-language conversation. AI Assistant offers the following functionality: Summarizes projects/tasks/issues/documents, provides instructions or reference information pulled from the Workfront documentation on Experience League, generates or refines formulas for calculated custom fields.  | <ul><li>**Summarize Project Input:** Summarize this project </li><li> **Summarize Project Output:** Returns brief descriptions of the project's purpose and status, gives examples of tasks that are completed and that are still pending, and provides some additional details and notes.</li><li> **Generate/Refine Formula Input:** "Rewrite this formula to remove the invalid expression error." </li><li> **Generate/Refine Formula Output:** Generated or refined formula. </li></ul>**Note:** AI Assistant may take a few moments to generate the revised formula, depending on the size and complexity of the formula. | No  | -->
