---
title: IA em aplicativos da Experience Cloud
description: Saiba mais sobre a IA gerativa e como os aplicativos do Experience Cloud usam a genAI e o  [!DNL AI Assistant].
solution: Experience Cloud
feature: AI Assistant, Generative AI
topic: Administration
role: Admin
level: Intermediate
exl-id: bdc51956-82aa-4aae-b627-a2018f80b5f5
source-git-commit: c97ace2c192517a49a01c4247d9f6b4220e0514d
workflow-type: tm+mt
source-wordcount: '1103'
ht-degree: 3%

---

# IA em produtos da Experience Cloud

Esta página ajuda você a saber quais produtos oferecem suporte à IA gerativa [!DNL AI Assistant] e se o Adobe Firefly é compatível. Você também pode encontrar links para recursos de ajuda específicos do produto sobre como usar a IA no Experience Cloud.

**Sobre a IA de geração**

A IA gerativa é um tipo de inteligência artificial que faz mais do que simplesmente responder a perguntas. Ele pode _criar_ conteúdo e _gerar uma resposta_ para suas perguntas ou instruções (conhecidos como _prompts_).

* **Crie:** a capacidade da IA de gerar conteúdo (texto, imagens, música ou vídeos) do zero, com base em seu treinamento e prompts de entrada. Esta habilidade é o aspecto _gerativo_ da IA gerativa.

* **Gerar uma resposta:** a IA está fornecendo uma resposta ou reação a um prompt, normalmente com base em seus dados disponíveis e repositórios de conhecimento.

Com a IA gerativa, você pode obter conhecimento sobre o produto rapidamente se for novo no Experience Cloud. Usuários experientes podem descobrir insights operacionais em segundos em vez de horas.

**O que é [!DNL AI Assistant]?**

[!DNL AI Assistant] é uma ferramenta conversacional com suporte no Experience Platform e em aplicativos relacionados. Esses aplicativos o usam de forma semelhante, mas com vantagens específicas do produto. Use-o para acelerar seus workflows, melhorar o conhecimento sobre produtos, solucionar problemas ou pesquisar informações e encontrar insights operacionais. Em certos aplicativos, o [!DNL AI Assistant] permite que você descubra insights operacionais imediatamente.

