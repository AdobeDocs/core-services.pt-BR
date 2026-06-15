---
description: Saiba mais sobre o recurso de Pesquisa unificada para determinados aplicativos no CX Enterprise.
solution: Experience Cloud
title: Pesquisa unificada da Experience Cloud
index: true
feature: Central Interface Components
topic: Administration
role: Admin
level: Beginner
exl-id: 70586f18-6f84-4308-bab3-1da7fab823d6
TQID: https://experienceleague.adobe.com/xE4H6kdjbKSwVygCsOV4zTBqPoBHAVMHfJMyYOummg0
product_v2: id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2: id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2: id: b75843fa-0a67-4a44-a6b1-cc627b0481dcid: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 50012e2564e88e1a6e16578e3331136c7df0cb21
workflow-type: tm+mt
source-wordcount: 660
ht-degree: 17%

---

# [!UICONTROL Pesquisa unificada] na CX Enterprise

A [!UICONTROL Pesquisa unificada] permite encontrar objetos ou entidades comerciais pesquisáveis por meio de uma experiência contínua, consistente e com apenas um clique. Essa pesquisa também exibe os objetos acessados recentemente.

![Pesquisar objetos e entidades globalmente](../assets/platform-search.png)

## Acessando [!UICONTROL Pesquisa Unificada]

A [!UICONTROL Pesquisa unificada] está disponível em todas as páginas do cabeçalho do CX Enterprise na parte superior da página. Você também pode usar o atalho de teclado `command /` ou `ctrl /` para acessar a pesquisa.

Esse recurso está disponível somente para os produtos compatíveis, que atualmente são:

* Experience Platform (AEP)
* Journey Optimizer (AJO)

À medida que mais conteúdo for indexado, esse recurso será adicionado aos aplicativos relevantes.

## Objetos e campos pesquisáveis

À medida que você digita, os principais resultados correspondentes aos objetos que você tem acesso são exibidos.

Nossos algoritmos mostram primeiro os registros mais relevantes. A ordem dos resultados depende de vários fatores, como:

Sua capacidade e permissões de objeto
Porcentagem de correspondência
Se há uma correspondência exata

![[!UICONTROL Pesquisa unificada] na CX Enterprise](../assets/unified-search-results.png)

Os objetos comerciais pesquisáveis incluem:

* Segmentos (nome, descrição, ID)
* Esquema (nome, descrição, ID)
* Conjuntos de dados (nome, descrição, ID)
* Fontes (nome, descrição, ID)
* Destinos (nome, descrição, ID)
* Consultas (nome, descrição, ID)
* Mensagens (nome, descrição, ID)
* Ofertas (nome, descrição, ID)
* Componentes (nome, descrição, ID)
* Jornadas (nome, descrição, ID)

Se uma palavra-chave corresponder a uma página de navegação, você poderá obter um link de acesso rápido para os conjuntos de dados de exemplo da página de navegação. A seção Principais resultados mostra os 30 principais resultados.

Você também encontrará os artigos de ajuda da Experience League e das comunidades. As consultas de linguagem natural são compatíveis.

Por exemplo, _Como criar um esquema_ produz resultados do Experience League em _[!UICONTROL Aprendizado]_:

![[!UICONTROL Pesquisa unificada] na Ajuda da CX Enterprise](../assets/unified-search-learning.png)

Os algoritmos de pesquisa exibem os registros mais relevantes primeiro. A ordem dos resultados depende de vários fatores, como:

* Permissões de usuário para acessar os objetos
* Porcentagem de correspondência
* Correspondências exatas
* A seção _[!UICONTROL Principais resultados]_ mostra os 30 principais resultados.

Para refinar a pesquisa, clique em uma das opções a seguir:

* **[!UICONTROL Todo o aprendizado]**: abre a pesquisa no Experience League.
* **[!UICONTROL Mostrar tudo...]**: permite refinar e filtrar mais os resultados.

## Recursos da [!UICONTROL Pesquisa Unificada]

Os seguintes recursos estão disponíveis na Pesquisa unificada.

| Recurso | Descrição |
| ------- | ------- |
| Suporte global a idiomas | A pesquisa global entende consultas e produz resultados para alemão, espanhol, francês, italiano, japonês, coreano, português e chinês. |
| Tolerância a erros de digitação | A pesquisa unificada oferece tolerância robusta a erros de digitação usando algoritmos avançados. Esses algoritmos calculam as edições e fornecem resultados apropriados. |
| Realce | A resposta da pesquisa destaca a palavra-chave correspondente na consulta de pesquisa, para que você possa encontrar facilmente a seção e as palavras que correspondem à consulta. O realce também funciona para palavras com erro ortográfico. |
| Trechos | Na resposta da pesquisa, você pode ver um trecho do resultado. Os trechos retornam as palavras correspondentes e algum conteúdo em torno das palavras-chave correspondentes. |
| Palavras de interrupção | Algumas palavras usadas com frequência em inglês são definidas como _palavras de interrupção_. Se palavras de interrupção forem incluídas na consulta de pesquisa, menos peso será dado a elas. <br>As palavras de interrupção incluem: _a, an, and, are, as, at, be, but, by, for, if, in, into, is, it, no, not, of, on ou, such, that, the, their, then, there, these, this, to, was, will, with_. <br>Não há suporte para palavras de interrupção em outros idiomas globais. |
| Consultas de linguagem natural | Ao procurar um artigo de ajuda ou uma discussão nas comunidades do Experience League, você pode digitar a pergunta em linguagem natural e obter a resposta. Exemplo de pesquisa: &quot;Como criar um esquema?&quot; |
| Pesquisa exata entre aspas | Você pode fazer uma pesquisa exata usando aspas na query. Nenhuma correção de erro de digitação é feita em consultas de correspondência exata. Por exemplo: &quot;Luma Jornada 2022&quot;. |
| Filtros | Você pode aplicar filtros como _Tipo de objeto_ e outros filtros específicos de objeto na janela pop-up de resultados da pesquisa completa. Quando você pressiona Enter depois de vincular a consulta de pesquisa, um pop-up de página inteira é aberto com os filtros. |

{style="table-layout:auto"}

## Não consegue encontrá-lo?

Experimente estas dicas:

* Insira um termo de pesquisa mais específico
* Verificar a ortografia
* Tentar escrever o termo de pesquisa completo
* Verifique se você tem permissões para objetos que você procura

