---
description: Remova os usuários que bloquearam todos os cookies em navegadores de computadores e de dispositivos móveis.
keywords: cookies; privacidade
seo-description: Remova os usuários que bloquearam todos os cookies em navegadores de computadores e de dispositivos móveis.
seo-title: Ativar as configurações de privacidade de cookies do navegador
solution: Experience Cloud,Analytics,Target,Social
title: Ativar as configurações de privacidade de cookies do navegador
uuid: f6a56e8b-b021-49db-8eb4-6c14af0c7243
index: y
internal: n
snippet: y
translation-type: tm+mt
source-git-commit: 426c1fecf16e1cf83cd28971e4de6fdb66b0e10d

---


# Ativar as configurações de privacidade de cookies do navegador{#enable-privacy-settings-for-browser-cookies}

Remova os usuários que bloquearam todos os cookies em navegadores de computadores e de dispositivos móveis.

Esta configuração permite respeitar a intenção de um usuário de parar o processamento do Analytics caso opte por bloquear todos os cookies nas configurações de cookies do navegador.

1. Navegue até **[!UICONTROL Ferramentas administrativas]** &gt; **[!UICONTROL Conjuntos de relatórios]**.
1. Clique em **[!UICONTROL Editar configurações]** &gt; **[!UICONTROL Geral]** &gt; **[!UICONTROL Configurações de privacidade]**.
1. Ativar as **[!UICONTROL Configurações de privacidade]** (para desktop ou dispositivos móveis).

   Ao ativar este recurso, os dados coletados em navegadores de computadores e de dispositivos móveis nos quais o usuário definiu seu navegador para bloquear todos os cookies serão excluídos dos relatórios do Analytics. Se a Adobe não reconhecer o navegador, os dados serão incluídos nos relatórios do Analytics.

>[!IMPORTANT]
>
>Observe que muitos aplicativos móveis (como o navegador interno do Facebook ou do Twitter) podem parecer navegadores de dispositivos móveis padrão, mas não permitem todos os cookies. Ativar este recurso pode excluir uma grande proporção de tráfego de dispositivos móveis dos relatórios do Analytics.

**Sobre as configurações de privacidade do navegador**

As orientações legislativas e regulamentares expressaram que a ação de um usuário ao bloquear cookies é similar à ação de um usuário ao evitar a identificação. Ao ativar este recurso, os dados coletados em navegadores de computadores e de dispositivos móveis nos quais o usuário definiu seu navegador para bloquear todos os cookies serão excluídos dos relatórios do Analytics. Se a Adobe não reconhecer o navegador da Web, os dados serão incluídos nos relatórios do Analytics.

Legisladores em todo o mundo determinaram (em orientações e declarações) que as configurações de cookies do navegador são uma indicação da preferência do usuário de rejeitar a determinação de perfis. Especificamente, esses legisladores definiram que a configuração do navegador para bloquear cookies de terceiros é uma solicitação para rejeitar o rastreamento de terceiros (entre sites); e o bloqueio de todos os cookies é uma solicitação para rejeitar todos os rastreamentos. Embora identificadores do lado do servidor (como endereço IP ou agente de usuário) possam ser uma opção desejável para ignorar as configurações de cookies do navegador, alguns legisladores os consideram uma evasão da escolha do usuário.