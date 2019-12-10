---
description: Como configurar o Experience Cloud Triggers.
keywords: integrations;Triggers
seo-description: Como configurar o Experience Cloud Triggers.
seo-title: Triggers
solution: Marketing Cloud
title: Triggers
uuid: dab536e3-1969-4661-919e-5b15f423fecd
translation-type: tm+mt
source-git-commit: ae97db27349940a8df7ee2ba6678683f57585678

---


# Triggers

## Visão geral do Triggers {#topic_4F21FCE9A64E46E8B6D51F494FA652A7}

*Triggers* permite identificar, definir e monitorar os comportamentos dos principais consumidores e gerar comunicação entre soluções para atrair os visitantes novamente. Você pode usar acionadores em personalizações e decisões em tempo real.

* Configure o remarketing com rapidez em abandonos de carrinho ou em abandonos de carrinho com produtos removidos
* Aplicativos e formulários incompletos
* Qualquer ação ou sequência de ações no site

![](assets/trigger-abandonment-2.png)

**Tipos de Triggers**

Geralmente, um acionador pode levar 15 a 90 minutos para iniciar uma campanha de marketing. Isso varia dependendo da implementação da coleção de dados, carga no pipeline, configuração personalizada do acionador definido e do fluxo de trabalho no Adobe Campaign.

