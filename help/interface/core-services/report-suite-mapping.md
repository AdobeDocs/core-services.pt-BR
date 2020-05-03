---
description: Saiba mais sobre como mapear um ou vários conjuntos de relatórios para uma organização.
seo-description: Saiba mais sobre como mapear um ou vários conjuntos de relatórios para uma organização.
seo-title: Mapear conjuntos de relatórios para uma organização
title: Mapear conjuntos de relatórios para uma organização
uuid: b983d5a6-b3d0-4137-ac53-bc5681d3e58b
translation-type: tm+mt
source-git-commit: 31811e718be130612c8688e80084cb7579e94f47

---


# Mapear conjuntos de relatórios para uma organização {#topic_7C4740559EAC4E0FA5F8DEF886B580DA}

Saiba mais sobre como mapear um ou vários conjuntos de relatórios para uma organização.

Os serviços da Experience Cloud (como o Serviço da Experience Cloud ID e [!UICONTROL Pessoas]) estão associados a uma organização em vez de a um conjunto de relatórios individual. Para garantir o funcionamento correto desses serviços, cada conjunto de relatórios do Analytics deve ser mapeado para uma organização. O processo de mapeamento:

* Define uma organização da Experience Cloud como a organização principal do conjunto de relatórios.
* Não altera quem pode acessar um conjunto de relatórios (o acesso ainda é determinado pela conta de logon do Adobe Analytics para cada usuário)

## Exigências

Você deve ser um administrador do Analytics de uma empresa de logon que tenha acesso ao conjunto de relatórios que deseja mapear. Além disso, essa conta deve estar [vinculada a uma organização](../admin-getting-started/organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1) da Experience Cloud para mapear conjuntos de relatórios para essa organização.

As organizações ficam esmaecidas caso você não tenha permissões de administrador do Analytics para uma empresa de logon sob a organização com acesso ao conjunto de relatórios em questão.

## Mapear um conjunto de relatórios para uma organização {#task_23993FE78DF6455FA8D7BE60686EA16C}

1. Click **[!UICONTROL Experience Cloud]** > **[!UICONTROL Administration]** > **[!UICONTROL Report Suite Mapping]**

1. Para ver as empresas de logon com acesso a cada conjunto de relatórios, clique em **[!UICONTROL Visível para empresas de logon]**.

   Essa exibição ajuda você a tomar decisões informadas sobre o mapeamento.

1. Clique no menu suspenso na coluna **[!UICONTROL Organização mapeada]** ao lado de um conjunto de relatórios e selecione a organização para a qual você deseja mapear.

   Consulte a próxima seção para obter dicas sobre como selecionar uma organização da Experience Cloud.

## Mapear diversos conjuntos de relatórios para uma organização {#task_94955B0D8ABA4CB1A38746ECF8E32711}

1. Click **[!UICONTROL Experience Cloud]** > **[!UICONTROL Administration]** > **[!UICONTROL Report Suite Mapping]**.

1. Selecione os conjuntos de relatórios que você deseja mapear.

   ![](assets/rs-mapping-multiple.png)

1. Selecione a organização (Outdoors Inc, nesse exemplo) e clique em **[!UICONTROL Selecionar]**.

   Consulte a próxima seção para obter dicas sobre como selecionar uma organização da Experience Cloud.

1. Clique em **[!UICONTROL Salvar mapeamento]**.

## Dicas para selecionar uma organização da Experience Cloud {#mapping-tips}

Esta seção contém dicas para ajudá-lo a selecionar a organização da Experience Cloud para a qual você deve mapear um conjunto de relatórios.

### Qual organização devo escolher?

