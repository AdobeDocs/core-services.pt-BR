---
description: Saiba mais sobre organizações (ID de organização IMS), como alternar contas e como vincular contas de soluções.
solution: Experience Cloud
title: Organizações e contas
uuid: ae47ad18-ac33-4efa-8b68-2bfaf77397aa
feature: Organizations
topic: Administration
role: Admin
level: Experienced
exl-id: 6eb58530-2a7a-48c7-9a5b-48a6e980a034
TQID: https://experienceleague.adobe.com/DCb0MQWwB0MOGALSDbLD-d4ik4B0C249xncB9eZbZMU
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2:
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2:
  - id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
  - id: bdea9bc8-5600-45db-b85e-d74bb59dfcff
  - id: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 9c2010694b8bb32c3922dd65f846375e43b2caac
workflow-type: tm+mt
source-wordcount: 506
ht-degree: 17%

---

# Organizações e contas

Uma *organização* (ID de organização) é a entidade que permite a um administrador configurar grupos e usuários e controlar o logon único no CX Enterprise.

A organização funciona como uma empresa de login que abrange todos os produtos e aplicativos CX Enterprise. Frequentemente, a organização é o nome da empresa. No entanto, uma empresa pode ter muitas organizações.

**Menu Organização**

![Organizações da CX Enterprise](../assets/organizations-menu.png)

Para verificar se você fez logon na organização correta, clique em **[!UICONTROL Perfil]** para ver o nome da organização padrão. Se você tiver acesso a mais de uma organização, também poderá visualizar e alternar para outra organização na barra do cabeçalho.

>[!NOTE]
>
>Alternar entre organizações permite que você acesse a Admin Console dessa organização específica. Se você não vir a organização desejada listada, talvez seja necessário solicitar acesso a um administrador nessa organização. (Se precisar mesclar várias instâncias do Admin Console, entre em contato com o Suporte ao cliente da Adobe para obter ajuda.)

## Federated IDs

Se sua organização usa Federated IDs, o CX Enterprise permite que você faça logon com o logon único de sua organização sem precisar inserir seu endereço de email e senha. Adicione `#/sso:@domain` ao CX Enterprise URL (`https://experience.adobe.com`) para realizar esta tarefa.

Por exemplo, para uma organização com Federated IDs e o domínio `example.com`, defina o link do URL para `https://experience.adobe.com/#/sso:@example.com`. Você também pode ir diretamente para um aplicativo específico marcando esse URL, anexado com o caminho do aplicativo. (Por exemplo, para Adobe Analytics, `https://experience.adobe.com/#/sso:@example.com/analytics`.)

## Contas de convidado federadas

Você pode habilitar o [acesso de convidado federado](https://helpx.adobe.com/br/business/enterprise/using/federated-guest-access.html) para autenticar com segurança os usuários convidados em seu próprio domínio. Se ativado, o menu Organization é alterado para permitir que esses usuários alternem entre contas dentro da organização existente em qualquer página do CX Enterprise.

Para alternar para uma conta de convidado federado, localize **[!UICONTROL Outras Contas]** no menu **[!UICONTROL Organização]** em qualquer página do [CX Enterprise](https://experience.adobe.com).

**Menu Organização para uma conta de convidado federada**

![Alternador de conta federada](../assets/federated-account-switcher.png)

## Exibir a ID da organização

Você pode localizar a ID da organização atribuída para fins de suporte. Você pode verificar se está na organização correta ou alternar entre organizações usando o seletor **[!UICONTROL Organização]** no cabeçalho.

A ID da organização é a ID associada à empresa provisionada pela CX Enterprise. A ID é uma string de 24 caracteres alfanuméricos seguidos por (e deve incluir) `@AdobeOrg`.

Você pode exibir a ID da organização, juntamente com outras informações da conta, usando o atalho de teclado **Ctrl+i** de qualquer página em `https://experience.adobe.com`.

**Para exibir a ID da organização**

1. No [CX Enterprise](https://experience.adobe.com), pressione **Ctrl+i** no teclado.

   ![ID da organização atribuída](../assets/assigned-organization.png)

1. Em **[!UICONTROL Informações do Usuário]**, procure a **[!UICONTROL ID da Organização Atual]** e localize a ID da organização.

   Como alternativa, os administradores podem fazer logon na Admin Console (acesse [https://adminconsole.adobe.com](https://adminconsole.adobe.com)) e visualizar a ID da organização na URL.

   Por exemplo, no URL a seguir:

   `https://adminconsole.adobe.com/C538193582390300A495CC9@AdobeOrg/overview`

   a ID é:

   `C538193582390300A495CC9@AdobeOrg`

## Especificar uma organização padrão

Você pode especificar uma organização padrão para usar ao fazer logon.

1. No cabeçalho, clique em **[!UICONTROL Perfil]** e em Preferências.

1. Em [!UICONTROL Geral], selecione uma organização padrão.


![Editar perfil](../assets/edit-profile.png)
