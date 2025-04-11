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
source-git-commit: 4d784762d7d533b672e0cfa6944a3f26ebca0eaa
workflow-type: tm+mt
source-wordcount: '1994'
ht-degree: 5%

---

# IA em aplicativos da Experience Cloud

Esta página ajuda você a entender como os aplicativos do Experience Cloud usam IA gerativa e onde encontrar as informações específicas do aplicativo. Saiba mais sobre as classes de perguntas, prompts e modelos de entrada e saída.

## Sobre a IA gerativa e o Assistente de IA

A IA gerativa é um tipo de inteligência artificial que pode _criar_ conteúdo novo e _responder_ às suas instruções e perguntas (prompts):

* **Criar:** refere-se à capacidade da IA de gerar novo conteúdo (texto, imagens, música ou vídeos) do zero, com base em seu treinamento e prompts de entrada. Esta habilidade é o aspecto _gerativo_ da IA gerativa.

* **Responder:** refere-se à IA que fornece uma resposta ou reação a uma pergunta, instrução ou prompt específico, normalmente com base em seu conhecimento ou recursos de raciocínio.

Determinados aplicativos da Experience Cloud aproveitam a IA gerativa, ajudando novos usuários a obter rapidamente conhecimento sobre o produto e usuários experientes a descobrir insights operacionais em segundos em vez de horas.

### Assistente de IA

O [Assistente de IA](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/landing) é uma ferramenta conversacional com suporte no Experience Platform e em aplicativos relacionados. Use-o para acelerar seus fluxos de trabalho, melhorar o conhecimento sobre o produto, solucionar problemas ou pesquisar informações. O Assistente de IA permite descobrir insights operacionais em segundos, em vez de horas.

