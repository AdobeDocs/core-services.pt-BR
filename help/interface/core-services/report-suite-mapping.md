---
description: Saiba mais sobre como mapear um ou vários conjuntos de relatórios para uma organização.
seo-description: Saiba mais sobre como mapear um ou vários conjuntos de relatórios para uma organização.
seo-title: Mapear conjuntos de relatórios para uma organização
title: Mapear conjuntos de relatórios para uma organização
uuid: b983d5a6-b3d0-4137-ac53-bc5681d3e58b
translation-type: tm+mt
source-git-commit: 73cb227d2b44024706ce24a9ae6aa06c57a8ce85

---


# Mapear conjuntos de relatórios para uma organização {#topic_7C4740559EAC4E0FA5F8DEF886B580DA}

Saiba mais sobre como mapear um ou vários conjuntos de relatórios para uma organização.

Os serviços da Experience Cloud (como o Serviço da Experience Cloud ID e o serviço principal de Pessoas) estão associados a uma organização em vez de a um conjunto de relatórios individual. Para garantir o funcionamento correto desses serviços, cada conjunto de relatórios do Analytics deve ser mapeado para uma organização. O processo de mapeamento:

* Define uma organização da Experience Cloud como a organização principal do conjunto de relatórios.
* Não muda quem pode acessar um conjunto de relatórios (o acesso ainda é determinado pela conta de logon do Adobe Analytics de cada usuário)

**Requisitos**

Você deve ser um administrador do Analytics de uma empresa de logon com acesso ao conjunto de relatórios que deseja mapear. Além disso, essa conta deve estar [vinculada a uma organização da Experience Cloud](../admin-getting-started/organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1) a fim de mapear conjuntos de relatórios para essa organização.

As organizações ficam esmaecidas caso você não tenha permissões de administrador do Analytics para uma empresa de logon sob a organização com acesso ao conjunto de relatórios em questão.

## Mapear um conjunto de relatórios para uma organização {#task_23993FE78DF6455FA8D7BE60686EA16C}

1. Clique em **[!UICONTROL Experience Cloud]** > **[!UICONTROL Administração]** > **[!UICONTROL Mapeamento de conjuntos de relatórios]**

1. Para ver as empresas de logon com acesso a cada conjunto de relatórios, clique em **[!UICONTROL Visível para empresas de logon]**.

   Essa exibição ajuda você a tomar decisões informadas sobre o mapeamento.

1. Clique no menu suspenso na coluna **[!UICONTROL Organização mapeada]** ao lado de um conjunto de relatórios e selecione a organização para a qual você deseja mapear.

   Consulte a próxima seção para obter dicas sobre como selecionar uma organização da Experience Cloud.

## Mapear diversos conjuntos de relatórios para uma organização {#task_94955B0D8ABA4CB1A38746ECF8E32711}

1. Clique em **[!UICONTROL Experience Cloud]** > **[!UICONTROL Administração]** > **[!UICONTROL Mapeamento de conjuntos de relatórios]**.

1. Selecione os conjuntos de relatórios que você deseja mapear.

   ![](assets/rs-mapping-multiple.png)

1. Selecione a organização (Outdoors Inc, nesse exemplo) e clique em **[!UICONTROL Selecionar]**.

   Consulte a próxima seção para obter dicas sobre como selecionar uma organização da Experience Cloud.

1. Clique em **[!UICONTROL Salvar mapeamento]**.

## Dicas para selecionar uma organização da Experience Cloud {#mapping-tips}

Esta seção contém dicas para ajudar a selecionar a organização da Experience Cloud para a qual você deve mapear um conjunto de relatórios.

**Qual organização devo escolher?**

