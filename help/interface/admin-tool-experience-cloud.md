---
description: Saiba mais sobre a Ferramenta do administrador da Experience Cloud. Exiba uma lista que pode ser classificada e filtrada de todos os usuários e políticas da Experience Cloud.
keywords: principais serviços
solution: Experience Cloud
title: 'Exibir usuários e detalhes do usuário da Experience Cloud '
index: true
feature: Admin Console
topic: Administração
role: Admin
level: Experienced
exl-id: 127eecdd-3862-48ba-8cf6-a8082d2b7bae
source-git-commit: 1fb1abc7311573f976f7e6b6ae67f60ada10a3e7
workflow-type: tm+mt
source-wordcount: '1248'
ht-degree: 91%

---

# Exibir usuários e políticas da Experience Cloud na Ferramenta administrativa

Os administradores podem exibir uma lista classificável e filtrável de todos os usuários e políticas da Experience Cloud e seus detalhes na Ferramenta de administração. Os detalhes do usuário incluem o acesso ao produto, as funções e as últimas informações acessadas de um usuário. Os detalhes da política incluem usuário (perfil de produto), grupo, desenvolvedor, integração e lista de administração de uma política, bem como permissões e informações detalhadas sobre recursos da política.

>[!NOTE]
>
>O gerenciamento de usuários e produtos está configurado no [Admin Console](admin-getting-started.md).

1. Faça logon no `https://experience.adobe.com/.`

   ![](assets/admin-tool.png)

1. Em [!UICONTROL Acesso rápido], selecione **[!UICONTROL Ferramenta de administração.]**

   (Como alternativa, no URL da página inicial, você pode substituir _início_ por _admin._)

   A página [!UICONTROL Usuários] é exibida.

## Página Usuários

Esta página exibe a lista completa de usuários com acesso à Experience Cloud na organização. Ela fornece informações sobre o direito e o último logon da solução. Pesquise, classifique e filtre exibições personalizadas da lista de usuários.

![](assets/admin-tool-users.png)

