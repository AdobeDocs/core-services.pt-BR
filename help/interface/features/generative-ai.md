---
title: IA gerada em aplicativos Experience Cloud
description: Saiba mais sobre a IA gerativa (GenAI) e como os aplicativos da Experience Cloud usam a GenAI e o [!UICONTROL Assistente de IA].
solution: Experience Cloud
feature: AI Assistant, Generative AI
topic: Administration
role: Admin
level: Intermediate
exl-id: bdc51956-82aa-4aae-b627-a2018f80b5f5
source-git-commit: 2e8ce339aaf3d90b7ee6da2cdec1565c88513e3d
workflow-type: tm+mt
source-wordcount: '1788'
ht-degree: 3%

---

# IA gerada em produtos da Experience Cloud

A IA gerativa (genAI) no Experience Cloud ajuda a automatizar tarefas criativas e cognitivas e melhorar a produtividade. Esta página descreve onde os aplicativos do Experience Cloud oferecem suporte ao genAI e ao Assistente de IA, e fornece links para saber mais sobre esses recursos.

**O que é genAI?**

A IA gerativa é um tipo de IA que pode criar conteúdo original. Por exemplo, ele pode criar texto, imagens, vídeo, áudio ou código de software em resposta ao prompt ou solicitação de um usuário.

* **Criar:** a capacidade de gerar conteúdo (texto, imagens, música ou vídeos) do zero, com base em seu treinamento e prompts de entrada. Esta habilidade é o aspecto _gerativo_ da IA gerativa.

* **Gerar uma resposta:** A IA fornece uma resposta ou reação a um prompt, normalmente com base em seus dados disponíveis e repositórios de conhecimento.

**O que é o [!UICONTROL Assistente de IA]?**

O [!UICONTROL Assistente de IA] é uma ferramenta conversacional com suporte no Experience Platform e em aplicativos relacionados. Use-o para obter rapidamente _conhecimento sobre o produto_ e _insights operacionais_ sobre os produtos suportados.

