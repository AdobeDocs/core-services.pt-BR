---
title: Gerenciar usuários e produtos
description: Faça logon no Admin Console e gerencie permissões de usuário e produtos do Experience Cloud (perfis de produto). Saiba mais sobre como delegar direitos administrativos a usuários da Experience Cloud e sobre o suporte a navegador na Experience Cloud.
solution: Admin
index: true
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: af9eda5b-d984-44b7-a7b3-52dfc4e03d8f
source-git-commit: f229ec33ff721527e6a4c920ea63eabb4102935a
workflow-type: tm+mt
source-wordcount: '1582'
ht-degree: 74%

---

# Gerenciar usuários e produtos no [!DNL Experience Cloud]

Saiba mais sobre como fazer logon no Admin Console, gerenciar permissões de usuário e perfis de produto da Experience Cloud e suporte ao navegador.

>[!IMPORTANT]
>
>As informações a seguir são especificamente para aplicativos da Experience Cloud. Essas informações complementam as informações administrativas mais amplas no [Guia do usuário de administração corporativa](https://helpx.adobe.com/br/enterprise/admin-guide.html) para todos os produtos de nuvem da Adobe.

Você pode ver uma lista classificável e filtrável de todos os usuários da Experience Cloud e seus detalhes na Ferramenta do administrador. Consulte [Exibir usuários da Experience Cloud na Ferramenta administrativa](admin-tool-experience-cloud.md).

## Aviso de atualização de provisionamento{#provisioning}

Atualizado em: **20 de julho de 2022**

>[!IMPORTANT]
>
>Veja o seguinte aviso sobre o provisionamento da Experience Cloud.

A Adobe está atualizando seu provisionamento para fornecer a todos os clientes da Experience Cloud acesso a recursos essenciais que ajudam na interoperabilidade entre alguns produtos da Experience Cloud. Os usuários terão a Adobe Experience Platform como um novo direito adicionado às suas organizações da Experience Cloud, com a [!UICONTROL Coleta de dados] como um serviço incluído.

A [!UICONTROL coleta de dados] da Adobe Experience Platform inclui [tags](https://experienceleague.adobe.com/en/docs/tags) para um gerenciamento universal de tags simplificado e oferece uma infraestrutura de transmissão de dados confiável, robusta e completa. As tags simplificam a coleta de dados da experiência do cliente e simplificam a entrega da experiência.

**As alterações no[!DNL Admin Console]**

Os administradores podem ver alterações ou adições à [!DNL Admin Console] do seguinte modo:

* A placa de produto Adobe Experience Platform no Admin Console inclui:

   * Places
   * Assurance
   * Namespace de identidade
   * Sandboxes
   * Experience Data Model
   * Esquemas
   * Datastreams
   * ID de visitante

  Para organizações que não estão usando o Experience Platform no momento, você verá a _Adobe Experience Platform_ produto na [!DNL Admin Console], incluindo os recursos listados acima.

  Para organizações que atualmente usam a Experience Platform, o _Places_ agora será consolidado ao cartão da Experience Platform.

* A coleta de dados (antigo Launch) e a privacidade da Adobe Experience Platform continuarão a ser exibidas como cartões de produto separados dos outros recursos da Experience Platform.

Para obter mais detalhes sobre os novos recursos, visite suas respectivas páginas na Experience League:

* [Coleta de dados](https://experienceleague.adobe.com/pt-br/docs/discontinued/using/reports-and-analytics)
* [Places](https://experienceleague.adobe.com/en/docs/places/using/home)
* [Assurance](https://experienceleague.adobe.com/docs/platform-learn/implement-mobile-sdk/app-implementation/assurance.html?lang=pt-BR)
* [Namespace de identidade](https://experienceleague.adobe.com/docs/experience-platform/identity/home.html?lang=pt-BR)
* [Sandboxes](https://experienceleague.adobe.com/docs/experience-platform/sandbox/home.html?lang=pt-BR)
* [Experience Data Model](https://experienceleague.adobe.com/docs/experience-platform/xdm/home.html?lang=pt-BR)
* [Esquemas](https://experienceleague.adobe.com/docs/experience-platform/xdm/schema/composition.html?lang=pt-BR)
* [Datastreams](https://experienceleague.adobe.com/docs/experience-platform/edge/datastreams/overview.html?lang=pt-BR)
* [ID de visitante](https://experienceleague.adobe.com/docs/core-services/interface/services/core-services.html?lang=pt-BR#section_3C9F6DF37C654D939625BB4D485E4354)
* [Privacidade](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html?lang=pt-BR)

## Autenticação de usuário da Experience Cloud (migração planejada){#migration}

A partir de fevereiro de 2022, a Adobe está atualizando seu sistema de gerenciamento de perfis para permitir que as organizações gerenciem melhor os direitos dos negócios a perfis individuais. Dessa forma, todos os usuários com um Perfil pessoal, que corresponde a uma Adobe ID individual (Type1), serão migrados para um novo Perfil comercial. Este perfil corresponde a uma _Business ID_ (Type2e).

Consulte [Tipos de identidade no Adobe [!DNL Admin Console]](https://helpx.adobe.com/br/enterprise/using/identity.html) para obter informações sobre tipos de identidade.

### Processo de migração

Quando for a hora da migração, os administradores da organização receberão um email de notificação 30 dias antes.

* A migração será agendada entre as 22h00 e as 6h00, com base no fuso horário principal da organização, ou no fim de semana.
* Durante a migração, o aplicativo Experience Cloud pode ficar inacessível por aproximadamente 15 minutos e [!DNL Admin Console] pode ficar inacessível por até 30 minutos. Caso contrário, essa migração será sem interrupções.

### Alterações após a migração

[!DNL Admin Console]

* Os administradores com várias contas podem ver um seletor de perfil ao entrar [!DNL Admin Console].
* Usuários individuais do Adobe ID são atualizados para a Business ID.
* O diretório da Business ID é adicionado em **[!UICONTROL Configurações]** > **[!UICONTROL Identidade]** > **[!UICONTROL Diretórios]**.

  ![[!DNL Admin Console] Identidade - Business ID](assets/identity-home.png)

### Fazer logon após a migração

Sua experiência de logon não é alterada com esta atualização:

1. Faça logon em `experience.adobe.com` usando as mesmas credenciais.

1. Um novo perfil associado à Business ID é criado. Você será solicitado a **[!UICONTROL Assinar agora]** ou **[!UICONTROL Ignorar]**.

1. Usar uma das opções levará a uma experiência de página de destino existente.

1. Um perfil de Adobe está associado a cada plano comercial e fornece a capacidade de organizar ativos criados de ofertas adicionais de nuvem de Adobe (Creative Cloud e Document Cloud).

Para obter mais informações, consulte [Introdução aos perfis da Adobe](https://helpx.adobe.com/br/enterprise/kb/introducing-adobe-profiles.html).

## O que é um perfil de produto? {#section_AB50558124D541CF80A0D3D76D35A4BF}

_[!UICONTROL Perfis de produto]_ são grupos de produtos e serviços que podem ser atribuídos a usuários. Na Experience Cloud, as permissões se baseiam no perfil de um produto, não no usuário. (No entanto, você pode delegar direitos administrativos a usuários específicos.)

Por exemplo, no Analytics é possível configurar uma coleção de ferramentas de relatório, como o Analysis Workspace e o Report Builder, além de conjuntos de relatórios, métricas e dimensões. Você pode conceder permissão a um perfil de produto adicionando usuários ao perfil.

* Consulte [Atribuir permissões de acesso ao Analytics a um perfil de produto](admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391) nesta página.
* Consulte [Delegar funções administrativas a usuários](#delegate-rights) nesta página.

## Gerenciar perfis de produto da Experience Cloud {#task_16335111C52D40E9BAC73D0699584DBF}

Você pode criar um perfil de produto e atribuí-lo a um grupo de permissão.

Ao convidar um usuário para uma organização, é possível concedê-lo acesso a produtos e perfis de produtos. Também é possível delegar a um usuário permissões administrativas limitadas. De maneira similar, é possível criar grupos de usuários, e depois adicionar o grupo a um perfil de produto para habilitar o acesso.

1. No [[!DNL Admin Console]](https://adminconsole.adobe.com/enterprise/), selecione **[!UICONTROL Produtos]**.
1. Clique no nome da sua organização.
1. Selecione **[!UICONTROL Novo perfil]**.
1. Configure os detalhes do perfil e selecione **[!UICONTROL Salvar]**.

Para obter mais informações (e para obter ajuda sobre o gerenciamento de produto da Creative Cloud e da Document Cloud), consulte [Identidade](https://helpx.adobe.com/br/enterprise/using/identity.html) no [Guia do usuário de administração](https://helpx.adobe.com/br/enterprise/using/users.html).

**Ajuda relacionada**

* [Gerenciar usuários](https://helpx.adobe.com/br/enterprise/using/users.html) in [!DNL Admin Console]
* [Gerenciar produtos e perfis](https://helpx.adobe.com/br/enterprise/using/manage-products.html) in [!DNL Admin Console].
* [Permissões de usuário corporativo](https://experienceleague.adobe.com/docs/target/using/administer/manage-users/enterprise/property-channel.html?lang=pt-BR) na ajuda do Adobe Target para obter mais informações.
* Vídeo: [Como configurar espaços de trabalho do Adobe Target no Adobe [!DNL Admin Console]](https://experienceleague.adobe.com/docs/experience-cloud-kcs/kbarticles/KA-17521.html?lang=pt-BR)

## Delegar funções administrativas aos usuários {#delegate-rights}

Entrada [!DNL Admin Console], você pode delegar direitos administrativos limitados a outras pessoas em sua organização. As funções delegadas permitem que os usuários administrem acesso a software para usuários finais, fornecem acesso aos recursos de implantação e funcionam como delegados de suporte.

Por exemplo, você pode:

* Permitir que o diretor criativo conceda acesso à Creative Cloud.
* Permitir que o diretor de marketing conceda acesso ao Experience Cloud.
* Mantenha essas duas funções separadas para que elas não possam ultrapassar as funções umas das outras.

Ao usar essas funções, você pode delegar simultaneamente o gerenciamento a outras pessoas sem fornecer mais recursos do que o necessário.

1. No [!DNL Admin Console], selecione **[!UICONTROL Usuários]** e, em seguida, selecione o nome do usuário.

   ![Direitos administrativos no [!DNL Admin Console]](assets/edit-admin-rights.png)

1. Selecione **[!UICONTROL Editar direitos administrativos]**.

   ![Editar direitos administrativos no [!DNL Admin Console]](assets/edit-admin-rights-page.png)

1. Especifique os direitos de administrador do usuário.
1. Selecione **[!UICONTROL Salvar]**.

## Gerenciar usuários e produtos do Analytics {#section_97DE101F92CD494AB073893680992F1A}

Você pode atribuir permissões de acesso a relatórios do Analytics (conjuntos de relatórios, métricas, dimensões e assim por diante) a um perfil de produto.

Por exemplo, você pode criar um perfil de produto que contenha várias ferramentas do Analytics ([!UICONTROL Analysis Workspace], [!UICONTROL Reports &amp; Analytics] e [!UICONTROL Report Builder]). Esses perfis contêm permissão para métricas e dimensões específicas (incluindo eVars) e recursos como segmentos ou criação de métricas calculadas.

1. Faça logon na [[!DNL Admin Console]](https://adminconsole.adobe.com/enterprise)e selecione **[!UICONTROL Produtos]**.
1. Na página [!UICONTROL Produtos], clique no produto e, em seguida, clique em **[!UICONTROL Permissões]** (disponível somente para administradores).
1. Configure as permissões do perfil:

| Elemento | Descrição |
|--- |--- |
| Conjuntos de relatórios | Ative permissões para conjuntos de relatórios específicos. |
| Métricas | Habilite permissões para tráfego, conversão, eventos personalizados, eventos de aplicativos, sensibilidade de conteúdo, entre outros. |
| Dimensões | Personalize detalhadamente o acesso dos usuários, incluindo eVars e relatórios de tráfego, de aplicativos e de caminho. |
| Ferramentas do conjunto de relatórios | Habilite permissões do usuário para Serviços da Web, Gerenciamento de conjuntos de relatórios, Ferramentas e relatórios, além de Itens do painel. |
| Ferramentas do Analytics | Habilite as permissões do usuário para itens gerais (faturamento, logs e assim por diante), Gerenciamento da empresa, Ferramentas, Acesso a serviços da Web, Report Builder e Integração de Data Connectors. Configurações da empresa em Personalizar [!DNL Admin Console] A categoria foi movida para Ferramentas do Analytics. |

**Migração de contas de usuário**

Uma ferramenta de migração de IDs de usuário do Analytics está disponível para ajudar os administradores do Analytics a migrar contas de usuário do Gerenciamento de usuários do Analytics para a [Adobe [!DNL Admin Console]](https://adminconsole.adobe.com/enterprise/).

A migração das contas está acontecendo em fases. O Adobe vai notificá-lo e ajudá-lo quando chegar a sua hora de migrar as contas de usuário existentes do **[!UICONTROL Ferramentas administrativas]** > **[!UICONTROL User Management]** para o [!DNL Admin Console].

Após a migração, os usuários fazem logon com a Adobe ID (ou Enterprise ID) e se autenticam em seus aplicativos e serviços da Experience Cloud em [experience.adobe.com](https://experience.adobe.com). Se os usuários tentarem fazer logon por meio de logins herdados ([!DNL my.omniture.com], [!DNL sc.omniture.com] e [!DNL experiencecloud.adobe.com]) eles serão redirecionados para [!DNL experience.adobe.com].

**Ajuda relacionada**

* [Analytics na [!DNL Admin Console]](https://experienceleague.adobe.com/docs/analytics/admin/admin-console/home.html?lang=pt-BR)
* [Migração de IDs de usuários do Analytics](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/user-product-management/migrate-users/c-migration-tool.html?lang=pt-BR)

## Gerenciar o Adobe Target — perfis de produto vs. espaços de trabalho {#section_3860AF177C9E4C7E9C390D36A414F353}

No Adobe Target, um espaço de trabalho é um perfil de produto. Ele permite que uma organização atribua um conjunto específico de usuários a um conjunto específico de propriedades. De muitas formas, um espaço de trabalho é semelhante a um conjunto de relatórios no Adobe Analytics.

Consulte:

* [Permissões de usuário empresarial](https://experienceleague.adobe.com/docs/target/using/administer/manage-users/enterprise/property-channel.html?lang=pt-BR)
* [Gerenciar produtos e perfis](https://helpx.adobe.com/br/enterprise/using/manage-products.html)
* Vídeo: [Como configurar espaços de trabalho do Adobe Target no Adobe [!DNL Admin Console]](https://experienceleague.adobe.com/docs/experience-cloud-kcs/kbarticles/KA-17521.html?lang=pt-BR)

## Gerenciar perfis de produtos, locatários e grupos de segurança do Campaign {#section_09CDF75366444CF5810CF321B7C712F3}

Um *locatário* do Campaign é exibido como um *produto* na página Produtos do Admin Console.

O *Grupo segurança* é exibido como um perfil de produto.

Consulte [Gerenciamento de grupos e usuários](https://experienceleague.adobe.com/docs/campaign-standard/using/administrating/users-and-security/managing-groups-and-users.html?lang=pt-BR) para obter informações sobre grupos de segurança e atribuição de usuários a grupos de segurança.

## Gerenciar coleção de dados da Experience Platform {#section_F2DA6778DD2D48AA8F794041971EE6B1}

A [!UICONTROL Coleção de dados] da Experience Platform é exibida na página [!UICONTROL Produtos] no [!UICONTROL Admin Console]. É possível incluir outros aplicativos e serviços em um perfil de produto de Coleção de dados.

Convide usuários para a [!UICONTROL Coleção de dados da Platform] e atribua funções e direitos de usuário.

Consulte [Permissões de usuário](https://experienceleague.adobe.com/docs/experience-platform/tags/admin/user-permissions.html?lang=pt-BR) para obter informações sobre permissões de usuário no [!DNL Admin Console] e sobre a configuração de direitos para perfis.

## Experience Manager as a Cloud Service

Os clientes do Adobe Enterprise são representados como Organizações no Adobe [!DNL Admin Console]. Os clientes do Experience Manager podem usar o Adobe [!DNL Admin Console] para gerenciar direitos de produto e autenticação IMS para o Experience Manager as a [!UICONTROL Cloud Service].

Consulte [Suporte de IMS para o Experience Manager as a Cloud Service](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/security/ims-support.html?lang=pt-BR).

## Audience Manager {#section_C31E3FA8A1E14463B1B3E07235F1983C}

Crie usuários no Audience Manager e os atribua a grupos. Também é possível visualizar limites (traços, segmentos, destinos e [!DNL AlgoModel]).

Consulte [Administração](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/administration/administration-overview.html?lang=pt-BR) na ajuda do Audience Manager.

## Navegadores compatíveis com o Experience Cloud

* [!DNL Microsoft® Edge] (A Microsoft® [encerrou o suporte](https://www.microsoft.com/pt-br/WindowsForBusiness/End-of-IE-support) para o Internet Explorer 8, 9 e 10. Por esse motivo, a Adobe deixará de corrigir problemas relatados nessas versões específicas do Internet Explorer.)
* [!DNL Google Chrome]
* [!DNL Firefox]
* [!DNL Safari]
* [!DNL Opera]

**Observação:** embora a interface da Experience Cloud seja compatível esses navegadores, os aplicativos individuais não oferecem suporte a todos os navegadores. (Por exemplo, o [Analytics](https://experienceleague.adobe.com/docs/analytics/admin/admin-overview/sys-reqs.html?lang=pt-BR) não é compatível com o [!DNL Opera] e o [!DNL Adobe Target] não é compatível com o [!DNL Safari]).

### Requisitos da solução e do produto

* [Analytics](https://experienceleague.adobe.com/docs/analytics/admin/admin-overview/sys-reqs.html?lang=pt-BR)
* [Report Builder](https://experienceleague.adobe.com/docs/analytics/analyze/report-builder/report-builder-setup/system-requirements.html?lang=pt-BR)
