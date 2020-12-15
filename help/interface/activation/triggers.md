---
description: Como configurar o Experience Cloud Triggers.
keywords: integrations;Triggers
seo-description: Como configurar o Experience Cloud Triggers.
seo-title: Triggers
solution: Experience Cloud
title: 'Visão geral dos acionadores '
uuid: dab536e3-1969-4661-919e-5b15f423fecd
translation-type: tm+mt
source-git-commit: 3f26c1af19a0838913eec2b4135304f5f3fcf0b4
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 99%

---


# Triggers

## Visão geral do Triggers {#topic_4F21FCE9A64E46E8B6D51F494FA652A7}

Triggers permitem identificar, definir e monitorar os comportamentos dos principais consumidores e gerar comunicação entre soluções para atrair os visitantes novamente. Você pode usar acionadores em personalizações e decisões em tempo real.

* Configure o remarketing com rapidez em abandonos de carrinho ou em abandonos de carrinho com produtos removidos
* Formulários e aplicativos incompletos
* Qualquer ação ou sequência de ações no site

![](assets/trigger-abandonment-2.png)

### Tipos de Triggers

Geralmente, um acionador pode levar 15 a 90 minutos para iniciar uma campanha de marketing. Isso varia dependendo da implementação da coleção de dados, carga no pipeline, configuração personalizada do acionador definido e do fluxo de trabalho no Adobe Campaign.

* **Abandono:** é possível criar um acionador para ser disparado quando um visitante visualizar um produto, mas não fizer adições ao carrinho.
* **Ação:** por exemplo, você pode criar acionadores para serem disparados depois de inscrições em newsletters, assinaturas por email ou aplicações para cartões de crédito (confirmações). Se você for um varejista, crie um acionador para um visitante que se inscreve em um programa de fidelidade. Em mídia e entretenimento, crie acionadores para visitantes que assistem a um certo programa que talvez você queira que respondam a uma pesquisa.
* **Início e término de sessão:** crie um acionador para o início da sessão e eventos de término de sessão.

## Criar um acionador da Experience Cloud {#task_821F37183AC045E5AC8EED20317598FE}

Crie um acionador e configure as condições para ele. Por exemplo, você pode especificar o critério das regras para um acionador durante uma visita. Alguns exemplos são métricas, como Abandono de carrinho, ou dimensões, como o nome do produto. O disparador é executado quando as regras são cumpridas.

>[!NOTE]
>
>No momento, há um limite técnico de 100 acionadores.

1. Na Experience Cloud, clique em ![](assets/menu-icon.png) e depois em **[!UICONTROL Launch]**.
2. Encontre o cartão [!UICONTROL Triggers] e clique em **[!UICONTROL Gerenciar acionadores]**.
3. Clique em **[!UICONTROL Novo acionador]** e especifique o tipo de acionador:

   ![Resultado da etapa](assets/add-trigger.png)

4. Preencha os seguintes campos e arraste métricas e itens de dimensão aos contêineres da regra para configurar o acionador:

   | Elemento | Descrição |
   |--- |--- |
   | Nome | O nome amigável deste acionador. |
   | Descrição | A descrição deste acionador, como você irá usá-lo etc. |
   | Conjunto de relatórios | O [conjunto de relatórios](https://docs.adobe.com/content/help/pt-BR/analytics/admin/manage-report-suites/report-suites-admin.html) do Analytics usado para esse acionador. Esta configuração identifica os dados de relatório que serão usados. |
   | A visita deve incluir o acionador<br>A visita não deve incluir<br>depois de nenhuma ação<br>Incluir metadados | Você pode definir critérios ou comportamentos de usuário que você deseja que ocorram, além de comportamentos que você não deseja que ocorram.  Por exemplo, as regras para um acionador de um simples abandono de carrinho de compras podem ser:<ul><li>A visita deve incluir: Adição ao carrinho (métrica) e Existe. (Mais tarde, você pode redefinir a regra com uma visualização de produto específica ou dimensões como Tipos de navegador.)</li><li>A visita não deve incluir: Check-out.</li><li>Acionar depois de nenhuma ação por: 10 minutos.</li><li>Incluir metadados: permite que você adicione uma dimensão de Campanha específica ou variáveis relevantes ao comportamento do visitante. Este campo pode ser útil ao criar o email de remarketing correto no Adobe Campaign.</li></ul><br>Você pode especificar a lógica Qualquer, E ou Ou dentro ou entre contêineres, dependendo dos critérios que determinar que são importantes para a regra. |
   | Contêiner | Nos contêineres você pode configurar e armazenar regras, condições ou filtros que definem um acionador. Se você desejar que eventos sejam executados ao mesmo tempo, coloque-os no mesmo contêiner. Ou seja, cada contêiner é processado de maneira independente no nível da ocorrência.  Por exemplo, se você tiver dois contêineres unidos pelo operador E, poderá esperar que as regras se qualifiquem quando duas ocorrências atenderem aos requisitos. |
   | Iniciar nova sessão após | Crie um acionador para o início da sessão e outro para o término. |

5. Clique em **[!UICONTROL Salvar]**.
6. Use os acionadores para o [remarketing em tempo real](https://docs.adobe.com/content/help/pt-BR/campaign-standard/using/integrating-with-adobe-cloud/working-with-campaign-and-triggers/about-adobe-experience-cloud-triggers.html) no [!DNL Adobe Campaign].

### Exemplos de acionadores

Exemplos de Experience Cloud Triggers:

#### Acionador de abandono do carrinho

Por exemplo, a página a seguir mostra regras que você poderia usar em um acionador de Abandono de carrinho, com base em produtos visualizados durante uma visita.

![](assets/abandonment-trigger.png)

#### Acionador referenciador

O acionador a seguir é disparado quando uma ocorrência acompanhar o produto de Botas masculinas e um referenciador do Facebook. Para que os dois critérios (*produtos* e *referenciador*) sejam avaliados na mesma ocorrência, eles devem ser adicionados ao mesmo contêiner.

![](assets/fb-boots-promo.png)
