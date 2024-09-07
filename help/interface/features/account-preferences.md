---
title: Preferências e Notificações de Conta
description: Saiba mais sobre perfis de usuário e preferências de conta no Experience Cloud. Inscreva-se nas notificações de produto para email e  [!DNL Slack] e configure alertas de produto.
solution: Experience Cloud
feature: Account Preferences, Notifications, Alerts
topic: Administration
role: Admin
level: Intermediate
exl-id: 1e34c6b2-a792-41c4-adb7-583de596237f
source-git-commit: b79d6c6fb7bb165fdd5d47061da16f65f6fc7579
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 21%

---

# Preferências e notificações da conta {#preferences}

As [preferências](https://experience.adobe.com/preferences) do Experience Cloud incluem notificações (no aplicativo, email e [!DNL Slack]), assinaturas e alertas.

Em preferências, é possível:

* Pesquisar por [Organizações](../administration/organizations.md)
* Especifique um tema escuro (nem todos os aplicativos oferecem suporte a esse tema).
* Configurar as preferências, notificações e assinaturas do usuário.
* Saia do Experience Cloud.

## Gerenciar preferências

Para gerenciar as preferências, selecione **[!UICONTROL Preferências]** no menu ![preferências](../assets/preferences-icon-sm.png) da conta.

Em [!UICONTROL Preferências da Experience Cloud], você pode configurar os seguintes recursos:

| Recurso | Descrição |
|--- |--- |
| Organização [padrão](../administration/organizations.md) | Selecione a organização que você deseja ver ao iniciar a Experience Cloud. |
| [!UICONTROL Coleção de dados do produto] | Selecione quais tecnologias a Adobe pode usar para coletar dados sobre como você usa seus produtos da Adobe. |
| [Notificações](#notifications-and-announcements) | Habilitar notificações de [!UICONTROL no aplicativo], [!UICONTROL email] ou [Slack](#slack-notifications). |
| [!UICONTROL Recomendações e promoções de aprendizado personalizadas] | Selecione onde deseja receber a [ajuda personalizada](personalized-learning.md) para seus produtos Adobe. Essa ajuda está disponível por email, no produto e nas comunidades Experience League. |
| [!UICONTROL Subscrições] | Selecione os produtos e categorias que deseja assinar. Notificações no popover [!UICONTROL Notificações] e por email. |
| [!UICONTROL Prioridade] | Selecione as categorias que você deseja que sejam consideradas de alta prioridade. Essas categorias são marcadas com uma marca [!UICONTROL High] e podem ser configuradas para entrega como alertas. |
| [!UICONTROL Alertas] | Selecione as notificações para as quais deseja que alertas sejam exibidos no navegador. Os alertas são exibidos no canto superior direito da janela por alguns segundos. |
| Emails | Especifique a frequência com que deseja receber emails de notificação. (Não enviar, instantâneo, diário ou semanal.) |

## Assinar notificações no Experience Cloud {#notifications}

Você pode selecionar os produtos e categorias que deseja assinar. As notificações aparecem no popover [!UICONTROL Notificações] (no aplicativo), no email ou em [Slack](#slack-notifications) (dependendo das suas assinaturas).

As notificações por email e Slack são úteis para situações em que você não está conectado ao Experience Cloud.

### Assinar notificações no aplicativo e por email

1. Navegue até Experience Cloud [preferências](https://experience.adobe.com/preferences).

1. Em **[!UICONTROL Notificações]**, habilite **[!UICONTROL No aplicativo]** ou **[!UICONTROL Email]**.

   As alterações nas notificações são salvas automaticamente.

### Assinar [!DNL Slack] notificações {#slack}

>[!NOTE]
>
>As notificações de Slack serão lançadas em: **11 de setembro de 2024**


Você pode configurar suas preferências de conta para enviar notificações de Experience Cloud para um canal [!DNL Slack].

**Pré-requisitos**

* Você deve ter uma conta Experience Cloud.
* Você deve ter uma conta [!DNL Slack]. O administrador de Slack habilita a integração de Experience Cloud com Slack.
* Você deve fazer parte de pelo menos um espaço de trabalho [!DNL Slack].

**Assinar notificações Slack**

1. Navegue até Experience Cloud [preferências](https://experience.adobe.com/preferences).

1. Localize [!DNL Slack] e clique em **[!UICONTROL Adicionar ao Slack]**.

   ![Adicionar ao Slack](../assets/add-to-slack.png)

   Se [!DNL Slack] estiver instalado, o aplicativo será aberto e uma mensagem de solicitação de permissão será exibida. Se o Slack não estiver instalado, você deve [solicitar permissão](#slack-troubleshoot).

1. Clique em **[!UICONTROL Permitir]**.

1. Em **[!UICONTROL Notificações]**, habilite as [!DNL Slack] notificações para os produtos e categorias desejados.

   ![Notificações Slack](../assets/slack.png)

   As atualizações das notificações são salvas automaticamente.

### Solicitar permissão no Slack {#slack-troubleshoot}

Se [!DNL Slack] não estiver instalado, uma mensagem _[!UICONTROL Solicitação de instalação]_ será exibida quando o Slack for aberto depois que você clicar em **[!UICONTROL Adicionar ao Slack]**.

![Solicitar Integração com o Slack](../assets/slack-request.png)

**Para solicitar permissões em Slack**

1. No Slack, escolha o espaço de trabalho no canto superior direito do aplicativo.

1. Para solicitar aprovação de aplicativo para o gerenciador de espaço de trabalho do Slack, clique em **[!UICONTROL Enviar]**.

1. Você receberá uma notificação em [!DNL Slack] depois que a solicitação de aplicativo for aprovada.

1. Após receber a aprovação [!DNL Slack], volte para a Experience Cloud **[!UICONTROL Notificações]** e [assine a Slack](#slack-notifications) (descrito acima).

### O que você verá em [!DNL Slack]

Depois de integrar o Slack com êxito, as notificações de Slack exibem as seguintes informações:

* A mensagem pessoal será recebida do nome do aplicativo _Adobe Experience Cloud_.
* A mensagem inclui o logotipo do produto para o aplicativo específico, como Adobe Experience Platform, Adobe Experience Manager e assim por diante.
* Um link para exibir todas as notificações no Experience Cloud.
* Um link para gerenciar preferências de notificação no Experience Cloud.

## Exibir [!UICONTROL notificações] e anúncios no Experience Cloud {#view-notifications}

No cabeçalho Experience Cloud, é possível exibir as notificações nas quais você [se inscreveu](#notifications), bem como exibir anúncios.

1. Clique no ícone de sino no cabeçalho. ![Notificações e anúncios](../assets/bell-icon.png)

1. Clique em **[!UICONTROL Notificações]** ou **[!UICONTROL Anúncios]**.

   É aqui que você recebe informações importantes sobre produtos, sua colaboração com outros usuários e outras atualizações relevantes. As atualizações incluem lançamentos de produtos, avisos de manutenção, itens compartilhados e solicitações de aprovação.