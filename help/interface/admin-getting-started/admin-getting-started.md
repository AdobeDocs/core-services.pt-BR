---
description: Saiba mais sobre como fazer logon no Admin Console, gerenciar permissões de usuário e perfis de produto da Experience Cloud e suporte ao navegador.
keywords: core services
seo-description: Saiba mais sobre como fazer logon no Admin Console, gerenciar permissões de usuário e perfis de produto da Experience Cloud e suporte ao navegador.
seo-title: Gerenciar usuários e produtos da Experience Cloud
solution: Experience Cloud
title: Gerenciar usuários e produtos da Experience Cloud
index: true
translation-type: tm+mt
source-git-commit: e54747dc6ff4e52b893924c5e0ebfa91ba824538

---


# Gerenciar usuários e produtos da Experience Cloud {#topic_3FCB4099640647E3B2411ADBFCE81909}

Saiba mais sobre como fazer logon no Admin Console, gerenciar permissões de usuário e perfis de produto da Experience Cloud e suporte ao navegador.

>[!IMPORTANT]
>
>O gerenciamento de usuários no Admin Console apresenta termos, interfaces e navegação novos. As informações a seguir descrevem essas alterações e fornecem links para recursos adicionais de ajuda. This help supplements the information in the [Enterprise Administration User Guide](https://helpx.adobe.com/enterprise/managing/user-guide.html) for all Adobe cloud products.

## Novidades no gerenciamento de usuários da Experience Cloud {#concept_06A0A13362F644FB90F947238407637A}

Saiba mais sobre os recursos mais recentes do gerenciamento de usuários da Experience Cloud.

<!-- ### Business ID type

Adobe is introducing an identity type called _Business ID_. This identity type improves the control of user and product management. Adobe is migrating all Adobe IDs (owned by individuals) that are used for business to the new enterprise Business IDs owned by your organization.

If you are an existing Experience Cloud customer, Adobe will migrate all your users on the Admin Console with Adobe IDs to Business IDs. If you are a new enterprise or teams customer, you will add users to the Admin Console using one of the available identity types: Business ID, Enterprise ID, or Federated ID.

Beginning May 2020, enterprise administrators cannot use the Adobe ID for new organizations created in the Admin Console. Latest: https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=engage&title=Type2e+DX+GTM

What to do

* Your users will need to accept Terms of Use (TOU) changes prior to accounts being migrated to Type2e. 
* Users that belong to multiple organizations might see a Profile Selection screen during the login workflow and need to select the correct one. This ensures that they are logging into the correct organization. (There might be multiple profiles to choose from if a users was a member of multiple organizations before the migration.) -->

### Ferramenta de administração

Os administradores podem visualização uma lista classificável e filtrável de todos os usuários da Experience Cloud e seus detalhes na Ferramenta de administração. Consulte Usuários da Experience Cloud da [Visualização na Ferramenta](admin-tool-experience-cloud.md)administrativa.

## Fazer logon no Admin Console {#section_705072FD4EBE4B70BC69EC81F2BB8669}

Os administradores não gerenciam mais os usuários nas soluções. O gerenciamento de usuários e produtos da Experience Cloud ocorre agora no Admin Console.

Para fazer logon no Admin Console:

1. Navigate to [https://adminconsole.adobe.com/enterprise/](https://adminconsole.adobe.com/enterprise/#).
1. Digite sua [Adobe ID ou Enterprise ID](https://helpx.adobe.com/enterprise/help/identity.html) e senha.

Alternatively, from the Experience Cloud menu ( ![](assets/menu-icon.png)), click **[!UICONTROL Administration]** > **[!UICONTROL Launch Admin Console]**.

**Ajuda relacionada**

[Guia](https://helpx.adobe.com/enterprise/using/users.html) do usuário de administração para a Creative Cloud e a Documento Cloud. Algumas informações são relevantes para o gerenciamento de usuários da Experience Cloud, como o [gerenciamento de tipos](https://helpx.adobe.com/enterprise/help/identity.html)de identidade.

[Faça logon e gerencie suas configurações](../admin-getting-started/getting-started-experience-cloud.md#topic_AC564B6795334DE39359ADD87F52F2E0) de perfil para gerenciar senhas, organizações e notificações.

## perfis e grupos de produtos {#section_AB50558124D541CF80A0D3D76D35A4BF}

A adição de perfis de produtos marca uma mudança na forma como os produtos e serviços da solução eram gerenciados anteriormente (usando grupos). No Admin Console, as permissões se baseiam em perfis de produtos, que são grupos de produtos e serviços que você pode atribuir aos usuários.

Por exemplo, no Analytics, é possível configurar uma coleção de ferramentas de relatórios, como a Área de trabalho da Análise e o Construtor de relatórios, além de conjuntos de relatórios, métricas, dimensões e assim por diante. Você pode permitir que os usuários acessem um perfil de produto adicionando-os ao perfil. See [Assign Analytics access permissions to a product profile](../admin-getting-started/admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391).

**Ajuda relacionada**

[Delegar privilégios de administração limitados](../admin-getting-started/admin-getting-started.md#task_3A072C4AA9734BC59FFA7E015271BC7E)

## Analytics {#section_97DE101F92CD494AB073893680992F1A}

Gerencie permissões de usuário e de produto do Analytics no Admin Console.

[Atribuir a um perfil de produto permissões de acesso ao Analytics](../admin-getting-started/admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391) (nesta página).

**Migração de contas de usuário**

Uma ferramenta de migração de IDs de usuário do Analytics está disponível para ajudar os administradores do Analytics a migrar contas de usuário do Gerenciamento de usuários do Analytics para o [Adobe Admin Console](https://adminconsole.adobe.com/enterprise/).

A migração das contas está acontecendo em fases. Adobe will notify and assist you when it is your time to migrate existing user accounts from **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** to the Admin Console.

After the migration, users sign in using their Adobe ID (or Enterprise ID) and authenticate to their Experience Cloud solutions and services at [experiencecloud.adobe.com](https://experiencecloud.adobe.com). Se algum usuário tentar fazer logon por meio de logons antigos ([!DNL my.omniture.com] e [!DNL sc.omniture.com]), será redirecionado para [!DNL experiencecloud.adobe.com].

**Ajuda relacionada**

[Migração de IDs de usuários do Analytics](https://docs.adobe.com/content/help/en/analytics/admin/user-product-management/user-management/migrate-users/c-migration-tool.html)

## Adobe Target - product profiles vs workspaces {#section_3860AF177C9E4C7E9C390D36A414F353}

No Adobe Público alvo, um espaço de trabalho é um perfil de produto. Ela permite que uma organização atribua um conjunto específico de usuários a um conjunto específico de propriedades. De muitas formas, um espaço de trabalho é semelhante a um conjunto de relatórios no Adobe Analytics.

Consulte:
* [Permissões de usuário empresarial](https://docs.adobe.com/content/help/en/target/using/administer/manage-users/enterprise/property-channel.html)
* [Gerenciar produtos e perfis](https://helpx.adobe.com/enterprise/using/manage-products-and-profiles.html)
* Vídeo: [Como configurar espaços de trabalho do Público alvo no Adobe Admin Console](https://helpx.adobe.com/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

## Campaign - perfis de produto, locatários e grupos de segurança {#section_09CDF75366444CF5810CF321B7C712F3}

Um *locatário* na Campanha é exibido como um *produto* na página Produtos do Admin Console.

*O grupo* Segurança é exibido como um perfil de produto.

Consulte [Gerenciamento de grupos e usuários](https://helpx.adobe.com/campaign/standard/administration/using/managing-groups-and-users.html) para obter informações sobre grupos de segurança e atribuição de usuários a grupos de segurança.

## Experience Platform Launch {#section_F2DA6778DD2D48AA8F794041971EE6B1}

O Experience Platform Launch é exibido na página Produtos no Admin Console. Você pode incluir outras soluções e serviços em um perfil de produto do Launch.

Consulte Gerenciamento [de](https://docs.adobelaunch.com/launch-reference/administration/user-permissions) usuários para obter informações sobre permissões de usuário no Admin Console e configurar opções específicas do Launch, incluindo a atribuição de direitos a perfis.

## Gerenciador dinâmico de tags {#section_3A41CF2BD5994B9891537D063571D4ED}

Convide usuários para o Dynamic Tag Management, atribua funções de usuário e adicione usuários a grupos.

See [Users and Permissions](https://docs.adobe.com/content/help/en/dtm/using/admin/users.html) for information about how to invite users to Dynamic Tag Management and assign user roles and add users to groups.

## Audience Manager {#section_C31E3FA8A1E14463B1B3E07235F1983C}

Crie usuários do Gerenciador de Audiências e os atribua a grupos. Você também pode visualização de limites (características, segmentos, destinos e [!DNL AlgoModel]).

Consulte [Administração](https://docs.adobe.com/content/help/en/dtm/using/admin/users.html) na ajuda do Gerenciador de Audiências.

## Gerenciar produtos da Experience Cloud {#task_16335111C52D40E9BAC73D0699584DBF}

Crie um perfil de produto e atribua-o a um grupo de permissões.

Ao convidar um usuário para uma organização, você pode conceder ao usuário acesso a produtos e perfis de produtos. Você também pode delegar permissões administrativas limitadas a um usuário. Da mesma forma, você pode criar grupos de usuários e, em seguida, adicionar o grupo a um perfil de produto para habilitar o acesso.

1. In the [Admin Console](https://adminconsole.adobe.com/enterprise/), click **[!UICONTROL Products]**.
1. Clique em **[!UICONTROL Novo perfil]**.
1. Configure os detalhes do perfil, e depois clique em **[!UICONTROL Próximo]**.
1. Clique em **[!UICONTROL Concluído]**.

Mais ajuda está disponível em:

* [Gerenciar produtos e perfis](https://helpx.adobe.com/enterprise/using/manage-products-and-profiles.html)
* [Permissões](https://docs.adobe.com/content/help/en/target/using/administer/manage-users/enterprise/property-channel.html) de usuário corporativo na ajuda do Público alvo Adobe para obter mais informações.
* Vídeo: [Como configurar espaços de trabalho do Público alvo no Adobe Admin Console](https://helpx.adobe.com/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

## Atribuir a um perfil de produto permissões de acesso ao Analytics {#task_040673FE3E3E429B9531FBCB8B6A4391}

Atribuir a um perfil de produto permissões de acesso a relatórios do Analytics (conjuntos de relatórios, métricas, dimensões e outros).

Por exemplo, é possível criar um perfil de produto que contenha várias ferramentas do Analytics ([!UICONTROL Analysis Workspace], [!UICONTROL Reports &amp; Analytics] e [!UICONTROL Report Builder]), com permissão para métricas e dimensões específicas (inclusive eVars), e recursos como criação de segmentos ou de métricas calculadas.

1. Sign in to the [Admin Console](https://adminconsole.adobe.com/enterprise), then click **[!UICONTROL Products]** (or click your product name).
1. No perfil do produto, clique em **[!UICONTROL Permissões]** (disponível somente para administradores).
1. Configure as permissões do perfil:

| Elemento | Descrição |
|--- |--- |
| Conjuntos de relatórios | Ative permissões para conjuntos de relatórios específicos. |
| Métricas | Ative permissões para tráfego, conversão, eventos personalizados, eventos de solução, sensíveis a conteúdo e assim por diante. |
| Dimensões | Personalize o acesso do usuário em um nível granular, incluindo eVars, relatórios de tráfego, relatórios de solução e relatórios de caminho. |
| Ferramentas do conjunto de relatórios | Ative permissões de usuário para Serviços da Web, Gerenciamento de conjuntos de relatórios, Ferramentas e relatórios e Itens de Painel. |
| Ferramentas do Analytics | Habilite permissões do usuário para obter integração a itens Gerais (faturas, logs etc.), Gerenciamento da empresa, Ferramentas, Acesso a serviços da Web, Report Builder e Data Connectors. As configurações da empresa feitas na categoria Personalizar o Admin Console foram movidas para as Ferramentas do Analytics. |

## Delegar funções administrativas aos usuários {#task_3A072C4AA9734BC59FFA7E015271BC7E}

No Admin Console, você pode delegar direitos administrativos limitados a outras pessoas em sua organização. As funções delegadas permitem que os usuários administrem acesso a software para usuários finais, fornecem acesso aos recursos de implantação e funcionam como delegados de suporte.

Por exemplo, você pode:

* Permita que o diretor criativo conceda acesso à Creative Cloud.
* Permita que o diretor de marketing conceda acesso à Experience Cloud.
* Mantenha essas duas funções separadas para que elas não possam ultrapassar as funções umas das outras.

Ao usar essas funções, você pode delegar simultaneamente o gerenciamento a outras pessoas sem fornecer mais recursos do que o necessário.

1. No Admin Console, clique em **[!UICONTROL Usuários]** e, em seguida, clique no nome do usuário.
1. Clique em **[!UICONTROL Editar direitos administrativos]**.
1. Configure os direitos de administrador do usuário.
1. Clique em **[!UICONTROL Próximo]** para analisar as configurações e clique em **[!UICONTROL Salvar]**.

## Navegadores suportados e requisitos de sistema {#concept_CDC4371EB9BF433E9534F8716DC8A088}

Navegadores compatíveis na Experience Cloud.

* [!DNL Microsoft Edge] (A Microsoft [encerrou o suporte](https://www.microsoft.com/en-us/WindowsForBusiness/End-of-IE-support) para o Internet Explorer 8, 9 e 10. Assim, a Adobe não corrigirá problemas relatados nessas versões específicas do Internet Explorer.)
* [!DNL Google Chrome]
* [!DNL Firefox]
* [!DNL Safari]
* [!DNL Opera]

**Observação:** embora a interface da Experience Cloud seja compatível com esses navegadores, as soluções individuais podem não ser compatíveis com todos os navegadores. (For example, [Analytics](https://docs.adobe.com/content/help/en/analytics/admin/sys-reqs.html) does not support [!DNL Opera], and [Adobe Target](https://docs.adobe.com/help/en/target/using/implement-target/before-implement/supported-browsers.html) does not support [!DNL Safari].)

### Requisitos da solução e do produto

* [Analytics](https://docs.adobe.com/content/help/en/analytics/admin/sys-reqs.html)
* [Report Builder](https://docs.adobe.com/content/help/en/analytics/analyze/report-builder/report-builder-setup/system-requirements.html)
* [Adobe Target](https://docs.adobe.com/help/en/target/using/implement-target/before-implement/supported-browsers.html)
