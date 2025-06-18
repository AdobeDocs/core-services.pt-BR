---
description: Saiba mais sobre fontes de dados de solução e como configurar assinaturas. As assinaturas permitem que o cliente atribua o fluxo de dados entre o Experience Cloud e os aplicativos (Analytics e Target).
solution: Experience Cloud
title: Como configurar assinaturas
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: cfa2aa5c-337f-401e-80eb-cbe36cb1d41e
source-git-commit: 2f126877f6a5f090884ebe093f35e4f6d90b4df6
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 75%

---

# Como configurar assinaturas na Experience Cloud

Saiba mais sobre fontes de dados de aplicativo e como configurar assinaturas. As assinaturas habilitam o fluxo de dados [!DNL customer attribute] entre o Experience Cloud e os aplicativos ([!DNL Analytics] e [!DNL Target]).

Por exemplo, uma assinatura do Adobe Analytics permite atribuir dados em relatórios. Se você usar o Adobe Target, é possível fazer upload de atributos do cliente para direcionamento e segmentação.

**[!UICONTROL Source de atributo do cliente]** > **[!UICONTROL Criar novo Source de atributo do cliente]** > **[!UICONTROL Novo]**

![Configurar assinaturas na Experience Cloud](assets/configure_subscription_page.png)

| Elemento | Descrição |
|--- |--- |
| Solução | **Adobe Analytics**<br> Selecione [!DNL Analytics], especifique os conjuntos de relatórios que você deseja que recebam dados de atributos, e quais deles serão incluídos.<br>**Adobe Target**<br>&#x200B;É possível fazer upload de atributos do cliente para direcionamento e segmentação. Esse recurso é útil se você deseja direcionar um teste com base em dados de atributos ou disponibilizar os dados para segmentação no Analytics.<br>Os dados de atributos do cliente enviados para um visitante estão disponíveis ao fazer logon em **[!DNL Target]** > **Públicos-alvo**.<br>Há suporte para diversas fontes de dados. Ao definir IDs do cliente do seu site, verifique se pelo menos um dos alias está inscrito no [!DNL Target]. |
| Report Suite (Adobe Analytics) | Os conjuntos de relatórios do Analytics.<br>Não é possível adicionar mais de dez conjuntos de relatórios às assinaturas do Analytics em uma única fonte de atributos. Ao escolher quais conjuntos de relatórios incluir, considere as seguintes sugestões:<ul><li>Escolher os conjuntos de relatórios que tenham um conjunto comum de clientes autenticados. Se os clientes autenticados em um conjunto de relatórios não se sobrepuserem aos clientes autenticados em outro conjunto de relatórios, separe esses conjuntos de relatórios em diferentes fontes de atributo.</li><li>Se possível, os conjuntos de relatórios incluídos em uma fonte de atributo devem ter um volume de tráfego semelhante.</li></ul><br>Se você tiver mais de dez conjuntos de relatórios que tenham um conjunto comum de clientes autenticados, será possível configurar outras fontes de atributo do cliente, cada uma com até dez conjuntos de relatórios. |
| atributos a serem incluídos (Analytics e [!DNL Target]) | Os atributos que deseja enviar para o aplicativo. <br>Ao configurar assinaturas e selecionar atributos, os seguintes limites poderão ser aplicados _por conjunto de relatórios,_ dependendo dos aplicativos que possui:<ul><li>Foundation: 0</li><li>Select: 3</li><li>Prime: 15</li><li>Ultimate: 200</li><li>Standard: total de 3</li><li>Premium: 200 por conjunto de relatórios</li><li>[!DNL Target] Standard: 5</li><li>[!DNL Target] Premium: 200</li></ul><br>**Observação:** quando você atualiza para o Analytics Premium, há um atraso de 24 horas antes de os atributos adicionais estarem disponibilizados. Você pode observar um erro de atributo Máximo de assinatura emitido durante esse atraso. |

{style="table-layout:auto"}