* **Abandono:** é possível criar um acionador para ser disparado quando um visitante visualizar um produto, mas não fizer adições ao carrinho. Configure [Pontuação de propensão](../activation/triggers.md#concept_A506150674AD45DB98D3CC07E560D334) para entender a tendência dos clientes para não retornar após abandonar um carrinho de compras.
* **Ação:** por exemplo, você pode criar acionadores para serem disparados depois de inscrições em newsletters, assinaturas por email ou aplicações para cartões de crédito (confirmações). Se você for um varejista, crie um acionador para um visitante que se inscreve em um programa de fidelidade. Em mídia e entretenimento, crie acionadores para visitantes que assistem a um certo programa que talvez você queira que respondam a uma pesquisa.
* **Início da sessão e término da sessão:** crie um acionador para os eventos de início da sessão e de término.

## Criar um acionador da Experience Cloud {#task_821F37183AC045E5AC8EED20317598FE}

Crie um acionador de abandono e configure as condições para o acionador e a pontuação de propensão. Por exemplo, você pode especificar o critério das regras para um acionador durante uma visita. Alguns exemplos são métricas, como Abandono de carrinho, ou dimensões, como o nome do produto. O acionador é executado quando as regras são correspondidas.

<!-- t_create-trigger.xml -->

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
   | Descrição | A descrição deste acionador, como você irá usá-lo etc. |
   | Conjunto de relatórios | O [conjunto de relatórios](https://docs.adobe.com/content/help/en/analytics/implementation/analytics-basics/ref-reports-report-suites.html) do Analytics usado para este acionador. Esta configuração identifica os dados de relatório que serão usados. |
   | A visita deve incluir<br>A visita não deve incluir<br>Acionar depois de nenhuma ação<br>Incluir metadados | Você pode definir critérios ou comportamentos de usuário que você deseja que ocorram, além de comportamentos que você não deseja que ocorram.  Por exemplo, as regras para um acionador de um simples abandono de carrinho de compras podem ser:<ul><li>A visita deve incluir: Adição ao carrinho (métrica) e Existe. (Mais tarde, você pode redefinir a regra com uma visualização de produto específica ou dimensões como Tipos de navegador.)</li><li>A visita não deve incluir: Check-out.</li><li>Acionar depois de nenhuma ação por: 10 minutos.</li><li>Incluir metadados: permite que você adicione uma dimensão de Campanha específica ou variáveis relevantes ao comportamento do visitante. Este campo pode ser útil ao criar o email de remarketing correto no Adobe Campaign.</li></ul><br>Você pode especificar a lógica Qualquer, E ou Ou dentro ou entre contêineres, dependendo dos critérios que determinar que são importantes para a regra. |
   | Contêiner | Nos contêineres você pode configurar e armazenar regras, condições ou filtros que definem um acionador. Se você desejar que eventos sejam executados ao mesmo tempo, coloque-os no mesmo contêiner. Ou seja, cada contêiner é processado de maneira independente no nível da ocorrência.  Por exemplo, se você tiver dois contêineres unidos pelo operador E, poderá esperar que as regras se qualifiquem quando duas ocorrências atenderem aos requisitos. |
   | Iniciar nova sessão após | Crie um acionador para o início da sessão e outro para o término. |

1. (Opcional) Em Acionadores de abandono, você pode aplicar a [Pontuação de propensão](../activation/triggers.md#concept_A506150674AD45DB98D3CC07E560D334).

   ![Resultado da etapa](assets/propensity-scoring.png)

1. Clique em **[!UICONTROL Salvar]**.
1. Use triggers for [real-time remarketing](https://docs.campaign.adobe.com/doc/standard/en/EMA_Transactional_messaging_Marketing_Cloud_Triggers.html) in [!DNL Adobe Campaign].

### Exemplos de acionadores

**Acionador de abandono de carrinho**

Por exemplo, a página a seguir mostra regras que você poderia usar em um acionador de Abandono de carrinho, com base em produtos visualizados durante uma visita.

![](assets/abandonment-trigger.png)

**Acionador referenciador**

O acionador a seguir é disparado quando uma ocorrência acompanhar o produto de Botas masculinas e um referenciador do Facebook. Para que os dois critérios ( *produtos* e *referenciador*) sejam avaliados na mesma ocorrência, eles devem ser adicionados ao mesmo container.

![](assets/fb-boots-promo.png)

## Pontuação de propensão {#concept_A506150674AD45DB98D3CC07E560D334}

<!-- propensity-scoring.xml -->

Saiba mais sobre a probabilidade de retorno de um cliente após abandonar um carrinho de compras. A pontuação de propensão é integrada ao Experience Cloud Triggers e disponível para acionadores de Abandono.

![Resultado da etapa](assets/propensity-scoring.png)

Por exemplo, alguns clientes abandonam carrinhos de compras para tirar usufruir de emails de incentivo para retornarem ao carrinho. Para reduzir a perda de lucro, o algoritmo de Pontuação de propensão ajuda a identificar os clientes que abandonam seus carrinhos e têm menos probabilidade de retornar sem o incentivo.

É possível:

* Evitar expor seus clientes excessivamente ao remarketing.
* Identificar os clientes certos que abandonam carrinhos e mapeie a atividade à mensagem apropriada.
* Ao saber quais clientes irão ou não retornar, o lucro aumentará.

## O valor da Pontuação de propensão {#section_CA99874A25434CC0BF01D0DA61608889}

Execute a descoberta de dados para identificar comportamentos ou padrões ocultos existentes pelos seus dados. Especificamente, a pontuação de propensão ajuda a identificar clusters de clientes semelhantes que usam meios mais objetivos e centralizados, em vez de filtragem ou segmentação simples. Além disso, a pontuação de propensão permite que você configure recursos preditivos para identificar comportamentos de clientes importantes para a sua empresa.

Depois de identificar o público-alvo de grande importância, você pode engajá-los para atingir o efeito principal. No caso de empresas entre empresas, pode haver leads de vendas que permitem sua classificação e a identificação da probabilidade de conversão offline. Devido ao custo de cada lead, a criação de um incentivo para identificar possíveis clientes com a maior probabilidade de conversão de uma venda é a maneira mais eficaz e econômica de focar nos seus recursos.

A pontuação de propensão fornece a capacidade de identificar os fatores mais preditivos de uma classificação específica, ou de identificar a probabilidade da ocorrência de um evento, mas também pode ser aplicada para responder às seguintes questões:

* O cliente fará conversões?
* O cliente responderá a um email?
* O cliente fará outras compras?

A pontuação de propensão permite que você responda a essas perguntas e identifique visitantes que tenham uma inclinação a ações que podem ser configuradas e classificadas.
