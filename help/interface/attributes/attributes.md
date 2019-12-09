---
description: Visão geral e pré-requisitos a respeito do upload de atributos do cliente na Experience Cloud.
keywords: core services;customer attributes
seo-description: Visão geral e pré-requisitos a respeito do upload de atributos do cliente na Experience Cloud.
seo-title: Atributos do cliente
solution: Experience Cloud
title: Atributos do cliente
uuid: 1621402d-990f-46f9-981a-473280559069
translation-type: tm+mt
source-git-commit: ae97db27349940a8df7ee2ba6678683f57585678

---


# Atributos do cliente

## Visão geral

Para localizar os [!UICONTROL atributos do cliente], navegue até **[!DNL Experience Platform]** &gt; **[!UICONTROL People]** &gt; **[!UICONTROL Atributos do cliente]**

Se você capturar os dados de clientes de empresas em um banco de dados de gerenciamento de relacionamento com o cliente (CRM), poderá fazer upload dos dados em uma fonte de dados do atributo do cliente na Experience Cloud. Depois de enviado, aproveite os dados no [!DNL Adobe Analytics] e no [!DNL Adobe Target].

![](assets/custom_reports.png)

## Pré-requisitos para fazer upload dos atributos do cliente {#section_BD38693AFBF34926BA28E964963B4EA0}


* **Ativação da solução:** [Ativar as soluções para os serviços principais](../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C).

* **Associação de grupo:** para fazer upload dos dados de atributos do cliente, os usuários devem ser membros do [grupo de Atributos do cliente](../admin-getting-started/admin-getting-started.md#task_3295A85536BF48899A1AB40D207E77E9). Você também deve pertencer a um grupo do Adobe Analytics ou do Adobe Target.

   Para saber se a empresa tem acesso aos atributos do cliente, o [!DNL Experience Cloud]administrador deve fazer logon na [!DNL Experience Cloud]. Navegue até **[!UICONTROL Administração]** &gt; **[!UICONTROL Iniciar Admin Console]** &gt; **[!UICONTROL Grupos]**. Se os *Atributos do cliente* forem exibidos como um dos grupos, você estará pronto para começar.

   Os usuários adicionados ao grupo Atributos do cliente visualizarão o item de menu [!UICONTROL Atributos do cliente] à esquerda da interface da Experience Cloud.

* **Mbox de destino:** mbox.js versão 58 ou superior é necessário para os atributos do cliente.


   Consulte [Implementação de mbox.js](https://docs.adobe.com/content/help/en/target/using/implement-target/client-side/mbox-implement/mbox-download.html).

* **at.js:** qualquer versão.

## O que são os dados de clientes de empresas? {#section_6F34C29F11414842AA57D2B1248FA3C6}

Os dados da empresa ficam em outros sistemas. Eles podem ser complexos e ter diferentes significados para pessoas diferentes. Esses dados podem incluir informações como associações, nível de fidelidade, idade, gênero, produtos adquiridos, interesses e valor da vida útil.

A imagem a seguir é um exemplo de um arquivo de dados que mostra os dados do assinante para produtos, incluindo IDs de membro, produtos qualificados, produtos mais lançados e assim por diante.

![](assets/01_crs_usecase.png)

Após a criação do arquivo de dados, faça upload dele para a fonte de atributos do cliente que você cria em **[!UICONTROL Experience Cloud]** &gt; **[!UICONTROL Atributos do cliente]**.

Consulte [Fazer upload dos dados de atributos do cliente](../attributes/t-crs-usecase.md#task_BCC327B2A0EF4A1BBB2934013AB92B78) para conhecer esse fluxo de trabalho.

## Casos de uso da solução {#section_4E77650F6CEE4C4ABCD0B3221A5AE5D9}

Uma vez na Experience Cloud, você pode personalizar e compartilhar os dados nas soluções para elaboração de relatórios, segmentação, atividades e campanhas.

Por exemplo:

| Solução | Vantagens e casos de uso |
|--- |--- |
| Adobe Analytics | Comerciantes e analistas podem entender:<ul><li>As campanhas online não são eficazes com clientes nível gold.</li><li>Os produtos pesquisados pelos clientes gold em comparação aos pesquisados por clientes platinum.</li><li>Se a reformulação do site afetou positivamente as taxas de conversão dos clientes mais antigos.</li><li>Quais produtos os clientes com um valor de vida útil pequeno costumam pesquisar no meu site.</li></ul> |
| Adobe Target | Dados de atributos permitem aos usuários do Target:<ul><li>Mostrar descontos e ofertas especiais para os membros do clube de fidelidade.</li><li>Recomendar produtos mais caros para os clientes de luxo.</li><li>Para clientes que já recebem emails, mostrar uma oferta de venda adicional no espaço normalmente reservado para cadastro de email</li></ul> |
