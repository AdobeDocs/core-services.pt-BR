---
description: Visão geral e pré-requisitos a respeito do upload de atributos do cliente na Experience Cloud.
keywords: core services;customer attributes
seo-description: Visão geral e pré-requisitos a respeito do upload de atributos do cliente na Experience Cloud.
seo-title: Atributos do cliente
solution: Experience Cloud
title: Atributos do cliente
uuid: 1621402d-990f-46f9-981a-473280559069
translation-type: tm+mt
source-git-commit: 43de353155c640b3ddc519147c94d7e9ffcafe4e

---


# Atributos do cliente

To locate [!UICONTROL customer attributes] navigate to **[!DNL Experience Platform]** > **[!UICONTROL People]** > **[!UICONTROL Customer Attributes]**

Se você capturar os dados de clientes de empresas em um banco de dados de gerenciamento de relacionamento com o cliente (CRM), poderá fazer upload dos dados em uma fonte de dados do atributo do cliente na Experience Cloud. Depois de enviado, aproveite os dados no [!DNL Adobe Analytics] e no [!DNL Adobe Target].

![](assets/custom_reports.png)

## Pré-requisitos para fazer upload dos atributos do cliente {#section_BD38693AFBF34926BA28E964963B4EA0}

* **Ativação da solução:** [Ativar as soluções para os serviços principais](../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C).

* **Associação de grupo:** para fazer upload dos dados de atributos do cliente, os usuários devem ser membros do [grupo de Atributos do cliente](../admin-getting-started/admin-getting-started.md#task_3295A85536BF48899A1AB40D207E77E9). Você também deve pertencer a um grupo do Adobe Analytics ou do Adobe Target.

   Para saber se a empresa tem acesso aos atributos do cliente, o [!DNL Experience Cloud]administrador deve fazer logon na [!DNL Experience Cloud]. Navigate to **[!UICONTROL Administration]** > **[!UICONTROL Launch Admin Console]** > **[!UICONTROL Groups]**. Se os *Atributos do cliente* forem exibidos como um dos grupos, você estará pronto para começar.

   Os usuários adicionados ao grupo Atributos do cliente visualizarão o item de menu [!UICONTROL Atributos do cliente] à esquerda da interface da Experience Cloud.

* **O Público alvo** da Adobe [!DNL at.js] (qualquer versão) ou [!DNL mbox.js] versão 58 ou posterior é necessário para os atributos do cliente.

   Consulte [Como implantar a Implementação](https://docs.adobe.com/content/help/en/target/using/implement-target/client-side/deploy-at-js/how-to-deployatjs.html) do at.js ou [Mbox.js](https://docs.adobe.com/content/help/en/target/using/implement-target/client-side/mbox-implement/mbox-download.html).

## What is enterprise customer data? {#section_6F34C29F11414842AA57D2B1248FA3C6}

Os dados da empresa ficam em outros sistemas. Eles podem ser complexos e ter diferentes significados para pessoas diferentes. Esses dados podem incluir informações como associações, nível de fidelidade, idade, gênero, produtos de propriedade, interesses e valor da vida útil.

A imagem a seguir é um exemplo de um arquivo de dados que mostra os dados do assinante para produtos, incluindo IDs de membro, produtos autorizados, produtos mais lançados e assim por diante.

![](assets/01_crs_usecase.png)

After you create the data file, you can upload it to the customer attribute source that you create in **[!UICONTROL Experience Cloud]** > **[!UICONTROL Customer Attributes]**.

Consulte [Fazer upload dos dados de atributos do cliente](../attributes/t-crs-usecase.md#task_BCC327B2A0EF4A1BBB2934013AB92B78) para conhecer esse fluxo de trabalho.

## Casos de uso da solução {#section_4E77650F6CEE4C4ABCD0B3221A5AE5D9}

Depois que os dados residirem na Experience Cloud, você poderá personalizá-los e compartilhá-los nas soluções para relatórios, segmentação, atividades e campanhas.

Por exemplo:

| Solução | Vantagens e casos de uso |
|--- |--- |
| Adobe Analytics | Profissionais de marketing e analistas podem entender:<ul><li>As campanhas on-line que são mais eficazes com seus clientes de nível ouro.</li><li>Os produtos que os clientes de nível ouro procuram em relação aos que os clientes de nível platinum procuram.</li><li>Se a reformulação do site está afetando positivamente as taxas de conversão de clientes mais antigos.</li><li>Quais produtos os clientes com um valor de vida útil baixo tendem a pesquisar no meu site.</li></ul> |
| Adobe Target | Os dados do atributo permitem que os usuários do Público alvo da Adobe:<ul><li>Mostrar descontos e ofertas especiais para membros do clube de fidelidade.</li><li>Recomendar produtos mais caros para seus clientes de luxo.</li><li>Para clientes que já recebem emails, exibam uma oferta de venda adicional no espaço normalmente reservado para inscrições em email</li></ul> |