If the Experience Cloud ID Service is currently deployed on the report suite, ensure the organization you select in the Report Suite Mapping tool is the same organization specified in the [!DNL visitorAPI.js] file on your site. You can use the instructions in [Test and Verify the Experience Cloud ID Service](https://docs.adobe.com/content/help/en/id-service/using/implementation-guides/test-verify.html) to find the org ID that is being used by the Visitor ID service.

Se o serviço de ID de Visitante ainda não estiver implantado nos sites que coletam dados para o conjunto de relatórios, se você implantar o serviço de ID de Visitante da Experience Cloud no futuro, será necessário garantir que sua implantação corresponda à organização selecionada na ferramenta Mapeamento de conjuntos de relatórios.

### Por que algumas organizações estão esmaecidas?

Isso indica que você não tem privilégios suficientes para mapear para o conjunto de relatórios esmaecido. Considere o exemplo a seguir:

![](assets/rs-mapping.png)

Nesse diagrama, a tecla azul indica privilégios de administrador. As linhas cinzas indicam visibilidade.

Esse usuário tem acesso a duas organizações da Experience Cloud. Ele fez o seguinte:

* Vinculou sua conta de administrador na empresa de logon [!UICONTROL chapek] do Analytics à conta de organização da [!UICONTROL Chapek] Corp Experience Cloud.
* Vinculou sua conta de não administrador na empresa de logon do [!UICONTROL doohan] Analytics à conta organizacional [!UICONTROL Chapek] Corp da Experience Cloud.
* Vinculou sua conta de não administrador na empresa de logon nigel do Analytics à conta organizacional Nigel Inc da Experience Cloud.

Os pontos a seguir listas das ações de mapeamento que esse usuário pode ou não executar em relação a esses conjuntos de relatórios:

* [!UICONTROL O conjunto de relatórios de produção] Chapek pode ser mapeado para a organização [!UICONTROL Chapek] Corp, pois esse usuário é um administrador de uma empresa de logon vinculada do Analytics ([!UICONTROL chapek]) e sua conta está vinculada a essa organização.
* [!UICONTROL O conjunto de relatórios de produção] Nigel não pode ser vinculado por esse usuário, pois ele não é um administrador em nenhuma empresa de logon na qual este conjunto de relatórios está visível.
* [!UICONTROL O conjunto de relatórios de produção] Doohan pode ser mapeado para a [!UICONTROL Chapek Corp] , pois esse usuário é um administrador de uma empresa de logon ([!UICONTROL chapek]) vinculada à organização da Experience Cloud (observe que ele não é um administrador da empresa de logon doohan do Analytics). É importante estar ciente de que o conjunto de relatórios de produção [!UICONTROL de] doohan também está qualificado para ser mapeado para a organização Nigel Inc da Experience Cloud, mesmo que esse usuário não possa realizar esse mapeamento. Nesse caso, ambas as organizações da Experience Cloud são exibidas na lista, mas a [!UICONTROL Nigel Inc] está esmaecida. Antes de mapear, esse usuário deve consultar um administrador da empresa de logon nigel para determinar qual organização é a melhor candidata para mapeamento. A interface do usuário exibe um aviso de conflito possível se você selecionar uma organização diferente daquela na qual o conjunto de relatórios foi criado originalmente.

## Perguntas frequentes {#section_099E485805994C929FF9C9F75219BEE1}

### Por que não vejo todos os meus conjuntos de relatórios?

Alguns de seus conjuntos de relatórios podem estar visíveis em uma empresa de logon diferente. Você pode alterar a empresa de login atual usando o menu suspenso na parte superior da tela.

### E se eu não reconhecer algumas das organizações listadas no menu suspenso de um dos meus conjuntos de relatórios?

The list shows you all the *possible* organizations your report suite could be mapped to, even you don’t have permission to map to all those report suites. Se não tiver certeza se o conjunto de relatórios deve ser mapeado para um dos conjuntos de relatórios esmaecidos na lista, consulte um administrador da Experience Cloud na organização para determinar a melhor opção.

### E se eu não reconhecer algumas Empresas de logon listadas para um conjunto de relatórios na coluna &quot;Visível para efetuar logon no Empresa&quot;?

Em algum momento, esse conjunto de relatórios foi compartilhado com outra empresa de logon que pode fazer parte de uma organização diferente da Experience Cloud.

### O que é esse erro de &quot;conflito possível&quot; sobre o conjunto de relatórios que está sendo gerado por outra organização? Por que isso importa?

Esta é uma notificação para ajudá-lo a tomar uma decisão informada sobre o mapeamento do conjunto de relatórios. Queremos informá-lo de que o conjunto de relatórios foi criado originalmente abaixo de uma organização diferente, caso essa organização seja mais apropriada para esse conjunto de relatórios.

### Como faço para saber se um conjunto de relatórios está mapeado?

Os conjuntos de relatórios mapeados serão exibidos em um formato não editável. Se precisar alterar um mapeamento, entre em contato com o Atendimento ao cliente.

### E se eu souber somente a ID organizacional da minha organização da Experience Cloud? Como faço para buscar o nome da minha ID organizacional?

Você pode encontrar o nome da sua organização em [Organizações e Configurações](https://docs.adobe.com/content/help/pt-BR/core-services/interface/manage-users-and-products/organizations.html)da conta.

### Vejo uma data na coluna &quot;Data de mapeamento&quot;. Quem fez esse mapeamento?

Consulte o Log de alterações do conjunto de relatórios na interface do Analytics para verificar a ID do usuário que fez a alteração. Procure o evento &quot;Suite associado à Organização IMS&quot;.
