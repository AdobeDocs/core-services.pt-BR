---
description: Saiba mais sobre como fazer logon no Admin Console e gerenciar permissões de usuário e perfis de produto da Experience Cloud.
keywords: principais serviços
seo-description: Saiba mais sobre como fazer logon no Admin Console e gerenciar permissões de usuário e perfis de produto da Experience Cloud.
seo-title: Gerenciar usuários e produtos da Experience Cloud
solution: Marketing Cloud
title: Gerenciar usuários e produtos da Experience Cloud
uuid: aea4e4c3-f543-4e8d-b553-d838418477d6
translation-type: ht
source-git-commit: 979b2202a70e2a5362aa86a65a17d7c4279b3a1a

---


# Gerenciar usuários e produtos da Experience Cloud {#topic_3FCB4099640647E3B2411ADBFCE81909}

Saiba mais sobre como fazer logon no Admin Console e gerenciar permissões de usuário e perfis de produto da Experience Cloud.


<!-- marketing-cloud-identity-management.xml -->

<!-- user_mgmt_admin.xml -->

<!-- domain change for 2018 
<ul id="ul_6654B3993EBE4DE0A3FBCFA5173A52D1"> 
 <li id="li_BE41EB31960B4C079E864FAA2E322BB4"> Private Beta - Support new domain alongside old domain for selected customers (June, 2018) </li> 
 <li id="li_0513CA457FAA4F37A9D5E514DEAF2067"> General Rollout - Serve both old and new domains seamlessly for all customers (Aug, 2018) </li> 
 <li id="li_AB89A6D00A274EB7863D0243757322DE"> Public Beta - Drive solution teams and customers to switch references from old domain to new domain (Aug - Oct, 2018) </li> 
 <li id="li_6FED48B1F361493082102E823EA335F4"> General Availability - Redirect all old domain requests to new domain (Oct, 2018) </li> 
</ul> -->

