---
description: Saiba mais sobre o recurso Pesquisa unificada para determinados aplicativos na Experience Cloud.
solution: Experience Cloud
title: Pesquisa unificada da Experience Cloud
index: true
feature: Central Interface Components
topic: Administration
role: Admin
level: Beginner
exl-id: 70586f18-6f84-4308-bab3-1da7fab823d6
source-git-commit: c447723f4d6c57bdccad6c4a8996693aec4a56fe
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 19%

---

# [!UICONTROL Unified Search] para objetos e entidades

A pesquisa do [!UICONTROL Unified Search] permite encontrar objetos ou entidades comerciais pesquisáveis por meio de uma experiência contínua, consistente e com apenas um clique. Essa pesquisa também exibe os objetos acessados recentemente.

![Pesquisar objetos e entidades globalmente](../assets/platform-search.png)

## Acesso à Pesquisa unificada

A Pesquisa unificada está disponível em todas as páginas no cabeçalho do Experience Cloud, na parte superior da página. Você também pode usar o atalho de teclado `command /` ou `ctrl /` para acessar a pesquisa.

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

![Pesquisa unificada na Experience Cloud](../assets/unified-search-results.png)

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

Por exemplo, _Como criar um esquema_ produz resultados do Experience League em _[!UICONTROL Learning]_:

![Ajuda para a Pesquisa unificada da Experience Cloud](../assets/unified-search-learning.png)

Os algoritmos de pesquisa exibem os registros mais relevantes primeiro. A ordem dos resultados depende de vários fatores, como:

* Permissões de usuário para acessar os objetos
* Porcentagem de correspondência
* Correspondências exatas
* A seção _[!UICONTROL Top Results]_&#x200B;mostra os 30 principais resultados.

Para refinar a pesquisa, clique em uma das opções a seguir:

* **[!UICONTROL All Learning]**: abre a pesquisa no Experience League.
* **[!UICONTROL Show all...]**: permite refinar e filtrar mais os resultados.

## Recursos de pesquisa unificada

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
