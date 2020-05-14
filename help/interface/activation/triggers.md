---
description: Como configurar o Experience Cloud Triggers.
keywords: integrations;Triggers
seo-description: Como configurar o Experience Cloud Triggers.
seo-title: Triggers
solution: Marketing Cloud
title: Triggers
uuid: dab536e3-1969-4661-919e-5b15f423fecd
translation-type: tm+mt
source-git-commit: fb03bf89bcc6ed4438daf18c8415de3052ba8fa4
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 63%

---


# Triggers

## Visão geral do Triggers {#topic_4F21FCE9A64E46E8B6D51F494FA652A7}

Acionadores permitem que você identifique, defina e monitore os principais comportamentos do consumidor, em seguida, gere comunicação entre soluções para engajar novamente os visitantes. Você pode usar acionadores em decisões e personalização em tempo real.

* Configure o remarketing rápido para abandonos de carrinho ou abandonos de carrinho com produtos removidos
* Formulários e aplicativos incompletos
* Qualquer ação ou sequência de ações no site

![](assets/trigger-abandonment-2.png)

### Tipos de Triggers

Geralmente, um acionador pode levar 15 a 90 minutos para iniciar uma campanha de marketing. Isso varia dependendo da implementação da coleção de dados, carga no pipeline, configuração personalizada do acionador definido e do fluxo de trabalho no Adobe Campaign.

* **Abandono:** é possível criar um acionador para ser disparado quando um visitante visualizar um produto, mas não fizer adições ao carrinho.
* **Ação:** por exemplo, você pode criar acionadores para serem disparados depois de inscrições em newsletters, assinaturas por email ou aplicações para cartões de crédito (confirmações). Se você for um varejista, crie um acionador para um visitante que se inscreve em um programa de fidelidade. Na mídia e no entretenimento, crie acionadores para visitantes que assistem a um determinado show, e talvez você queira responder com uma pesquisa.
* **Start da sessão e Fim da sessão:** Crie um acionador para o start da sessão e eventos de término da sessão.

## Criar um acionador da Experience Cloud {#task_821F37183AC045E5AC8EED20317598FE}

Crie um acionador e configure as condições para o acionador. Por exemplo, você pode especificar o critério das regras para um acionador durante uma visita. Alguns exemplos são métricas, como Abandono de carrinho, ou dimensões, como o nome do produto. Quando as regras são cumpridas, o acionador é executado.

>[!NOTE]
>
>No momento, há um limite técnico de 100 acionadores.

1. In the Experience Cloud, click ![](assets/menu-icon.png), then click **[!UICONTROL Launch]**.
2. Locate the [!UICONTROL Triggers] card, then click **[!UICONTROL Manage Triggers]**.
3. Clique em **[!UICONTROL Novo acionador]** e especifique o tipo de acionador:

   ![Resultado da etapa](assets/add-trigger.png)

4. Preencha os seguintes campos e arraste métricas e itens de dimensão aos contêineres da regra para configurar o acionador:

   | Elemento | Descrição |
   |--- |--- |
   | Nome | O nome amigável deste acionador. |
   | Descrição | A descrição desse acionador, como você o usará e assim por diante. |
   | Conjunto de relatórios | O conjunto [de](https://docs.adobe.com/content/help/en/analytics/implementation/analytics-basics/ref-reports-report-suites.html) relatórios do Analytics usado para esse acionador. Essa configuração identifica os dados do relatórios a serem usados. |
   | Visit must include<br>Visit must not include<br>Trigger after no action<br>Include meta data | Você pode definir critérios ou comportamentos de usuário que você deseja que ocorram, além de comportamentos que você não deseja que ocorram.  Por exemplo, as regras para um acionador de um simples abandono de carrinho de compras podem ser:<ul><li>A visita deve incluir: Adição ao carrinho (métrica) e Existe. (Mais tarde, você pode redefinir a regra com uma visualização de produto específica ou dimensões como Tipos de navegador.)</li><li>A visita não deve incluir: Check-out.</li><li>Acionar depois de nenhuma ação por: 10 minutos.</li><li>Incluir metadados: permite que você adicione uma dimensão de Campanha específica ou variáveis relevantes ao comportamento do visitante. Este campo pode ser útil ao criar o email de remarketing correto no Adobe Campaign.</li></ul><br>Você pode especificar a lógica Qualquer, E ou Ou dentro ou entre contêineres, dependendo dos critérios que determinar que são importantes para a regra. |
   | Container | Nos contêineres você pode configurar e armazenar regras, condições ou filtros que definem um acionador. Se você desejar que eventos sejam executados ao mesmo tempo, coloque-os no mesmo contêiner. Ou seja, cada contêiner é processado de maneira independente no nível da ocorrência.  Por exemplo, se você tiver dois contêineres unidos pelo operador E, poderá esperar que as regras se qualifiquem quando duas ocorrências atenderem aos requisitos. |
   | Start de nova sessão após | Crie um acionador para o start da sessão e eventos de término da sessão. |

5. Clique em **[!UICONTROL Salvar]**.
6. Use triggers for [real-time remarketing](https://docs.campaign.adobe.com/doc/standard/en/EMA_Transactional_messaging_Marketing_Cloud_Triggers.html) in [!DNL Adobe Campaign].

### Exemplos de acionadores

Exemplos de acionadores da Experience Cloud:

#### Acionador de abandono do carrinho

Por exemplo, a página a seguir mostra regras que você pode usar para um acionador de Abandono de carrinho, com base em produtos exibidos durante uma visita.

![](assets/abandonment-trigger.png)

#### Quem indicou acionadora

O acionador a seguir é disparado quando uma ocorrência acompanhar o produto de Botas masculinas e um referenciador do Facebook. Para que os dois critérios ( *produtos* e *referenciador*) sejam avaliados na mesma ocorrência, eles devem ser adicionados ao mesmo container.

![](assets/fb-boots-promo.png)
