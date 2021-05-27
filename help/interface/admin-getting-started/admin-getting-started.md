---
description: Saiba como gerenciar permissões de usuário e perfis de produto da Adobe Experience Cloud. Saiba mais sobre como fazer logon no Adobe Admin Console e sobre o suporte de navegadores para a Experience Cloud.
solution: Admin
title: 'Gerenciamento de usuários e de produtos '
index: true
feature: Admin Console
topic: Administração
role: Administrator
level: Experienced
exl-id: af9eda5b-d984-44b7-a7b3-52dfc4e03d8f
source-git-commit: dc1d672c352396f919c239bf44e2162ff1deafb6
workflow-type: tm+mt
source-wordcount: '1415'
ht-degree: 97%

---

# Gerenciar usuários e produtos da Experience Cloud {#topic_3FCB4099640647E3B2411ADBFCE81909}

Saiba mais sobre como fazer logon no Admin Console, gerenciar permissões de usuário e perfis de produto da Experience Cloud e suporte ao navegador.

>[!IMPORTANT]
>
>O gerenciamento de usuários no Admin Console apresenta termos, interfaces e navegação novos. As informações a seguir descrevem essas alterações e fornecem links para recursos adicionais de ajuda. Esta ajuda complementa as informações no [Guia do usuário de administração de empresas](https://helpx.adobe.com/br/enterprise/managing/user-guide.html) para todos os produtos na nuvem da Adobe.

## Novidades no gerenciamento de usuários da Experience Cloud {#concept_06A0A13362F644FB90F947238407637A}

Saiba mais sobre os recursos mais recentes do gerenciamento de usuários e produtos da Experience Cloud.

<!-- ### Business ID type

Adobe is introducing an identity type called Business ID. This identity type improves the control of user and product management. Adobe is migrating all Adobe IDs (owned by individuals) that are used for business to the new enterprise Business IDs owned by your organization.

If you are an existing Experience Cloud customer, Adobe will migrate all your users with Adobe IDs in the Admin Console to Business IDs. If you are a new enterprise or teams customer, you will add users to the Admin Console using one of the available identity types: Business ID, Enterprise ID, or Federated ID.

What to do

* Your users will need to accept Terms of Use (TOU) changes prior to accounts being migrated to Type2e. 
* Users that belong to multiple organizations might see a Profile Selection screen during the login workflow and need to select the correct one. This ensures that they are logging into the correct organization. (There might be multiple profiles to choose from if a user was a member of multiple organizations before the migration.)

Beginning May 2020, enterprise administrators cannot use the Adobe ID for new organizations created in the Admin Console. Latest: https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=engage&title=Type2e+DX+GTM-->

### Ferramenta de administração

Os administradores podem exibir uma lista classificável e filtrável de todos os usuários da Experience Cloud e seus detalhes na Ferramenta de administração. Consulte [Exibir usuários da Experience Cloud na Ferramenta administrativa](admin-tool-experience-cloud.md).

## Fazer logon no Admin Console {#section_705072FD4EBE4B70BC69EC81F2BB8669}

Os administradores não gerenciam mais os usuários nas soluções de produto específicas. O gerenciamento de usuários e de produtos da Experience Cloud agora acontece no Admin Console.

Para fazer logon no Admin Console:

1. Navegue até [https://adminconsole.adobe.com/enterprise/](https://adminconsole.adobe.com/enterprise/#).
1. Digite sua [Adobe ID ou Enterprise ID](https://helpx.adobe.com/br/enterprise/help/identity.html) e senha.

Como alternativa, no menu da Experience Cloud (![](assets/menu-icon.png)), clique em **[!UICONTROL Administração]** > **[!UICONTROL Iniciar o Admin Console]**.

**Ajuda relacionada**

[Guia do usuário de administração](https://helpx.adobe.com/br/enterprise/using/users.html) para a Creative Cloud e a Document Cloud. Algumas informações são relevantes para o gerenciamento de usuários da Experience Cloud, como o [gerenciamento de tipos de identidade](https://helpx.adobe.com/enterprise/help/identity.html).

## Grupos e perfis de produto {#section_AB50558124D541CF80A0D3D76D35A4BF}

A adição dos perfis de produto marca uma mudança em como os produtos e serviços das soluções eram gerenciados anteriormente (com o uso de grupos). No Admin Console, as permissões são baseadas em perfis de produto, que são grupos de produtos e serviços que você pode atribuir aos usuários.

Por exemplo, no Analytics é possível configurar uma coleção de ferramentas de relatório, como a Analysis Workspace e o Report Builder, além de conjuntos de relatórios, métricas, dimensões e outros. É possível permitir que usuários acessem um perfil de produto ao adicioná-los ao perfil. Consulte [Atribuir permissões de acesso ao Analytics a um perfil de produto](../admin-getting-started/admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391) nesta página.

**Delegar direitos administrativos**

Consulte [Delegar privilégios administrativos limitados](../admin-getting-started/admin-getting-started.md#task_3A072C4AA9734BC59FFA7E015271BC7E) nesta página.

## Analytics {#section_97DE101F92CD494AB073893680992F1A}

Gerencie permissões de usuário e de produto do Analytics no Admin Console.

[Atribuir a um perfil de produto permissões de acesso ao Analytics](../admin-getting-started/admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391) (nesta página).

**Migração de contas de usuário**

Uma ferramenta de migração de IDs de usuário do Analytics está disponível para ajudar os administradores do Analytics a migrar contas de usuário do Gerenciamento de usuários do Analytics para o [Adobe Admin Console](https://adminconsole.adobe.com/enterprise/).

A migração das contas está acontecendo em fases. A Adobe vai notificá-lo e ajudá-lo quando chegar a sua hora de migrar as contas de usuário existentes de **[!UICONTROL Ferramentas administrativas]** > **[!UICONTROL Gerenciamento de usuários]** para o Admin Console.

Após a migração, os usuários farão logon usando sua Adobe ID (ou Enterprise ID) e se autenticarão em suas soluções e serviços do Experience Cloud em [experience.adobe.com](https://experience.adobe.com). Se os usuários tentarem fazer logon por meio de logons antigos ([!DNL my.omniture.com], [!DNL sc.omniture.com] e [!DNL experiencecloud.adobe.com]), serão redirecionados para [!DNL experience.adobe.com].

**Ajuda relacionada**

[Migração de IDs de usuários do Analytics](https://docs.adobe.com/content/help/pt-BR/analytics/admin/user-product-management/user-management/migrate-users/c-migration-tool.html)

## Adobe Target - perfis de produto versus espaços de trabalho {#section_3860AF177C9E4C7E9C390D36A414F353}

No Adobe Target, um espaço de trabalho é um perfil de produto. Ele permite que uma organização atribua um conjunto específico de usuários a um conjunto específico de propriedades. De muitas formas, um espaço de trabalho é semelhante a um conjunto de relatórios no Adobe Analytics.

Consulte:

* [Permissões de usuário empresarial](https://docs.adobe.com/content/help/pt-BR/target/using/administer/manage-users/enterprise/property-channel.html)
* [Gerenciar produtos e perfis](https://helpx.adobe.com/br/enterprise/using/manage-products-and-profiles.html)
* Vídeo: [Como configurar espaços de trabalho do Adobe Target no Adobe Admin Console](https://helpx.adobe.com/br/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

## Campaign - perfis de produto, locatários e grupos de segurança {#section_09CDF75366444CF5810CF321B7C712F3}

Um *locatário* do Campaign é exibido como um *produto* na página Produtos do Admin Console.

O *Grupo segurança* é exibido como um perfil de produto.

Consulte [Gerenciamento de grupos e usuários](https://docs.adobe.com/content/help/pt-BR/campaign-standard/using/administrating/users-and-security/managing-groups-and-users.html) para obter informações sobre grupos de segurança e atribuição de usuários a grupos de segurança.

## Experience Platform Launch {#section_F2DA6778DD2D48AA8F794041971EE6B1}

O Experience Platform Launch é exibido na página Produtos do Admin Console. É possível incluir outras soluções e serviços em um perfil de produto do Launch.

Consulte [Gerenciamento de usuários](https://docs.adobe.com/content/help/pt-BR/launch/using/reference/admin/user-permissions.html) para obter informações sobre permissões de usuário no Admin Console e configurar opções específicas do Launch, incluindo a atribuição de direitos a perfis.

## Experience Manager as a Cloud Service

Os clientes do Adobe Enterprise são representados como Organizações do IMS no Adobe Admin Console. Este é o portal usado pelos clientes da Adobe para gerenciar os direitos de produto para usuários e grupos. Os clientes do AEM podem usar o Adobe Admin Console para gerenciar seus direitos de produto e a autenticação IMS para o AEM as a Cloud Service.

Consulte [Suporte IMS para o AEM as a Cloud Service](https://docs.adobe.com/content/help/pt-BR/experience-manager-cloud-service/security/ims-support.html#managing-products-and-user-access-in-admin-console).

## Experience Platform Launch {#section_3A41CF2BD5994B9891537D063571D4ED}

Convide usuários para o [!UICONTROL Platform Launch] e atribua funções e direitos de usuário.

Consulte [Permissões de usuário](https://experienceleague.adobe.com/docs/launch/using/admin/user-permissions.html?lang=pt-BR#admin).

## Audience Manager {#section_C31E3FA8A1E14463B1B3E07235F1983C}

Crie usuários no Audience Manager e os atribua a grupos. Também é possível visualizar limites (características, segmentos, destinos e [!DNL AlgoModel]).

Consulte [Administração](https://docs.adobe.com/content/help/pt-BR/dtm/using/admin/users.html) na ajuda do Audience Manager.

## Gerenciar produtos da Experience Cloud {#task_16335111C52D40E9BAC73D0699584DBF}

Crie um perfil de produto e o atribua a um grupo de permissões.

Ao convidar um usuário para uma organização, é possível concedê-lo acesso a produtos e perfis de produtos. Também é possível delegar a um usuário permissões administrativas limitadas. De maneira similar, é possível criar grupos de usuários, e depois adicionar o grupo a um perfil de produto para habilitar o acesso.

1. No [Admin Console](https://adminconsole.adobe.com/enterprise/), clique em **[!UICONTROL Produtos]**.
1. Clique em **[!UICONTROL Novo perfil]**.
1. Configure os detalhes do perfil, e depois clique em **[!UICONTROL Próximo]**.
1. Clique em **[!UICONTROL Concluído]**.

Mais ajuda disponível em:

* [Gerenciar produtos e perfis](https://helpx.adobe.com/enterprise/using/manage-products-and-profiles.html)
* [Permissões de usuário corporativo](https://docs.adobe.com/content/help/en/target/using/administer/manage-users/enterprise/property-channel.html) na ajuda do Adobe Target para obter mais informações.
* Vídeo: [Como configurar espaços de trabalho do Adobe Target no Adobe Admin Console](https://helpx.adobe.com/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

## Atribuir a um perfil de produto permissões de acesso ao Analytics {#task_040673FE3E3E429B9531FBCB8B6A4391}

Atribuir a um perfil de produto permissões de acesso a relatórios do Analytics (conjuntos de relatórios, métricas, dimensões e outros).

Por exemplo, é possível criar um perfil de produto que contenha várias ferramentas do Analytics ([!UICONTROL Analysis Workspace], [!UICONTROL Reports &amp; Analytics] e [!UICONTROL Report Builder]), com permissão para métricas e dimensões específicas (inclusive eVars), e recursos como criação de segmentos ou de métricas calculadas.

1. Faça logon no [Admin Console](https://adminconsole.adobe.com/enterprise), depois clique em **[!UICONTROL Produtos]** (ou clique no nome do produto).
1. No perfil do produto, clique em **[!UICONTROL Permissões]** (disponível somente para administradores).
1. Configure as permissões do perfil:

| Elemento | Descrição |
|--- |--- |
| Conjuntos de relatórios | Ative permissões para conjuntos de relatórios específicos. |
| Métricas | Habilite permissões para tráfego, conversão, eventos personalizados, eventos de soluções e sensíveis a conteúdo, entre outros. |
| Dimensões | Personalize detalhadamente o acesso dos usuários, inclusive a eVars e relatórios de tráfego, de soluções e de definição de caminho. |
| Ferramentas do conjunto de relatórios | Habilite permissões do usuário para Serviços da Web, Gerenciamento de conjuntos de relatórios, Ferramentas e relatórios, além de Itens do painel. |
| Ferramentas do Analytics | Habilite permissões do usuário para obter integração a itens Gerais (faturas, logs etc.), Gerenciamento da empresa, Ferramentas, Acesso a serviços da Web, Report Builder e Data Connectors. As configurações da empresa feitas na categoria Personalizar o Admin Console foram movidas para as Ferramentas do Analytics. |

## Delegar funções administrativas aos usuários {#task_3A072C4AA9734BC59FFA7E015271BC7E}

No Admin Console, você pode delegar direitos administrativos limitados a outras pessoas em sua organização. As funções delegadas permitem que os usuários administrem acesso a software para usuários finais, fornecem acesso aos recursos de implantação e funcionam como delegados de suporte.

Por exemplo, você pode:

* Permitir que o diretor criativo conceda acesso à Creative Cloud.
* Permitir que o diretor de marketing conceda acesso à Experience Cloud.
* Mantenha essas duas funções separadas para que elas não possam ultrapassar as funções umas das outras.

Ao usar essas funções, você pode delegar simultaneamente o gerenciamento a outras pessoas sem fornecer mais recursos do que o necessário.

1. No Admin Console, clique em **[!UICONTROL Usuários]** e, em seguida, clique no nome do usuário.
1. Clique em **[!UICONTROL Editar direitos administrativos]**.
1. Configure os direitos de administrador do usuário.
1. Clique em **[!UICONTROL Próximo]** para analisar as configurações e clique em **[!UICONTROL Salvar]**.

## Navegadores suportados e requisitos de sistema {#concept_CDC4371EB9BF433E9534F8716DC8A088}

Navegadores compatíveis com a Experience Cloud.

* [!DNL Microsoft Edge] (a Microsoft [encerrou o suporte](https://www.microsoft.com/pt-br/WindowsForBusiness/End-of-IE-support) ao Internet Explorer 8, 9 e 10. Por esse motivo, a Adobe deixará de corrigir problemas relatados nessas versões do Internet Explorer.)
* [!DNL Google Chrome]
* [!DNL Firefox]
* [!DNL Safari]
* [!DNL Opera]

**Observação:** embora a interface da Experience Cloud seja compatível com esses navegadores, as soluções individuais podem não ser compatíveis com todos os navegadores. (Por exemplo, o [Analytics](https://docs.adobe.com/content/help/pt-BR/analytics/admin/sys-reqs.html) não é compatível com o [!DNL Opera] e o [ Adobe Target](https://docs.adobe.com/help/pt-BR/target/using/implement-target/before-implement/supported-browsers.html) não é compatível com o [!DNL Safari].)

### Requisitos da solução e do produto

* [Analytics](https://docs.adobe.com/content/help/en/analytics/admin/sys-reqs.html)
* [Report Builder](https://docs.adobe.com/content/help/pt-BR/analytics/analyze/report-builder/report-builder-setup/system-requirements.html)
* [Adobe Target](https://docs.adobe.com/help/en/target/using/implement-target/before-implement/supported-browsers.html)
