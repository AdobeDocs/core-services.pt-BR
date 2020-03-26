---
description: Remova os usuários que bloquearam todos os cookies em navegadores de computadores e de dispositivos móveis. Essa configuração de privacidade exclui os usuários que opt out da coleta de dados do Analytics.
keywords: cookies;privacy
seo-description: Remova os usuários que bloquearam todos os cookies em navegadores de computadores e de dispositivos móveis. Essa configuração de privacidade exclui os usuários que opt out da coleta de dados do Analytics.
seo-title: Ativar as configurações de privacidade de cookies do navegador
solution: Marketing Cloud,Adobe Analytics,Adobe Target,Adobe Social
title: Ativar as configurações de privacidade de cookies do navegador
uuid: f6a56e8b-b021-49db-8eb4-6c14af0c7243
translation-type: tm+mt
source-git-commit: f7ec8bf6087a18be41c9efbf05f60e6cfd24e566

---


# Ativar as configurações de privacidade de cookies do navegador{#enable-privacy-settings-for-browser-cookies}

Você pode remover usuários que bloquearam todos os cookies em navegadores para desktop e móveis. Este recurso é uma configuração de privacidade que exclui os usuários que opt out da coleta de dados, permitindo que você respeite a intenção de um usuário de interromper o processamento do Analytics.

**Para ativar as configurações de privacidade dos cookies do navegador**

1. Navigate to **[!UICONTROL Admin Tools]** > **[!UICONTROL Report Suites]**.
1. Click **[!UICONTROL Edit Settings]** > **[!UICONTROL General]** > **[!UICONTROL Privacy Settings]**.
1. Ativar as **[!UICONTROL Configurações de privacidade]** (para desktop ou dispositivos móveis).

>[!IMPORTANT]
>
>Observe que muitos aplicativos móveis (como o navegador no aplicativo para Facebook ou Twitter) podem aparecer como um navegador móvel padrão, mas não permitem todos os cookies. Ativar esse recurso poderia excluir uma grande proporção do tráfego móvel dos relatórios do Analytics.

**Sobre as configurações de privacidade do navegador**

As orientações legislativas e regulamentares expressaram que a ação de um usuário para bloquear cookies é a mesma ação de um usuário para opt out a criação de perfis. Ao ativar esse recurso, os dados coletados em navegadores de desktop, nos quais o usuário definiu o navegador para bloquear todos os cookies, serão excluídos dos relatórios do Analytics. Se a Adobe não reconhecer o navegador da Web, os dados serão incluídos nos relatórios do Analytics.

Legisladores de todo o mundo declararam (tanto em orientações quanto em acordos) que as configurações de cookies do navegador são uma indicação da preferência do usuário para opt out a definição de perfis. Especificamente, esses legisladores declararam que a configuração do navegador para bloquear cookies de terceiros é uma solicitação de não participação do rastreamento de terceiros (entre sites). Bloquear todos os cookies é uma solicitação de não participação para todo o rastreamento. Embora os identificadores do lado do servidor (como endereço IP ou agente do usuário) possam ser uma opção desejável que ignora as configurações do navegador de cookies, alguns legisladores os visualizações como uma evasão da escolha do usuário.