**Conhecimento do Produto:** o conhecimento do produto refere-se a conceitos e tópicos com base na documentação do Experience League. As respostas do Experience League são verificáveis e citadas com links. Saiba mais sobre os tipos de [prompts baseados em objetivos](https://experienceleague.adobe.com/pt-br/docs/experience-platform/ai-assistant/home) para aproveitar ao máximo o [!DNL AI Assistant].

**Insights Operacionais:** os insights operacionais se referem às respostas que o Assistente de IA gera sobre os objetos de metadados (atributos, públicos, fluxos de dados, conjuntos de dados, destinos, jornadas, esquemas e fontes), incluindo contagens, pesquisas e impacto de linhagem.

[Saiba mais](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/landing)

<!-- **Your data remains yours**

In AI Assistant, security is the priority:

* Customer data is not used to train language models.
* AI Assistant looks at only the documents that you tell it to. You are in control.
* Your people can use AI Assistant only on documents they can access.
* It's audit-ready: Responses are attributable to source documents.
* Enterprise controls are in place to manage who has AI access in the company. -->

## Disponibilidade de IA em produtos da Experience Cloud

Saiba mais sobre o suporte para IA gerativa ou [!DNL AI Assistant] em produtos da Experience Cloud e se há suporte para o Adobe Firefly.

* [[!DNL GenStudio for Performance Marketing]](#gspm)
* [[!DNL Experience Manager Sites]](#aem-sites)
* [[!DNL Journey Optimizer]](#journey-optimizer)
* [[!DNL Journey Optimizer] Prime e Ultimate](#ajo-prime-ultimate)
* [B2B edition [!DNL Journey Optimizer]](#ajo-b2b)
* [Interface do usuário da Web do [!DNL Campaign] v8](#campaign-cs)
* [[!DNL Customer Journey Analytics]](#cja)
* [[!DNL Customer Journey Analytics]](#cja-captions)
* [[!DNL Real-Time CDP]](#rtcdp)
* [[!DNL Marketo]](#marketo)
* [[!DNL Workfront]](#workfront)

## GenStudio para marketing de desempenho {#gspm}

O [!DNL GenStudio for Performance Marketing] é uma plataforma orientada por IA que permite gerar e gerenciar conteúdo de marketing que segue os padrões da sua marca e está em conformidade com as políticas da empresa. Gere conteúdo para emails, Meta anúncios, anúncios do LinkedIn, anúncios de exibição e banners.

Você também pode treinar a GenStudio for Performance Marketing em sua marca usando exemplos, descrições de personas e produtos do cliente e diretrizes de marca.

[Saiba mais](https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/home)

Compatibilidade com o Adobe Firefly: **Sim**

## [!DNL Experience Manager Sites] {#aem-sites}

No AEM Sites, você pode usar [!UICONTROL Gerar Variações] para criar variações de conteúdo com base em prompts. Esses prompts são fornecidos pela Adobe ou criados e gerenciados por você.

Depois de criar variações, você pode usar o conteúdo em seu site e medir seu sucesso usando o recurso Experimentação no Edge Delivery Services. Você também tem a opção de gerar imagens no Adobe Express usando os recursos de IA geradores do Firefly.

[Saiba mais](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations-integrated-editor)

Compatibilidade com o Adobe Firefly: **Sim**

## [!DNL Journey Optimizer] {#journey-optimizer}

Em [!DNL Journey Optimizer], use o [!DNL AI Assistant] para obter conhecimento sobre o produto e insights operacionais. Por exemplo, pergunte _Quantas atividades online posso ter em uma sandbox da Journey Optimizer?_ Você receberá imediatamente sua resposta do Experience League e de outros armazenamentos de dados da Adobe.

[!DNL AI Assistant] também ajuda com insights operacionais (beta). Por exemplo, você pode saber rapidamente quantas Jornadas foram criadas nos últimos sete dias.

Para insights operacionais, [!DNL AI Assistant] consulta um armazenamento de dados específico do cliente. O repositório de dados contém dados operacionais e centralizados sobre [!UICONTROL Jornada]. Esse recurso é independente do cliente e extrai metadados somente de objetos de negócios. Ele não acessa dados na sandbox.

[Saiba mais](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant).

Compatibilidade com o Adobe Firefly: **Não**

## [!DNL Journey Optimizer] Prime e Ultimate {#ajo-prime-ultimate}

O [!DNL Journey Optimizer] Prime e o Ultimate usam o [!DNL AI Assistant] para geração de conteúdo, a fim de oferecer sugestões proativas de variação de conteúdo para texto e imagens.

Esse recurso está disponível para email, notificações por push, página da Web, conteúdo e canais SMS. Ele fornece geração de texto e imagem com base em prompt. A saída da geração de conteúdo no AJO Prime e no Ultimate é indenizada.

[Saiba mais](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative)

Compatibilidade com o Adobe Firefly: **Sim**

## [!DNL Journey Optimizer B2B Edition] {#ajo-b2b}

O Journey Optimizer B2B edition usa o [!DNL AI Assistant] para ajudá-lo com o conhecimento do produto.

[Saiba mais](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/ai-assistant/ai-assistant-overview)

Compatibilidade com o Adobe Firefly: **Não**

## Interface do usuário da Web do [!DNL Campaign] v8 {#campaign-cs}

O Campaign Managed Cloud Services usa [!DNL AI Assistant] para geração de conteúdo. Esse recurso permite gerar automaticamente conteúdo personalizado, envolvente e eficaz com base em seu objetivo de marketing, com conteúdo otimizado para estilos, layouts, tons e muito mais. Você pode usá-lo em canais como email, SMS e push.

**Observação:** a saída da geração de conteúdo no Campaign Managed Cloud Services é indenizada.

[Saiba mais](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-gs)

Compatibilidade com o Adobe Firefly: **Sim**

## [!DNL Customer Journey Analytics] {#cja}

O Customer Journey Analytics usa o [!DNL AI Assistant] para ajudar você a descobrir o conhecimento e os insights do produto no Experience League. Se você for um novo usuário, aprenda rapidamente os conceitos do Customer Journey Analytics e integre-se aos produtos e recursos.

Usuários experientes obtêm casos de uso avançados ou aprendem estratégias para executar tarefas em um ritmo rápido. Entenda conceitos, solucione problemas ou pesquise informações.

[Saiba mais](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/cja-b2c-overview/ai-assistant)

Compatibilidade com o Adobe Firefly: **Não**

## [!DNL Customer Journey Analytics] {#cja-captions}

Você pode usar as _Legendas inteligentes_ no [!DNL Customer Journey Analytics] para obter insights de linguagem natural para as visualizações do Workspace usadas com mais frequência. As legendas inteligentes são ideais para analistas que precisam de narrativas e contexto para compartilhar com outros usuários. Os usuários empresariais podem usá-lo para descobrir rapidamente os principais pontos de partida.

Por exemplo:

* **Entrada:** no CJA, execute uma visualização com suporte (incluindo Linha, Área, Gráfico de barras, Fluxo ou Fallout) e clique em **[!UICONTROL Legendas inteligentes]**.

* **Saída:** Exibir legendas geradas automaticamente em linguagem natural mostrando contexto e principais argumentos. Em seguida, é possível realizar ações nos dados gerados, como revisar, copiar e compartilhá-los com sua organização. [Veja como](https://video.tv.adobe.com/v/3420131/?quality=12&learn=on#_blank)

[Saiba mais](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions)

Compatibilidade com o Adobe Firefly: **Não**

## [!DNL Real-Time CDP] {#rtcdp}

A Real-Time CDP usa o [!DNL AI Assistant] para ajudá-lo com o conhecimento do produto da Experience League. Ele também oferece insights operacionais (em beta). O [!DNL AI Assistant] consulta um repositório de dados de insights operacionais específicos do cliente que contém dados operacionais centralizados, particionados em sua sandbox da AEP. O sistema extrai metadados somente de Atributos, Públicos-alvo, Fluxos de dados, Conjuntos de dados, Destinos, Esquemas e Fontes e não acessa dados na sandbox.

Por exemplo, se você consultar sobre um público-alvo, [!DNL AI Assistant] pode acessar o nome do público-alvo e outros metadados associados, mas não pode acessar os perfis desse público-alvo.

[Saiba mais](https://experienceleague.adobe.com/pt-br/docs/experience-platform/ai-assistant/home)

Compatibilidade com o Adobe Firefly: **Não**

## [!DNL Marketo] {#marketo}

Os recursos alimentados por IA gerativa no Adobe Dynamic Chat permitem otimizar a produtividade de seus agentes de vendas, obter insights sobre a intenção de visitante do site e responder às perguntas do visitante de maneira segura. Você pode pré-aprovar as perguntas, as respostas e o resumo da conversa.

[Saiba mais](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/overview)

Compatibilidade com o Adobe Firefly: **Não**

## [!DNL Workfront] {#workfront}

O [!DNL AI Assistant] no [!DNL Workfront] ajuda você a realizar seu trabalho oferecendo informações e sugestões no aplicativo. É possível:

* Obtenha resumos de alguns objetos, fornecendo uma exibição de alto nível da intenção ou dos detalhes do objeto.
* Faça perguntas e deixe [!DNL AI Assistant] encontrar respostas no Experience League.
* Obtenha fórmulas geradas com base em seus prompts. Você também pode resolver erros em suas expressões personalizadas inválidas em campos calculados.
* Localize projetos, tarefas e problemas.

[Saiba mais](https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview)

Compatibilidade com o Adobe Firefly: **Não**
