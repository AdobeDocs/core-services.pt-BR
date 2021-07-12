---
description: Como ativar as configurações de privacidade para cookies do navegador. É possível remover os usuários que bloquearam todos os cookies em navegadores de computadores e de dispositivos móveis.
keywords: cookies; privacidade
solution: Experience Cloud, Analytics, Target, Social
title: 'Configurações de privacidade de cookies do navegador '
uuid: f6a56e8b-b021-49db-8eb4-6c14af0c7243
feature: Cookies
topic: Administração
role: Admin
level: Experienced
exl-id: 5d852e0e-4004-4f94-a6f7-3a14a96cd42f
source-git-commit: 1fb1abc7311573f976f7e6b6ae67f60ada10a3e7
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 57%

---

# Ativar as configurações de privacidade de cookies do navegador{#enable-privacy-settings-for-browser-cookies}

É possível remover os usuários que bloquearam todos os cookies em navegadores de computadores e de dispositivos móveis. Esse recurso é uma configuração de privacidade que exclui os usuários que optam por não participar da coleta de dados, permitindo que você respeite a intenção de um usuário de interromper o processamento do Analytics.

**Para ativar as configurações de privacidade de cookies do navegador**

1. Navegue até **[!UICONTROL Ferramentas administrativas]** > **[!UICONTROL Conjuntos de relatórios]**.
1. Vá para **[!UICONTROL Editar configurações]** > **[!UICONTROL Geral]** > **[!UICONTROL Configurações de privacidade]**.
1. Ativar as **[!UICONTROL Configurações de privacidade]** (para desktop ou dispositivos móveis).

>[!IMPORTANT]
>
>Muitos aplicativos móveis (como o navegador interno do Facebook ou Twitter) podem parecer navegadores de dispositivos móveis padrão, mas não permitem todos os cookies. Ativar esse recurso poderia excluir uma grande parte do tráfego móvel dos relatórios do Analytics.

**Sobre as configurações de privacidade do navegador**

As orientações legislativas e regulamentares expressaram que a ação de um usuário de bloquear cookies é a mesma ação de um usuário de não participar na criação de perfis. Ao ativar esse recurso, os dados coletados em navegadores de desktop, onde o usuário definiu o navegador para bloquear todos os cookies, são excluídos dos relatórios do Analytics. Se o Adobe não conseguir reconhecer o navegador da Web, os dados serão incluídos nos relatórios [!DNL Analytics].

Legisladores de todo o mundo declararam (tanto em orientações quanto em acordos) que as configurações de cookies do navegador são uma indicação da preferência do usuário em não participar da definição de perfis. Especificamente, esses legisladores declararam que a configuração do navegador para bloquear cookies de terceiros é uma solicitação de não participação no rastreamento de terceiros (entre sites). Bloquear todos os cookies é uma solicitação de não participação para todo o rastreamento. Embora identificadores do lado do servidor (como endereço IP ou agente do usuário) possam ser uma opção desejável que ignore as configurações de cookies do navegador, alguns legisladores os consideram uma evasão da escolha do usuário.
