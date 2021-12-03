---
title: Gerenciar usuários e produtos
description: Saiba como fazer logon no Admin Console e gerenciar permissões de usuário e perfis de produto da Experience Cloud. Saiba mais sobre como delegar direitos administrativos a usuários da Experience Cloud e sobre o suporte a navegador na Experience Cloud.
solution: Admin
index: true
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: af9eda5b-d984-44b7-a7b3-52dfc4e03d8f
source-git-commit: 3507af336715eb3664f8ce5176ddaf74ecbd7bcd
workflow-type: tm+mt
source-wordcount: '1281'
ht-degree: 100%

---

# Gerenciar usuários e produtos da Experience Cloud

Saiba mais sobre como fazer logon no Admin Console, gerenciar permissões de usuário e perfis de produto da Experience Cloud e suporte ao navegador.

>[!IMPORTANT]
>
>As informações a seguir são especificamente para aplicativos da Experience Cloud. Essas informações complementam as informações administrativas mais amplas no [Guia do usuário de administração corporativa](https://helpx.adobe.com/br/enterprise/admin-guide.html) para todos os produtos de nuvem da Adobe.

Você pode ver uma lista classificável e filtrável de todos os usuários da Experience Cloud e seus detalhes na Ferramenta do administrador. Consulte [Exibir usuários da Experience Cloud na Ferramenta administrativa](admin-tool-experience-cloud.md).

## O que é um perfil de produto? {#section_AB50558124D541CF80A0D3D76D35A4BF}

[!UICONTROL Perfis de produto] são grupos de produtos e serviços que podem ser atribuídos a usuários. Na Experience Cloud, as permissões se baseiam no perfil de um produto, não no usuário. (No entanto, você pode delegar direitos administrativos a usuários específicos.)

Por exemplo, no Analytics é possível configurar uma coleção de ferramentas de relatório, como o Analysis Workspace e o Report Builder, além de conjuntos de relatórios, métricas e dimensões. Você pode conceder permissão a um perfil de produto adicionando usuários ao perfil.

* Consulte [Atribuir permissões de acesso ao Analytics a um perfil de produto](admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391) nesta página.
* Consulte [Delegar funções administrativas a usuários](#delegate-rights) nesta página

## Gerenciar perfis de produto da Experience Cloud {#task_16335111C52D40E9BAC73D0699584DBF}

Você pode criar um perfil de produto e atribuí-lo a um grupo de permissão.

Ao convidar um usuário para uma organização, é possível concedê-lo acesso a produtos e perfis de produtos. Também é possível delegar a um usuário permissões administrativas limitadas. De maneira similar, é possível criar grupos de usuários, e depois adicionar o grupo a um perfil de produto para habilitar o acesso.

1. No [Admin Console](https://adminconsole.adobe.com/enterprise/), selecione **[!UICONTROL Produtos]**.
1. Clique no nome da sua organização.
1. Selecione **[!UICONTROL Novo perfil]**.
1. Configure os detalhes do perfil e selecione **[!UICONTROL Salvar]**.

Para obter mais informações (e para obter ajuda sobre o gerenciamento de produto da Creative Cloud e da Document Cloud), consulte [Identidade](https://helpx.adobe.com/br/enterprise/admin-guide.html/br/enterprise/using/identity.ug.html) no [Guia do usuário de administração](https://helpx.adobe.com/br/enterprise/admin-guide.html/br/enterprise/using/users.ug.html).

**Ajuda relacionada**

* [Gerenciar produtos e perfis](https://helpx.adobe.com/br/enterprise/admin-guide.html/br/enterprise/using/manage-products.ug.html) no Guia do usuário de administração.
* [Permissões de usuário corporativo](https://experienceleague.adobe.com/docs/target/using/administer/manage-users/enterprise/property-channel.html?lang=pt-BR) na ajuda do Adobe Target para obter mais informações.
* Vídeo: [Como configurar espaços de trabalho do Adobe Target no Adobe Admin Console](https://helpx.adobe.com/br/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

<!-- ## What's new in Experience Cloud user management {#concept_06A0A13362F644FB90F947238407637A}

Learn about the latest features in Experience Cloud user and product management.

### Business ID type

Adobe is introducing an identity type called Business ID. This identity type improves the control of user and product management. Adobe is migrating all Adobe IDs (owned by individuals) that are used for business to the new enterprise Business IDs owned by your organization.

If you are an existing Experience Cloud customer, Adobe will migrate all your users with Adobe IDs in the Admin Console to Business IDs. If you are a new enterprise or teams customer, you will add users to the Admin Console using one of the available identity types: Business ID, Enterprise ID, or Federated ID.

What to do

* Your users will need to accept Terms of Use (TOU) changes prior to accounts being migrated to Type2e. 
* Users that belong to multiple organizations might see a Profile Selection screen during the login workflow and need to select the correct one. This ensures that they are logging into the correct organization. (There might be multiple profiles to choose from if a user was a member of multiple organizations before the migration.)

Beginning May 2020, enterprise administrators cannot use the Adobe ID for new organizations created in the Admin Console. Latest: https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=engage&title=Type2e+DX+GTM-->

## Delegar funções administrativas aos usuários {#delegate-rights}

No Admin Console, você pode delegar direitos administrativos limitados a outras pessoas em sua organização. As funções delegadas permitem que os usuários administrem acesso a software para usuários finais, fornecem acesso aos recursos de implantação e funcionam como delegados de suporte.

Por exemplo, você pode:

* Permitir que o diretor criativo conceda acesso à Creative Cloud.
* Permitir que o diretor de marketing conceda acesso à Experience Cloud.
* Mantenha essas duas funções separadas para que elas não possam ultrapassar as funções umas das outras.

Ao usar essas funções, você pode delegar simultaneamente o gerenciamento a outras pessoas sem fornecer mais recursos do que o necessário.

1. No Admin Console, selecione **[!UICONTROL Usuários]** e, em seguida, selecione o nome do usuário.

   ![Direitos administrativos no Admin Console](assets/edit-admin-rights.png)

1. Selecione **[!UICONTROL Editar direitos do administrador]**.

   ![Editar direitos administrativos no Admin Console](assets/edit-admin-rights-page.png)

1. Especifique os direitos de administrador do usuário.
1. Selecione **[!UICONTROL Salvar]**.

## Gerenciar usuários e produtos do Analytics {#section_97DE101F92CD494AB073893680992F1A}

Você pode atribuir permissões de acesso a relatórios do Analytics (conjuntos de relatórios, métricas, dimensões e assim por diante) a um perfil de produto.

Por exemplo, você pode criar um perfil de produto que contenha várias ferramentas do Analytics ([!UICONTROL Analysis Workspace], [!UICONTROL Reports &amp; Analytics] e [!UICONTROL Report Builder]). Esses perfis contêm permissão para métricas e dimensões específicas (incluindo eVars) e recursos como segmentos ou criação de métricas calculadas.

1. Faça logon no [Admin Console](https://adminconsole.adobe.com/enterprise) e clique em **[!UICONTROL Produtos]**.
1. Na página [!UICONTROL Produtos], clique no produto e, em seguida, clique em **[!UICONTROL Permissões]** (disponível somente para administradores).
1. Configure as permissões do perfil:

| Elemento | Descrição |
|--- |--- |
| Conjuntos de relatórios | Ative permissões para conjuntos de relatórios específicos. |
| Métricas | Habilite permissões para tráfego, conversão, eventos personalizados, eventos de aplicativos, sensibilidade de conteúdo, entre outros. |
| Dimensões | Personalize detalhadamente o acesso dos usuários, incluindo eVars e relatórios de tráfego, de aplicativos e de caminho. |
| Ferramentas do conjunto de relatórios | Habilite permissões do usuário para Serviços da Web, Gerenciamento de conjuntos de relatórios, Ferramentas e relatórios, além de Itens do painel. |
| Ferramentas do Analytics | Habilite as permissões do usuário para itens gerais (faturamento, logs e assim por diante), Gerenciamento da empresa, Ferramentas, Acesso a serviços da Web, Report Builder e Integração de Data Connectors. As configurações da empresa feitas na categoria Personalizar o Admin Console foram movidas para as Ferramentas do Analytics. |

**Migração de contas de usuário**

Uma ferramenta de migração de IDs de usuário do Analytics está disponível para ajudar os administradores do Analytics a migrar contas de usuário do Gerenciamento de usuários do Analytics para o [Adobe Admin Console](https://adminconsole.adobe.com/enterprise/).

A migração das contas está acontecendo em fases. A Adobe vai notificá-lo e ajudá-lo quando chegar a sua hora de migrar as contas de usuário existentes de **[!UICONTROL Ferramentas administrativas]** > **[!UICONTROL Gerenciamento de usuários]** para o Admin Console.

Após a migração, os usuários fazem logon com a Adobe ID (ou Enterprise ID) e se autenticam em seus aplicativos e serviços da Experience Cloud em [experience.adobe.com](https://experience.adobe.com). Se os usuários tentarem fazer logon por meio de logins herdados ([!DNL my.omniture.com], [!DNL sc.omniture.com] e [!DNL experiencecloud.adobe.com]) eles serão redirecionados para [!DNL experience.adobe.com].

**Ajuda relacionada**

Para obter mais informações, consulte [Migração de IDs de usuários do Analytics](https://experienceleague.adobe.com/docs/analytics/admin/user-product-management/migrate-users/c-migration-tool.html?lang=pt-BR).

## Gerenciar o Adobe Target — perfis de produto vs. espaços de trabalho {#section_3860AF177C9E4C7E9C390D36A414F353}

No Adobe Target, um espaço de trabalho é um perfil de produto. Ele permite que uma organização atribua um conjunto específico de usuários a um conjunto específico de propriedades. De muitas formas, um espaço de trabalho é semelhante a um conjunto de relatórios no Adobe Analytics.

Consulte:

* [Permissões de usuário empresarial](https://experienceleague.adobe.com/docs/target/using/administer/manage-users/enterprise/property-channel.html?lang=en)
* [Gerenciar produtos e perfis](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/manage-products.ug.html)
* Vídeo: [Como configurar espaços de trabalho do Adobe Target no Adobe Admin Console](https://helpx.adobe.com/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

## Gerenciar perfis de produtos, locatários e grupos de segurança do Campaign {#section_09CDF75366444CF5810CF321B7C712F3}

Um *locatário* do Campaign é exibido como um *produto* na página Produtos do Admin Console.

O *Grupo segurança* é exibido como um perfil de produto.

Consulte [Gerenciamento de grupos e usuários](https://experienceleague.adobe.com/docs/campaign-standard/using/administrating/users-and-security/managing-groups-and-users.html?lang=pt-BR) para obter informações sobre grupos de segurança e atribuição de usuários a grupos de segurança.

## Gerenciar a coleta de dados da Experience Platform (Launch) {#section_F2DA6778DD2D48AA8F794041971EE6B1}

A coleção de dados da [!UICONTROL Experience Platform] ([!UICONTROL Launch]) é exibida na página [!UICONTROL Produtos] no [!UICONTROL Admin Console]. É possível incluir outros aplicativos e serviços em um perfil de produto do Launch.

Convide usuários para o [!UICONTROL Platform Launch] e atribua funções e direitos de usuário.

Consulte [Permissões de usuário](https://experienceleague.adobe.com/docs/experience-platform/tags/admin/user-permissions.html?lang=pt-BR) para obter informações sobre as permissões do usuário no Admin Console e sobre a configuração de opções específicas do Launch, incluindo a atribuição de direitos aos perfis.

## Experience Manager as a Cloud Service

Os clientes da Adobe Enterprise são representados como Organizações no Adobe [!UICONTROL Admin Console]. Os clientes do Experience Manager podem usar o Adobe [!UICONTROL Admin Console] para gerenciar direitos de produto e autenticação IMS para o Experience Manager as a [!UICONTROL Cloud Service].

Consulte [Suporte de IMS para o Experience Manager as a Cloud Service](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/security/ims-support.html?lang=pt-BR).

## Audience Manager {#section_C31E3FA8A1E14463B1B3E07235F1983C}

Crie usuários no Audience Manager e os atribua a grupos. Também é possível visualizar limites (características, segmentos, destinos e [!DNL AlgoModel]).

Consulte [Administração](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/administration/administration-overview.html?lang=pt-BR) na ajuda do Audience Manager.

## Navegadores compatíveis com a Experience Cloud

* [!DNL Microsoft® Edge] (A Microsoft® [encerrou o suporte](https://www.microsoft.com/pt-br/WindowsForBusiness/End-of-IE-support) para o Internet Explorer 8, 9 e 10. Por esse motivo, a Adobe deixará de corrigir problemas relatados nessas versões específicas do Internet Explorer.)
* [!DNL Google Chrome]
* [!DNL Firefox]
* [!DNL Safari]
* [!DNL Opera]

**Observação:** embora a interface da Experience Cloud seja compatível esses navegadores, os aplicativos individuais não oferecem suporte a todos os navegadores. (Por exemplo, o [Analytics](https://experienceleague.adobe.com/docs/analytics/admin/sys-reqs.html?lang=pt-BR) não é compatível com o [!DNL Opera] e o [ Adobe Target](https://experienceleague.adobe.com/docs/target/using/implement-target/before-implement/supported-browsers.html?lang=pt-BR) não é compatível com o [!DNL Safari].)

### Requisitos da solução e do produto

* [Analytics](https://experienceleague.adobe.com/docs/analytics/admin/sys-reqs.html?lang=en)
* [Report Builder](https://experienceleague.adobe.com/docs/analytics/analyze/report-builder/report-builder-setup/system-requirements.html?lang=pt-BR)
* [Adobe Target](https://experienceleague.adobe.com/docs/target/using/implement-target/before-implement/supported-browsers.html?lang=en)
