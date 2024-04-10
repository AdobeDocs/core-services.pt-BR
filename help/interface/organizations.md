---
description: Saiba mais sobre organizações (ID de organização IMS) e como vincular contas de soluções à Experience Cloud.
solution: Experience Cloud
title: Organizações e vinculação de contas
uuid: ae47ad18-ac33-4efa-8b68-2bfaf77397aa
feature: Organizations
topic: Administration
role: Admin
level: Experienced
exl-id: 6eb58530-2a7a-48c7-9a5b-48a6e980a034
source-git-commit: f229ec33ff721527e6a4c920ea63eabb4102935a
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 67%

---

# Organizações na Experience Cloud

Um *organização* A (ID da organização) é a entidade que permite ao administrador configurar grupos e usuários, além de controlar o logon único no Experience Cloud.

A organização funciona como uma empresa para logon que abrange todos os produtos e aplicativos Experience Cloud. Frequentemente, a organização é o nome da empresa. No entanto, uma empresa pode ter muitas organizações.

![Organizações Experience Cloud](assets/organizations-menu.png)

Para verificar se você fez logon na organização correta, clique no avatar do perfil para ver o nome da organização. Se você tiver acesso a mais de uma organização, também poderá visualizar e alternar para outra organização na barra do cabeçalho.

## Federated IDs

Se sua organização usa Federated IDs, a Experience Cloud permite conectar-se por meio do logon único de sua organização sem precisar inserir seu endereço de email e senha. Adicione `#/sso:@domain` ao URL da Experience Cloud (`https://experience.adobe.com`) para realizar essa tarefa.

Por exemplo, para uma organização com Federated IDs e o domínio `adobecustomer.com`, defina o link do URL para `https://experience.adobe.com/#/sso:@adobecustomer.com`. Você também pode ir diretamente para um aplicativo específico marcando esse URL, anexado com o caminho do aplicativo. (Por exemplo, para Adobe Analytics, `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics`.)

## Exibir a ID da organização {#concept_EA8AEE5B02CF46ACBDAD6A8508646255}

Você pode localizar a ID da organização atribuída para fins de suporte. Você pode verificar se está na organização correta ou alternar entre organizações usando o menu **[!UICONTROL Organização]**.

A ID da organização é a ID associada à empresa provisionada pela Experience Cloud. A ID é uma string de 24 caracteres alfanuméricos seguidos por (e deve incluir) `@AdobeOrg`.

É possível visualizar a ID da organização, juntamente com outras informações da conta, usando o atalho de teclado **Ctrl+I** de qualquer página em `https://experience.adobe.com`.

**Para visualizar a ID da organização**

1. Entrada [Experience Cloud](https://experience.adobe.com), pressione **Ctrl+I** no teclado.

   ![ID da organização atribuída](assets/assigned-organization.png)

1. Em **[!UICONTROL Informações do usuário]**, procure **[!UICONTROL ID da organização atual]**, e você verá a ID da organização.

   Como alternativa, os administradores podem fazer logon no Admin Console (acesse [https://adminconsole.adobe.com](https://adminconsole.adobe.com)) e exiba sua ID da organização no URL.

   Por exemplo, no URL a seguir:

   `https://adminconsole.adobe.com/C538193582390300A495CC9@AdobeOrg/overview`

   a ID é:

   `C538193582390300A495CC9@AdobeOrg`

## Vincular uma conta do aplicativo a uma Adobe ID {#task_FD389E78640848919E247AC5E95B8369}

Geralmente, os administradores da Experience Cloud concedem acesso a aplicativos e serviços. Em raras circunstâncias, você pode vincular as credenciais do aplicativo a uma Adobe ID.

1. Siga as etapas no convite por email para o Experience Cloud.

1. Faça logon usando a Adobe ID ou Enterprise ID.

1. Selecione o seletor de aplicativos. ( ![menu](assets/menu-icon.png)).

   ![Vincular uma conta do aplicativo a uma Adobe ID](assets/solutions-active.png)

   Os aplicativos que você pode acessar são coloridos.

1. Selecione o aplicativo desejado.

   ![Selecione o aplicativo desejado](assets/analytics-link-accounts.png)

   Esse tipo de mensagem será exibido se você fizer parte do grupo adequado (e tiver permissão para o aplicativo), mas ainda não tiver vinculado as credenciais da conta à Adobe ID.

1. Selecione **[!UICONTROL Vincular conta]** e forneça suas credenciais.

## Especificar uma organização e uma página de destino padrões {#concept_6A191B42A9874A9780882903BA18F071}

Você pode especificar uma organização padrão e uma página de destino para usar ao fazer o logon.

Em seu perfil, selecione **[!UICONTROL Editar perfil]**.

![Editar perfil](assets/edit-profile.png)

Em Organização padrão e Página de destino, é possível personalizar a experiência de logon.

![Organização padrão e Página de destino](assets/default-organization.png)

## Solução de problemas de vinculação de contas {#concept_DFCB29A3B4834FC59AA29E0BBA301584}

Ajuda sobre problemas que surgem da vinculação de contas.

Normalmente, a vinculação de contas falha porque a Adobe ID está vinculada a um usuário anterior. Quando a vinculação de contas falhar, você poderá:

* [Entrar em contato com o Suporte da Adobe](https://experienceleague.adobe.com/?support-solution=General&amp;lang=pt-BR#support).
* Acesse o aplicativo através do logon padrão enquanto o problema estiver sendo resolvido.