Todas as respostas de conhecimento do produto são verificáveis e citadas com links para a documentação do produto no Experience League. [Saiba mais sobre o Assistente de IA](https://experienceleague.adobe.com/pt-br/docs/experience-platform/ai-assistant/home) e os tipos de prompts baseados em objetivos para aproveitar ao máximo o Assistente de IA.

## Aplicativos Experience Cloud que usam IA

>[!TIP]
>
>Versão do subtítulo (apenas um início)...


* [Adobe GenStudio for Performance Marketing](#gspm)
* [Adobe Experience Manager Sites (Cloud Service)](#aem-sites)
* [Adobe Journey Optimizer](#journey-optimizer)
* [ADOBE JOURNEY OPTIMIZER PRIME e ULTIMATE](#ajo-prime-ultimate)

### GenStudio para marketing de desempenho {#gspm}

[GenStudio for Performance Marketing](https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/home) é uma plataforma gerativa orientada por IA. Ele integra o ciclo de vida da criação de conteúdo aos recursos de IA gerativa que transformam a forma como o conteúdo de marketing é criado, revisado, compartilhado e analisado.

O _GenStudio for Performance Marketing Create_ aproveita o potencial do Adobe GenAI para capacitar profissionais de marketing e equipes distribuídas a criar experiências de alto desempenho na marca. Gerar conteúdo para:

* Emails
* Meta ads
* Anúncios do LinkedIn
* Exibir anúncios
* Banners

Você pode treinar a GenStudio for Performance Marketing em sua marca usando exemplos, descrições de personas e produtos de clientes e diretrizes de marca. [Saiba mais.](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview)

**Compatibilidade com o Adobe Firefly:** planejada

### Experience Manager Sites {#aem-sites}

O AEM Sites usa [Gerar Variações](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations). Gerar variações usa IA gerativa para criar variações de conteúdo com base em prompts. Esses prompts são fornecidos por [Adobe Systems](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#get-started) ou criados e gerenciados pelos [usuários](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#create-prompt).

Depois de criar variações, você pode usar o conteúdo em seu site e medir seu sucesso usando a funcionalidade Experimentação do Edge Delivery Services.

**Entrada:** Os campos de entrada incluem:

* Número de variações a serem geradas
* Audience Source
* Target do público-alvo
* Contexto adicional
* Prompts orientados pelo cliente

**Output:** conteúdo gerado/ Cópia de mercado. Você também tem a opção de gerar imagens no Adobe Systems Express usando as capacidades generativas de IA do Firefly.

Consulte [Gerar Imagem](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#generate-image).

**Compatibilidade com o Adobe Firefly:** Sim

## Journey Optimizer {#journey-optimizer}

O Journey Optimizer usa o [Assistente de IA](https://experienceleague.adobe.com/pt-br/docs/experience-platform/ai-assistant/home) com duas classes de perguntas:

**Conhecimento sobre o produto** - Consulta armazenamentos de dados da Adobe (como a documentação do produto da Experience League) para o insight do produto. Essa saída é independente do cliente. Exemplo:

* Quantas atividades ativas posso ter em uma sandbox da Adobe Journey Optimizer?

**Insights Operacionais (Beta)** - consulta um repositório de dados de insights operacionais específicos do cliente que contém dados operacionais centralizados sobre o Jornada, particionados pela sandbox do cliente. Extrai metadados somente de objetos comerciais e não acessa dados na sandbox.

* Quantas Jornadas foram criadas nos últimos sete dias?

A saída dos Insights operacionais depende dos metadados extraídos dos objetos comerciais do cliente.

O Jornada é o único objeto disponível para o Assistente de IA no Journey Optimizer e os metadados são obtidos da sandbox atual.

Consulte [Trabalhar com o Assistente de IA](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant) e [Disponibilidade do campo](https://fieldreadiness-adobe.highspot.com/items/6661f1c132683fd5e6a8adf4?lfrm=srp.1#11) para obter mais informações.

**Compatibilidade com Adobe Systems Firefly:** Não

## Journey Optimizer Prime e Ultimate {#ajo-prime-ultimate}

O Journey Optimizer Prime e o Ultimate usam [o Assistente de IA para acelerador](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative) de conteúdo para trazer sugestões proativas conteúdo variações para texto e imagens.

Esse recurso está disponível para canais email, push, Web e SMS. Ele fornece geração de texto e imagem com base em prompt.

**Email** : gere um email, texto ou apenas uma imagem completo. [Saiba mais...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-email)

**Notificação por push** - Gere uma notificação por push completa, somente texto ou somente imagem. [Saiba mais...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-push)

**SMS** - Gere um SMS completo ou somente texto. [Saiba mais](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-sms)

**Página da Web** - Gerar imagens ou texto de página da Web. [Saiba mais...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-web)

**Conteúdo** - Gerar conteúdo para várias campanhas de mensagens. [Saiba mais...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-experimentation)

**Observação:** a saída do Acelerador de Conteúdo no AJO Prime e no Ultimate é indenizada.

**Compatibilidade com o Adobe Firefly:** Sim

## Journey Optimizer edição B2B {#ajo-b2b}

Usa o [Assistente de IA](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant) para obter prompts de conhecimento do produto.

**Conhecimento sobre o produto** - Consulta armazenamentos de dados da Adobe (como a documentação do produto da Experience League) para o insight do produto. Essa saída é independente do cliente. | <ul><li>**Entrada:** Como faço para enviar um email em uma jornada de conta?</li><li>**Saída:** o Conhecimento do Produto é extraído do Experience League (documentação pública). [Saiba mais...](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant)</li></ul>   | Não   |

## Aplicativos Experience Cloud que usam IA

>[!TIP]
>
>Versão da tabela...


Saiba como os aplicativos do Experience Cloud usam o assistente de IA ou o assistente de IA generativo e se o Adobe Firefly é compatível.

| Aplicativo | Como a IA gerativa é usada | Exemplos | Adobe Firefly? |
|----------|------------|-----------|----------------|
| GenStudio para marketing de desempenho | [GenStudio for Performance Marketing](https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/home) é uma plataforma gerativa orientada por IA. Ele integra o ciclo de vida da criação de conteúdo aos recursos de IA gerativa que transformam a forma como o conteúdo de marketing é criado, revisado, compartilhado e analisado.<br>Você pode treinar a GenStudio for Performance Marketing na sua marca usando exemplos, descrições de personas e produtos de clientes e diretrizes de marca. | O _GenStudio for Performance Marketing Create_ permite gerar conteúdo para emails, Meta ads, anúncios do LinkedIn, anúncios de exibição e banners. <br>**Entradas:** <ul><li>Use modelos para iniciar o processo de criação de conteúdo. </li><li>Adicione parâmetros como Marcas, Produtos e Personalidades (diretrizes) e Conteúdo (ativos) para modelar a experiência gerada. </li><li>Insira prompts descritivos que descrevam o contexto ou a experiência que você pretende gerar. [Saiba mais...](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview)</li></ul> | Sim |
| Adobe Experience Manager Sites (Cloud Service) | O AEM Sites usa [Gerar Variações](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations). <br>Gerar variações usa IA generativa para criar conteúdo variações com base em prompts. Esses prompts são fornecidos pela Adobe ou criados e gerenciados pelos usuários. | Depois de criar variações, você pode usar o conteúdo em seu site e medir seu sucesso usando a funcionalidade Experimentação do Edge Delivery Services. <br>**Entrada:** Os campos de entrada incluem Número de Variações a serem geradas; Source de Público-alvo/Público-alvo; Contexto Adicional e prompts orientados pelo cliente. <ul><li>[Modelo de prompt do Adobe](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#get-started) </li><li>[Prompt gerado pelo usuário](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#create-prompt)</li></ul> **Output:** conteúdo gerado/ Cópia de mercado. Você também tem a opção de gerar imagens no Adobe Systems Express usando as capacidades generativas de IA do Firefly. Consulte [Gerar Imagem](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#generate-image). | Sim |
| Adobe Journey Optimizer | O Journey Optimizer usa o [Assistente de IA](https://experienceleague.adobe.com/pt-br/docs/experience-platform/ai-assistant/home) com duas classes de perguntas:<ul><li>**Conhecimento sobre o produto** - Consulta armazenamentos de dados da Adobe (como a documentação do produto da Experience League) para o insight do produto. Essa saída é independente do cliente. </li><li>**Insights Operacionais (Beta)** - consulta um repositório de dados de insights operacionais específicos do cliente que contém dados operacionais centralizados sobre o Jornada, particionados pela sandbox do cliente. Extrai metadados somente de objetos comerciais e não acessa dados na sandbox.</li></ul> | <ul><li>**Entrada de Conhecimento do Produto:** Quantas atividades ativas posso ter em uma sandbox da Adobe Journey Optimizer?</li><li>**Saída de Conhecimento do Produto:** Extração de Conhecimento do Produto da Experience League (documentação pública). </li><li>**Entrada de Insights Operacionais:** Quantas Jornadas foram criadas nos últimos sete dias? </li><li>**Saída dos Insights Operacionais:** a saída dos Insights Operacionais depende dos metadados obtidos dos objetos comerciais do cliente. O Jornada é o único objeto disponível no AJO e os metadados são obtidos da sandbox atual. </li></ul> Consulte [Trabalhar com o Assistente de IA](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant) e [Disponibilidade do campo](https://fieldreadiness-adobe.highspot.com/items/6661f1c132683fd5e6a8adf4?lfrm=srp.1#11) | Não |
| Journey Optimizer: _Prime_ e _Ultimate_ | O [Assistente de IA para Acelerador de Conteúdo](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative) oferece sugestões de variação de conteúdo pró-ativo para texto e imagens. Ele está disponível para canais de email, push, Web e SMS. Esse novo recurso oferece geração de texto e imagem com base em prompt. | <ul><li> **Email** : gere um email, texto ou apenas uma imagem completo. [Saiba mais...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-email) </li><li> **Notificação** por push - Gere uma notificação de push completa, somente texto ou imagem. [Saiba mais...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-push) </li><li> **SMS** - Gere um SMS completo ou somente texto. [Saiba mais](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-sms) </li><li> **Página da Web** - Gerar imagens ou texto de página da Web. [Saiba mais...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-web) </li><li> **Conteúdo** - Gerar conteúdo para várias campanhas de mensagens. [Saiba mais...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-experimentation)</li></ul> **Observação:** a saída do Acelerador de Conteúdo no AJO Prime e no Ultimate é indenizada. | Sim |
| Journey Optimizer edição B2B | Usa o [Assistente de IA](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant) com uma classe de perguntas: <br> **Conhecimento sobre o produto** - Consulta armazenamentos de dados da Adobe (como a documentação do produto da Experience League) para o insight do produto. Essa saída é independente do cliente. | <ul><li>**Entrada:** Como faço para enviar um email em uma jornada de conta?</li><li>**Saída:** o Conhecimento do Produto é extraído do Experience League (documentação pública). [Saiba mais...](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant)</li></ul> | Não |
| Cloud Services gerenciados pelo Campaign | O [Assistente de IA para Acelerador de Conteúdo](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-gs) gera automaticamente conteúdo personalizado, envolvente e eficaz com base no objetivo de marketing, com conteúdo otimizado para estilos, layouts, tons e muito mais em canais como email, SMS e push. | <ul><li> **Email** - Gerar um email completo, somente texto ou somente imagem. [Saiba mais](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-content) </li><li> **SMS** - Gerar somente SMS completo ou texto. [Saiba mais...](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-sms) </li><li> **Push** - Criar mensagens atraentes e gerar conteúdo. [Saiba mais...](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-push) </li></ul> **Observação:** a saída do Acelerador de Conteúdo no Campaign Managed Cloud Services é indenizada. | Sim |
| Customer Journey Analytics | O CJA usa o [Assistente de IA](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant) para ajudar você a descobrir o conhecimento e os insights do produto no Experience League. <br>Por exemplo, novos usuários podem usá-lo para aprender conceitos do Customer Journey Analytics e se integrar a produtos e recursos com os quais você não está familiarizado. <br>Usuários experientes podem usar o AI Assistant para apresentar casos de uso mais avançados ou dicas e truques e executar tarefas em um ritmo mais rápido. Entenda conceitos, solucione problemas ou pesquise informações. [Saiba mais...](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant#knowledge) | <ul><li>**Entrada de Conhecimento do Produto:** Como criar uma métrica calculada? </li><li> **Saída de Conhecimento do Produto:** Extração de Conhecimento do Produto da Experience League (documentação pública). </li></ul> | Não |
| Customer Journey Analytics | [Legendas inteligentes](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions) fornecem insights de linguagem natural para visualizações de linha em visualizações Workspace. | <ul><li>**Entrada:** visualizações de linha. As legendas são geradas automaticamente com base nessas visualizações de linha quando você clica em **Legendas inteligentes**. </li><li> **Saída:** Legendas de linguagem natural geradas automaticamente.</li></ul> | Não |
| Real-Time CDP | Usa o [Assistente de IA](https://experienceleague.adobe.com/pt-br/docs/experience-platform/ai-assistant/home) para ajudá-lo a descobrir conhecimentos e insights sobre produtos da Experience League. Ele consulta um banco de dados e traduz os dados do banco de dados em uma resposta legível. Duas classes de perguntas: <br> **Conhecimento sobre o produto** - Consulta armazenamentos de dados da Adobe (como a documentação do produto da Experience League) para o insight do produto. Essa saída é independente do cliente. <br> **Insights Operacionais (Beta)** - Consulta um repositório de dados de insights operacionais específicos do cliente que contém dados operacionais centralizados, particionados pela sandbox da AEP do cliente. Extrai metadados somente de Atributos, Públicos-alvo, Fluxos de dados, Conjuntos de dados, Destinos, Esquemas e Fontes, e não acessa dados na sandbox. <br>Por exemplo, para uma consulta sobre uma audiência, [!DNL AI Assistant] pode acessar o nome da audiência e outros metadados associados, mas não pode acessar os perfis dessa audiência. | <ul><li>**Entrada de Conhecimento do Produto:** Como é calculada a riqueza do perfil? </li><li>**Saída de Conhecimento do Produto:** Extração de Conhecimento do Produto da Experience League (documentação pública). </li><li> **Entrada de Insights Operacionais:** Quantos conjuntos de dados eu tenho? </li><li> **Saída dos Insights Operacionais:** a saída dos Insights Operacionais depende dos metadados obtidos dos objetos comerciais do Cliente (Atributos, Públicos, Fluxos de Dados, Conjuntos de Dados, Destinos, Esquemas e Fontes) e inclui um link para uma página de interface do usuário específica contendo os dados consultados. </li></ul>Para obter exemplos, consulte as tabelas de entrada _Conhecimento do Produto_ e _Insights Operacionais_ no [Assistente de IA no Experience Platform](https://experienceleague.adobe.com/pt-br/docs/experience-platform/ai-assistant/home) | Não |
| Marketo | O [Dynamic Chat](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview) cria conversas assistidas por IA com perguntas e respostas personalizadas e pré-aprovadas, bem como um resumo da conversa | <ul><li> **Gerar Perguntas** Forneça URLs das quais o conteúdo é extraído e usado para gerar perguntas/respostas. </li><li> **Resumo da Conversa:** gera um resumo de uma conversa de chat. </li></ul> [Saiba mais...](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/response-library) | Não |
| Workfront | O [Assistente de IA](https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview) do Workfront ajuda você a realizar seu trabalho, oferecendo informações e sugestões no aplicativo em uma conversa em idioma natural. O AI Assistant oferece a seguinte funcionalidade: resume projetos/tarefas/problemas/documentos, fornece instruções ou informações de referência extraídas da documentação do Workfront no Experience League, gera ou refina fórmulas para campos personalizados calculados. | <ul><li>**Resumir a Entrada do Projeto:** Resuma este projeto </li><li> **Resumir Output do projeto:** Retorna breves descrições da finalidade e status do projeto, fornece exemplos de tarefas que estão concluídas e que ainda estão pendentes, além de fornecer alguns detalhes e observações adicionais.</li><li> **Entrada de fórmula gerar/refinar:** &quot;Reescreva essa fórmula para remover o inválido expressão erro&quot;. </li><li> **Gerar/refinar o Output fórmula:** fórmula gerada ou refinada. </li></ul>**Observação:** o Assistente de IA pode levar alguns momentos para gerar a fórmula revisada, dependendo do tamanho e da complexidade da fórmula. | Não |
