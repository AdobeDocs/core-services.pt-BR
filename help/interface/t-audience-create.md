---
description: Saiba mais sobre como usar as regras de atributo para criar um público-alvo e definir um público composto na Adobe Experience Cloud.
keywords: principais serviços
solution: Experience Cloud
title: 'Criar um público-alvo '
uuid: 7e622539-296e-4ff3-93b0-ec1c08b35429
feature: Biblioteca de público-alvo
topic: Administração
role: Administrator
level: Experienced
exl-id: b65a12f5-fa89-400a-b279-13c381cd6c22
source-git-commit: d2ff52ce1a591c7c607598b5f2892dbcca74594b
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 95%

---

# Criar um público-alvo

Saiba mais sobre como usar as regras de atributo para criar um público-alvo e definir um público composto na Experience Cloud.

Este artigo ajuda você a entender como:

* Criar um público-alvo
* Criar uma regra
* Usar regras para definir um público-alvo composto

O gráfico a seguir representa duas regras em um público-alvo composto.

![](assets/audience_sharing.png)

Cada círculo representa uma regra que define a associação do público-alvo. Visitantes que se qualificam como membros em ambas as regras de público-alvo se sobrepõem para se tornarem o público-alvo composto e definido.

>[!NOTE]
>
>O público-alvo é totalmente definido após a conclusão da coleção de dados pelo período especificado.

O exemplo a seguir mostra como criar as regras para um público-alvo composto. Este público-alvo é composto de:

* Seção Casa e jardim derivada dos dados da página ou dos dados brutos de análise.
* Usuários do Chrome e do Safari derivados de um [!DNL Adobe Analytics] segmento [publicado](audience-library.md#task_32FEEFE0B32E4E388CD4D892D727282A) no [!DNL Experience Cloud].

   ![](assets/audience_create.png)

**Para criar um público-alvo**

1. Na [!DNL Experience Cloud], em [!DNL Experience Platform], clique em **[!UICONTROL Pessoas]** > **[!UICONTROL Biblioteca de públicos-alvo].**
1. Na página [!UICONTROL Públicos-alvo], clique em **[!UICONTROL Novo]**. ![](assets/add_icon_small.png)

   ![Resultado da etapa](assets/audience_create_new.png)

1. Na página [!UICONTROL Criar novo público-alvo], especifique um título e uma descrição.
1. Em [!UICONTROL Regras], selecione uma fonte de atributo:

   * **[!UICONTROL Dados do Real-Time Analytics:]**  (ou dados brutos) são dados de atributos derivados de solicitações de imagem do Real-Time Analytics e incluem dados como eVars e eventos. Você deve selecionar um conjunto de relatórios ao usar essa fonte de atributo e definir a dimensão ou evento que será incluído. Essa seleção de conjunto de relatórios fornece a estrutura variável usada pelo conjunto de relatórios.
   >[!NOTE]
   >
   >Devido a questões relacionadas ao cache, conjuntos de relatórios excluídos no Analytics permanecem exibidos na Experience Cloud por 12 horas após a exclusão.

   * **[!UICONTROL Experience Cloud:]** os dados de atributo nas fontes da [!DNL Experience Cloud]. Por exemplo, tais dados podem ser de segmentos de público-alvo criados no [!DNL Analytics], ou dados do [!DNL Audience Manager].

1. Defina as regras de público-alvo e clique em **[!UICONTROL Salvar].**

>[!NOTE]
>
>Você deve conhecer suas variáveis de implementação ao criar essas regras.

Em [!UICONTROL Regras], defina as *`Home & Garden`* seleções de atributo:

* **[!UICONTROL Fonte de atributo:]** dados brutos do Analytics
* **[!UICONTROL Report Suite:]** Report Suite 31
* Dimensão = **[!UICONTROL Loja (Merch) (v6)]** > **[!UICONTROL igual a]** > **[!UICONTROL Casa e Jardim]**

![](assets/home_garden.png)

Os *Visitantes do Chrome e do Safari* são um segmento de público-alvo compartilhado do Analytics:

* **[!UICONTROL Fonte do atributo:]** Experience Cloud
* **[!UICONTROL Dimensão:]** Chrome &amp; Safari Visitors

![](assets/chrome_safari.png)

Para comparar, adicione uma regra *OR* para ver todos os visitantes de uma seção do site como Patio &amp; Furniture.

![](assets/audiences_rule_patio.png)

A regra resultante é um público-alvo definido pela inclusão dos usuários do Chrome &amp; Safari que visitaram o Home &amp; Garden. O segmento Terraço e mobília fornece informações adicionais sobre todos os visitantes que visitam a seção do site.

![](assets/defined_audience.png)

* **Estimativa do histórico:** (círculo pontilhado) representa as regras criadas com base nos dados do [!DNL Analytics].
* **Público-alvo real:** (círculo contínuo) toda regra criada com 30 dias de dados no Audience Manager. Quando os dados do Audience Manager atingem 30 dias, a linha se torna sólida e representa os números reais.

Depois que a coleta de dados é concluída pelo período especificado, os círculos se combinam para mostrar uma audiência definida.

Quando salvo, o público-alvo fica disponível para outras soluções. Por exemplo, você pode incluir uma audiência compartilhada em uma atividade do Adobe Target.
