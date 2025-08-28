---
title: '[!DNL Customer Attributes]'
description: Saiba mais sobre  [!DNL Customer Attributes]  na Experience Cloud. Descubra como fazer upload dos dados de atributo de cliente para uso no Adobe Analytics e Adobe Target.
solution: Experience Cloud,Target,Analytics
feature: Customer Attributes
role: Admin
topic: Administration
level: Experienced
exl-id: fe8ad013-76da-49f8-aa51-dc5f6c1b1d79
source-git-commit: fc60b49af0839769fdd8d18fd61863c8b28bbd57
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 73%

---

# [!DNL Customer Attributes] na Experience Cloud

O serviço de [!DNL Customer Attributes] na Experience Cloud permite que você faça upload de dados corporativos capturados de um banco de dados de gerenciamento de relacionamento com o cliente (CRM). É possível fazer upload dos dados para uma fonte de dados de atributo do cliente na Experience Cloud e, em seguida, usar os dados no [!DNL Adobe Analytics] e no [!DNL Adobe Target].

## Localizar o recurso de [!DNL Customer Attributes] 

1. Faça logon em [!DNL Experience Cloud] e selecione o ícone Menu ![menu](assets/menu-icon.png).

1. Selecione **[!DNL Customer Attributes]**.

![Visão geral dos atributos do cliente](assets/custom_reports.png)

## Pré-requisitos para fazer upload dos dados de atributos do cliente {#prerequisites}

* **Associação de grupo:** para carregar dados de atributos do cliente, os usuários devem ser membros do grupo de Atributos do Cliente. Você também deve pertencer a um grupo do Adobe Analytics ou do Adobe Target.

  Para saber se a empresa tem acesso aos atributos do cliente, o administrador do [!DNL Experience Cloud] deve fazer logon na [Experience Cloud](https://experience.adobe.com). Navegue até **[!UICONTROL Admin Console]** > **[!UICONTROL Produtos]**. Se *[!DNL Customer Attributes]* for exibido como um dos [!UICONTROL perfis de produto], está tudo pronto para você começar.

  Os usuários adicionados a [!DNL Customer Attributes] verão o item de menu [!DNL Customer Attributes] à esquerda da interface do Experience Cloud.

* O **Adobe Target** `at.js` (qualquer versão) ou `mbox.js` versão 58 ou posterior é necessário para os atributos do cliente.

  Consulte [Como implantar at.js](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/overview.html).

## O que são os dados de clientes de empresas? {#enterprise_data}

Os dados da empresa ficam em outros sistemas. Eles podem ser complexos e ter diferentes significados para pessoas diferentes. Esses dados podem incluir informações como associações, nível de fidelidade, idade, gênero, produtos de propriedade, interesses e valor da vida útil.

A imagem a seguir é um exemplo de um arquivo de dados que mostra os dados do assinante para produtos, incluindo IDs de membro, produtos autorizados, produtos mais iniciados e assim por diante.

![O que são os dados de clientes corporativos?](assets/01_crs_usecase.png)

Após a criação do arquivo de dados, é possível carregá-lo na fonte de atributos do cliente que você cria em **[!UICONTROL Experience Cloud]** > **[!UICONTROL Atributos do cliente]**.

Consulte [Fazer upload dos dados de atributos do cliente](t-crs-usecase.md) para conhecer esse fluxo de trabalho.

## Exemplos de atributos do cliente no Analytics e no Target {#examples}

Depois que os dados estiverem na Experience Cloud, é possível personalizá-los e compartilhá-los com soluções de relatório, segmentação, atividades e campanhas.

Por exemplo:

| Solução | Vantagens e casos de uso |
|--- |--- |
| Adobe Analytics | Profissionais de marketing e analistas podem entender:<ul><li>As campanhas online que são mais eficazes com seus clientes de nível gold.</li><li>Os produtos que os clientes de nível gold procuram em relação aos que os clientes de nível platinum procuram.</li><li>Se a reformulação do site está afetando positivamente as taxas de conversão de clientes mais antigos.</li><li>Quais produtos os clientes com baixo valor vitalício tendem a pesquisar no meu site.</li></ul> |
| Adobe Target | Os dados de atributo permitem que os usuários do Adobe Target:<ul><li>Mostrem descontos e ofertas especiais para membros do clube de fidelidade.</li><li>Recomendem produtos mais caros para seus clientes de luxo.</li><li>Para clientes que já recebem emails, mostrem uma oferta de venda adicional no espaço normalmente reservado para inscrições em email.</li></ul> |

{style="table-layout:auto"}