* **Conhecimento do produto:** o conhecimento do produto refere-se a conceitos e tópicos com base na documentação do Experience League. Saiba como criar [prompts efetivos e baseados em objetivos](https://experienceleague.adobe.com/pt-br/docs/experience-platform/ai-assistant/home) para aproveitar ao máximo o [!UICONTROL Assistente de IA]. Todas as respostas do Experience League são verificáveis e citadas com links.

* **Insights operacionais:** [Os insights operacionais](https://experienceleague.adobe.com/pt-br/docs/experience-platform/ai-assistant/questions#objects-questions) referem-se a respostas geradas sobre seus objetos de metadados (atributos, públicos, fluxos de dados, conjuntos de dados e assim por diante). Com o [!UICONTROL Assistente de IA], você pode concluir em segundos o que, de outra forma, poderia levar horas ou dias.

O Assistente de IA também inclui recursos de IA de agente de conversa (conhecidos como _IA de agente_) nos aplicativos compatíveis:

* **Suporte ao produto:** O [Agente de Suporte ao Produto](https://experienceleague.adobe.com/pt-br/docs/experience-platform/ai-assistant/new-features/customer-support) é um recurso de depuração de autoatendimento e solução de problemas do [!UICONTROL Assistente de IA] que você pode usar para recursos e aplicativos do Experience Platform. Solucione problemas de suporte sem sair dos workflows, crie tíquetes de suporte ao cliente e rastreie o progresso do caso usando o Assistente de IA.

[Saiba mais sobre o Assistente de IA](https://experienceleague.adobe.com/pt-br/docs/experience-platform/ai-assistant/landing)

## Disponibilidade do GenAI em produtos da Experience Cloud {#products}

Os aplicativos do Experience Cloud a seguir oferecem suporte à IA gerativa ou ao [!UICONTROL Assistente de IA]. O suporte para Adobe Firefly também é indicado por produto.

Atualizado em: **9 de junho de 2025**

* [[!DNL GenStudio for Performance Marketing]](#gspm)
* [[!DNL Experience Manager]](#aem)
* [[!DNL Journey Optimizer]](#journey-optimizer)
* [B2B edition [!DNL Journey Optimizer]](#ajo-b2b)
* [[!DNL Campaign] Managed Cloud Services](#campaign-cs)
* [[!DNL Customer Journey Analytics]](#cja)
* [[!DNL Real-Time CDP]](#rtcdp)
* [[!DNL Marketo]](#marketo)
* [[!DNL Workfront]](#workfront)

## GenStudio para marketing de desempenho {#gspm}

O [!DNL GenStudio for Performance Marketing] é um aplicativo de IA gerativa projetado para ajudar as equipes de marketing empresariais a criar, ativar e otimizar conteúdo de campanha online em canais como mídia paga, email e anúncios de exibição.

Os profissionais de marketing de desempenho podem usar prompts de linguagem natural para gerar ativos personalizados e compatíveis com a marca. O GenStudio for Performance Marketing acelera a execução da campanha, dimensiona a produção de conteúdo sem comprometer a integridade da marca e fornece análises de desempenho para melhorar o ROI geral.

[Saiba mais](https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/home)

Compatibilidade com o Adobe Firefly: **Sim**

## [!DNL Experience Manager] {#aem}

As seções a seguir descrevem brevemente a IA gerativa em aplicativos do AEM.

### Experience Manager Sites

No AEM Sites, você pode usar _[!UICONTROL Gerar Variações]_. Esse recurso usa inteligência artificial geradora para criar variações de conteúdo com base nos prompts de entrada. Os prompts são fornecidos pela Adobe ou criados e gerenciados por você.

Depois de criar variações, você pode usar o conteúdo no seu site e medir seu sucesso usando o recurso [Experimentação](https://www.aem.live/docs/experimentation) no Edge Delivery Services. Você também tem a opção de gerar imagens no Adobe Express usando os recursos de IA geradores do Firefly.

**Exemplos de entrada e saída**

Os campos de entrada incluem:

* Número de variações a serem geradas
* Audience Source
* Público-alvo
* Contexto adicional
* Solicitações orientadas pelo cliente

A saída é conteúdo gerado ou cópia de mercado.

Compatibilidade com o Adobe Firefly: **Sim**

[Saiba mais](https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/generative-ai/generate-variations-integrated-editor)

### Sites Optimizer {#sites-optimizer}

O AEM Sites Optimizer usa IA gerativa para analisar e melhorar o desempenho e a eficácia das experiências da Web. Esses insights estão agrupados nas principais áreas de oportunidade: Envolvimento, Aquisição de tráfego, Postura de segurança e Integridade do site. Cada categoria destaca maneiras específicas de aprimorar o site, seja aumentando a interação do visitante, melhorando a descoberta, fortalecendo a segurança ou mantendo a estabilidade do site. [Saiba mais](https://experienceleague.adobe.com/pt-br/docs/experience-manager-sites-optimizer/content/opportunity-types/overview)

### Experience Manager Assets {#aem-assets}

No AEM Assets, você pode usar IA gerativa em **Content Hub** e **Tags inteligentes geradas por IA**.

Compatibilidade com o Adobe Firefly: **Sim**

**Content Hub**

O [!UICONTROL Content Hub] está disponível como parte do [!DNL Experience Manager Assets as a Cloud Service] para democratizar o acesso a conteúdo sobre a marca para organizações e seus parceiros comerciais. Ele se concentra na distribuição de ativos para ativação em escala e criação de variantes de conteúdo na marca para melhorar a agilidade de marketing.

No Content Hub, você pode criar conteúdo com o Adobe Express (se tiver direitos ao Adobe Express). Você pode editar o conteúdo existente com ferramentas simples, produzir variações na marca com modelos e elementos da marca e criar conteúdo com os recursos mais recentes da GenAI do [!DNL Adobe Firefly]. [Saiba mais](https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/content-hub/product-overview)

**Marcas Inteligentes**

Em vez de depender da entrada manual, a IA pode atribuir tags descritivas automaticamente a ativos digitais. Essas tags geradas por IA melhoram a qualidade dos metadados, tornando os ativos mais fáceis de pesquisar, categorizar e recomendar.

Por exemplo, se o ativo for uma imagem, a IA pode identificar objetos, cenas, emoções ou até mesmo logotipos de marca. Ele pode gerar tags relevantes como _pôr do sol_, _praia_, _férias_ ou _sorrir_. [Saiba mais](https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/manage/smart-tags#ai-smart-tags)

## Adobe [!DNL Journey Optimizer] {#journey-optimizer}

No [!DNL Journey Optimizer] (AJO), você pode usar o [Assistente de IA](https://experienceleague.adobe.com/pt-br/docs/journey-optimizer/using/get-started/ai-assistant) para obter _conhecimento sobre o produto_ e _insights operacionais_ (beta).

### Exemplos de uso do Assistente de IA no AJO

Este é um exemplo de entrada para o conhecimento do produto:

* _Quantas atividades ativas posso ter em uma sandbox da Journey Optimizer?_

  A saída é gerada pelo Experience League e outros armazenamentos de dados da Adobe.

Este é um exemplo de entrada para insights operacionais:

* _Quantas Jornadas foram criadas nos últimos sete dias?_

  Para saída, o Assistente de IA consulta um armazenamento de dados específico do cliente. O repositório de dados contém dados operacionais e centralizados sobre [!UICONTROL Jornada]. Esse recurso é independente do cliente e extrai metadados somente de objetos de negócios. Ele não acessa dados na sandbox.

[Saiba mais](https://experienceleague.adobe.com/pt-br/docs/journey-optimizer/using/get-started/ai-assistant)

Compatibilidade com Adobe Firefly: **Não**

### Assistente de IA para geração de conteúdo (AJO Prime e Ultimate) {#ajo-prime}

No AJO _Prime_ e no _Ultimate_, você pode usar a [geração de conteúdo](https://experienceleague.adobe.com/pt-br/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative) para gerar conteúdo e fornecer sugestões de variação de conteúdo pró-ativo para texto e imagens.

Esse recurso está disponível para email, notificações por push, página da Web, conteúdo e canais SMS. Ele fornece geração de texto e imagem com base em prompt. A saída da geração de conteúdo no AJO Prime e no Ultimate é indenizada.

[Saiba mais](https://experienceleague.adobe.com/pt-br/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative)

Compatibilidade com o Adobe Firefly: **Sim**

## [!DNL Journey Optimizer B2B Edition] {#ajo-b2b}

O Journey Optimizer B2B edition usa o [!UICONTROL Assistente de IA] para ajudá-lo com o conhecimento sobre o produto.

Exemplo de entrada:

* _Como faço para enviar um email em uma jornada de conta?_

  A saída de conhecimento do produto é obtida do Experience League.

[Saiba mais](https://experienceleague.adobe.com/pt-br/docs/journey-optimizer-b2b/user/ai-assistant/ai-assistant-overview)

Compatibilidade com Adobe Firefly: **Não**

## [!DNL Campaign] Managed Cloud Services {#campaign-cs}

O Campaign Managed Cloud Services usa o [!UICONTROL Assistente de IA] para geração de conteúdo. Esse recurso permite gerar automaticamente conteúdo personalizado, envolvente e eficaz com base em seu objetivo de marketing, com conteúdo otimizado para estilos, layouts, tons e muito mais. Você pode usá-lo em canais como email, SMS e push.

**Observação:** a saída da geração de conteúdo no Campaign Managed Cloud Services é indenizada.

[Saiba mais](https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/content/ai-assistant/generative-gs)

Compatibilidade com o Adobe Firefly: **Sim**

## [!DNL Customer Journey Analytics] {#cja}

O Customer Journey Analytics permite usar a IA gerativa ou o Assistente de IA das seguintes maneiras:

* [Assistente de IA](https://experienceleague.adobe.com/pt-br/docs/analytics-platform/using/cja-overview/cja-b2c-overview/ai-assistant) para obter conhecimento sobre o produto.
* [Agente de Suporte ao Produto](https://experienceleague.adobe.com/pt-br/docs/experience-platform/ai-assistant/new-features/customer-support) para criar tíquetes de suporte ao cliente, preenchidos com detalhes de contexto e sessão de suas interações com o Assistente de IA.
* [Data Insights Agent](https://experienceleague.adobe.com/pt-br/docs/analytics-platform/using/cja-overview/cja-b2c-overview/data-analysis-ai) para obter respostas a perguntas sobre seus dados. Ele cria visualizações relevantes no Analysis Workspace usando componentes da visualização de dados e usando seus dados reais.
* [Legendas inteligentes](https://experienceleague.adobe.com/pt-br/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions) para fornecer insights importantes para as visualizações do Workspace usadas com mais frequência em linguagem natural.
* [Content Analytics](https://experienceleague.adobe.com/pt-br/docs/analytics-platform/using/content-analytics/report/report#template) para atribuir todos os metadados de ativos automaticamente.

Compatibilidade com Adobe Firefly: **Não**

**Assistente de IA**

Conheça o produto da Experience League. Se você for um novo usuário, aprenda rapidamente os conceitos do Customer Journey Analytics e integre-se aos produtos e recursos. Por exemplo:

* _Como faço para enviar um email em uma jornada de conta?_

Usuários experientes obtêm casos de uso avançados ou aprendem estratégias para executar tarefas em um ritmo rápido. Você pode entender rapidamente os conceitos, solucionar problemas ou pesquisar informações.

[Saiba mais](https://experienceleague.adobe.com/pt-br/docs/analytics-platform/using/cja-overview/cja-b2c-overview/ai-assistant)

**Legendas inteligentes**

Você pode usar as _Legendas inteligentes_ no [!DNL Customer Journey Analytics] para obter insights de linguagem natural para as visualizações do Workspace usadas com mais frequência. As legendas inteligentes são ideais para analistas que precisam de narrativas e contexto para compartilhar com outros usuários. Os usuários empresariais podem usá-lo para descobrir rapidamente os principais pontos de partida.

Por exemplo:

* **Entrada:** no CJA, execute uma visualização com suporte (incluindo Linha, Área, Gráfico de barras, Fluxo ou Fallout) e clique em **[!UICONTROL Legendas inteligentes]**.

* **Saída:** Exibir legendas geradas automaticamente em linguagem natural mostrando contexto e principais argumentos. Em seguida, é possível realizar ações nos dados gerados, como revisar, copiar e compartilhá-los com sua organização. [Veja como](https://video.tv.adobe.com/v/3443143/?quality=12&learn=on#_blank&captions=por_br)

[Saiba mais](https://experienceleague.adobe.com/pt-br/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions)

**Content Analytics**

O Content Analytics usa IA e GenAI para atribuir todos os metadados de ativos automaticamente, como assuntos, cenas, cores de primeiro plano e assim por diante. Um atributo é uma tag de metadados atribuída pela IA que descreve o que está em um ativo ou experiência.

Por exemplo: primeiro plano `color: red` é um atributo atribuído automaticamente. As visualizações ajudam a identificar quais atributos de seus ativos contribuem mais para a conversão. [Saiba mais](https://experienceleague.adobe.com/pt-br/docs/analytics-platform/using/content-analytics/report/report#template)

## [!DNL Real-Time CDP] {#rtcdp}

A Real-Time CDP usa o [!UICONTROL Assistente de IA] para ajudá-lo com o conhecimento sobre o produto da Experience League. Ele também oferece insights operacionais (em beta). O [!UICONTROL Assistente de IA] consulta um armazenamento de dados de insights operacionais específicos do cliente que contém dados operacionais centralizados, particionados em sua sandbox da AEP. O sistema extrai metadados somente de Atributos, Públicos-alvo, Fluxos de dados, Conjuntos de dados, Destinos, Esquemas e Fontes e não acessa dados na sandbox.

Por exemplo, se você consultar um público-alvo, o [!UICONTROL Assistente de IA] poderá acessar o nome do público-alvo e outros metadados associados, mas não poderá acessar os perfis desse público-alvo.

[Saiba mais](https://experienceleague.adobe.com/pt-br/docs/experience-platform/ai-assistant/home)

Compatibilidade com Adobe Firefly: **Não**

## [!DNL Marketo] {#marketo}

No Marketo, a IA gerativa está disponível em Webinars interativos e no Dynamic Chat.

**Webinars interativos**

Gere capítulos e resumos automaticamente para os webinars gravados, tornando-os mais acessíveis e fáceis de navegar para o público-alvo. Os recursos incluem:

* Geração automática de capítulo
* Resumo de texto gerado por IA
* Conteúdo editável - Modificar capítulos e resumos gerados
* Fácil integração - adicione capítulos e resumos às páginas de aterrissagem copiando o código do HTML para o editor de páginas da Web de sua escolha

[Saiba mais](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/gen-ai)

**Dynamic Chat**

Os recursos alimentados por IA gerativa no Adobe Dynamic Chat permitem otimizar a produtividade de seus agentes de vendas, obter insights sobre a intenção de visitante do site e responder às perguntas do visitante de maneira segura. Você pode pré-aprovar as perguntas, as respostas e o resumo da conversa. O Dynamic Chat inclui uma versão gratuita e uma versão premium.

[Saiba mais](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/overview)

Compatibilidade com Adobe Firefly: **Não**

## [!DNL Workfront] {#workfront}

O [!UICONTROL Assistente de IA] do [!DNL Workfront] ajuda você a realizar seu trabalho oferecendo informações e sugestões no aplicativo. É possível:

* Obtenha resumos de alguns objetos, fornecendo uma exibição de alto nível da intenção ou dos detalhes do objeto.
* Faça perguntas e deixe o [!UICONTROL Assistente de IA] encontrar respostas no Experience League.
* Obtenha fórmulas geradas com base em seus prompts. Você também pode resolver erros em suas expressões personalizadas inválidas em campos calculados.
* Localize projetos, tarefas e problemas.

[Saiba mais](https://experienceleague.adobe.com/pt-br/docs/workfront/using/basics/ai-assistant/ai-assistant-overview)

Compatibilidade com Adobe Firefly: **Não**

## Recursos adicionais

* [Recursos de IA Responsáveis na Central de Confiabilidade](https://www.adobe.com/trust/responsible-ai.html)<!-- * [Customer AI Propensity Scoring Model Card](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/model-cards/ai-model-cards/customer-ai) -->

**Aviso de isenção de responsabilidade:** as informações desta página são somente para fins informativos gerais. Embora sejam feitos esforços para garantir que as informações permaneçam precisas e atuais, os recursos de software e IA gerativa podem mudar com frequência. Portanto, não garantimos a integridade, a precisão ou a confiabilidade das informações em todos os momentos. Verifique todos os detalhes importantes antes de tomar decisões com base nesse conteúdo.

