---
description: Saiba mais sobre o fluxo de trabalho de alto nível do Gerenciamento de ofertas, incluindo criação de ofertas e disposições, inserção de atividades de ofertas e exibição de relatórios.
seo-description: Saiba mais sobre o fluxo de trabalho de alto nível do Gerenciamento de ofertas, incluindo criação de ofertas e disposições, inserção de atividades de ofertas e exibição de relatórios.
seo-title: Fluxo de trabalho do gerenciamento de ofertas
title: Fluxo de trabalho do gerenciamento de ofertas
uuid: c95ec474-88de-4e6e-92bf-f49f3a7b32c5
index: y
internal: n
snippet: y
translation-type: tm+mt
source-git-commit: 2f0c2eb70313c42da9e7ac1d75429ec768dea10d

---


# Fluxo de trabalho do gerenciamento de ofertas{#offer-management-workflow}

Saiba mais sobre o fluxo de trabalho de alto nível do Gerenciamento [!UICONTROL de]ofertas, incluindo criação de ofertas e disposições, inserção de atividades de ofertas e exibição de relatórios.

## Etapa 1 - Determine onde em seus modelos de e-mail você precisa de ofertas personalizadas {#section_F184E589428B403EA8EB921BF230CF87}

Identifique em quais campanhas de email você deseja inserir ofertas personalizadas. A partir daí, determine os locais em seu modelo de email para inserir essas ofertas. Por exemplo, você pode modificar a oferta de produto com base no setor ou na pessoa do cliente, alterar a mensagem com base nos mesmos critérios e variar a imagem com base na geografia do cliente.

![](assets/workflow1.png)

## Etapa 2 - Determine quais atributos do Campaign você deseja segmentar e compartilhá-los com o Gerenciamento de ofertas {#section_1461F1FAC0B943E5BBDED6B3B00E9D5C}

Ao criar uma oferta no Gerenciamento [!UICONTROL de]ofertas, você pode definir regras de qualificação que restrinjam quais perfis podem receber determinadas ofertas. Essas regras de elegibilidade podem ser definidas com base nos atributos (ou campos) existentes no Adobe Campaign. Esses campos devem ser compartilhados do Campaign por um usuário de nível administrativo antes de serem exibidos no construtor de regras de qualificação do Gerenciamento de [!UICONTROL ofertas] .

Para obter informações sobre como compartilhar esses atributos, consulte [Compartilhar atributos da Campanha para o Gerenciamento](campaign.md#task_4DFA9A20D7B04E1F9AFF4774D67B6EBC)de ofertas.

## Etapa 3 - Inserir disposições necessárias no Gerenciamento [!UICONTROL de] ofertas {#section_71619756A86F4DB58B8200D8A1CE1B87}

Uma disposição ajuda a garantir que o conteúdo da oferta certa seja exibido no local certo no modelo de e-mail. Ao adicionar conteúdo a uma oferta, você será solicitado a selecionar uma disposição na qual o conteúdo possa ser exibido.

É possível ter vários locais com a mesma disposição. No exemplo a seguir, há duas disposições para duas imagens de tamanho diferente e uma única disposição para o texto que é exibida na parte superior e inferior do modelo.

Depois de determinar as disposições necessárias, adicione-as à guia [!UICONTROL Posicionamento] .

![](assets/workflow2.png)

## Etapa 4 - Criar suas ofertas {#section_C4F9732B0596425EB0BD5AE76E4BA6EF}

Crie as ofertas que você usará em sua campanha por email. Há dados e conteúdo que podem ser adicionados à oferta para determinar a melhor oferta para servir e determinar que conteúdo mostrar. Ao criar uma representação de conteúdo, associe-a a uma das disposições definidas em [Disposições](placements.md). Após criar e enviar uma oferta, ela estará disponível para uso em uma atividade de oferta.

![](assets/workflow3.png)

## Etapa 5 - Crie sua campanha por email e insira uma atividade de oferta {#section_6FD36404759B4C6E9FD3A65ACABB26C8}

Agora que você criou suas ofertas, pode usá-las em uma campanha por email. No editor de conteúdo, você pode selecionar um bloco e inserir uma atividade de oferta. Uma atividade de oferta permite que você selecione um grupo de ofertas do seu inventário de ofertas, a partir do qual o mecanismo de decisão determinará a melhor oferta para atender cada usuário.

![](assets/workflow4.png)

## Etapa 6 - Prepare e envie sua campanha por email {#section_EDD8EA4696664130A678D7C4483DA806}

Agora, ao preparar sua campanha por email, o [!UICONTROL Gerenciamento] de ofertas determinará a melhor oferta para atender cada visitante com base na data atual, nos atributos do perfil e na prioridade. Também determina se há uma representação de conteúdo disponível para a colocação desse local.

No exemplo a seguir, suponha que você tenha configurado uma campanha por email com uma atividade de oferta contendo 3 ofertas (A, B, C). Você pode determinar qual oferta deve servir em um dos locais em nosso email. No momento da preparação, o Gerenciamento [!UICONTROL de] ofertas:

1. Analise a data atual, os dados de perfil de cada usuário e a prioridade.
1. Compare essas informações com os dados das ofertas.
1. Determine a melhor oferta para servir.

![](assets/workflow5.png)

## Etapa 7 - Exibir relatórios {#section_2104BAACAE154DE29B6EEB967C46F226}

Você pode exibir um relatório sobre quais ofertas foram fornecidas e como elas foram executadas em uma atividade de oferta. Esse relatório pode ser visualizado selecionando a guia relatórios na página inicial do Adobe Campaign Standard.