>[!IMPORTANT]
>
>O gerenciamento de usuários no Admin Console apresenta termos, interfaces e navegação novos. As informações a seguir descrevem essas alterações e fornecem links para recursos adicionais de ajuda. Esta ajuda complementa as informações no [Guia do usuário de administração de empresas](https://helpx.adobe.com/br/enterprise/managing/user-guide.html) para todos os produtos na nuvem da Adobe.

## Novidades no gerenciamento de usuários da Experience Cloud {#concept_06A0A13362F644FB90F947238407637A}

Saiba mais sobre os recursos mais recentes do gerenciamento de usuários da Experience Cloud.


## Fazer logon no Admin Console {#section_705072FD4EBE4B70BC69EC81F2BB8669}

Administradores não gerenciam mais os usuários nas soluções. O gerenciamento de usuários e de produtos da Experience Cloud agora acontece no Admin Console.

**Para fazer logon no Admin Console**

1. Navegue até [https://adminconsole.adobe.com/enterprise/](https://adminconsole.adobe.com/enterprise/#).
1. Digite sua [Adobe ID ou Enterprise ID](https://helpx.adobe.com/br/enterprise/help/identity.html) e senha.


Como alternativa, no menu da Experience Cloud ( ![](assets/menu-icon.png) ), clique em **[!UICONTROL Administração]** &gt; **[!UICONTROL Iniciar o Admin Console]**.

**Ajuda relacionada**

[Guia do usuário de administração](https://helpx.adobe.com/br/enterprise/using/users.html) para a Creative Cloud e Document Cloud. Algumas informações são relevantes para o gerenciamento de usuários da Experience Cloud, como [o gerenciamento dos tipos de identidade](https://helpx.adobe.com/br/enterprise/help/identity.html).

[Fazer logon e gerenciar as configurações do seu perfil](../admin-getting-started/getting-started-experience-cloud.md#topic_AC564B6795334DE39359ADD87F52F2E0) para gerenciar senhas, organizações e notificações.

## Grupos e perfis de produto {#section_AB50558124D541CF80A0D3D76D35A4BF}

A adição dos perfis de produto marca uma mudança em como os produtos e serviços das soluções eram gerenciados anteriormente (com o uso de grupos). No Admin Console, as permissões são baseadas em perfis de produto, que são grupos de produtos e serviços que você pode atribuir aos usuários.

Por exemplo, no Analytics é possível configurar uma coleção de ferramentas de relatório, como a Analysis Workspace e o Report Builder, além de conjuntos de relatórios, métricas, dimensões e outros. É possível permitir que usuários acessem um perfil de produto ao adicioná-los ao perfil. Consulte [Atribuir a um perfil de produto permissões de acesso ao Analytics](../admin-getting-started/admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391).

**Ajuda relacionada**

[Delegar privilégios de administração limitados](../admin-getting-started/admin-getting-started.md#task_3A072C4AA9734BC59FFA7E015271BC7E)

## Analytics {#section_97DE101F92CD494AB073893680992F1A}

Gerencie permissões de usuário e de produto do Analytics no Admin Console.

[Atribuir a um perfil de produto permissões de acesso ao Analytics](../admin-getting-started/admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391) (nesta página).

**Migração de contas de usuário**

Uma ferramenta de migração de IDs de usuário do Analytics está disponível para ajudar os administradores do Analytics a migrar contas de usuário do Gerenciamento de usuários do Analytics para o [Adobe Admin Console](https://adminconsole.adobe.com/enterprise/).

A migração das contas está acontecendo em fases. A Adobe vai notificá-lo e assisti-lo quando chegar a sua hora de migrar as contas de usuário existentes de **[!UICONTROL Ferramentas administrativas]** &gt; **[!UICONTROL Gerenciamento de usuários]** para o Admin Console.

Após a migração, os usuários farão logon com a Adobe ID (ou a Enterprise ID) e se autenticarão nas soluções e nos serviços da Experience Cloud, em [marketing.adobe.com](https://marketing.adobe.com/). Se algum usuário tentar fazer logon por meio de logons antigos ([!DNL my.omniture.com] e [!DNL sc.omniture.com]), será redirecionado para [!DNL marketing.adobe.com].

**Ajuda relacionada**

[Migração de IDs de usuário do Analytics](https://marketing.adobe.com/resources/help/pt_BR/experience-cloud/admin-console/analytics-migration/)

## Target - perfis de produto versus espaços de trabalho {#section_3860AF177C9E4C7E9C390D36A414F353}

No Target, um espaço de trabalho é um perfil de produto. Isso permite que uma organização atribua um conjunto específico de usuários a um conjunto específico de propriedades. De muitas formas, um espaço de trabalho é semelhante a um conjunto de relatórios no Adobe Analytics.

Consulte:
* [Permissões de usuários corporativos](https://marketing.adobe.com/resources/help/pt_BR/target/target/?f=property_channel)
* [Gerenciar produtos e perfis](https://helpx.adobe.com/br/enterprise/using/manage-products-and-profiles.html)
* Vídeo: [Como configurar espaços de trabalho do Target no Adobe Admin Console](https://helpx.adobe.com/br/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)




## Campaign - perfis de produto, locatários e grupos de segurança {#section_09CDF75366444CF5810CF321B7C712F3}

Um *locatário* do Campaign é exibido como um *produto* na página Produtos do Admin Console.

O *Grupo de segurança* é exibido como um perfil de produto.

Consulte [Gerenciamento de grupos e usuários](https://helpx.adobe.com/br/campaign/standard/administration/using/managing-groups-and-users.html) para obter informações sobre grupos de segurança e atribuir usuários a grupos de segurança.

## Experience Platform Launch{#section_F2DA6778DD2D48AA8F794041971EE6B1}

O Experience Platform Launch é exibido na página Produtos do Admin Console. É possível incluir outras soluções e principais serviços em um perfil de produto do Launch.

Consulte [Gerenciamento de usuários](https://marketing.adobe.com/resources/help/en_US/experience-cloud/launch/?f=user-management) para obter informações sobre permissões de usuário no Admin Console e configurar opções específicas para o Launch, incluindo a atribuição de direitos a perfis.

## Gerenciador dinâmico de tags {#section_3A41CF2BD5994B9891537D063571D4ED}

Convide usuários para o Dynamic Tag Management, atribua funções de usuário e adicione usuários a grupos.

Consulte [Usuários e permissões](https://marketing.adobe.com/resources/help/pt_BR/dtm/?f=users) para obter informações sobre como convidar usuários para o Dynamic Tag Management, atribuir funções de usuário e adicionar usuários a grupos.

## Audience Manager {#section_C31E3FA8A1E14463B1B3E07235F1983C}

Crie usuários no Audience Manager e os atribua a grupos. Também é possível visualizar limites (características, segmentos, destinos e o AlgoModel).

Consulte [Administração](https://marketing.adobe.com/resources/help/en_US/aam/?f=c_administration) na ajuda do Audience Manager.

## Gerenciar produtos da Experience Cloud {#task_16335111C52D40E9BAC73D0699584DBF}

Crie um perfil de produto e o atribua a um grupo de permissões.

Ao convidar um usuário para uma organização, é possível concedê-lo acesso a produtos e perfis de produtos. Também é possível delegar a um usuário permissões administrativas limitadas. De maneira similar, é possível criar grupos de usuários, e depois adicionar o grupo a um perfil de produto para habilitar o acesso.

1. Em [Admin Console](https://adminconsole.adobe.com/enterprise/), clique em **[!UICONTROL Produtos]**.
1. Clique em **[!UICONTROL Novo perfil]**.
1. Configure os detalhes do perfil, e depois clique em **[!UICONTROL Próximo]**.
1. Clique em **[!UICONTROL Concluído]**.

Mais ajuda disponível em:

* [Gerenciar produtos e perfis](https://helpx.adobe.com/br/enterprise/using/manage-products-and-profiles.html)
* [Permissões de usuários corporativos](https://marketing.adobe.com/resources/help/pt_BR/target/target/?f=property_channel) na ajuda do Target para obter mais informações.
* Vídeo: [Como configurar espaços de trabalho do Target no Adobe Admin Console](https://helpx.adobe.com/br/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)


## Atribuir a um perfil de produto permissões de acesso ao Analytics {#task_040673FE3E3E429B9531FBCB8B6A4391}

Atribuir a um perfil de produto permissões de acesso a relatórios do Analytics (conjuntos de relatórios, métricas, dimensões e outros).

Por exemplo, é possível criar um perfil de produto que contenha várias ferramentas do Analytics ([!UICONTROL Analysis Workspace], [!UICONTROL Reports &amp; Analytics] e [!UICONTROL Report Builder]), com permissão para métricas e dimensões específicas (inclusive eVars), e recursos como criação de segmentos ou de métricas calculadas.

1. Faça logon no [Admin Console](https://adminconsole.adobe.com/enterprise), depois clique em **[!UICONTROL Produtos]**(ou clique no nome do produto).
1. No perfil do produto, clique em **[!UICONTROL Permissões]** (disponível somente para administradores).
1. Configure as permissões do perfil:


| Elemento | Descrição |
|--- |--- |
| Conjuntos de relatórios | Habilite permissões para conjuntos de relatórios específicos. |
| Métricas | Habilite permissões para tráfego, conversão, eventos personalizados, eventos de soluções e sensíveis a conteúdo, entre outros. |
| Dimensões | Personalize detalhadamente o acesso dos usuários, inclusive a eVars e relatórios de tráfego, de soluções e de definição de caminho. |
| Ferramentas do conjunto de relatórios | Habilite permissões do usuário para Serviços da Web, Gerenciamento de conjuntos de relatórios, Ferramentas e relatórios, além de Itens do painel. |
| Ferramentas do Analytics | Habilite permissões do usuário para obter integração a itens Gerais (faturas, logs etc.), Gerenciamento da empresa, Ferramentas, Acesso a serviços da Web, Report Builder e Data Connectors. As configurações da empresa feitas na categoria Personalizar o Admin Console foram movidas para as Ferramentas do Analytics. |



## Delegar funções administrativas aos usuários {#task_3A072C4AA9734BC59FFA7E015271BC7E}


<!-- t_admin-roles.xml -->
No Admin Console, você pode delegar direitos administrativos limitados a outros na organização. As funções delegadas permitem que os usuários administrem o acesso ao software para usuários finais, fornecem acesso aos recursos de implantação e funcionam como atribuições de suporte.

Por exemplo, você pode:

* Permitir que o diretor criativo conceda acesso à Creative Cloud.
* Permitir que o diretor de marketing conceda acesso à Experience Cloud.
* Manter essas duas funções separadas para que elas não se sobreponham.


Ao usar essas funções, você pode delegar simultaneamente o gerenciamento a outras pessoas sem fornecer mais recursos do que o necessário.

1. No Admin Console, clique em **[!UICONTROL Usuários]** e, em seguida, clique no nome do usuário.
1. Clique em **[!UICONTROL Editar direitos administrativos]**.
1. Configure os direitos de administrador do usuário.
1. Clique em **[!UICONTROL Próximo]** para analisar as configurações e clique em **[!UICONTROL Salvar]**.

## Navegadores suportados e requisitos de sistema {#concept_CDC4371EB9BF433E9534F8716DC8A088}

Navegadores suportados na Experience Cloud.


<!-- browsers.xml -->
**Serviços principais da Experience Cloud**

* A versão mais recente do Microsoft Internet Explorer. (A Microsoft [descontinuou o suporte](https://www.microsoft.com/pt-br/WindowsForBusiness/End-of-IE-support) para o Internet Explorer 8, 9 e 10. Por esse motivo, a Adobe não corrigirá problemas relatados nessas versões do Internet Explorer.)
* Google Chrome
* Mozilla Firefox
* Apple Safari


**Soluções e requisitos de produto**

* [Analysis Workspace e Reports &amp; Analytics](https://marketing.adobe.com/resources/help/pt_BR/sc/user/?f=requirements) (inclui o Adobe Social)
* [Report Builder](https://marketing.adobe.com/resources/help/pt_BR/arb/?f=system_requirements)
* [Ad Hoc Analysis](https://marketing.adobe.com/resources/help/pt_BR/dsc/index.html?f=c_sys_reqs)
* [Data Workbench](https://marketing.adobe.com/resources/help/en_US/insight/install/?f=c_Data_Workbench_Client_install)
* [Adobe Target](https://marketing.adobe.com/resources/help/pt_BR/target/ov/?f=r_supported_browsers)
* [Adobe Audience Manager](https://marketing.adobe.com/resources/help/en_US/aam/?f=c_supported_browsers)
* [Adobe Campaign Standard](https://helpx.adobe.com/br/campaign/standard/start/using/compatible-browsers.html)
* [Adobe Campaign Classic](https://helpx.adobe.com/br/campaign/kb/compatibility-matrix.html)
