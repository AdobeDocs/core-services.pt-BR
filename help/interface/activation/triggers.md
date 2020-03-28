---
description: Como configurar o Experience Cloud Triggers.
keywords: integrations;Triggers
seo-description: Como configurar o Experience Cloud Triggers.
seo-title: Triggers
solution: Marketing Cloud
title: Triggers
uuid: dab536e3-1969-4661-919e-5b15f423fecd
translation-type: tm+mt
source-git-commit: 43de353155c640b3ddc519147c94d7e9ffcafe4e

---


# Triggers

## Visão geral do Triggers {#topic_4F21FCE9A64E46E8B6D51F494FA652A7}

*Acionadores* permitem que você identifique, defina e monitore os principais comportamentos do consumidor, em seguida, gere comunicação entre soluções para engajar novamente os visitantes. Você pode usar acionadores em decisões e personalização em tempo real.

* Configure o remarketing rápido para abandonos de carrinho ou abandonos de carrinho com produtos removidos
* Formulários e aplicativos incompletos
* Qualquer ação ou sequência de ações no site

![](assets/trigger-abandonment-2.png)

### Tipos de Triggers

Geralmente, um acionador pode levar 15 a 90 minutos para iniciar uma campanha de marketing. Isso varia dependendo da implementação da coleção de dados, carga no pipeline, configuração personalizada do acionador definido e do fluxo de trabalho no Adobe Campaign.

