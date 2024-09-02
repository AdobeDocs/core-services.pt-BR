---
description: Saiba mais sobre os componentes da interface central para a Experience Cloud. Obtenha ajuda sobre a administração de usuários e produtos no Admin Console, habilite os aplicativos para os serviços da Experience Cloud. Obtenha ajuda sobre a Biblioteca de público-alvo, Atributos do cliente, Ativos da Experience Cloud e mais.
title: Documentação da interface da Experience Cloud
uuid: aec6f689-e617-4876-ae6c-e961cfcb991a
feature: Central Interface Components
topic: Administration
role: Admin
level: Experienced
exl-id: aedad5cb-3282-4a97-8e7e-6d65f7b75ba9
source-git-commit: 2a80851c0a7d4ef7dbcc2565177b239f3e063164
workflow-type: ht
source-wordcount: '714'
ht-degree: 100%

---

# Visão geral da interface central da Experience Cloud

O [Experience Cloud](https://experience.adobe.com) é a família integrada de aplicativos de marketing digital, produtos e serviços da Adobe. Por meio da interface intuitiva, você pode acessar rapidamente seus aplicativos em nuvem, recursos do produto e serviços.

![Experience Cloud](assets/landing.png)

No cabeçalho do Experience Cloud, você pode:

* Acessar seus aplicativos e serviços
* No menu Ajuda, pesquise pela documentação de produto, tutoriais e publicações da comunidade. Veja os resultados na Experience League.
* Pesquise objetos comerciais globalmente usando uma pesquisa global (somente usuários da Experience Platform) no campo Pesquisa.
* Gerenciar suas preferências de conta (alertas, notificações e assinaturas)

## Faça logon na Experience Cloud {#signin}

Faça logon e verifique se você está na [organização](administration/organizations.md) correta.

1. Acesse a [Adobe Experience Cloud](https://experience.adobe.com).
1. Digite seu endereço de email da Adobe e selecione **[!UICONTROL Continuar]**.
1. Selecione uma conta.
1. Insira sua senha.
1. Verifique se você está na organização correta.

   ![Verifique se você está na organização correta](assets/organizations-menu.png)

   **Verificar sua organização**

   Para verificar se você fez logon na [organização](administration/organizations.md) correta, clique no avatar do perfil para ver o nome da organização. Se você tiver acesso a mais de uma organização, também poderá visualizar e mudar para outra organização diretamente na barra do cabeçalho.

   Se sua organização usa Federated IDs, a Experience Cloud permite conectar-se por meio do logon único de sua organização sem precisar inserir seu endereço de email e senha. Adicione `#/sso:@domain` ao URL da Experience Cloud (`https://experience.adobe.com`) para realizar essa tarefa.

   Por exemplo, para uma organização com Federated IDs e o domínio `adobecustomer.com`, defina o link do URL para `https://experience.adobe.com/#/sso:@adobecustomer.com`. Você também pode ir diretamente para um aplicativo específico marcando esse URL, anexado com o caminho do aplicativo. (Por exemplo, para Adobe Analytics, `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics`.)

## Acessar aplicativos da Experience Cloud {#navigation}

Após fazer logon na Experience Cloud, você pode acessar rapidamente todos os aplicativos, serviços e organizações pelo cabeçalho unificado.

Para acessar os aplicativos e serviços da Experience Cloud fornecidos para você em sua organização, acesse o ![menu](assets/menu-icon.png) do seletor de aplicativos.

![Acessar aplicativos da Experience Cloud](assets/platform-core-services.png)

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
* Pesquisar por [Organizações](administration/organizations.md)
* Fazer logoff
* Configurar as preferências, notificações e assinaturas da conta

Para gerenciar as preferências, selecione **[!UICONTROL Preferências]** no menu ![preferências](assets/preferences-icon-sm.png) da conta.

![Perfil do usuário e preferências da conta](assets/preferences-page.png)

Em [!UICONTROL Preferências da Experience Cloud], você pode configurar os seguintes recursos:

| Recurso | Descrição |
|--- |--- |
| Organização [padrão](administration/organizations.md) | Selecione a organização que você deseja ver ao iniciar a Experience Cloud. |
| [!UICONTROL Coleção de dados do produto] | Selecione quais tecnologias a Adobe pode usar para coletar dados sobre como você usa seus produtos da Adobe. |
| [!UICONTROL Recomendações e promoções de aprendizado personalizadas] | Selecione onde deseja receber ajuda personalizada para seus produtos da Adobe. Essa ajuda está disponível por email, no produto e nas comunidades da Experience League. [Saiba mais.](features/personalized-learning.md) |
| [!UICONTROL Subscrições] | Selecione os produtos e categorias que deseja assinar. Notificações no pop-over [!UICONTROL Notificações] e por email. |
| [!UICONTROL Prioridade] | Selecione as categorias que você deseja que sejam consideradas de alta prioridade. Essas categorias são marcadas com uma tag Alta e podem ser configuradas para entrega, como alertas. |
| [!UICONTROL Alertas] | Selecione as notificações para as quais deseja que alertas sejam exibidos no navegador. Os alertas são exibidos no canto superior direito da janela por alguns segundos. |
| Emails | Especifique a frequência com que deseja receber emails de notificação. (Não enviar, instantâneo, diário ou semanal.) |

{style="table-layout:auto"}

## Notificações e anúncios {#notifications}

Selecione **[!UICONTROL Notificações]** para ser alertado de atualizações relevantes e práticas, incluindo lançamentos de produtos, avisos de manutenção, itens compartilhados e solicitações de aprovação.

![Notificações e anúncios](assets/notifications-menu-small.png)
