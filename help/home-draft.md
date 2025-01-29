---
description: Saiba mais sobre os componentes da interface central para a Experience Cloud. Obtenha ajuda sobre a administração de usuários e produtos no Admin Console, habilite os aplicativos para os serviços da Experience Cloud. Obtenha ajuda sobre a Biblioteca de público-alvo, Atributos do cliente, Ativos da Experience Cloud e mais.
title: Documentação da interface da Experience Cloud
uuid: aec6f689-e617-4876-ae6c-e961cfcb991a
feature: Central Interface Components
topic: Administration
role: Admin
level: Experienced
exl-id: aedad5cb-3282-4a97-8e7e-6d65f7b75ba9
source-git-commit: 163dc8ef83fb83a0e51879520bcb3ae697c95144
workflow-type: tm+mt
source-wordcount: '790'
ht-degree: 94%

---

# Visão geral da interface central da Experience Cloud

O [Experience Cloud](https://experience.adobe.com) é a família integrada de aplicativos de marketing digital, produtos e serviços da Adobe. Por meio da interface intuitiva, você pode acessar rapidamente seus aplicativos em nuvem, recursos do produto e serviços.

![Experience Cloud](assets/landing.png)

No cabeçalho do Experience Cloud, você pode:

* Acesse todos os seus aplicativos e serviços da Experience Cloud
* No menu Ajuda, pesquise pela documentação de produto, tutoriais e publicações da comunidade. Veja os resultados na Experience League.
* Pesquise objetos comerciais globalmente usando uma pesquisa global (somente usuários da Experience Platform) no campo Pesquisa.
* Gerencie as [preferências](features/account-preferences.md) da sua conta (alertas, notificações e assinaturas)

## Faça logon na Experience Cloud {#signin}

Faça logon e verifique se você está na [organização](administration/organizations.md) correta.

1. Acesse a [Adobe Experience Cloud](https://experience.adobe.com).
1. Digite seu endereço de email do Adobe e clique em **[!UICONTROL Continuar]**.
1. Selecione uma conta.
1. Insira sua senha.
1. Verifique se você está na organização correta.

   ![Verifique se você está na organização correta](assets/organizations-menu.png)

   **Verificar sua organização**

   A [organização](administration/organizations.md) é exibida no cabeçalho da interface.

   Se sua organização usa Federated IDs, a Experience Cloud permite conectar-se por meio do logon único de sua organização sem precisar inserir seu endereço de email e senha. Adicione `#/sso:@domain` ao URL da Experience Cloud (`https://experience.adobe.com`) para realizar essa tarefa.

   Por exemplo, para uma organização com Federated IDs e o domínio `adobecustomer.com`, defina o link do URL para `https://experience.adobe.com/#/sso:@adobecustomer.com`. Você também pode ir diretamente para um aplicativo específico marcando esse URL, anexado com o caminho do aplicativo. (Por exemplo, para Adobe Analytics, `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics`.)

## Acessar aplicativos da Experience Cloud {#navigation}

Após fazer logon na Experience Cloud, você pode acessar rapidamente todos os aplicativos, serviços e organizações pelo cabeçalho unificado.

Para acessar os aplicativos e serviços da Experience Cloud fornecidos para você em sua organização, acesse o ![menu](assets/menu-icon.png) do seletor de aplicativos.

![Acessar aplicativos da Experience Cloud](assets/platform-core-services.png)

## Obter ajuda e suporte {#support}

Acesse o aprendizado e a ajuda usando a **[!UICONTROL Central de ajuda]** (![recurso](assets/help-icon.png)) no cabeçalho, incluindo conteúdo de ajuda (documentação, tutoriais e cursos) na [Experience League](https://experienceleague.adobe.com/?lang=pt-BR#home), bem como recursos adicionais para aplicativos individuais. Você também pode enviar feedback aberto e criar tíquetes de suporte priorizados.

![Obter ajuda e suporte](assets/search-menu.png)

O menu [!UICONTROL Ajuda] também oferece acesso a:

* **[!UICONTROL Suporte]:** crie um tíquete de suporte ou entre em contato com o [!UICONTROL Suporte] pelo Twitter.
* **[!UICONTROL Feedback]:** compartilhe um feedback sobre a sua experiência com o Experience Cloud. Seu feedback é usado para melhorar os produtos e serviços do Adobe.
* **[!UICONTROL Status]:** acesse `https://status.adobe.com/experience_cloud` e verifique o status operacional do produto e [!UICONTROL Gerenciar assinaturas].
* **[!UICONTROL Developer Connection]:** acesse `adobe.io` e encontre a documentação do desenvolvedor.

## Gerenciar seu perfil de usuário

No menu [!UICONTROL Perfil], é possível:

* Especificar um tema escuro (nem todos os aplicativos são compatíveis com esse tema)
* Gerenciar as [Preferências](features/account-preferences.md) da Experience Cloud
* Selecione ou pesquise por uma [Organização](administration/organizations.md)
* Exibir [!UICONTROL Avisos legais]
* Fazer logoff
* Configurar as preferências, notificações e assinaturas da conta

## Exibir notificações e avisos no produto {#notifications}

Clique no ícone de sino para exibir notificações e avisos. Os avisos podem ser atualizações relevantes e acionáveis, incluindo lançamentos de produtos, avisos de manutenção, itens compartilhados e solicitações de aprovação.

![Notificações e anúncios](assets/notifications-menu-small.png)

Para gerenciar notificações e alertas, consulte [Preferências e notificações da conta](features/account-preferences.md)


## Novidades

Saiba mais sobre as melhorias mais recentes nos componentes da interface central do Experience Cloud.

>[!BEGINTABS]

>Integração do [!TAB Slack com o Experience Cloud]

Você pode configurar suas preferências de conta para enviar notificações de Experience Cloud para um canal [!DNL Slack].

[!BADGE Beta]{type=Informative url="https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences#notifications" tooltip="Saiba mais sobre o Slack"}


>[!TAB Nova interface de usuário do Adobe Campaign Web]

Explore a nova interface de usuário do Adobe Campaign. Mais moderna, intuitiva e dinâmica.

[![imagem](assets/do-not-localize/learn-more-button.svg)](start/campaign-ui.md#ac-web-ui)


>[!TAB Próximas alterações no canal de push]

Algumas alterações importantes no serviço Firebase Cloud Messaging (FCM) para Android serão lançadas em 2024 e poderão afetar sua implementação do Adobe Campaign. A configuração dos serviços de assinatura para mensagens por push no Android pode precisar ser atualizada para oferecer suporte a essa alteração. É recomendado verificar isso antecipadamente e tomar as devidas ações.

[![imagem](assets/do-not-localize/learn-more-button.svg)](../technotes/upgrades/push-technote.md)



>[!ENDTABS]

## Comece com as noções básicas

<table style="table-layout:fixed">
  <tr style="border: 0;">
    <td>
    <a href="start/whats-new.md"><img src="assets/do-not-localize/start-capabilities.png"></a>
    <div><strong>Principais recursos</strong><br/>Explore os principais recursos do Adobe Campaign v8 para gerenciamento de campanhas em vários canais.</div>
    </td>
    <td>
    <a href="start/connect.md"><img src="assets/do-not-localize/start-connect.jpeg"></a>
    <div><strong>Conectar-se ao Campaign v8</strong><br/>Saiba como se conectar ao Adobe Campaign v8 e iniciar rapidamente sua jornada de gerenciamento de campanhas instalando e configurando o console do cliente.</div><br/>
    </td>
    <td>
    <a href="start/create-message.md"><img src="assets/do-not-localize/start-send.jpeg"></a>
    <div><strong>Enviar mensagens</strong><br/>Aprenda a enviar mensagens através de vários canais, como email, SMS, notificações por push, entre outros.
    </div></td>
    <td>
    <a href="audiences/create-profiles.md"><img src="assets/do-not-localize/start-profiles.png"></a>
    <div><strong>Importar perfis</strong><br/>Explore a criação de perfis no banco de dados do Adobe Campaign v8 com facilidade. Adicione perfis manualmente ou por meio de importações, refinando os dados de clientes e personalizando campanhas facilmente.</div>
    </td>
  </tr>
  <tr style="border: 0;">
    <td align="center"><a href="start/whats-new.md"><img src="assets/do-not-localize/learn-more-button.svg"></a></td>
    <td align="center"><a href="start/connect.md"><img src="assets/do-not-localize/learn-more-button.svg"></a></td>
    <td align="center"><a href="start/create-message.md"><img src="assets/do-not-localize/learn-more-button.svg"></a></td>
    <td align="center"><a href="audiences/create-profiles.md"><img src="assets/do-not-localize/learn-more-button.svg"></a></td>
    </tr>
</table>

## Explorar a documentação

<table style="table-layout:auto">
  <tr style="border: 0;">
    <td>
      <img src="assets/do-not-localize/icon-start.svg" width="35px">
    <br/>
      <strong>Introdução</strong><br/><a href="start/campaign-ui.md">Interface do usuário</a> – <a href="start/ac-components.md">Componentes e processos</a> – <a href="start/v7-to-v8.md">Do Classic v7 para o v8</a> – <a href="start/campaign-faq.md">Perguntas frequentes</a>
    </td>
    <td>
      <img src="assets/do-not-localize/icon-experience.svg" width="35px">
    <br/>
      <strong>Experiência do cliente</strong><br/><a href="../automation/workflow/about-workflows.md" target="_blank">Automatizar com fluxos de trabalho</a> – <a href="../automation/campaigns/set-up-campaigns.md" target="_blank">Orquestração de campanha</a> – <a href="interaction/interaction.md">Gestão de decisões</a> – <a href="send/personalize.md">Personalização</a>
    </td>
    <td>
      <img src="assets/do-not-localize/icon-send.svg" width="35px">
    <br/>
      <strong>Enviar mensagens</strong><br/><a href="start/create-message.md">Introdução</a> – <a href="send/preview-and-proof.md">Visualização e provas</a> – <a href="send/predictive.md">Otimização da hora de envio</a> – <a href="reporting/gs-reporting.md">Relatórios e análises</a>
    </td>
  </tr>
  <tr style="border: 0;">
    <td>
      <img src="assets/do-not-localize/icon_profile-audience.svg" width="35px">
    <br/>
     <strong>Perfis e públicos-alvo</strong><br/><a href="audiences/create-profiles.md">Adicionar perfis</a> – <a href="audiences/create-audiences.md">Criar públicos-alvo</a> – <a href="start/subscriptions.md">Gerenciar assinaturas</a> – <a href="start/privacy.md">Privacidade</a>
    </td>
    <td>
      <img src="assets/do-not-localize/icon-configure.svg" width="35px">
    <br/>
      <strong>Arquitetura e configuração</strong><br/><a href="architecture/architecture.md">Arquitetura</a> – <a href="start/implement.md">Implementação do Campaign v8</a> – <a href="connect/integration.md">Conectar-se a outras soluções</a> – <a href="start/gs-permissions.md">Usuários e permissões</a>
    </td>
    <td>
      <img src="assets/do-not-localize/icon-dev.svg" width="35px">
    <br/>
      <strong>Recursos do desenvolvedor</strong><br/><a href="dev/datamodel.md">Modelo de dados do Campaign v8</a> – <a href="dev/schemas.md">Esquemas</a> – <a href="dev/api.md">APIs</a>
    </td>
  </tr>
</table>

## Recursos adicionais

[Descrição do produto Adobe Campaign v8](https://helpx.adobe.com/br/legal/product-descriptions/adobe-campaign-managed-cloud-services.html){target="_blank"} – [Documentação da interface do usuário do Adobe Campaign Web](https://experienceleague.adobe.com/docs/campaign-web/v8/campaign-web-home.html?lang=pt-BR){target="_blank"} – [Tutoriais](https://experienceleague.adobe.com/docs/campaign-learn/tutorials/overview.html?lang=pt-BR){target="_blank"} – [[!DNL Adobe Campaign] Guia de automação](https://experienceleague.adobe.com/docs/campaign/automation/home.html?lang=pt-BR){target="_blank"} – [Painel de controle do Campaign v8](https://experienceleague.adobe.com/docs/control-panel/using/discover-control-panel/key-features.html?lang=pt-BR){target="_blank"}