* **Abandono:** é possível criar um acionador para ser disparado quando um visitante visualizar um produto, mas não fizer adições ao carrinho. Configure [Pontuação de propensão](../activation/triggers.md#concept_A506150674AD45DB98D3CC07E560D334) para entender a tendência dos clientes para não retornar após abandonar um carrinho de compras.
* **Ação:** por exemplo, você pode criar acionadores para serem disparados depois de inscrições em newsletters, assinaturas por email ou aplicações para cartões de crédito (confirmações). Se você for um varejista, crie um acionador para um visitante que se inscreve em um programa de fidelidade. Na mídia e no entretenimento, crie acionadores para visitantes que assistem a um determinado show, e talvez você queira responder com uma pesquisa.
* **Start da sessão e Fim da sessão:** Crie um acionador para o start da sessão e eventos de término da sessão.

## Criar um acionador da Experience Cloud {#task_821F37183AC045E5AC8EED20317598FE}

Crie um acionador de abandono e configure as condições para o acionador e a pontuação de propensão. Por exemplo, você pode especificar o critério das regras para um acionador durante uma visita. Alguns exemplos são métricas, como Abandono de carrinho, ou dimensões, como o nome do produto. Quando as regras são cumpridas, o acionador é executado.

>[!NOTE]
>
>No momento, há um limite técnico de 100 acionadores.

1. Na Experience Cloud, clique em ![](assets/menu-icon.png) e depois em **[!UICONTROL Activation]**.
1. Encontre o cartão [!UICONTROL Triggers] e clique em **[!UICONTROL Inicializar]**.

   ![Resultado da etapa](assets/activation-triggers.png)

1. Clique em **[!UICONTROL Novo acionador]** e especifique o tipo de acionador:

   ![Resultado da etapa](assets/add-trigger.png)

1. Preencha os seguintes campos e arraste métricas e itens de dimensão aos contêineres da regra para configurar o acionador:

   | Elemento | Descrição |
   |--- |--- |
   | Nome | O nome amigável deste acionador. |
   | Descrição | A descrição desse acionador, como você o usará e assim por diante. |
   | Conjunto de relatórios | O conjunto [de](https://docs.adobe.com/content/help/en/analytics/implementation/analytics-basics/ref-reports-report-suites.html) relatórios do Analytics usado para esse acionador. Essa configuração identifica os dados do relatórios a serem usados. |
   | Visit must include<br>Visit must not include<br>Trigger after no action<br>Include meta data | Você pode definir critérios ou comportamentos de usuário que você deseja que ocorram, além de comportamentos que você não deseja que ocorram.  Por exemplo, as regras para um acionador de um simples abandono de carrinho de compras podem ser:<ul><li>A visita deve incluir: Adição ao carrinho (métrica) e Existe. (Mais tarde, você pode redefinir a regra com uma visualização de produto específica ou dimensões como Tipos de navegador.)</li><li>A visita não deve incluir: Check-out.</li><li>Acionar depois de nenhuma ação por: 10 minutos.</li><li>Incluir metadados: permite que você adicione uma dimensão de Campanha específica ou variáveis relevantes ao comportamento do visitante. Este campo pode ser útil ao criar o email de remarketing correto no Adobe Campaign.</li></ul><br>Você pode especificar a lógica Qualquer, E ou Ou dentro ou entre contêineres, dependendo dos critérios que determinar que são importantes para a regra. |
   | Container | Nos contêineres você pode configurar e armazenar regras, condições ou filtros que definem um acionador. Se você desejar que eventos sejam executados ao mesmo tempo, coloque-os no mesmo contêiner. Ou seja, cada contêiner é processado de maneira independente no nível da ocorrência.  Por exemplo, se você tiver dois contêineres unidos pelo operador E, poderá esperar que as regras se qualifiquem quando duas ocorrências atenderem aos requisitos. |
   | Start de nova sessão após | Crie um acionador para o start da sessão e eventos de término da sessão. |

1. (Optional) In [!UICONTROL Abandonment triggers], you can apply [Propensity Scoring](../activation/triggers.md#concept_A506150674AD45DB98D3CC07E560D334).

   ![Resultado da etapa](assets/propensity-scoring.png)

1. Clique em **[!UICONTROL Salvar]**.
1. Use triggers for [real-time remarketing](https://docs.campaign.adobe.com/doc/standard/en/EMA_Transactional_messaging_Marketing_Cloud_Triggers.html) in [!DNL Adobe Campaign].

### Exemplos de acionadores

Exemplos de acionadores da Experience Cloud:

#### Acionador de abandono do carrinho

Por exemplo, a página a seguir mostra regras que você pode usar para um acionador de Abandono de carrinho, com base em produtos exibidos durante uma visita.

![](assets/abandonment-trigger.png)

#### Quem indicou acionadora

O acionador a seguir é disparado quando uma ocorrência acompanhar o produto de Botas masculinas e um referenciador do Facebook. Para que os dois critérios ( *produtos* e *referenciador*) sejam avaliados na mesma ocorrência, eles devem ser adicionados ao mesmo container.

![](assets/fb-boots-promo.png)

## Pontuação de propensão {#concept_A506150674AD45DB98D3CC07E560D334}

Saiba mais sobre a probabilidade de retorno de um cliente após abandonar um carrinho de compras. A pontuação de propensão é integrada ao Experience Cloud Triggers e disponível para acionadores de Abandono.

![Resultado da etapa](assets/propensity-scoring.png)

Por exemplo, alguns clientes abandonam carrinhos de compras para tirar usufruir de emails de incentivo para retornarem ao carrinho. Para reduzir a perda de receita, o algoritmo de Pontuação de propensão ajuda a identificar os abandonadores de carrinho relevantes que provavelmente não retornariam sem o incentivo.

É possível:

* Evite expor seus clientes em excesso ao remarketing.
* Identifique os clientes certos que abandonam carrinhos e mapeie sua atividade para a mensagem correta.
* Aumente a receita sabendo quais clientes retornarão ou não.

### O valor da pontuação de propensão {#section_CA99874A25434CC0BF01D0DA61608889}

Execute a descoberta de dados para identificar comportamentos ou padrões ocultos existentes pelos seus dados. Especificamente, a pontuação de propensão ajuda a identificar clusters de clientes semelhantes que usam meios mais objetivos e centralizados, em vez de filtragem ou segmentação simples. Além disso, a pontuação de propensão permite configurar recursos preditivos para identificar o comportamento do cliente de alto valor da empresa.

Depois de identificar o público-alvo de grande importância, você pode engajá-los para atingir o efeito principal. No caso de empresas entre empresas, pode haver leads de vendas que permitem sua classificação e a identificação da probabilidade de conversão offline. Como cada lead aumenta os custos, criar um incentivo para identificar possíveis clientes com a maior probabilidade de conversão de uma venda é a maneira mais eficiente e mais barata de focalizar seus recursos.

A pontuação de propensão fornece a capacidade de identificar os fatores que são mais preditivos de uma pontuação específica ou de aumentar a probabilidade de um evento ocorrer, mas também pode ser aplicada para responder a perguntas específicas:

* O cliente fará a conversão?
* O cliente responderá a um email?
* O cliente fará uma nova compra?

A pontuação de propensão permite que você responda a essas perguntas e identifique visitantes com uma inclinação de ação que pode ser configurada e pontuada.
