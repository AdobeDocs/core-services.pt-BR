---
title: Preferências e Notificações de Conta
description: Saiba mais sobre perfis de usuário, preferências de conta e dados de uso do produto no CX Enterprise. Inscreva-se nas notificações de produto para email e  [!DNL Slack] e configure alertas de produto.
solution: Experience Cloud
feature: Account Preferences, Notifications, Alerts
topic: Administration
role: Admin
level: Intermediate
exl-id: 1e34c6b2-a792-41c4-adb7-583de596237f
TQID: https://experienceleague.adobe.com/2IL6hUlA1oNxJIFMwbVQUbxEGkJoghVUTyMi5wSRBsE
product_v2: id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2: id: e1eba07e-ab89-466f-9ab5-ceb891d7a67did: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2: id: b75843fa-0a67-4a44-a6b1-cc627b0481dcid: bdea9bc8-5600-45db-b85e-d74bb59dfcffid: dc42f745-24d2-44a4-99c3-dece518fa4bcid: eaef3029-0844-43fe-9e1c-7666a24f4d03id: eb1ae5c4-ef16-4998-851c-73cc9f0b7f06id: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 1a77ef8d31211fb11c790152e78037a8c3b238a2
workflow-type: tm+mt
source-wordcount: 802
ht-degree: 5%

---

# Preferências e notificações da conta

Para localizar as preferências do CX Enterprise, clique em **[!UICONTROL Profile]** ![preferências](../assets/preferences-icon-sm.png) no cabeçalho e, em seguida, clique em **[!UICONTROL Preferences]**.

![preferências](../assets/preferences-navigation.png){width="100" zoomable="yes"}

Na página [!UICONTROL CX Enterprise preferences], você pode gerenciar os seguintes recursos da conta:

