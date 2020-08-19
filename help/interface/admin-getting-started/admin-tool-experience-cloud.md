---
description: Saiba mais sobre a Ferramenta de administração de Experience Cloud, para visualização de uma lista classificável e filtrável de todos os usuários e políticas de Experience Cloud.
keywords: core services
seo-description: Saiba mais sobre a Ferramenta de administração de Experience Cloud, para visualização de uma lista classificável e filtrável de todos os usuários e políticas de Experience Cloud.
seo-title: Exibir usuários e detalhes do usuário da Experience Cloud
solution: Experience Cloud
title: 'Exibir usuários e detalhes do usuário da Experience Cloud '
index: true
translation-type: tm+mt
source-git-commit: 82b0b42d8b06388e396bf2959503fe484c8b3a66
workflow-type: tm+mt
source-wordcount: '1271'
ht-degree: 52%

---


# Usuários e políticas da visualização na Ferramenta de administração

Os administradores podem visualização uma lista classificável e filtrável de todos os usuários e políticas de Experience Cloud com detalhes na Ferramenta de administração. Os detalhes do usuário incluem o acesso ao produto, as funções e as últimas informações acessadas de um usuário. Os detalhes da política incluem usuário (perfil de produto), grupo, desenvolvedor, integração e lista de administração de uma política, bem como permissões e informações detalhadas sobre recursos para a política.

>[!NOTE]
>
>User and product management is configured in the [Admin Console](admin-getting-started.md).

1. Efetue logon no `https://experience.adobe.com/.`

   ![](assets/admin-tool.png)

1. Em Acesso [!UICONTROL rápido], clique em Ferramenta **[!UICONTROL administrativa.]**

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

## Página Políticas

Esta página exibe a lista completa das políticas de Experience Cloud na sua organização. Fornece informações sobre produtos, instâncias, usuários e desenvolvedores. Você pode pesquisar, classificar e filtrar visualizações personalizadas da lista de políticas.

![](assets/admin-tool-policies.png)

| Elemento | Descrição |
|---|---|
| [!UICONTROL Perfil de produto] | O nome do perfil do produto. A coluna pode ser classificada como A->Z, Z->A. Clique no nome do perfil do produto para ver mais detalhes sobre a política. |
| [!UICONTROL Produto] | O produto associado ao perfil do produto. A coluna pode ser classificada como A->Z, Z->A. |
| [!UICONTROL Instância] | A instância (por exemplo, locatário ou empresa de login) associada ao perfil do produto. Os produtos que não têm instâncias ou locatários exclusivos exibirão um &quot; - &quot; para o valor. A coluna pode ser classificada como A->Z, Z->A. |
| [!UICONTROL Número de usuários] | Contagem exclusiva de usuários associados ao perfil do produto, incluindo atribuição direta e atribuição de grupo. A coluna pode ser classificada de menor para maior ou maior para menor. |
| [!UICONTROL Número de desenvolvedores] | Contagem de funções de desenvolvedor associadas ao perfil do produto. A coluna pode ser classificada de menor para maior ou maior para menor. |

## Personalizar a visualização de lista de políticas

Você pode pesquisar, classificar ou filtrar as colunas para personalizar a lista de políticas.

* Procure perfis de produtos por nome. As pesquisas correspondem à cadeia de caracteres de texto digitada.
* Classifique a coluna por valores crescentes ou decrescentes. Isso se aplica ao Perfil [!UICONTROL do produto,] [!UICONTROL produto,] [!UICONTROL instância,] [!UICONTROL número de usuários,] e [!UICONTROL número de desenvolvedores,] colunas.
* Click the **[!UICONTROL Filter By]** icon to apply multiple filters to list product profiles with specific criteria. Quando várias categorias de filtro são aplicadas, as pesquisas contêm Grupos associados à `AND` Solução de instância `AND` .

| Elemento | Descrição |
|---------|----------|
| [!UICONTROL Filtro de instâncias] | Procure sequências de caracteres na coluna de instância para restringir os resultados a uma ou várias instâncias. Adicione vários filtros pressionando Enter após cada termo de pesquisa. |
| Filtro [!UICONTROL Solução] | Escolha dentre as soluções disponíveis. Vários filtros de solução pesquisam resultados que contêm a Solução 1 `OR` Solução 2. |

## Detalhes da política de visualização

Na página [!UICONTROL Políticas] , para visualização dos detalhes de uma política, clique no nome do perfil do produto.

![](assets/admin-tool-policy-detail.png)

Uma visualização detalhada de cada perfil de produto exibe detalhes importantes sobre os assuntos do perfil de produto (usuários, grupos e assim por diante). Ele também exibe permissões e recursos habilitados pelo perfil do produto.

Detalhes do perfil do produto podem ser exportados para arquivos CSV. A opção [!UICONTROL Exportar CSV] produz dois arquivos CSV:

* Detalhes do assunto (usuários, grupos de usuários, desenvolvedores, integrações, administradores)
* Itens de permissões e recursos

## Seção Resumo

Esta seção exibe um resumo do perfil do produto, incluindo:

* Nome do perfil do produto
* Número de usuários
* Número de desenvolvedores
* Número de integrações
* Produtos associados
* Instância

## Lista detalhada

Esta seção exibe uma lista completa de todos os usuários, grupos de usuários, desenvolvedores, integrações e administradores atribuídos ao perfil do produto.

| Tabulação | Descrição |
|---------|----------|
| [!UICONTROL Usuários] | Lista de usuários incluída no perfil do produto. A associação do grupo de usuários será exibida na coluna [!UICONTROL Atribuído por grupo] . |
| [!UICONTROL Grupos de usuários] | Lista de grupos de usuários associados ao perfil do produto. |
| [!UICONTROL Desenvolvedores] | Lista de desenvolvedores associados ao perfil do produto. |
| [!UICONTROL Integrações] | Lista de integrações associadas ao perfil do produto. |
| [!UICONTROL Administradores] | Lista de administradores associados ao perfil do produto. |

## Listas detalhadas de permissões e recursos

Esta seção exibe uma lista completa de permissões e recursos disponíveis para o perfil do produto. As permissões e os recursos incluídos no perfil do produto foram marcados com um &quot; ✔&quot;. As listas de permissões e recursos foram categorizadas em guias e colunas para facilitar a visualização. Tabulações e colunas exibem a lista de seções que se aplicam ao produto atual.
