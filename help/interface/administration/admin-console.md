---
title: Gerenciamento de licenças de usuários e produtos
description: Gerencie usuários e licenças de produtos no Admin Console para aplicativos da Experience Cloud.
application: Experience Cloud
index: true
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: c82821c4-aa5d-48ae-8bef-5937fede8db2
source-git-commit: ce65c5292caaa4a24945e2119e78fd97a7d84109
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 7%

---

# Gerenciamento de usuários e licenças de produto

Você pode gerenciar usuários e licenças de produtos na Adobe [Admin Console](https://adminconsole.adobe.com/enterprise/). Para obter ajuda sobre o gerenciamento de identidade geral aplicável a todos os aplicativos da Adobe, consulte o [Guia de administração de empresas e equipes](https://helpx.adobe.com/br/enterprise/admin-guide.html).

Esta página fornece informações úteis especificamente para administradores do Experience Cloud, define funções e fornece links para tópicos comuns de gerenciamento de usuários e produtos no guia corporativo.

## Funções administrativas no Admin Console

O Admin Console fornece três funções administrativas principais, cada uma com níveis específicos de acesso e responsabilidade:

| Função | Descrição |
| ------- | ------- |
| Administrador do sistema | Acesso completo - Gerencia todos os aspectos do console. <br>Principais responsabilidades: <br><ul><li>Adicionar, remover e gerenciar usuários.</li><li>Atribuir e revogar licenças de produto.</li><li>Definir configurações de identidade e autenticação</li><li>Exibir e gerenciar informações de faturamento.</li><li>Configurar administradores adicionais e funções de delegado.</li></ul> **Recomendado para:** administradores de TI ou líderes de equipe que supervisionam todo o ambiente Adobe da organização. |
| Administrador do produto | Gerenciamento específico do produto - Controla o acesso e as permissões de produtos específicos da Adobe.<br>Principais responsabilidades:<ul><li>Atribuir e gerenciar licenças para um produto específico.</li><li>Crie e gerencie perfis de produto.</li><li>Adicionar ou remover usuários nos produtos atribuídos.</li></ul>   **Recomendado para:** equipes/usuários que gerenciam softwares específicos, como o Marketo Engage ou o Adobe Creative Cloud. |
| Administrador do perfil do produto | Gerenciamento de função granular - concentra-se no gerenciamento de grupos de usuários e permissões em um produto.<br>Principais responsabilidades:<ul><li>Crie e gerencie perfis de produto.</li><li>Atribua permissões e acesso a recursos nos perfis.</li><li>Adicionar ou remover usuários em perfis.</li></ul> **Recomendado para:** Líderes de departamento ou gerentes de equipe que supervisionam grupos menores com necessidades especializadas. Os administradores do <br> podem combinar funções para obter maior flexibilidade, dependendo dos requisitos organizacionais. |

## Admin Console para Experience Cloud

Para gerenciar licenças de identidade e de produto para aplicativos Experience Cloud, navegue até a [Admin Console](https://adminconsole.adobe.com/enterprise/).

Estes são recursos que você pode precisar ao começar a usar o administrador no Admin Console:

### Configurar recursos

| Link de ajuda | Descrição |
| ------- | ------ |
| [Configurar identidade e logon único](https://helpx.adobe.com/br/enterprise/using/set-up-identity.html) | **[!UICONTROL Admin Console]** > **[!UICONTROL Configurações]** <br> Saiba como configurar as contas dos seus usuários com tipos de ID diferentes com ou sem logon único (SSO). Configure o SSO para o software Adobe, defina as configurações do SAML e passe pelas perguntas e erros mais comuns. |
| [Configurar organização via relação de confiança de diretório](https://helpx.adobe.com/enterprise/using/directory-trust.html) | Autentique seus usuários em um domínio já reivindicado por outra organização. Para obter informações sobre como localizar e alternar organizações, consulte [Organizações na Experience Cloud](organizations.md). |
| [Configurações de autenticação (empresa)](https://helpx.adobe.com/enterprise/using/authentication-settings.html) | O Admin Console oferece suporte a vários níveis de proteção por senha e políticas para garantir a segurança. Você pode optar por usar um nível de proteção por senha para aplicar a todos os usuários em sua organização. |
| [Contatos de privacidade e segurança](https://helpx.adobe.com/enterprise/using/security-contacts.html) | Proteja os dados de sua organização e de seus usuários. Se ocorrer um incidente de segurança envolvendo nossas soluções de software, as notificações serão enviadas aos responsáveis pela conformidade apropriados. As empresas têm pessoal cuja função é específica para proteção de dados, integridade e outros assuntos de conformidade. Portanto, as informações de contato dessa equipe são essenciais para ajudar a garantir uma notificação imediata no caso de um incidente de segurança. |

### Gerenciamento de usuários

| Link de ajuda | Descrição |
| ------- | ------- |
| [Gerenciar vários usuários](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) | **[!UICONTROL Admin Console]** > **[!UICONTROL Usuários]** <br>Saiba como gerenciar vários usuários por meio do carregamento em massa de CSV para a Admin Console. |
| [Tipos de identidade](https://helpx.adobe.com/br/enterprise/using/identity.html) | Os tipos de identidade permitem que a organização tenha diferentes níveis de controle sobre as contas e os dados dos usuários. Sua escolha de modelo de identidade afeta como sua organização armazena e compartilha ativos. Embora os modelos do Federated ID e do Enterprise ID sejam criados e gerenciados pela organização, as Adobe IDs são criadas e gerenciadas pelo indivíduo. |
| [Ferramenta de Sincronização de Usuário](https://helpx.adobe.com/enterprise/using/user-sync.html) (UST) | A Ferramenta de sincronização de usuários do Adobe é um aplicativo de desktop usado para automatizar a sincronização de dados de usuários entre o sistema de gerenciamento de identidades de uma organização (como o Ative Diretory) e a Adobe Admin Console. A ferramenta permite que os administradores simplifiquem o provisionamento, as atualizações e a desativação de usuários nos produtos da Adobe. |
| [Exibir detalhes do usuário (Ferramenta Administrativa)](admin-tool-experience-cloud.md) | Exiba uma lista classificável e filtrável de todos os usuários e políticas da Experience Cloud com detalhes na [!UICONTROL Ferramenta do administrador]. |

### Relatórios e logs

| Link de ajuda | Descrição |
| ------- |------- |
| [Log de auditoria](https://helpx.adobe.com/enterprise/using/audit-logs.html) | **[!UICONTROL Insights]** > **[!UICONTROL Logs]** > **[!UICONTROL Log de auditoria]** <br> Rastreie todas as alterações feitas na Admin Console. |


## Recursos específicos do aplicativo

Esses links ajudam a encontrar informações de administração para aplicativos Experience Cloud específicos.

<!-- | Application | Link to resource|
| ------- | ------- |
|  [!DNL Analytics] <p>Customer Journey Analytics| [Analytics in the Adobe Admin Console overview](https://experienceleague.adobe.com/en/docs/analytics/admin/admin-console/home) <p>[Administration requirements](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/workspace-faq/frequently-asked-questions-analysis-workspace) |
| [!DNL Audience Manager] | [Audience Manager user migration to Admin Console](https://experienceleague.adobe.com/en/docs/audience-manager/user-guide/features/administration/admin-console-migration) |
| [!DNL Campaign] v8 |  [Get started with permissions](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/gs-permissions) |
| [!DNL Campaign Standard] to [!DNL Campaign v8] | [User access management from Campaign Standard to Campaign V8](https://experienceleague.adobe.com/en/docs/campaign-web/acs-to-ac/user-management-acs) |
| [!DNL Commerce] | [Configure the Commerce Admin Integration with Adobe ID](https://experienceleague.adobe.com/en/docs/commerce-admin/start/admin/ims/adobe-ims-config) |
| [!DNL Dynamic Media Classic] | [Administration setup](https://experienceleague.adobe.com/en/docs/dynamic-media-classic/using/setup/administration-setup#user_administration) |
| [!DNL Experience Manager as a Cloud Service] |  [Accessing the Admin Console](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/onboarding/journey/admin-console) |
| [!DNL Experience Platform] <p>[!DNL Data Collection] | [Access control UI overview](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/ui/overview) <p>[Permission management for data collection in Experience Platform](https://experienceleague.adobe.com/en/docs/experience-platform/collection/permissions)|
| [!DNL GenStudio for Performance Marketing] | [Provision Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/product-provisioning) |
| [!DNL Journey Optimizer] | [Manage users and roles](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/access-control/permissions) |
| [!DNL Journey Optimizer B2B Edition] | [User management](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/admin/user-management) |
|[!DNL  Journey Orchestration] | [Access management](https://experienceleague.adobe.com/en/docs/journeys/using/starting-with-journeys/access-management) |
| [!DNL Marketo Engage] | [Understanding Marketo Subscription and User Migration to the Adobe Admin Console](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console) |
| [!DNL Marketo Measure] | [Adobe Admin Console Setup](https://experienceleague.adobe.com/en/docs/marketo-measure/using/configuration-and-setup/getting-started-with-marketo-measure/adobe-admin-console-setup) |
| [!DNL Mix Modeler] | [Access controls](https://experienceleague.adobe.com/en/docs/mix-modeler/using/data-governance/access-controls) |
| [!DNL Pass] | [Get started with Account IQ](https://experienceleague.adobe.com/en/docs/pass/aiq-help/get-started) |
| [!DNL Target] | [Administrator first steps](https://experienceleague.adobe.com/en/docs/target/using/administer/start-target) <p> [User management](https://experienceleague.adobe.com/en/docs/target/using/administer/manage-users/user-management) |
| [!DNL Workfront] | [Manage users in the Adobe Admin Console](https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/add-users/create-manage-users/admin-console) |

 -->

* [Analytics](https://experienceleague.adobe.com/en/docs/analytics/admin/admin-console/home)
* [Customer Journey Analytics](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/workspace-faq/frequently-asked-questions-analysis-workspace)
* [Audience Manager](https://experienceleague.adobe.com/en/docs/audience-manager/user-guide/features/administration/admin-console-migration)
* [Campaign v8](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/admin/permissions/gs-permissions)
* [Campaign Standard](https://experienceleague.adobe.com/en/docs/campaign-web/acs-to-ac/user-management-acs)
* [Comércio](https://experienceleague.adobe.com/en/docs/commerce-admin/start/admin/ims/adobe-ims-config)
* [Dynamic Media Classic](https://experienceleague.adobe.com/en/docs/dynamic-media-classic/using/setup/administration-setup#user_administration)
* [Experience Manager as a Cloud Service](https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/onboarding/journey/admin-console)
* [Experience Platform](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/ui/overview) e [Coleção de dados](https://experienceleague.adobe.com/en/docs/experience-platform/collection/permissions)
* [GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/product-provisioning)
* [Journey Optimizer](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/access-control/permissions)
* [Journey Optimizer B2B edition](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/admin/user-management)
* [Journey Orchestration](https://experienceleague.adobe.com/en/docs/journeys/using/starting-with-journeys/access-management)
* [Marketo Engage](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console)
* [Marketo Measure](https://experienceleague.adobe.com/en/docs/marketo-measure/using/configuration-and-setup/getting-started-with-marketo-measure/adobe-admin-console-setup)
* [Mix Modeler](https://experienceleague.adobe.com/en/docs/mix-modeler/using/data-governance/access-controls)
* [Adobe Pass](https://experienceleague.adobe.com/en/docs/pass/aiq-help/get-started)
* [Target](https://experienceleague.adobe.com/en/docs/target/using/administer/start-target)
* [Workfront](https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/add-users/create-manage-users/admin-console)

A maior parte da ajuda do Admin Console para todos os aplicativos da Adobe está documentada no [Guia de administração de empresas e equipes](https://helpx.adobe.com/br/enterprise/admin-guide.html).