| Recurso | Descrição |
| --- | --- |
| [!UICONTROL Profile] | Atualize seu [Perfil de Conta da Adobe](https://account.adobe.com/profile). <p>A foto e o nome do seu perfil aparecem ao fazer logon em Adobe.com, produtos e serviços da Adobe e em sites voltados ao público, como o [!DNL Behance]. |
| [!UICONTROL General] | Selecione uma [organização](../administration/organizations.md).<p>Essa organização é a padrão usada ao fazer logon na CX Enterprise. |
| [!UICONTROL Product usage data] | É possível controlar quais dados de uso do produto são compartilhados com a Adobe ao usar os aplicativos da CX Enterprise. Esses são dados sobre como você usa nossos produtos, não sobre o conteúdo ou os dados de sua organização. A Adobe usa essas informações para ajudar a melhorar nossos produtos, fornecer suporte aprimorado no produto e personalizar sua experiência e as comunicações conosco. <p>Para saber mais, consulte [Dados de uso do produto](#product-usage-data) (nesta página). |
| [!UICONTROL Notifications] | Configure como e quando você deseja [notificações](#subscribe-to-notifications-in-experience-cloud) e alertas do produto: <ul><li>Selecione os produtos que deseja assinar para receber alertas</li><li>Configurar o tipo de notificação ([!UICONTROL in-app], [!UICONTROL email] ou [Slack](#slack-notifications))</li><li>Especifique a frequência com que deseja receber emails de notificação. (Não enviar, instantâneo, diário ou semanal.)</li><li>Determine a prioridade do alerta. Os alertas no aplicativo são exibidos no canto superior direito da janela por alguns segundos. Ou você pode especificar se os alertas devem ser exibidos até você descartá-los.</li></ul> |

## [!UICONTROL Product usage data]

Os dados de uso do produto que você escolhe para compartilhar com a Adobe incluem os seguintes tipos de informações sobre como você usa e interage com os aplicativos da Adobe:

* Informações do navegador e do dispositivo, como modelo e sistema operacional do dispositivo, informações de software e hardware, configurações do navegador e do dispositivo, identificadores exclusivos (como endereço IP, ID de cookie ou ID do dispositivo), quantidade de memória instalada, configurações de idioma e resolução da tela;
* Como você interage com os aplicativos do Adobe CX Enterprise, incluindo os recursos usados e as opções selecionadas;
* Informações sobre o produto Adobe, como número de versão;
* Informações sobre seu conteúdo e documentos, como número de páginas e identificadores exclusivos, mas não o conteúdo em si;
* Informações de uso de conteúdo, como quantas vezes você acessa o conteúdo e como interage com seu conteúdo no aplicativo;
* Logs de falhas e erros.

A Adobe usa essas informações para ajudar a melhorar nossos produtos, fornecer suporte no produto e por meio do atendimento ao cliente, e personalizar sua experiência e as comunicações conosco. Saiba mais sobre [experiências personalizadas](personalized-learning.md).

## Assinar notificações no CX Enterprise

Você pode selecionar os produtos e categorias que deseja assinar. As notificações aparecem no popover [!UICONTROL Notifications] (no aplicativo), no email ou no [Slack](#slack-notifications) (dependendo das suas assinaturas).

As notificações por email e pelo Slack são úteis para situações em que você não está conectado ao CX Enterprise.

### Assinar notificações no aplicativo e por email

1. Navegue até CX Enterprise [preferências](https://experience.adobe.com/preferences).

1. Em **[!UICONTROL Notifications]**, habilite **[!UICONTROL In-app]** ou **[!UICONTROL Email]**.

   As alterações nas notificações são salvas automaticamente.

### Assinar [!DNL Slack] notificações

Você pode configurar suas preferências de conta para enviar notificações do CX Enterprise para um canal [!DNL Slack].

**Pré-requisitos**

* É necessário ter uma conta do CX Enterprise.
* Você deve ter uma conta [!DNL Slack]. O administrador do [!DNL Slack] habilita a integração do CX Enterprise com o [!DNL Slack].
* Você deve fazer parte de pelo menos um espaço de trabalho [!DNL Slack].

**Assinar [!DNL Slack] notificações**

1. Navegue até CX Enterprise [Preferências](https://experience.adobe.com/preferences).

1. Localize [!DNL Slack] e clique em **[!UICONTROL Add to Slack]**.

   ![Adicionar ao Slack](../assets/add-to-slack.png)

   Se [!DNL Slack] estiver instalado, o aplicativo será aberto e uma mensagem de solicitação de permissão será exibida. Se o Slack não estiver instalado, você deve [solicitar permissão](#slack-troubleshoot).

1. Clique em **[!UICONTROL Allow]**.

1. Em **[!UICONTROL Notifications]**, habilite as notificações do [!DNL Slack] para os produtos e categorias desejados.

   ![Notificações do Slack](../assets/slack.png)

   As atualizações das notificações são salvas automaticamente.

### Solicitar permissão em [!DNL Slack] (solução de problemas)

Se o [!DNL Slack] não estiver instalado, uma mensagem _[!UICONTROL Request to install]_será exibida quando o Slack for aberto depois que você clicar em **[!UICONTROL Add to Slack]**. Por exemplo:

![Solicitar Integração com o Slack](../assets/slack-workspace.png)

**Para solicitar permissões no Slack**

1. Em [!DNL Slack], selecione o espaço de trabalho no menu **[!UICONTROL Workspace]** (canto superior direito).

1. Para solicitar aprovação de aplicativo para o gerenciador de espaço de trabalho [!DNL Slack], clique em **[!UICONTROL Submit]**.

1. Você receberá uma notificação em [!DNL Slack] depois que a solicitação de aplicativo for aprovada.

1. Após receber a aprovação de [!DNL Slack], volte para o CX Enterprise **[!UICONTROL Notifications]** e siga as etapas para [assinar o Slack](#slack-notifications) (descritas acima).

### O que você verá em [!DNL Slack]

Depois de integrar com êxito o [!DNL Slack], as notificações do [!DNL Slack] exibem as seguintes informações:

* A mensagem pessoal será recebida do nome do aplicativo _Adobe[!DNL CX Enterprise]_.
* A mensagem inclui o logotipo do produto para o aplicativo específico, como Adobe [!DNL Experience Platform], Adobe [!DNL Experience Manager] e assim por diante.
* Um link para exibir todas as notificações no CX Enterprise.
* Um link para gerenciar as preferências de notificação no CX Enterprise.

## Exibir [!UICONTROL notifications] e anúncios no CX Enterprise

No cabeçalho [!DNL CX Enterprise], é possível exibir as notificações nas quais você [se inscreveu](#notifications), bem como exibir anúncios.

1. Clique no ícone de sino no cabeçalho. ![Notificações e anúncios](../assets/bell-icon.png)

1. Clique em **[!UICONTROL Notifications]** ou **[!UICONTROL Announcements]**.

   É aqui que você recebe informações importantes sobre produtos, sua colaboração com outros usuários e outras atualizações relevantes. As atualizações incluem lançamentos de produtos, avisos de manutenção, itens compartilhados e solicitações de aprovação.

