---
description: Saiba mais sobre os componentes de interface central para o Experience Cloud. Este guia inclui ajuda sobre a administração de usuários e produtos no Admin Console, como habilitar aplicativos para serviços do Experience Cloud e ajuda sobre a biblioteca de público-alvo, atributos do cliente, ativos do Experience Cloud e muito mais.
solution: Experience Cloud
title: Ajuda e documentação da interface do Experience Cloud
uuid: aec6f689-e617-4876-ae6c-e961cfcb991a
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: aedad5cb-3282-4a97-8e7e-6d65f7b75ba9
source-git-commit: 013a05d68f3fdf0dc71e048dfa6144be08cdfe6a
workflow-type: tm+mt
source-wordcount: '1337'
ht-degree: 96%

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
1. Digite seu endereço de email da Adobe e selecione **[!UICONTROL Continuar]**.

   Administradores, consultem [Autenticação de usuário da Experience Cloud](admin-getting-started.md#migration) para obter atualizações importantes sobre tipos de identidade (Business ID).

1. Selecione uma conta.
1. Insira sua senha.
1. Verifique se você está na organização correta.

   ![Verifique se você está na organização correta](assets/organizations-menu.png)

   **Verificar sua organização**

   Para verificar se você fez logon na [organização](organizations.md) correta, clique no avatar do perfil para ver o nome da organização. Se você tiver acesso a mais de uma organização, também poderá visualizar e mudar para outra organização diretamente na barra do cabeçalho.

   Se sua organização usa Federated IDs, a Experience Cloud permite conectar-se por meio do logon único de sua organização sem precisar inserir seu endereço de email e senha. Adicione `#/sso:@domain` ao URL da Experience Cloud (`https://experience.adobe.com`) para realizar essa tarefa.

   Por exemplo, para uma organização com Federated IDs e o domínio `adobecustomer.com`, defina o link do URL para `https://experience.adobe.com/#/sso:@adobecustomer.com`. Você também pode ir diretamente para um aplicativo específico marcando esse URL, anexado com o caminho do aplicativo. (Por exemplo, para Adobe Analytics, `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics`.)

## Acessar aplicativos da Experience Cloud {#navigation}

Após fazer logon na Experience Cloud, você pode acessar rapidamente todos os aplicativos, serviços e organizações pelo cabeçalho unificado.

Para acessar os aplicativos e serviços da Experience Cloud fornecidos para você em sua organização, acesse o ![menu](assets/menu-icon.png) do seletor de aplicativos.

![Acessar aplicativos da Experience Cloud](assets/platform-core-services.png)

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

## Obter ajuda e suporte {#support}

Acesse o aprendizado e a ajuda usando o ícone Ajuda (![asset](assets/help-icon.png)) no cabeçalho, incluindo o conteúdo da ajuda (documentação, tutoriais e cursos) em [Experience League](https://experienceleague.adobe.com/?lang=pt-BR#home), bem como recursos adicionais para aplicativos individuais. Você também pode enviar feedback aberto e criar tíquetes de suporte priorizados.

![Obter ajuda e suporte](assets/search-menu.png)

O menu [!UICONTROL Ajuda] também oferece acesso a:

* **[!UICONTROL Suporte]:** crie um tíquete de suporte ou entre em contato com o [!UICONTROL Suporte] pelo Twitter.
* **[!UICONTROL Feedback]:** compartilhe um feedback sobre a sua experiência com o Experience Cloud. Seu feedback é usado para melhorar os produtos e serviços do Adobe.
* **[!UICONTROL Status]:** acesse `https://status.adobe.com/experience_cloud` e verifique o status operacional do produto e [!UICONTROL Gerenciar assinaturas].
* **[!UICONTROL Developer Connection]:** acesse `adobe.io` e encontre a documentação do desenvolvedor.

## Perfil do usuário e preferências da conta {#preferences}

As preferências da Experience Cloud incluem notificações, assinaturas e alertas. No menu de preferências da conta, é possível:

* Especificar um tema escuro (nem todos os aplicativos são compatíveis com esse tema)
* Pesquisar por [Organizações](organizations.md)
* Fazer logoff
* Configurar as preferências, notificações e assinaturas da conta

Para gerenciar as preferências, selecione **[!UICONTROL Preferências]** no menu ![preferências](assets/preferences-icon-sm.png) da conta.

![Perfil do usuário e preferências da conta](assets/preferences-page.png)

Em [!UICONTROL Preferências da Experience Cloud], você pode configurar os seguintes recursos:

| Recurso | Descrição |
|--- |--- |
| Organização [padrão](organizations.md) | Selecione a organização que você deseja ver ao iniciar a Experience Cloud. |
| [!UICONTROL Coleta de dados do produto] | Selecione quais tecnologias o Adobe pode usar para coletar dados sobre como você usa seus produtos de Adobe. |
| [!UICONTROL Recomendações e promoções de aprendizado personalizado] | Selecione onde deseja receber ajuda personalizada para seus produtos Adobe. Essa ajuda está disponível por email, no produto e no Experience League Communities. Saiba mais. |
| [!UICONTROL Subscrições] | Selecione os produtos e categorias que deseja assinar. Notificações no pop-over [!UICONTROL Notificações] e por email. |
| [!UICONTROL Prioridade] | Selecione as categorias que você deseja que sejam consideradas de alta prioridade. Essas categorias são marcadas com uma tag Alta e podem ser configuradas para entrega, como alertas. |
| [!UICONTROL Alertas] | Selecione as notificações para as quais deseja que alertas sejam exibidos no navegador. Os alertas são exibidos no canto superior direito da janela por alguns segundos. |
| Emails | Especifique a frequência com que deseja receber emails de notificação. (Não enviar, instantâneo, diário ou semanal.) |

{style=&quot;table-layout:auto&quot;}

## Notificações e anúncios {#notifications}

Selecione **[!UICONTROL Notificações]** para ser alertado de atualizações relevantes e práticas, incluindo lançamentos de produtos, avisos de manutenção, itens compartilhados e solicitações de aprovação.

![Notificações e anúncios](assets/notifications-menu-small.png)

## Domínios Experience Cloud {#domains}

O Experience Cloud usa os hosts a seguir para fornecer o aplicativo, melhorar o desempenho e a experiência do produto. A Adobe recomenda adicionar esses domínios à lista de permissões do firewall para obter uma experiência ideal. Domínios adicionais também podem estar em uso para aplicativos Experience Cloud específicos, como o Adobe Analytics. Consulte a documentação desses aplicativos para obter mais informações.

| Tecnologia | Domínios |
|--- |--- |
| Domínios da Adobe Experience Cloud | `adobe.com`, `adobe.net`, `adobe.io` |
| Adobe Identity Management Service (IMS) | `adobelogin.com` |
| Fontes da Experience Cloud | `typekit.net` |
| Coleção de dados da Adobe (para orientação e ajuda do produto) | `adobedtm.com` |
| Gainsight (para orientação e ajuda do produto) | `esp.aptrinsic.com` |

## Obter ajuda sobre administração e serviços entre aplicativos

Este guia fornece acesso à ajuda sobre o usuário da Experience Cloud e a administração do produto no Admin Console, habilitando os aplicativos a realizarem serviços de plataforma. Você também pode acessar a ajuda da Biblioteca de público-alvo, Atributos do cliente, Ativos da Experience Cloud e muito mais:

* [[!UICONTROL Biblioteca de público-alvo]](audience-library.md)
* [[!UICONTROL Atributos do cliente]](attributes.md)
* [[!UICONTROL Triggers]](triggers.md)
* [[!UICONTROL Ativos] da Experience Cloud](experience-cloud-assets.md)
* [Cookies da Experience Cloud](cookies-privacy.md)
* [Gerenciamento de usuários e de produtos](admin-getting-started.md) (Admin Console)
* [Habilitar os aplicativos para os serviços principais](core-services.md)
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
* [[!UICONTROL Dynamic Tag Management]](https://experienceleague.adobe.com/docs/experience-platform/tags/home.html?lang=pt-BR)

## Tutoriais

Aproveite os tutoriais de autoajuda e instruções rápidas na Experience League:

* [Todos os tutoriais na Experience League](https://experienceleague.adobe.com/?lang=pt-BR#quick-how-tos)
* [Tutoriais da Experience Platform](https://experienceleague.adobe.com/docs/platform-learn/data-collection/overview.html?lang=pt-BR)
* [Real-time Customer Data Platform](https://experienceleague.adobe.com/docs/platform-learn/tutorials/application-services/rtcdp/understanding-the-real-time-customer-data-platform.html?lang=pt-BR)

## Notas de versão e ajuda relacionada à Experience Cloud

* [Documentação de produto de todos os aplicativos da Experience Cloud](https://experienceleague.adobe.com/docs/home.html?lang=pt-BR) - Buscar ajuda na Aprendizagem e Suporte da Experience Cloud
* [Notas de versão e atualizações de produtos](https://experienceleague.adobe.com/docs/release-notes/experience-cloud/current.html?lang=pt-BR) - Novidades na Experience Cloud e assinatura para obter atualizações
* [Tutoriais para implementar os serviços principais](https://experienceleague.adobe.com/docs/platform-learn/data-collection/overview.html?lang=en) - Explore vídeos e tutoriais sobre os serviços principais
* [Ajuda de especialistas na Experience League](https://experienceleague.adobe.com/?lang=pt-BR) - Obtenha um aprendizado orientado de especialistas e da comunidade
* [Educação e treinamento](https://helpx.adobe.com/br/learning.html?promoid=KAUDK) - interaja com a Adobe para garantir o aproveitamento máximo de nossos produtos
* [Blog de experiência do cliente](https://blog.adobe.com/br/topics/digital-transformation) - Leia o blog da Experience Cloud
* [Atendimento ao cliente](https://experienceleague.adobe.com/?support-solution=General&amp;lang=pt-BR#support) - Entre em contato com o Atendimento ao cliente da Adobe
