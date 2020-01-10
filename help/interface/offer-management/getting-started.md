---
description: Uma visão geral do Gerenciamento de ofertas, como acessá-lo e como conceder permissões de usuário.
seo-description: Uma visão geral do Gerenciamento de ofertas, como acessá-lo e como conceder permissões de usuário.
seo-title: Introdução
title: Introdução
uuid: 28d83606-ee36-4bbf-b52d-bbe8b097f6d5
index: y
internal: n
snippet: y
translation-type: tm+mt
source-git-commit: 2f0c2eb70313c42da9e7ac1d75429ec768dea10d

---


# Gerenciamento de ofertas da Adobe {#section_07CBD4C01F4049A5A19781737D2DCD35}

[!UICONTROL O Gerenciamento de ofertas proporciona a oportunidade de criar, gerenciar, e tomar decisões em todos os canais na Experience Cloud. ] Ele serve como um catálogo de ofertas central onde você pode associar regras de qualificação e vários conteúdos a cada _objeto de oferta._ Você pode publicar essas ofertas em canais e locais e oferecer a melhor oferta para cada cliente em cada interação. Esses recursos permitem que você forneça continuamente a melhor oferta aos seus clientes de uma forma consistente e coordenada em toda a sua experiência.

Os benefícios incluem:

* Aprimoramento do desempenho da campanha por email ao fornecer ofertas mais personalizadas em seus emails.
* Fluxo de trabalho aprimorado: Em vez de criar várias entregas ou campanhas, as equipes de marketing podem melhorar o fluxo de trabalho criando uma única entrega e variar as ofertas em diferentes partes do modelo.
* Permite que você crie, gerencie e aprove ofertas fora do fluxo de trabalho da campanha de email do Adobe Campaign Standard.
* Controle do número de vezes que uma oferta é exibida em campanhas de email e clientes.

## Acessar ofertas {#task_DEB6F6A4B6E04E15AD3E1817D700688E}

Saiba como acessar o Gerenciamento de ofertas.

1. Entre em contato com a Adobe para obter o provisionamento.

   Uma organização da Experience Cloud deve ter uma instância do Campaign Standard. A Adobe também pode ativar um recurso no Campaign que permite criar atividades de oferta dentro de e-mails.

1. No menu de navegação da Experience Cloud, clique no seletor de soluções e clique em **[!UICONTROL Ofertas]**.

   ![](assets/access-offers.png)

   Para acessar Ofertas no Campaign Standard, clique no ícone **[!UICONTROL Ofertas]**em um modelo de email.

   ![](assets/campaign-add-offer.png)

   Depois que você vir ambos os itens na Marketing Cloud e na sua conta do Adobe Campaign, você será configurado com a funcionalidade necessária para começar.

## Usuários e permissões {#concept_81F0ABB07ACC49E099EDCD87AA0436E1}

Os administradores podem adicionar usuários ao Gerenciamento [!UICONTROL de] ofertas no Admin Console. Um convite por email é enviado ao novo usuário com instruções sobre como acessar o produto. Depois que um usuário é adicionado, você pode ajustar suas permissões, permitindo que ele tenha acesso a diferentes funcionalidades em todo o [!UICONTROL Gerenciamento]de ofertas.

Para obter mais informações sobre como usar o Admin Console, consulte a documentação [do Admin Console no](https://helpx.adobe.com/enterprise/help/aedash.html)HelpX.

No Campaign, os usuários padrão têm automaticamente o direito de incorporar atividades de oferta em um modelo de email.

>[!NOTE]
>
>Para beta, não há permissões em vigor. Todos os usuários adicionados às Ofertas terão acesso total a todas as funcionalidades no [!UICONTROL Gerenciamento]de ofertas.

## Criar um perfil de produto para o Gerenciamento de ofertas

Um perfil de produto é um conjunto de permissões que podem ser combinadas para criar uma função de usuário em um produto. Os perfis de produto devem ser criados e os usuários ou grupos atribuídos a eles.

1. Navegue até o Adobe [Admin Console](https://adminconsole.adobe.com/).

1. Clique no seu projeto (**[!UICONTROL Ofertas]**, por exemplo).

1. Na página Pofiles [!UICONTROL do] produto, clique em **[!UICONTROL Novo perfil]**.

1. Digite um nome e uma descrição para o perfil do produto e clique em **[!UICONTROL Concluído]**.

1. Clique em **[!UICONTROL Salvar]**.

### Permissões - definições

Uma descrição das permissões de Gerenciamento [!UICONTROL de] ofertas disponíveis para perfis de produtos no Console [!UICONTROL de]administração.

| Elemento | Descrição |
|--- |--- |
| Criar e editar ofertas | Fornece aos usuários acesso para criar e editar ofertas no [!UICONTROL Gerenciamento]de ofertas. Se um usuário tiver essa permissão, mas não a permissão _Aprovar ofertas_ , ele poderá apenas criar uma oferta e enviá-la para aprovação. Ele não pode ser usado em uma atividade de oferta até que tenha sido aprovado. |
| Excluir ofertas | Concede aos usuários acesso para excluir ofertas. |
| Aprovar ofertas | Dá aos usuários a capacidade de aprovar uma oferta. Os usuários com essa permissão verão uma notificação ao fazer logon no Gerenciamento de ofertas se alguma oferta precisar de aprovação. Se um usuário tiver essa permissão e a permissão _criar e editar ofertas_ , ele poderá criar e aprovar ofertas em um único fluxo de trabalho. |
| Ofertas de arquivamento | Oferece aos usuários a capacidade de arquivar uma oferta. |
| Criar rótulos | Oferece aos usuários a capacidade de criar rótulos, tanto na guia Rótulo quanto em linha na tela de criação da oferta. Sem essa permissão, um usuário só poderá selecionar ofertas pré-criadas ao criar uma oferta. |
| Editar rótulos | Permite que o usuário edite rótulos na guia Rótulos. |
| Excluir rótulos | Fornece ao usuário a capacidade de excluir rótulos na guia Rótulos. |
| Criar disposições | Fornece ao usuário a capacidade de criar disposições na guia Disposições. |
| Editar disposições | Fornece ao usuário a capacidade de editar disposições na guia Disposições. |
| Excluir disposições | Fornece ao usuário a capacidade de excluir disposições na guia Disposições. **** Observação: Somente disposições não usadas em uma atividade de oferta podem ser excluídas. |