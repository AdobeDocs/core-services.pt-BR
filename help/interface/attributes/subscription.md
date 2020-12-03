---
description: Saiba mais sobre fontes de dados de solução e como configurar assinaturas. As assinaturas permitem que o cliente atribua o fluxo de dados entre a Experience Cloud e as soluções (Analytics e Target).
keywords: Customer Attributes;core services
seo-description: Saiba mais sobre fontes de dados de solução e como configurar assinaturas. As assinaturas permitem que o cliente atribua o fluxo de dados entre a Experience Cloud e as soluções (Analytics e Target).
seo-title: Configurar assinaturas
solution: Experience Cloud
title: Configurar assinaturas
uuid: f74a8155-0a21-46b3-9b1e-4c838f72f24f
translation-type: tm+mt
source-git-commit: 0bc7032d0052ba03beac1140dfbfd630e1802bfd
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 100%

---


# Configurar assinaturas

Saiba mais sobre fontes de dados de solução e como configurar assinaturas. As assinaturas permitem que o cliente atribua o fluxo de dados entre a Experience Cloud e as soluções (Analytics e [!DNL Target]).

Por exemplo, uma assinatura do Adobe Analytics permite atribuir dados em relatórios. Se você usar o Adobe Target, é possível fazer upload de atributos do cliente para direcionamento e segmentação.

**[!UICONTROL Fonte de atributos do cliente]** > **[!UICONTROL Criar nova fonte de atributos do cliente]** > **[!UICONTROL Novo]**

![](assets/configure_subscription_page.png)

| Elemento | Descrição |
|--- |--- |
| Solução | **Adobe Analytics**<br> Selecione Analytics, especifique os conjuntos de relatórios que você deseja que recebam dados de atributos, e quais deles serão incluídos.<br>**Adobe Target**<br>&#x200B;É possível fazer upload de atributos do cliente para direcionamento e segmentação. Esse recurso é útil se você deseja direcionar um teste com base em dados de atributos ou disponibilizar os dados para segmentação no Analytics.<br>Os dados de atributos do cliente enviados para um visitante estão disponíveis ao fazer logon em **[!DNL Target]** > **Públicos-alvo**.<br>Há suporte para diversas fontes de dados. Ao [definir IDs do cliente](../core-services/core-services.md) do seu site, verifique se pelo menos um dos alias está inscrito no [!DNL Target]. |
| Report Suite (Analytics) | Os conjuntos de relatórios do Analytics.<br>Não é possível adicionar mais de dez conjuntos de relatórios às assinaturas do Analytics em uma única fonte de atributos. Ao escolher quais conjuntos de relatórios incluir, considere as seguintes sugestões:<ul><li>Escolher os conjuntos de relatórios que tenham um conjunto comum de clientes autenticados. Se os clientes autenticados em um conjunto de relatórios não se sobrepuserem aos clientes autenticados em outro conjunto de relatórios, separe esses conjuntos de relatórios em diferentes fontes de atributo.</li><li>Se possível, os conjuntos de relatórios incluídos em uma fonte de atributo devem ter um volume de tráfego semelhante.</li></ul><br>Se você tiver mais de dez conjuntos de relatórios que tenham um conjunto comum de clientes autenticados, será possível configurar outras fontes de atributo do cliente, cada uma com até dez conjuntos de relatórios. |
| Atributos a serem incluídos (Analytics e [!DNL Target]) | Os atributos que deseja enviar para a solução. <br>Ao configurar assinaturas e selecionar atributos, os seguintes limites poderão ser aplicados _por conjunto de relatórios,_ dependendo das suas soluções:<ul><li>Foundation: 0</li><li>Select: 3</li><li>Prime: 15</li><li>Ultimate: 200</li><li>Standard: total de 3</li><li>Premium: 200 por conjunto de relatórios</li><li>[!DNL Target] Standard: 5</li><li>[!DNL Target] Premium: 200</li></ul><br>**Observação:** quando você atualiza para o Analytics Premium, há um atraso de 24 horas antes de os atributos adicionais estarem disponibilizados. Você pode observar um erro Máximo de assinatura de atributo emitido durante esse atraso. |
