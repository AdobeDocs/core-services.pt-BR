---
description: Saiba mais sobre o CX Enterprise (antigo Experience Cloud). Aborda logon, navegação, pesquisa, preferências, administração e serviços compartilhados, como Biblioteca de público-alvo, Atributos do cliente e Assets.
title: Guia de administração e interface corporativa do CX
uuid: aec6f689-e617-4876-ae6c-e961cfcb991a
feature: Central Interface Components
topic: Administration
role: Admin
level: Experienced
exl-id: aedad5cb-3282-4a97-8e7e-6d65f7b75ba9
TQID: https://experienceleague.adobe.com/7vFfu0DyoTnsrlrWVApm0LLW4jsC0LoXb55jJ3jdxeY
product_v2:
  - id: e1971122-7081-4556-9222-8a31bd71800c
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 25446910430bf15dcfa0fc70e25e0681f9faeb95
workflow-type: tm+mt
source-wordcount: 563
ht-degree: 44%

---

# Guia de administração e interface corporativa do Adobe CX

O [Adobe CX Enterprise](https://experience.adobe.com) (Customer Experience Enterprise) é a família integrada de aplicativos de marketing digital, produtos e serviços da Adobe. Por meio da interface intuitiva, você pode acessar rapidamente seus aplicativos em nuvem, recursos do produto e serviços.

<!-- ![CX Enterprise](assets/landing.png) -->

No cabeçalho do CX Enterprise, é possível:

* Acesse todos os aplicativos e serviços do CX Enterprise
* No menu Ajuda, pesquise pela documentação de produto, tutoriais e publicações da comunidade. Veja os resultados na Experience League.
* Pesquise objetos comerciais globalmente usando uma pesquisa global (somente usuários da Experience Platform) no campo Pesquisa.
* Gerencie as [preferências](features/account-preferences.md) da sua conta (alertas, notificações e assinaturas)

## Fazer logon no CX Enterprise

Faça logon e verifique se você está na [organização](administration/organizations.md) correta.

1. Navegue até [Adobe CX Enterprise](https://experience.adobe.com).
1. Digite seu endereço de email do Adobe e clique em **[!UICONTROL Continuar]**.
1. Clique em uma conta.
1. Insira sua senha.
1. Verifique se você está na organização correta.

   ![Verifique se você está na organização correta](assets/organizations-menu.png)

   **Verificar sua organização**

   A [organização](administration/organizations.md) é exibida no cabeçalho da interface.

   Se sua organização usa Federated IDs, o CX Enterprise permite que você faça logon com o logon único de sua organização sem precisar inserir seu endereço de email e senha. Adicione `#/sso:@domain` ao CX Enterprise URL (`https://experience.adobe.com`) para realizar esta tarefa.

   Por exemplo, para uma organização com Federated IDs e o domínio `example.com`, defina o link do URL para `https://experience.adobe.com/#/sso:@example.com`. Você também pode ir diretamente para um aplicativo específico marcando esse URL, anexado com o caminho do aplicativo. (Por exemplo, para Adobe Analytics, `https://experience.adobe.com/#/sso:@example.com/analytics`.)

   **Observação:** o administrador de sua organização pode restringir o acesso aos produtos da Adobe por endereços IP. Em caso afirmativo, você poderá receber um erro depois de fazer logon no CX Enterprise ou mudar para uma organização com essa opção ativada. Mais informações disponíveis em [Limitar o acesso ao produto por endereços IP](https://helpx.adobe.com/br/enterprise/using/ip-based-access.html).


## Acesse os aplicativos corporativos da CX

Depois de fazer logon no CX Enterprise, você pode acessar rapidamente todos os seus aplicativos, serviços e organizações pelo cabeçalho unificado.

Para acessar os aplicativos e serviços do CX Enterprise fornecidos para você em sua organização, acesse o seletor de aplicativos ![menu](assets/apps-icon.png).

![Acessar aplicativos CX Enterprise](assets/platform-core-services.png)

## Obter ajuda e suporte

Acesse o aprendizado e a ajuda usando a **[!UICONTROL Central de ajuda]** (![asset](assets/help-icon.png)) no cabeçalho, incluindo o conteúdo da ajuda (documentação, tutoriais e cursos) no [Experience League](https://experienceleague.adobe.com/pt-br?lang=pt-BR#home), bem como recursos adicionais para aplicativos individuais. Você também pode enviar feedback aberto e criar tíquetes de suporte priorizados.

![Obter ajuda e suporte](assets/search-menu.png)

O menu [!UICONTROL Ajuda] também fornece acesso a:

* **[!UICONTROL Suporte]:** crie um tíquete de suporte ou contate o [!UICONTROL Suporte] usando o Twitter.
* **[!UICONTROL Feedback]:** Compartilhe um feedback sobre a sua experiência com o CX Enterprise. Seu feedback é usado para melhorar os produtos e serviços do Adobe.
* **[!UICONTROL Status]:** navegue até `https://status.adobe.com/pt-br/experience_cloud` e verifique o status operacional do produto e [!UICONTROL Gerenciar assinaturas].
* **[!UICONTROL Developer Connection]:** Navegue até `adobe.io` e encontre a documentação do desenvolvedor.

## Gerenciar seu perfil de usuário

No menu [!UICONTROL Perfil], você pode:

* Especificar um tema escuro (nem todos os aplicativos são compatíveis com esse tema)
* Gerenciar [Preferências](features/account-preferences.md) da CX Enterprise
* Selecione ou pesquise por uma [Organização](administration/organizations.md)
* Exibir [!UICONTROL Avisos legais]
* Fazer logoff
* Configurar as preferências, notificações e assinaturas da conta

## Exibir notificações e avisos no produto

Clique no ícone de sino para exibir notificações e avisos. Os avisos podem ser atualizações relevantes e acionáveis, incluindo lançamentos de produtos, avisos de manutenção, itens compartilhados e solicitações de aprovação.

![Notificações e anúncios](assets/notifications-menu-small.png)

Para gerenciar notificações e alertas, consulte [Preferências e notificações da conta](features/account-preferences.md)


