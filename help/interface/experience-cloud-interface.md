---
description: 'Saiba como fazer logon e sobre os componentes da interface central na Experience Cloud. Saiba mais sobre pesquisa global, suas preferências de conta, como navegar na interface e obter ajuda. '
solution: Experience Cloud
title: 'Componentes da interface do usuário central da Experience Cloud '
feature: Central Interface Components
topic: Administration
role: Admin, User
level: Beginner, Intermediate, Experienced
source-git-commit: c073b3bacf5505c01017d4ba2507621df8ef877e
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 99%

---

# Ajuda da interface da Experience Cloud

Os componentes da interface central da Experience Cloud incluem recursos que permitem:

* Fazer logon e acessar aplicativos e serviços
* Encontrar ajuda e objetos de negócios do produto usando uma pesquisa global
* Gerenciar suas preferências de conta (alertas, notificações e assinaturas)

## Suporte ao navegador na Experience Cloud {#browser}

Para obter o melhor desempenho, a Experience Cloud é otimizada para os navegadores mais populares, incluindo a versão mais recente, além das duas versões anteriores.

* Google Chrome
* Edge
* Firefox
* Opera
* Safari

Se o seu navegador não estiver listado, talvez ainda seja suportado, mas é recomendável usar um dos navegadores listados.

>[!NOTE]
>
>Nem todos os aplicativos em execução no domínio Experience Cloud dão suporte a todos os navegadores. Se não tiver certeza, confira a documentação de um aplicativo específico.

## Suporte de idiomas na Experience Cloud {#languages}

A Experience Cloud oferece suporte a idiomas preferenciais para cada usuário, conforme definido nas preferências de sua conta de usuário da Adobe. Os idiomas suportados atualmente são:

* Chinês
* Inglês
* Francês
* Alemão
* Italiano
* Japonês
* Coreano
* Português
* Espanhol
* Mandarim taiwanês

Embora todas as equipes de aplicativos estejam comprometidas com o suporte global aos idiomas, nem todos os aplicativos são oferecidos em cada um dos idiomas indicados acima. Se o seu idioma principal não tiver suporte em um aplicativo Experience Cloud, também será possível definir um idioma secundário como padrão, quando aplicável. Isso pode ser feito em [Preferências de usuário da Experience Cloud](https://experience.adobe.com/preferences).

## Faça logon na Experience Cloud {#signin}

Faça logon e verifique se você está na [organização](organizations.md) correta.

1. Acesse a [Adobe Experience Cloud](https://experience.adobe.com).
1. Selecione **[!UICONTROL Fazer logon com uma Adobe ID]**.
1. Verifique se você está na organização correta.

   ![Verificar sua organização](assets/organizations-menu.png)

   Para verificar se você fez logon na [organização](organizations.md) correta, clique no avatar do perfil para ver o nome da organização. Se você tiver acesso a mais de uma organização, também poderá visualizar e mudar para outra organização diretamente na barra do cabeçalho.

   Se sua organização usa Federated IDs, a Experience Cloud permite fazer logon com o logon único de sua organização sem precisar digitar o endereço de email e a senha. Para usar esse recurso, adicione `#/sso:@domain` ao URL da Experience Cloud (`https://experience.adobe.com`).

   Por exemplo, para uma organização com Federated IDs e o domínio `adobecustomer.com`, defina o link do URL para `https://experience.adobe.com/#/sso:@adobecustomer.com`. Você também pode ir diretamente para um aplicativo específico marcando esse URL, anexado com o caminho do aplicativo. (Por exemplo, para Adobe Analytics, `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics`.)

## Acessar aplicativos da Experience Cloud {#navigation}

Após fazer logon na Experience Cloud, você pode acessar rapidamente todos os aplicativos, serviços e organizações pelo cabeçalho unificado.

Selecione o seletor de aplicativos ![](assets/menu-icon.png) para acessar os serviços da Experience Cloud que você tem.

![Acessar aplicativos da Experience Cloud](assets/platform-core-services.png)

## Pesquisa e suporte na Experience Cloud {#search}

A pesquisa na Experience Cloud permite procurar ajuda (documentação, tutoriais e cursos) na [Experience League](https://experienceleague.adobe.com/?lang=pt-BR#home).

![Pesquisa e suporte na Experience Cloud](assets/search-menu.png)

O menu [!UICONTROL Ajuda] também oferece acesso a:

* **[!UICONTROL Suporte]:** crie um tíquete de suporte ou entre em contato com o [!UICONTROL Suporte] pelo Twitter.
* **[!UICONTROL Feedback]:** entre em contato com a Adobe usando o Feedback e dê a sua opinião.
* **[!UICONTROL Status]:** acesse `https://status.adobe.com/experience_cloud` e verifique o status operacional do produto e [!UICONTROL Gerenciar assinaturas].
* **[!UICONTROL Developer Connection]:** acesse `adobe.io` e encontre a documentação do desenvolvedor.

## Preferências da conta {#account-menu}

No menu de preferências da conta, é possível:

* Especificar um tema escuro (nem todos os aplicativos são compatíveis com esse tema)
* Pesquisar por [Organizações](organizations.md)
* Fazer logoff
* Configurar as [preferências, notificações e assinaturas](#preferences) da conta

### Gerenciar as [!UICONTROL Preferências] da Experience Cloud {#preferences}

As preferências da Experience Cloud incluem notificações, assinaturas e alertas.

Selecione **[!UICONTROL Preferências]** no menu da conta ![](assets/preferences-icon-sm.png) para gerenciar as preferências.

![Gerenciar Experience Cloud](assets/preferences-page.png)

Em [!UICONTROL Preferências da Experience Cloud], você pode configurar os seguintes recursos:

| Recurso | Descrição |
|--- |--- |
| Organização [padrão](organizations.md) | Selecione a organização que você deseja ver ao iniciar a Experience Cloud. |
| [!UICONTROL Subscrições] | Selecione os produtos e categorias que deseja assinar. Notificações no pop-over [!UICONTROL Notificações] e por email. |
| [!UICONTROL Priority] | Selecione as categorias que você deseja que sejam consideradas de alta prioridade. Essas categorias são marcadas com uma tag Alta e podem ser configuradas para entrega, como alertas. |
| [!UICONTROL Alertas] | Selecione as notificações para as quais deseja que alertas sejam exibidos no navegador. Os alertas são exibidos no canto superior direito da janela por alguns segundos. |
| Emails | Especifique a frequência com que deseja receber emails de notificação. (Não enviar, instantâneo, diário ou semanal.) |

{style=&quot;table-layout:auto&quot;}

## Notificações e anúncios {#notifications}

Selecione **[!UICONTROL Notificações]** para ver as notificações que são importantes para você e os anúncios da Adobe.

![Notificações e anúncios](assets/notifications-menu-small.png)

Você pode configurar notificações em [Preferências da Experience Cloud](#preferences).
