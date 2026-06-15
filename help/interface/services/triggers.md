---
description: Saiba como configurar o CX Enterprise Triggers.
solution: Experience Cloud
title: Visão geral do Triggers
uuid: dab536e3-1969-4661-919e-5b15f423fecd
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: 9dc26e2f-479b-49a5-93ce-b877559fea43
TQID: https://experienceleague.adobe.com/1R70ZEmKiP9VhhSRVCXHjGoJbOb7Mh8spKRm4FgNRPc
product_v2: id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2: id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2: id: b75843fa-0a67-4a44-a6b1-cc627b0481dcid: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: d3cdead0-685a-4489-9250-4bb709942f66id: e0eb8757-182f-49f3-94a4-1587d16f5094id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 50012e2564e88e1a6e16578e3331136c7df0cb21
workflow-type: tm+mt
source-wordcount: 726
ht-degree: 72%

---

# CX Enterprise Triggers

[!UICONTROL Triggers] no CX Enterprise permite que você identifique, defina e monitore os comportamentos dos principais consumidores e gere comunicação entre aplicativos para atrair os visitantes novamente. Você pode usar acionadores em personalizações e decisões em tempo real.

Por exemplo:

* Configure o remarketing com rapidez em abandonos de carrinho ou em abandonos de carrinho com produtos removidos
* Formulários e aplicativos incompletos
* Qualquer ação ou sequência de ações no site

![Exemplo de acionador](../assets/trigger-abandonment-2.png)

>[!NOTE]
>
>Mais informações sobre o uso de [!UICONTROL Triggers] estão disponíveis em [Campaign Standard](https://experienceleague.adobe.com/docs/campaign-standard/using/integrating-with-adobe-cloud/working-with-campaign-and-triggers/using-triggers-in-campaign.html).

## Tipos de acionadores

Geralmente, um acionador pode levar 15 a 90 minutos para iniciar uma campanha de marketing. Esse atraso varia dependendo da implementação da coleção de dados, da carga no pipeline, da configuração personalizada do acionador definido e do fluxo de trabalho no Adobe Campaign.

* **Abandono:** é possível criar um acionador para ser disparado quando um visitante visualizar um produto, mas não fizer adições ao carrinho.
* **Ação:** por exemplo, você pode criar acionadores para serem disparados depois de inscrições em newsletters, assinaturas por email ou aplicações para cartões de crédito (confirmações). Se você for um varejista, crie um acionador para um visitante que se inscreve em um programa de fidelidade. Em mídia e entretenimento, crie acionadores para visitantes que assistem a um certo programa que talvez você queira que respondam a uma pesquisa.
* **Início e término de sessão:** crie um acionador para o início da sessão e eventos de término de sessão.

## Criar um acionador do CX Enterprise

Crie um acionador e configure as condições para ele. Por exemplo, você pode especificar o critério das regras para um acionador durante uma visita. Alguns exemplos são métricas, como Abandono de carrinho, ou dimensões, como o nome do produto. O acionador é executado quando as regras são cumpridas.

>[!NOTE]
>
>No momento, há um limite técnico de 100 acionadores.

1. No CX Enterprise, clique em ![menu](../assets/menu-icon.png) e em **[!UICONTROL Coleção de dados/Launch]**.
1. No cartão [!UICONTROL Triggers], clique em **[!UICONTROL Gerenciar Triggers]**.
1. Clique em **[!UICONTROL Novo acionador]** e especifique o tipo de acionador:

   ![Resultado da etapa](../assets/add-trigger.png)

1. Preencha os seguintes campos e arraste métricas e itens de dimensão aos contêineres da regra para configurar o acionador:

   | Elemento | Descrição |
   | --- | --- |
   | [!UICONTROL Nome] | O nome amigável deste acionador. |
   | [!UICONTROL Descrição] | A descrição deste acionador, como você o usará etc. |
   | [!UICONTROL Conjunto de Relatórios] | O [conjunto de relatórios](https://experienceleague.adobe.com/docs/analytics/admin/manage-report-suites/report-suites-admin.html?lang=pt-BR) do Analytics usado para esse acionador. Esta configuração identifica os dados de relatório que serão usados. |
   | A visita deve incluir o acionador<br>A visita não deve incluir<br>depois de nenhuma ação<br>Incluir metadados | Você pode definir critérios ou comportamentos de usuário que você deseja que ocorram, além de comportamentos que você não deseja que ocorram. Por exemplo, as regras para o acionador de um simples abandono de carrinho de compras podem ser:<ul><li>A visita deve incluir: [!UICONTROL Adição ao carrinho] (métrica) e [!UICONTROL Existe]. (Mais tarde, você pode redefinir a regra com uma visualização de produto específica ou dimensões como Tipos de navegador.)</li><li>A visita não deve incluir: [!UICONTROL Check-out].</li><li>Acionar depois de nenhuma ação por: 10 minutos.</li><li>[!UICONTROL Incluir dados do Meta]: permite adicionar uma dimensão [!DNL Campaign] específica ou variáveis relevantes ao comportamento do visitante. Este campo pode ser útil ao criar o email de remarketing correto no Adobe Campaign.</li></ul><br>Você pode especificar a lógica [!UICONTROL Qualquer], [!UICONTROL E] ou [!UICONTROL Ou] dentro de ou entre contêineres, dependendo dos critérios que você determinar que são importantes para a regra. |
   | [!UICONTROL Contêiner] | [!UICONTROL Nos contêineres] você pode configurar e armazenar regras, condições ou filtros que definem um gatilho. Se você desejar que eventos sejam executados ao mesmo tempo, coloque-os no mesmo contêiner. Ou seja, cada contêiner é processado de maneira independente no nível da ocorrência. Por exemplo, se você tiver dois contêineres unidos pelo operador AND, poderá esperar que as regras se qualifiquem quando duas ocorrências atenderem aos requisitos. |
   | Iniciar nova sessão após | Crie um acionador para o início da sessão e outro para o término. |

   {style="table-layout:auto"}

1. Clique em **[!UICONTROL Save]**.
1. Use os acionadores para o [remarketing em tempo real](https://experienceleague.adobe.com/docs/campaign-standard/using/integrating-with-adobe-cloud/working-with-campaign-and-triggers/about-adobe-experience-cloud-triggers.html?lang=pt-BR) no [!DNL Adobe Campaign].

## Exemplos de acionadores

Exemplos de CX Enterprise Triggers:

### Acionador de Abandono do carrinho

Por exemplo, a página a seguir mostra regras que você poderia usar em um acionador de [!UICONTROL Abandono do carrinho], com base em produtos visualizados durante uma visita.

![Acionador de Abandono do carrinho](../assets/abandonment-trigger.png)

### Acionador do referenciador

O acionador a seguir é disparado quando uma ocorrência acompanhar o produto de Botas masculinas e um referenciador do Facebook. Para que os dois critérios (*produtos* e *referenciador*) sejam avaliados na mesma ocorrência, eles devem ser adicionados ao mesmo contêiner.

![Acionador do referenciador](../assets/fb-boots-promo.png)

