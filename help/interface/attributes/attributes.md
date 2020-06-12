---
description: Visão geral e pré-requisitos sobre como fazer upload dos Atributos do cliente na Experience Cloud.
keywords: core services;Customer Attributes
seo-description: Visão geral e pré-requisitos sobre como fazer upload dos Atributos do cliente na Experience Cloud.
seo-title: Atributos do cliente
solution: Experience Cloud
title: Atributos do cliente
uuid: 1621402d-990f-46f9-981a-473280559069
translation-type: tm+mt
source-git-commit: 75d3d045964aa42f7ac6b32b25cfd77aa7f663a9
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 71%

---


# Atributos do cliente

Navegue até **[!DNL Experience Platform]** > **[!UICONTROL Pessoas]** > Atributos **[!UICONTROL do cliente]**

Se você capturar os dados de clientes de empresas em um banco de dados de gerenciamento de relacionamento com o cliente (CRM), poderá fazer upload dos dados em uma fonte de dados do atributo do cliente na Experience Cloud. Depois de enviado, aproveite os dados no [!DNL Adobe Analytics] e no [!DNL Adobe Target].

![](assets/custom_reports.png)

## Pré-requisitos para fazer upload dos atributos do cliente {#section_BD38693AFBF34926BA28E964963B4EA0}

* **Ativação da solução:** [Ative suas soluções para os serviços](../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C)da plataforma Experience.

* **Associação a grupos:** Para carregar os dados do Atributo do cliente, os usuários devem ser membros do grupo [Atributos do](../admin-getting-started/admin-getting-started.md#task_3295A85536BF48899A1AB40D207E77E9)cliente. Você também deve pertencer a um grupo do Adobe Analytics ou do Adobe Target.

   To know whether your company has access to Customer Attributes, your [!DNL Experience Cloud] administrator should log into the [Experience Cloud](https://experience.adobe.com). Navigate to **[!UICONTROL Administration]** > **[!UICONTROL Admin Console]** > **[!UICONTROL Products]**. If *Customer Attributes* displays as one of the [!UICONTROL Product Profiles], you are ready to begin.

   Users that are added to the Customer Attributes will see the [!UICONTROL Customer Attributes] menu item on the left side of the Experience Cloud interface.

* **O Adobe Target** [!DNL at.js] (qualquer versão) ou a [!DNL mbox.js] versão 58 ou posterior é necessário para os Atributos do cliente.

   Consulte [Como implantar at.js](https://docs.adobe.com/content/help/pt-BR/target/using/implement-target/client-side/deploy-at-js/how-to-deployatjs.html) ou [Implementação do Mbox.js](https://docs.adobe.com/content/help/pt-BR/target/using/implement-target/client-side/mbox-implement/mbox-download.html).

## O que são os dados de clientes de empresas? {#section_6F34C29F11414842AA57D2B1248FA3C6}

Os dados da empresa ficam em outros sistemas. Eles podem ser complexos e ter diferentes significados para pessoas diferentes. Esses dados podem incluir informações como associações, nível de fidelidade, idade, gênero, produtos de propriedade, interesses e valor da vida útil.

A imagem a seguir é um exemplo de um arquivo de dados que mostra os dados do assinante para produtos, incluindo IDs de membro, produtos autorizados, produtos mais iniciados e assim por diante.

![](assets/01_crs_usecase.png)

Após a criação do arquivo de dados, faça upload dele para a fonte de atributos do cliente que você cria em **[!UICONTROL Experience Cloud]** > **[!UICONTROL Atributos do cliente]**.

Consulte [Fazer upload dos dados de atributos do cliente](../attributes/t-crs-usecase.md#task_BCC327B2A0EF4A1BBB2934013AB92B78) para conhecer esse fluxo de trabalho.

## Casos de uso da solução {#section_4E77650F6CEE4C4ABCD0B3221A5AE5D9}

Depois que os dados residirem na Experience Cloud, você poderá personalizá-los e compartilhá-los nas soluções para relatórios, segmentação, atividades e campanhas.

Por exemplo:

| Solução | Vantagens e casos de uso |
|--- |--- |
| Adobe Analytics | Profissionais de marketing e analistas podem entender:<ul><li>As campanhas online que são mais eficazes com seus clientes de nível gold.</li><li>Os produtos que os clientes de nível gold procuram em relação aos que os clientes de nível platinum procuram.</li><li>Se a reformulação do site está afetando positivamente as taxas de conversão de clientes mais antigos.</li><li>Quais produtos os clientes com um valor de vida útil baixo tendem a pesquisar no meu site.</li></ul> |
| Adobe Target | Os dados de atributo permitem que os usuários do Adobe Target:<ul><li>Mostrem descontos e ofertas especiais para membros do clube de fidelidade.</li><li>Recomendem produtos mais caros para seus clientes de luxo.</li><li>Para clientes que já recebem emails, mostrem uma oferta de venda adicional no espaço normalmente reservado para inscrições em email.</li></ul> |
