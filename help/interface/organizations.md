---
description: Saiba mais sobre organizações e como vincular contas de soluções à Experience Cloud.
keywords: Serviços da Adobe Experience Cloud
solution: Experience Cloud
title: 'Organizações e vinculação de contas '
uuid: ae47ad18-ac33-4efa-8b68-2bfaf77397aa
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: 6eb58530-2a7a-48c7-9a5b-48a6e980a034
source-git-commit: c073b3bacf5505c01017d4ba2507621df8ef877e
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 75%

---

# Organizações na Experience Cloud

Saiba mais sobre como gerenciar e trocar organizações na Experience Cloud.

## Identificar a organização {#concept_384D169B0B724B799D573B8ECB5C39BF}

Uma *organização* é a entidade que permite ao administrador configurar grupos e usuários, além de controlar o logon único na Experience Cloud. A organização funciona como uma empresa de login que abrange todos os produtos e aplicativos do Experience Cloud. Frequentemente, a organização é o nome da empresa. No entanto, uma empresa pode ter muitas organizações.

Para verificar se você fez logon na organização correta, clique no avatar do perfil para ver o nome da organização. Se você tiver acesso a mais de uma organização, também poderá visualizar e mudar para outra organização diretamente na barra do cabeçalho.

Se sua organização usa Federated IDs, a Experience Cloud permite fazer logon com o logon único de sua organização sem precisar digitar o endereço de email e a senha. Para usar esse recurso, adicione `#/sso:@domain` ao URL da Experience Cloud (`https://experience.adobe.com`).

Por exemplo, para uma organização com Federated IDs e o domínio `adobecustomer.com`, defina o link do URL para `https://experience.adobe.com/#/sso:@adobecustomer.com`. Você também pode ir diretamente para um aplicativo específico marcando esse URL, anexado com o caminho do aplicativo. (Por exemplo, para o Adobe Analytics, `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics`.)

![Resultado da etapa](assets/organization-switch.png)

## Encontrar a ID da organização {#concept_EA8AEE5B02CF46ACBDAD6A8508646255}

Além disso, pode ser necessário localizar a ID da organização para fins de suporte. Você pode verificar se está na organização correta ou alternar entre organizações usando o menu **[!UICONTROL Organização]**.

A **ID da organização** é a ID associada à empresa provisionada pela Experience Cloud. A ID é uma sequência de 24 caracteres alfanuméricos seguidos por (e deve incluir) @AdobeOrg.

Para exibir a ID da organização, navegue até a página de aterrissagem da Experience Cloud ou selecione ( ![](assets/menu-icon.png)) e, em seguida, **[!UICONTROL Administração]**. É possível encontrar a ID da organização na parte inferior da página [!UICONTROL Introdução à Experience Cloud] ou na página [!UICONTROL Administração].

![](assets/administration-page.png)

## Vincular uma conta do aplicativo a uma Adobe ID {#task_FD389E78640848919E247AC5E95B8369}

Normalmente, os administradores do Experience Cloud concedem acesso a aplicativos e serviços. Em raras circunstâncias, pode ser necessário vincular credenciais de aplicativo a uma Adobe ID.

1. Siga as etapas no convite por email na Experience Cloud.
1. Faça logon usando a Adobe ID ou Enterprise ID.
1. Selecione o seletor de aplicativos. ( ![](assets/menu-icon.png)).

   ![Vincular uma conta do aplicativo a uma Adobe ID](assets/solutions-active.png)

   Os aplicativos aos quais você tem acesso são coloridos.
1. Selecione o aplicativo desejado.

   ![Selecione o aplicativo desejado](assets/analytics-link-accounts.png)

   Esse tipo de mensagem será exibido se você fizer parte do grupo apropriado (e tiver permissão para o aplicativo), mas ainda não vinculou suas credenciais de conta à Adobe ID.
1. Selecione **[!UICONTROL Vincular conta]** e forneça suas credenciais.

## Especificar uma organização e uma página de aterrissagem padrões {#concept_6A191B42A9874A9780882903BA18F071}

Você pode especificar uma organização padrão e uma página de aterrissagem para usar ao fazer o logon.

Em seu perfil, selecione **[!UICONTROL Editar perfil]**.

![Editar perfil](assets/edit-profile.png)

Em Organização &amp; página inicial padrão, você pode personalizar a experiência de logon.

![Organização padrão e página de aterrissagem](assets/default-organization.png)

## Solução de problemas de vinculação de contas {#concept_DFCB29A3B4834FC59AA29E0BBA301584}

Ajuda sobre problemas que surgem da vinculação de contas.

Normalmente, a vinculação de contas falha porque a Adobe ID está vinculada a um usuário anterior. Quando a vinculação de contas falhar, você poderá:

* [Entrar em contato com o Suporte da Adobe](https://experienceleague.adobe.com/?support-solution=General&amp;lang=pt-BR#support).
* Acesse seu aplicativo usando o logon padrão enquanto o problema estiver sendo resolvido.
