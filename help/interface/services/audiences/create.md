---
title: Como criar um público-alvo na Biblioteca de público-alvo
description: Descubra como usar as regras de atributo para criar um público-alvo compartilhável na Biblioteca de público-alvo. Saiba como configurar uma regra e definir um público-alvo composto.
solution: Experience Cloud
uuid: 7e622539-296e-4ff3-93b0-ec1c08b35429
feature: Audience Library
topic: Administration
role: Admin
level: Experienced
exl-id: b65a12f5-fa89-400a-b279-13c381cd6c22
source-git-commit: e63dd988abba199049da2b3620eed9ebf51043d1
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 62%

---

# Criar um público-alvo

No [!UICONTROL Audience Library], você pode usar as regras de atributo para criar um público-alvo e definir um público-alvo composto para compartilhar em aplicativos Experience Cloud.

Este artigo ajuda você a entender como:

* Criar um público-alvo
* Criar uma regra
* Usar regras para definir um público-alvo composto

O gráfico a seguir representa duas regras em um público-alvo composto.

![Duas regras em um público-alvo composto](assets/audience_sharing.png)

Cada círculo representa uma regra que define a associação do público-alvo. Visitantes que se qualificam como membros em ambas as regras de público-alvo se sobrepõem para se tornarem o público-alvo composto e definido.

>[!NOTE]
>
>O público-alvo é totalmente definido após a conclusão da coleção de dados pelo período especificado.

O exemplo a seguir mostra como criar as regras para um público-alvo composto. Este público-alvo é composto de:

* Seção Casa e jardim derivada dos dados da página ou dos dados brutos de análise.
* Usuários do Chrome e do Safari derivados de um [!DNL Adobe Analytics] segmento [publicado](overview.md) a [!DNL Experience Cloud].

  ![Criar as regras para um público-alvo composto](assets/audience_create.png)

**Para criar um público-alvo**

1. Clique em [!DNL Experience Cloud] aplicativos (![Ícone de aplicativos](assets/apps-icon.png)) e em **[!UICONTROL People]** > **[!UICONTROL Audience Library].**

1. Na página [!UICONTROL Audiences], clique em **[!UICONTROL New]**. ![Novo público-alvo](assets/add_icon_small.png)

   ![Criar um público-alvo](assets/audience_create_new.png)

1. Na página [!UICONTROL Create New Audience], preencha os campos **[!UICONTROL Title]** e **[!UICONTROL Description]**.
1. Em [!UICONTROL Rules], selecione um conjunto de relatórios de referência e, em seguida, uma fonte de atributo:

   * **[!UICONTROL Real-Time Analytics Data:]** (ou dados brutos) Estes são dados de atributo derivados de solicitações de imagem do Real-Time Analytics. Inclui eVars e eventos. Você deve selecionar um conjunto de relatórios ao usar essa fonte de atributo e definir a dimensão ou evento que será incluído. Essa seleção de conjunto de relatórios fornece a estrutura variável usada pelo conjunto de relatórios.

   >[!NOTE]
   >
   >Devido a questões relacionadas ao cache, conjuntos de relatórios excluídos no Analytics permanecem exibidos no Experience Cloud por 12 horas após a exclusão.

   * **[!UICONTROL Experience Cloud:]** dados do atributo derivados de [!DNL Experience Cloud] fontes. Por exemplo, tais dados podem ser de segmentos de público-alvo criados no [!DNL Analytics], ou dados do [!DNL Audience Manager].

1. Defina as regras de audiência e clique em **[!UICONTROL Save].**

**Exemplo: definir regras para público-alvo composto**

>[!NOTE]
>
>Você deve conhecer suas variáveis de implementação ao criar essas regras de público-alvo.

Em [!UICONTROL Rules], defina as *`Home & Garden`* seleções de atributo:

* **[!UICONTROL Attribute Source:]** Dados brutos do Analytics
* **[!UICONTROL Report Suite:]** Conjunto de relatórios 31
* Dimension = **[!UICONTROL Store (Merch) (v6)]** > **[!UICONTROL Equals]** > **[!UICONTROL Home & Garden]**

![Seleção de atributos na Biblioteca de público-alvo](assets/home_garden.png)

Os *Visitantes do Chrome e do Safari* são um segmento de público-alvo compartilhado do Analytics:

* Experience Cloud **[!UICONTROL Attribute Source:]**
* **[!UICONTROL Dimension:]** Visitantes do Chrome e Safari

![Visitantes do Chrome e Safari](assets/chrome_safari.png)

Para comparação, adicione uma regra *OU* para ver todos os visitantes de uma seção do site, como Pátio e Mobília.

![Regra OU para um público-alvo](assets/audiences_rule_patio.png)

A regra resultante é um público-alvo definido pela inclusão dos usuários do Chrome &amp; Safari que visitaram o Home &amp; Garden. O segmento Terraço e mobília fornece informações adicionais sobre todos os visitantes que visitam a seção do site.

![Público-alvo definido na Experience Cloud](assets/defined_audience.png)

* **Estimativa do histórico:** (círculo pontilhado) representa as regras criadas com base nos dados do [!DNL Analytics].
* **Público-alvo real:** (círculo contínuo) toda regra criada com 30 dias de dados no Audience Manager. Quando os dados do Audience Manager atingem 30 dias, a linha se torna sólida e representa os números reais.

Depois que a coleta de dados é concluída pelo período especificado, os círculos se combinam para mostrar um público-alvo definido.

Depois que o público-alvo é salvo, ele é disponibilizado para outros aplicativos da Experience Cloud. Por exemplo, você pode incluir um público-alvo compartilhado em uma [atividade](https://experienceleague.adobe.com/pt-br/docs/target/using/activities/activities) do Adobe Target.
