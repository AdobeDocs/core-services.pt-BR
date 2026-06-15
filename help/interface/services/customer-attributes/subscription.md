---
description: Saiba como configurar assinaturas no [!DNL Customer Attributes] para o Analytics e o Target e ativar uma fonte de dados.
solution: Experience Cloud
title: Como configurar assinaturas no  [!DNL Customer Attributes]
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: cfa2aa5c-337f-401e-80eb-cbe36cb1d41e
TQID: https://experienceleague.adobe.com/I--LZ-Nqu0VdVAAs8qvv88pZTcaRQ97XiHWXd15WQcE
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2:
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2:
  - id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
  - id: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 50012e2564e88e1a6e16578e3331136c7df0cb21
workflow-type: tm+mt
source-wordcount: 421
ht-degree: 46%

---

# Configurar assinaturas de atributo do cliente

As assinaturas do [!DNL Customer Attributes] habilitam o fluxo de dados de atributos do cliente entre o CX Enterprise e os aplicativos ([!DNL Analytics] e [!DNL Target]).

Por exemplo, uma assinatura do Adobe Analytics permite atribuir dados em relatórios. Se você usar [!DNL Adobe Target], é possível carregar atributos do cliente para direcionamento e segmentação.

**Para configurar assinaturas e ativar a fonte de dados**

1. Localize sua fonte de dados em [!DNL Customer Attributes] para edição:

   Em [!DNL CX Enterprise], clique em **[!UICONTROL Aplicativos]** ![menu](assets/menu-icon.png) > **[!DNL Customer Attributes]**.

1. Em [!UICONTROL Editar Source de Atributos do Cliente], clique em **[!UICONTROL Upload de Arquivo]**.

1. Clique em **[!UICONTROL Configurar assinaturas]**.

   ![Configurar assinaturas na CX Enterprise](assets/configure-subscriptions.png)

1. Para ativar a fonte de atributo do cliente, clique em **[!UICONTROL Ativo]** e em **[!UICONTROL Salvar]**.

1. Para configurar uma assinatura para [!DNL Analytics] ou [!DNL Target], clique em **[!UICONTROL Configurar]**.

   O exemplo a seguir mostra uma assinatura [!DNL Target]:

   ![Resultado da etapa](assets/subscription-target.png)

   | Elemento | Descrição |
   | --- | --- |
   | Solução | **Adobe Analytics**<br> Selecione [!DNL Analytics], especifique os conjuntos de relatórios que você deseja que recebam dados de atributos, e quais deles serão incluídos.<br>**Adobe Target**<br>&#x200B;É possível fazer upload de atributos do cliente para direcionamento e segmentação. Este recurso é útil se você deseja direcionar um teste com base em dados de atributos ou disponibilizar os dados para segmentação no Analytics.<br>Os dados de atributos do cliente carregados para um visitante estão disponíveis ao entrar, em **[!DNL Target]** > **Públicos-alvo**.<br>Há suporte para várias fontes de dados. Ao definir IDs do cliente do seu site, verifique se pelo menos um dos alias está inscrito no [!DNL Target]. |
   | Report Suite (Adobe Analytics) | Os conjuntos de relatórios do Analytics.<br>Não é possível adicionar mais de dez conjuntos de relatórios às assinaturas do Analytics em uma única fonte de atributo. Ao escolher quais conjuntos de relatórios incluir, considere as seguintes sugestões:<ul><li>Escolher os conjuntos de relatórios que tenham um conjunto comum de clientes autenticados. Se os clientes autenticados em um conjunto de relatórios não se sobrepuserem aos clientes autenticados em outro conjunto de relatórios, separe esses conjuntos de relatórios em diferentes fontes de atributo.</li><li>Se possível, os conjuntos de relatórios incluídos em uma fonte de atributo devem ter um volume de tráfego semelhante.</li></ul><br>Se você tiver mais de dez conjuntos de relatórios que tenham um conjunto comum de clientes autenticados, será possível configurar outras fontes de atributo do cliente, cada uma com até dez conjuntos de relatórios. |
   | Atributos a serem incluídos (Analytics e [!DNL Target]) | Os atributos que deseja enviar para o aplicativo. <br>Ao configurar assinaturas e selecionar atributos, os seguintes limites poderão ser aplicados _por conjunto de relatórios,_ dependendo dos aplicativos que possui:<ul><li>Foundation: 0</li><li>Select: 3</li><li>Prime: 15</li><li>Ultimate: 200</li><li>Standard: total de 3</li><li>Premium: 200 por conjunto de relatórios</li><li>[!DNL Target] Standard: 5</li><li>[!DNL Target] Premium: 200</li></ul><br>**Observação:** quando você atualiza para o Analytics Premium, há um atraso de 24 horas antes de os atributos adicionais estarem disponibilizados. Você pode observar um erro de atributo Máximo de assinatura emitido durante esse atraso. |

1. Clique em **[!UICONTROL Save]**.
