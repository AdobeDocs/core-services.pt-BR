---
description: Saiba mais sobre a Ferramenta administrativa da Experience Cloud para ver uma lista classificável e filtrável de todos os usuários da Experience Cloud.
keywords: core services
seo-description: Saiba mais sobre a Ferramenta administrativa da Experience Cloud para ver uma lista classificável e filtrável de todos os usuários da Experience Cloud.
seo-title: Exibir usuários e detalhes do usuário da Experience Cloud
solution: Experience Cloud
title: 'Exibir usuários e detalhes do usuário da Experience Cloud '
index: true
translation-type: ht
source-git-commit: 43de353155c640b3ddc519147c94d7e9ffcafe4e
workflow-type: ht
source-wordcount: '693'
ht-degree: 100%

---


# Exibir usuários da Experience Cloud na Ferramenta administrativa

Os administradores podem exibir uma lista classificável e filtrável de todos os usuários da Experience Cloud e seus detalhes na Ferramenta de administração. Os detalhes do usuário incluem o acesso ao produto, as funções e as últimas informações acessadas de um usuário. (**Observação:** o gerenciamento de usuários e produtos está configurado no [Admin Console](admin-getting-started.md).)

1. Efetue logon no `https://experience.adobe.com/.`

   ![](assets/admin-tool.png)

1. Na página inicial da Experience Cloud, clique em **[!UICONTROL Admin Tool.]**

   (Como alternativa, no URL da página inicial, você pode substituir _início_ por _admin._)

   A página [!UICONTROL Usuários] é exibida.

## Página Usuários

Esta página exibe a lista completa de usuários com acesso à Experience Cloud na organização. Ela fornece informações sobre o direito e o último logon da solução. Pesquise, classifique e filtre exibições personalizadas da lista de usuários.

![](assets/admin-tool-users.png)

| Elemento | Descrição |
|---|---|
| [!UICONTROL Nome] | O nome e sobrenome do usuário. É possível classificar essa coluna de A a Z e Z a A. Clique no nome de um usuário para ver mais detalhes sobre ele. |
| [!UICONTROL Email] | O endereço de email associado ao usuário. A coluna pode ser classificada como A->Z, Z->A. |
| [!UICONTROL Tipo de ID] | O tipo de identidade da conta do usuário. O filtro pode ser aplicado a tipos de ID específicos da exibição. Consulte [Gerenciar tipos de identidade](https://helpx.adobe.com/br/enterprise/using/identity.html) para obter mais informações. |
| [!UICONTROL Soluções] | Resumo das soluções da Experience Cloud que o usuário pode acessar. Aplique filtros para restringir a lista de usuários com acesso específico à solução. |
| [!UICONTROL Último logon] | Hora e data do logon mais recente do usuário na Experience Cloud. Essa coluna pode ser classificada por datas crescentes ou decrescentes. <br> **Importante:** a partir de 13 de janeiro de 2020, os últimos dados de logon do usuário serão mantidos por 365 dias. Essas informações são destinadas a mostrar a atividade de logon atual na Experience Cloud e não uma recomendação para tomar medidas em contas inativas antes de 13 de janeiro de 2020. |

## Personalizar a exibição da lista de usuários

Pesquise, classifique ou filtre as colunas para personalizar a lista de usuários.

* Procure usuários por Nome ou Email. As pesquisas correspondem à cadeia de caracteres de texto digitada.
* Classifique a coluna por valores crescentes ou decrescentes. Isso se aplica às colunas [!UICONTROL Nome,] [!UICONTROL Email] e [!UICONTROL Último logon].
* Clique no ícone **[!UICONTROL Filtrar por]** para aplicar vários filtros a usuários da lista com critérios específicos. Quando várias categorias de filtro são aplicadas, as pesquisas contêm a Solução `AND` TIPO DE ID `AND` de domínio de email.

| Elemento | Descrição |
|---------|----------|
| Filtro de [!UICONTROL domínio de email] | Procure por cadeias de caracteres na coluna Email para restringir os resultados a um ou vários domínios. Adicione vários filtros pressionando Enter após cada termo de pesquisa. |
| Filtro [!UICONTROL Tipo de ID] | Escolha dentre os Tipos de ID disponíveis. Vários tipos de ID podem ser usados como filtro. |
| Filtro [!UICONTROL Solução] | Escolha dentre as soluções disponíveis. Vários filtros de solução pesquisam resultados que contêm a Solução 1 `OR` Solução 2. |

## Visualizar detalhes do usuário

Na página [!UICONTROL Usuários], para visualizar os detalhes do usuário, clique no email do usuário.

![](assets/admin-tool-user-details.png)

Uma exibição detalhada de cada usuário exibe detalhes importantes sobre o acesso à solução do usuário, as funções de administrador e de produto e as informações acessadas pela última vez.

## Sobre a seção

Esta seção exibe um resumo da conta do usuário incluindo:

* Avatar do usuário e selo de administrador do sistema (se aplicável)
* Nome
* Email
* Nome de usuário (contas Federated ID podem ter nomes de usuário diferentes do endereço de email)
* [Tipo de ID](https://helpx.adobe.com/br/enterprise/using/identity.html)
* País
* Último logon

## Resumo das soluções

Esta seção exibe um resumo das soluções da Experience Cloud que o usuário pode acessar. Inclui a função administrativa do produto quando aplicável.

## Lista detalhada de acesso ao produto

Esta seção exibe uma lista completa de todos os perfis de produtos associados ao usuário.

| Elemento | Descrição |
|---------|----------|
| [!UICONTROL Produto] | Nome do produto associado ao perfil do produto. |
| [!UICONTROL Instância] | Nome da instância (como empresa de logon ou locatário) associada ao produto e ao perfil do produto. |
| [!UICONTROL Perfil de produto] | Nome exclusivo do perfil do produto. |
| [!UICONTROL Atribuído por grupo] | Nome do grupo de usuários que associa o usuário a um perfil de produto. Os resultados em branco indicam que o usuário foi atribuído ao perfil do produto diretamente, não por meio de um grupo. |
| [!UICONTROL Funções do produto] | Atribuição de função do usuário no perfil do produto. No momento, essas informações se aplicam somente aos perfis de produtos do Adobe Target. |
