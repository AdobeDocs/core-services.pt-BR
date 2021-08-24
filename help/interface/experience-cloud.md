---
description: Saiba mais sobre os componentes de interface central para o Experience Cloud. Este guia inclui ajuda sobre a administração de usuários e produtos no Admin Console, como habilitar aplicativos para serviços do Experience Cloud e ajuda sobre a biblioteca de público-alvo, atributos do cliente, ativos do Experience Cloud e muito mais.
solution: Experience Cloud
title: Ajuda e documentação da interface do Experience Cloud
uuid: aec6f689-e617-4876-ae6c-e961cfcb991a
feature: '"Atributos do cliente"'
topic: Administração
role: Admin
level: Experienced
exl-id: aedad5cb-3282-4a97-8e7e-6d65f7b75ba9
source-git-commit: 4534f764ea821576c3ac5cd1959d387a3689e837
workflow-type: tm+mt
source-wordcount: '1306'
ht-degree: 63%

---

# Guia de componentes de interface central do Experience Cloud

O [Experience Cloud](https://experience.adobe.com) é a família integrada de aplicativos de marketing digital, produtos e serviços da Adobe. Por meio da interface intuitiva, você pode acessar rapidamente seus aplicativos em nuvem, recursos do produto e serviços.

![Experience Cloud](assets/landing.png)

No cabeçalho do Experience Cloud, você pode:

* Acessar seus aplicativos e serviços
* Pesquisar por documentações de produtos, tutoriais e publicações da comunidade
* Pesquisar objetos comerciais globalmente usando uma pesquisa global (somente usuários do Experience Platform)
* Gerenciar suas preferências de conta (alertas, notificações e assinaturas)

## Faça logon na Experience Cloud {#signin}

Faça logon e verifique se você está na [organização](organizations.md) correta.

1. Acesse a [Adobe Experience Cloud](https://experience.adobe.com).
1. Selecione **[!UICONTROL Fazer logon com uma Adobe ID]**.
1. Verifique se você está na organização correta.

   ![](assets/organizations-menu.png)

   **Verificar sua organização**

   Para verificar se você fez logon no [Organization](organizations.md) correto, clique no avatar do perfil para ver o nome da organização. Se você tiver acesso a mais de uma organização, também poderá visualizar e alternar para outra organização diretamente na barra de cabeçalho.

   Se sua organização usa Federated IDs, o Experience Cloud permite fazer logon com o logon único de sua organização sem precisar digitar o endereço de email e a senha. Para fazer isso, adicione `#/sso:@domain` ao URL de Experience Cloud (`https://experience.adobe.com`).

   Por exemplo, para uma organização com Federated IDs e o domínio `adobecustomer.com`, defina o link do URL para `https://experience.adobe.com/#/sso:@adobecustomer.com`. Você também pode ir diretamente para um aplicativo específico marcando esse URL, anexado com o caminho do aplicativo. (Por exemplo, para Adobe Analytics, `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics`.)

## Acessar aplicativos da Experience Cloud {#navigation}

Após fazer logon na Experience Cloud, você pode acessar rapidamente todos os aplicativos, serviços e organizações pelo cabeçalho unificado.

Para acessar os aplicativos e serviços do Experience Cloud fornecidos para você em sua organização, acesse o seletor de aplicativos ![](assets/menu-icon.png).

![](assets/platform-core-services.png)

## Suporte ao navegador no Experience Cloud {#browser}

Para obter o melhor desempenho, o Experience Cloud é otimizado para os navegadores mais populares, incluindo a versão mais recente, além das duas versões anteriores.

* Google Chrome
* Edge
* Firefox
* Opera
* Safari

Se o seu navegador não estiver listado, talvez ainda seja suportado, mas é recomendável usar um dos navegadores listados.

>[!NOTE]
>
>Nem todos os aplicativos em execução no domínio Experience Cloud suportam todos os navegadores. Se não tiver certeza, verifique a documentação de um aplicativo específico.

## Suporte de idiomas no Experience Cloud {#languages}

O Experience Cloud oferece suporte a idiomas preferenciais para cada usuário, conforme definido nas preferências da conta de usuário do Adobe. Os idiomas suportados atualmente são:

* Chinês
* Inglês
* Francês
* Alemão
* Italiano
* Japonês
* Coreano
* Português
* Espanhol
* Taiwan

Embora todas as equipes de aplicativos estejam comprometidas com o suporte a idiomas globais, nem todos os aplicativos são oferecidos em todos os idiomas anotados acima. Se o seu idioma primário não for suportado em um aplicativo Experience Cloud, você também poderá definir um idioma secundário como padrão quando aplicável. Isso pode ser feito em [Experience Cloud user preferences](https://experience.adobe.com/preferences).

## Obter ajuda e suporte {#support}

Acesse o aprendizado e a ajuda usando o ícone Ajuda (![asset](assets/help-icon.png)) no cabeçalho, incluindo o conteúdo da ajuda (documentação, tutoriais e cursos) em [Experience League](https://experienceleague.adobe.com/?lang=pt-BR#home), bem como recursos adicionais para aplicativos individuais. Você também pode enviar feedbacks e criar tíquetes de suporte priorizados.

![](assets/search-menu.png)

O menu [!UICONTROL Ajuda] também oferece acesso a:

* **[!UICONTROL Suporte]:** crie um tíquete de suporte ou entre em contato com o [!UICONTROL Suporte] pelo Twitter.
* **[!UICONTROL Feedback]:** compartilhe um feedback sobre a sua experiência com o Experience Cloud. Seu feedback é usado para melhorar os produtos e serviços do Adobe.
* **[!UICONTROL Status]:** acesse `https://status.adobe.com/experience_cloud` e verifique o status operacional do produto e [!UICONTROL Gerenciar assinaturas].
* **[!UICONTROL Developer Connection]:** acesse `adobe.io` e encontre a documentação do desenvolvedor.

## Pesquisar objetos e entidades globalmente {#search}

A pesquisa global permite encontrar objetos ou entidades comerciais pesquisáveis em uma experiência contínua, consistente e com apenas um clique. Essa pesquisa exibe os objetos acessados recentemente.

![](assets/platform-search.png)

>[!NOTE]
>
>A pesquisa global não está disponível em todos os aplicativos Experience Cloud, mas como mais conteúdo é indexado, ele será adicionado aos aplicativos relevantes. Disponibilidade a partir de julho de 2021:

* Experience Platform
* Journey Optimizer

## Perfil do usuário e preferências da conta {#preferences}

As preferências da Experience Cloud incluem notificações, assinaturas e alertas. No menu de preferências da conta, é possível:

* Especificar um tema escuro (nem todos os aplicativos são compatíveis com esse tema)
* Pesquisar por [Organizações](organizations.md)
* Fazer logoff
* Configurar as preferências, notificações e assinaturas da conta

Para gerenciar preferências, selecione **[!UICONTROL Preferências]** no menu da conta ![](assets/preferences-icon-sm.png).

![](assets/preferences-page.png)

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

Selecione **[!UICONTROL Notificações]** para ser alertado sobre atualizações relevantes e acionáveis, incluindo versões de produtos, avisos de manutenção, itens compartilhados e solicitações de aprovação.

![](assets/notifications-menu-small.png)

## Domínios Experience Cloud {#domains}

O Experience Cloud usa os seguintes hosts para fornecer o aplicativo, melhorar o desempenho e a experiência do produto. O Adobe recomenda adicionar esses domínios à lista de permissões do firewall para obter uma experiência ideal. Domínios adicionais também podem estar em uso para aplicativos Experience Cloud específicos, como o Adobe Analytics. Consulte a documentação desses aplicativos para obter mais informações.

| Tecnologia | Domínios |
|--- |--- |
| Domínios Adobe Experience Cloud | `adobe.com`, `adobe.net`, `adobe.io` |
| Adobe Identity Management Service (IMS) | `adobelogin.com` |
| Experience Cloud fonts | `typekit.net` |
| Gainsight (para orientação e ajuda do produto) | `esp.aptrinsic.com` |

## Obter ajuda sobre administração e serviços entre aplicativos

Este guia fornece acesso à ajuda sobre o usuário da Experience Cloud e a administração do produto no Admin Console, permitindo soluções para os serviços da plataforma. Você também pode acessar a ajuda da Biblioteca de público-alvo, Atributos do cliente, Ativos da Experience Cloud e muito mais:

* [[!UICONTROL Biblioteca de público-alvo]](audience-library.md)
* [[!UICONTROL Atributos do cliente]](attributes.md)
* [[!UICONTROL Triggers]](triggers.md)
* [[!UICONTROL Ativos] da Experience Cloud](experience-cloud-assets.md)
* [Cookies da Experience Cloud](cookies-privacy.md)
* [Gerenciamento de usuários e de produtos](admin-getting-started.md) (Admin Console)
* [Ativar as soluções dos serviços principais](core-services.md)
* [Perguntas frequentes](admin-getting-started.md)
* [Organizações e vinculação de contas](organizations.md)
* [Integrações](marketing-cloud-integrations.md)
* [Integração do Adobe Target à Experience Cloud](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4t.html?lang=pt-BR)
* [Visão geral da privacidade e da segurança da Experience Cloud](assets/Adobe-Marketing-Cloud-Privacy-and-Security-Overview.pdf)
* [Pré-busca DNS](admin-getting-started.md#concept_6BC8C6856E3644F8956D7AD0A96383B7)

## Guias

Os guias relacionados da Experience Cloud incluem:

* [Adobe Mobile](https://experienceleague.adobe.com/docs/mobile-services/using/home.html?lang=pt-BR)
* [Gráfico cooperativo da Experience Platform](https://experienceleague.adobe.com/docs/device-co-op/using/home.html?lang=pt-BR)
* [Exchange](https://exchange.adobe.com/experiencecloud)
* [Serviço da Experience Cloud ID](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=pt-BR)
* [Coleta de dados do Experience Platform/Launch](https://experienceleague.adobe.com/docs/launch.html?lang=pt-BR)
* [Experience Cloud Debugger](https://experienceleague.adobe.com/docs/debugger/using/experience-cloud-debugger.html?lang=pt-BR)
* [API do Regulamento Geral sobre a Proteção de Dados (GDPR)](https://www.adobe.io/apis/experiencecloud/gdpr.html)
* [[!UICONTROL Dynamic Tag Management]](https://experienceleague.adobe.com/docs/experience-platform/tags/home.html?lang=en)

## Tutoriais

Aproveite os tutoriais de autoajuda e instruções rápidas na Experience League:

* [Todos os tutoriais na Experience League](https://experienceleague.adobe.com/?lang=pt-BR#quick-how-tos)
* [Tutoriais da Experience Platform](https://experienceleague.adobe.com/docs/launch-learn/tutorials/overview.html?lang=pt-BR)
* [Plataforma de dados do cliente em tempo real](https://experienceleague.adobe.com/docs/platform-learn/tutorials/application-services/rtcdp/understanding-the-real-time-customer-data-platform.html?lang=pt-BR)

## Notas de versão e ajuda relacionada à Experience Cloud

* [Documentação do produto para todas as soluções da Experience Cloud](https://experienceleague.adobe.com/docs/home.html?lang=pt-BR) - Procure ajuda na Aprendizagem e suporte da Experience Cloud
* [Notas de versão e atualizações de produtos](https://experienceleague.adobe.com/docs/release-notes/experience-cloud/current.html?lang=pt-BR) - Novidades na Experience Cloud e assinatura para obter atualizações
* [Tutoriais para implementar os serviços principais](https://experienceleague.adobe.com/docs/launch-learn/tutorials/overview.html?lang=en) - Explore vídeos e tutoriais sobre os serviços principais
* [Ajuda de especialistas na Experience League](https://experienceleague.adobe.com/?lang=pt-BR) - Obtenha um aprendizado orientado de especialistas e da comunidade
* [Educação e treinamento](https://helpx.adobe.com/br/learning.html?promoid=KAUDK) — interaja com a Adobe para garantir o aproveitamento máximo de nossos produtos
* [Blog de experiência do cliente](https://blog.adobe.com/br/topics/digital-transformation.html) - Leia o blog da Experience Cloud
* [Atendimento ao cliente](https://experienceleague.adobe.com/?support-solution=General&amp;lang=pt-BR#support) - Entre em contato com o Atendimento ao cliente da Adobe
