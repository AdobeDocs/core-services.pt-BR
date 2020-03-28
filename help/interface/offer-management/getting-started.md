---
description: Uma visão geral do Gerenciamento de Ofertas, como acessá-lo e como conceder permissões de usuário.
seo-description: Uma visão geral do Gerenciamento de Ofertas, como acessá-lo e como conceder permissões de usuário.
seo-title: Introdução
title: Introdução
uuid: 28d83606-ee36-4bbf-b52d-bbe8b097f6d5
index: y
internal: n
snippet: y
translation-type: tm+mt
source-git-commit: 43de353155c640b3ddc519147c94d7e9ffcafe4e

---


# Gerenciamento de Ofertas da Adobe {#section_07CBD4C01F4049A5A19781737D2DCD35}

[!UICONTROL O Gerenciamento] de Ofertas oferece criação, gerenciamento e decisão de ofertas em todos os canais da Experience Cloud. Ele serve como um catálogo de oferta central, onde você pode associar regras de elegibilidade e vários conteúdos a cada _objeto de oferta._ Você pode publicar essas ofertas em canais e locais e fornecer a melhor oferta para cada cliente em cada interação. Esses recursos permitem que você forneça continuamente a melhor oferta aos seus clientes de uma forma consistente e coordenada em toda a sua experiência.

Os benefícios incluem:

* Desempenho de campanha de e-mail aprimorado ao fornecer ofertas mais personalizadas em seus e-mails.
* Fluxo de trabalho aprimorado: Em vez de criar vários delivery ou campanhas, as equipes de marketing podem melhorar o fluxo de trabalho criando um único delivery e variar as ofertas em diferentes partes do modelo.
* Permite que você crie, gerencie e aprove ofertas fora do fluxo de trabalho da campanha de e-mail do Adobe Campaign Standard.
* Controle o número de vezes que uma oferta é exibida em campanhas de e-mail e clientes.

## Acesso ao Oferta {#task_DEB6F6A4B6E04E15AD3E1817D700688E}

Saiba como acessar o Gerenciamento de Ofertas.

1. Entre em contato com a Adobe para obter o provisionamento.

   Uma organização da Experience Cloud deve ter uma instância de Campaign Standard. A Adobe também pode ativar um recurso na Campanha que permite criar atividades de oferta em e-mails.

1. No menu de navegação da Experience Cloud, clique no seletor de soluções e, em seguida, clique em **[!UICONTROL Oferta]**.

   ![](assets/access-offers.png)

   Para acessar o Oferta no Campaign Standard, clique no ícone do **[!UICONTROL Oferta]** em um modelo de email.

   ![](assets/campaign-add-offer.png)

   Depois de ver ambos os itens na Marketing Cloud e na sua conta do Adobe Campaign, você foi configurado com a funcionalidade necessária para começar.

## Users and Permissions {#concept_81F0ABB07ACC49E099EDCD87AA0436E1}

Os administradores podem adicionar usuários ao Gerenciamento [!UICONTROL de] Ofertas no Admin Console. Um convite por email é enviado ao novo usuário com instruções sobre como acessar o produto. Depois que um usuário é adicionado, você pode ajustar suas permissões, dando a ele acesso a diferentes funcionalidades no Gerenciamento de [!UICONTROL Ofertas].

Para obter mais informações sobre como usar o Admin Console, consulte a documentação [do Admin Console no](https://helpx.adobe.com/enterprise/help/aedash.html)HelpX.

Na Campanha, os usuários padrão têm automaticamente o direito de incorporar atividades de oferta em um modelo de email.

>[!NOTE]
>
>Para beta, não há permissões em vigor. Todos os usuários adicionados ao Oferta terão acesso total a todas as funcionalidades no Gerenciamento [!UICONTROL de]Ofertas.

## Criar um perfil de produto para Gerenciamento de Ofertas

Um perfil de produto é um conjunto de permissões que podem ser combinadas para criar uma função de usuário em um produto. Os perfis do produto devem ser criados e os usuários ou grupos atribuídos a eles.

1. Navegue até o Adobe [Admin Console](https://adminconsole.adobe.com/).

1. Clique no seu projeto (**[!UICONTROL Oferta]**, por exemplo).

1. Na página Perfis [!UICONTROL de] produto, clique em **[!UICONTROL Novo Perfil]**.

1. Digite um nome e uma descrição para o perfil do produto e clique em **[!UICONTROL Concluído]**.

1. Clique em **[!UICONTROL Salvar]**.

### Permissões - definições

Uma descrição das permissões de Gerenciamento [!UICONTROL de] Ofertas disponíveis para perfis de produtos no Console [!UICONTROL de]administração.

| Elemento | Descrição |
|--- |--- |
| Criar e editar ofertas | Fornece aos usuários acesso para criar e editar ofertas no Gerenciamento [!UICONTROL de]Ofertas. Se um usuário tiver essa permissão, mas não a permissão _Aprovar oferta_ , ele só poderá criar uma oferta e enviá-la para aprovação. Não pode ser utilizado numa atividade de oferta até ter sido aprovada. |
| Excluir ofertas | Concede aos usuários acesso para excluir ofertas. |
| Aprovar ofertas | Dá aos usuários a capacidade de aprovar uma oferta. Os usuários com essa permissão verão uma notificação ao fazer logon no Gerenciamento de Ofertas se qualquer oferta precisar de aprovação. Se um usuário tiver essa permissão e a permissão _criar e editar o oferta_ , ele poderá criar e aprovar o oferta em um único fluxo de trabalho. |
| ofertas de arquivamento | Oferece aos usuários a capacidade de arquivar uma oferta. |
| Criar rótulos | Oferece aos usuários a capacidade de criar rótulos, tanto na guia Rótulo quanto em linha na tela de criação da oferta. Sem essa permissão, um usuário só poderá selecionar ofertas pré-criadas ao criar uma oferta. |
| Editar rótulos | Dá ao usuário a capacidade de editar rótulos na guia Rótulos. |
| Excluir rótulos | Fornece ao usuário a capacidade de excluir rótulos na guia Rótulos. |
| Criar disposições | Fornece ao usuário a capacidade de criar disposições na guia Disposições. |
| Editar disposições | Fornece ao usuário a capacidade de editar disposições na guia Disposições. |
| Excluir disposições | Fornece ao usuário a capacidade de excluir disposições na guia Disposições. **Observação:** Somente as disposições não usadas em uma atividade de oferta podem ser excluídas. |