If the Experience Cloud ID Service is currently deployed on the report suite, ensure the organization you select in the Report Suite Mapping tool is the same organization specified in the [!DNL visitorAPI.js] file on your site. Você pode usar as instruções em [Testar e verificar o serviço da Experience Cloud ID](https://docs.adobe.com/content/help/en/id-service/using/implementation-guides/test-verify.html) para encontrar a ID da organização em uso pelo serviço de ID do visitante.

Se o serviço de ID do visitante ainda não estiver implantado nos sites que coletam dados do conjunto de relatórios e você implantar o serviço de ID de visitante da Experience Cloud futuramente, verifique se a implantação corresponde à organização selecionada na ferramenta de Mapeamento de conjuntos de relatórios.

**Por que algumas organizações estão esmaecidas?**

Isso indica que você não tem privilégios suficientes para mapear para o conjunto de relatórios esmaecido. Considere o exemplo a seguir:
![](assets/rs-mapping.png) Nesse diagrama, a tecla azul indica privilégios de administrador. As linhas cinzas indicam visibilidade.

Esse usuário tem acesso a duas organizações da Experience Cloud. Ele fez o seguinte:

* Vinculou sua conta de administrador na empresa de logon chapek do Analytics à conta organizacional Chapek Corp da Experience Cloud.
* Vinculou sua conta de não administrador na empresa de logon doohan do Analytics à conta organizacional Chapek Corp da Experience Cloud.
* Vinculou sua conta de não administrador na empresa de logon nigel do Analytics à conta organizacional Nigel Inc da Experience Cloud.

Os pontos a seguir listam as ações de mapeamento que o usuário pode ou não executar com relação aos conjuntos de relatórios:

* O conjunto de relatórios de produção Chapek pode ser mapeado para a organização Chapek Corp, pois esse usuário é um administrador de uma empresa de logon vinculada do Analytics (chapek) e sua conta está vinculada a essa organização.
* O conjunto de relatórios de produção Nigel não pode ser vinculado por esse usuário, pois ele não é um administrador em nenhuma empresa de logon na qual o conjunto de relatórios está visível.
* O conjunto de relatórios de produção Doohan pode ser mapeado para a Chapek Corp, pois esse usuário é um administrador de uma empresa de logon (chapek) vinculada à organização da Experience Cloud (observe que ele não é um administrador da empresa de logon doohan do Analytics). É importante reconhecer que o conjunto de relatórios de produção doohan também está qualificado para ser mapeado para a organização Nigel Inc da Experience Cloud, mesmo que esse usuário não possa realizar esse mapeamento. Nesse caso, as organizações da Experience Cloud são exibidas na lista, mas Nigel Inc aparece esmaecida. Antes de mapear, o usuário deve consultar um administrador na empresa de logon nigel a fim de determinar qual organização é a melhor candidata para o mapeamento. A interface do usuário exibirá um aviso de conflito possível se você selecionar uma organização diferente daquela em que o conjunto de relatórios foi criado originalmente.

## Perguntas frequentes {#section_099E485805994C929FF9C9F75219BEE1}

**Por que não consigo ver todos os meus conjuntos de relatórios?**

Alguns dos conjuntos de relatórios podem ser visíveis em uma empresa de logon diferente. Você pode alterar a empresa de logon atual usando o menu suspenso na parte superior da tela.

**O que acontece se eu não reconhecer algumas das organizações listadas no menu suspenso de um dos meus conjuntos de relatórios?**

A lista mostra todas as *organizações *possíveis para as quais o conjunto de relatórios pode ser mapeado, mesmo que você não tenha permissão para mapear para todos esses conjuntos de relatórios. Caso não tenha certeza se o conjunto de relatórios deve estar mapeado para um dos conjuntos de relatórios esmaecidos na lista, consulte um administrador da Experience Cloud na organização para determinar a melhor opção.

**O que acontece se eu não reconhecer algumas das empresas de logon listadas para um conjunto de relatórios na coluna “Visível para empresas de logon”?**

Em algum momento, esse conjunto de relatórios foi compartilhado com outra empresa de logon que pode fazer parte de uma organização diferente da Experience Cloud.

**O que é o erro de “conflito possível” sobre o conjunto de relatórios gerado por outra organização? Por que isso é importante?**

Essa é uma notificação que ajuda você a tomar decisões informadas sobre o mapeamento do conjunto de relatórios. Você deve reconhecer que o conjunto de relatórios foi criado originalmente sob uma organização diferente, caso essa organização seja mais adequada para o conjunto de relatórios.

**Como faço para saber se um conjunto de relatórios já está mapeado?**

Os conjuntos de relatórios mapeados serão exibidos em um formato não editável. Se for necessário alterar o mapeamento, entre em contato com o Atendimento ao cliente.

**Como devo proceder se souber somente a ID organizacional da minha organização da Experience Cloud? Como faço para buscar o nome da minha ID organizacional?**

É possível encontrar o nome da organização em [Organizações e configurações da conta](https://docs.adobe.com/content/help/en/core-services/interface/manage-users-and-products/organizations.html).

**Vejo uma data na coluna “Data de mapeamento”. Quem fez esse mapeamento?**

Você pode consultar o Log de alterações do conjunto de relatórios na interface do Analytics para verificar a ID do usuário que fez a alteração. Procure o evento “Suite associated to IMS Organization”.