| Elemento | Descrição |
|---|---|
| [!UICONTROL Nome] | O nome e sobrenome do usuário. Você pode classificar essa coluna de A a Z e Z a A. Selecione o nome de um usuário para ver mais detalhes sobre ele. |
| [!UICONTROL Email] | O endereço de email associado ao usuário. A coluna pode ser classificada como A->Z, Z->A. |
| [!UICONTROL Tipo de ID] | O tipo de identidade da conta do usuário. O filtro pode ser aplicado a tipos de ID específicos da exibição. Consulte [Gerenciar tipos de identidade](https://helpx.adobe.com/br/enterprise/using/identity.html) para obter mais informações. |
| [!UICONTROL Soluções] | Resumo das soluções da Experience Cloud que o usuário pode acessar. Aplique filtros para restringir a lista de usuários com acesso específico à solução. |
| [!UICONTROL Último logon] | Hora e data do logon mais recente do usuário na Experience Cloud. Essa coluna pode ser classificada por datas crescentes ou decrescentes. <br> **Importante:** a partir de 13 de janeiro de 2020, os últimos dados de logon do usuário serão mantidos por 365 dias. Essas informações são destinadas a mostrar a atividade de logon atual na Experience Cloud e não são uma recomendação para tomar medidas em contas inativas antes de 13 de janeiro de 2020. |

## Personalizar a exibição da lista de usuários

Pesquise, classifique ou filtre as colunas para personalizar a lista de usuários.

* Procure usuários por Nome ou Email. As pesquisas correspondem à cadeia de caracteres de texto digitada.
* Classifique a coluna por valores crescentes ou decrescentes. Isso se aplica às colunas [!UICONTROL Nome], [!UICONTROL Email] e [!UICONTROL Último logon].
* Para aplicar vários filtros a usuários da lista com critérios específicos, selecione o ícone **[!UICONTROL Filtrar por]**. Quando várias categorias de filtro são aplicadas, as pesquisas contêm a Solução `AND` TIPO DE ID `AND` de domínio de email.

| Elemento | Descrição |
|---------|----------|
| Filtro de [!UICONTROL domínio de email] | Procure por cadeias de caracteres na coluna Email para restringir os resultados a um ou vários domínios. Adicione vários filtros pressionando Enter após cada termo de pesquisa. |
| Filtro [!UICONTROL Tipo de ID] | Escolha dentre os Tipos de ID disponíveis. Vários tipos de ID podem ser usados como filtro. |
| Filtro [!UICONTROL Solução] | Escolha dentre as soluções disponíveis. Vários filtros de solução pesquisam resultados que contêm a Solução 1 `OR` Solução 2. |

## Visualizar detalhes do usuário

Na página [!UICONTROL Users], para visualizar os detalhes do usuário, selecione o email do usuário.

![](assets/admin-tool-user-details.png)

Uma exibição detalhada de cada usuário exibe detalhes importantes sobre o acesso à solução do usuário, as funções de administrador e de produto e as informações acessadas pela última vez.

## Seção Sobre

Esta seção exibe um resumo da conta do usuário incluindo:

* Avatar do usuário e selo de administrador do sistema (se aplicável)
* Nome
* Email
* Nome de usuário (contas do Federated ID podem ter nomes de usuário diferentes do endereço de email)
* [Tipo de ID](https://helpx.adobe.com/enterprise/using/identity.html)
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

## Página de políticas

Esta página exibe a lista completa das políticas da Experience Cloud na sua organização. Ela fornece informações sobre produtos, instâncias, usuários e desenvolvedores. Pesquise, classifique e filtre exibições personalizadas da lista de políticas.

![](assets/admin-tool-policies.png)

| Elemento | Descrição |
|---|---|
| [!UICONTROL Perfil de produto] | O nome do perfil do produto. A coluna pode ser classificada como A->Z, Z->A. Para ver mais detalhes sobre a política, selecione o nome do perfil de produto. |
| [!UICONTROL Produto] | O produto associado ao perfil do produto. A coluna pode ser classificada como A->Z, Z->A. |
| [!UICONTROL Instância] | A instância (por exemplo, locatário ou empresa de logon) associada ao perfil do produto. Os produtos que não tiverem instâncias ou locatários únicos exibirão um &quot; - &quot; como valor. A coluna pode ser classificada como A->Z, Z->A. |
| [!UICONTROL Número de usuários] | Contagem específica de usuários associados ao perfil do produto, incluindo atribuição direta e atribuição de grupo. A coluna pode ser classificada da menor para a maior ou da maior para a menor. |
| [!UICONTROL Número de desenvolvedores] | Número de funções de desenvolvedor associadas ao perfil do produto. A coluna pode ser classificada da menor para a maior ou da maior para a menor. |

## Personalizar a exibição da lista de políticas

Pesquise, classifique ou filtre as colunas para personalizar a lista de políticas.

* Pesquise os perfis de produto por nome. As pesquisas correspondem à cadeia de caracteres de texto digitada.
* Classifique a coluna por valores crescentes ou decrescentes. Essa classificação se aplica às colunas [!UICONTROL Perfil do produto], [!UICONTROL Produto], [!UICONTROL Instância], [!UICONTROL Número de usuários], e [!UICONTROL Número de desenvolvedores].
* Selecione o ícone **[!UICONTROL Filtrar por]** para aplicar vários filtros para listar perfis de produto com critérios específicos. Quando várias categorias de filtro são aplicadas, as pesquisas contêm Grupos associados `AND` Instância `AND` Solução.

| Elemento | Descrição |
|---------|----------|
| [!UICONTROL Filtro de] instância | Pesquise por cadeias de caracteres na coluna de instâncias para restringir os resultados a uma ou várias instâncias. Adicione vários filtros pressionando Enter após cada termo de pesquisa. |
| Filtro [!UICONTROL Solução] | Escolha dentre as soluções disponíveis. Vários filtros de solução pesquisam resultados que contêm a Solução 1 `OR` Solução 2. |

## Exibir detalhes da política

Na página [!UICONTROL Policies], para visualizar os detalhes de uma política, selecione o nome do perfil de produto.

![](assets/admin-tool-policy-detail.png)

Uma visualização detalhada de cada perfil de produto exibe detalhes importantes sobre os assuntos do perfil de produto (usuários, grupos e assim por diante). Ela também exibe permissões e recursos habilitados pelo perfil do produto.

Detalhes do perfil do produto podem ser exportados para arquivos CSV. A opção [!UICONTROL Exportar CSV] produz dois arquivos CSV:

* Detalhes do assunto (usuários, grupos de usuários, desenvolvedores, integrações, administradores)
* Itens de permissões e recursos

## Seção de resumo

Esta seção exibe um resumo do perfil de produto com estas informações:

* Nome do perfil do produto
* Número de usuários
* Número de desenvolvedores
* Número de integrações
* Produtos associados
* Instância

## Lista detalhada do assunto

Esta seção exibe uma lista completa de todos os usuários, grupos de usuários, desenvolvedores, integrações e administradores atribuídos ao perfil do produto.

| Tabulação | Descrição |
|---------|----------|
| [!UICONTROL Usuários] | Lista de usuários incluída no perfil do produto. A associação do grupo de usuários será exibida na coluna [!UICONTROL Atribuído por grupo]. |
| [!UICONTROL Grupos de usuários] | Lista de grupos de usuários associados ao perfil do produto. |
| [!UICONTROL Desenvolvedores] | Lista de desenvolvedores associados ao perfil do produto. |
| [!UICONTROL Integrações] | Lista de integrações associadas ao perfil do produto. |
| [!UICONTROL Administradores] | Lista de administradores associados ao perfil do produto. |

## Listas detalhadas de permissões e recursos

Esta seção exibe uma lista completa de permissões e recursos disponíveis para o perfil do produto. As permissões e os recursos incluídos no perfil do produto foram marcados com um &quot; ✔&quot;. As listas de permissões e recursos foram categorizadas em guias e colunas para facilitar a visualização. Tabulações e colunas exibem a lista de seções que se aplicam ao produto atual.
