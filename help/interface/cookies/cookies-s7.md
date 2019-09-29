---
description: O Scene7 usa cookies para armazenar informações úteis que podem ser usadas para fornecer mídia dinâmica ao navegador.
keywords: cookies; privacidade
seo-description: O Scene7 usa cookies para armazenar informações úteis que podem ser usadas para fornecer mídia dinâmica ao navegador.
seo-title: Cookies do Scene7
solution: Experience Cloud,Analytics,Target,Social
title: Cookies do Scene7
uuid: f9b9d13a-17e5-4139-8c84-6fe5d22c4196
index: y
internal: n
snippet: y
translation-type: tm+mt
source-git-commit: 7137e608ddece5bf2a3983b3b18909ba89d607a6

---


# Cookies do Scene7{#scene-cookies}

O Scene7 usa cookies para armazenar informações úteis que podem ser usadas para fornecer mídia dinâmica ao navegador.

O Scene7 armazena informações localmente para alguns visualizadores mais antigos baseados em AS2 Flash.

Para visualizadores AS2, os cookies:

* Rastreiam o estado da sessão de um usuário, como a página atual e a imagem visualizada, o nível de zoom atual, etc.
* Determinam quanto tempo se passou desde a última sessão do usuário. O visualizador usa estas informações para decidir se deve continuar uma sessão anterior ou criar uma nova. Estas informações também são enviadas para os servidores Scene7, mas não são usadas.

Para visualizadores AS2 Flash eCatalog, os cookies:

* Armazenam conteúdo gerado pelo usuário (a maioria do conteúdo é inserido pelo usuário no recurso de "notas adesivas" do visualizador de catálogo eletrônico). Este conteúdo é restabelecido quando o usuário retoma uma sessão.
* Quando o usuário inicia um email para compartilhar o catálogo eletrônico com outro usuário, o conteúdo das notas adesivas do segundo marcador do visualizador AS2 é copiado para os nossos servidores para que o forneçamos ao destinatário. Quando o destinatário inicia a sessão de visualizador, o conteúdo das notas adesivas é recuperado do servidor e copiado em um cookie. Este recurso é pouco usado, portanto não expira e o conteúdo antigo não é removido. No momento, persiste no servidor por tempo indeterminado.

Os visualizadores AS3 mais recentes não implementam persistência de sessão.

**Nome do cookie: VatLogin.jsp**

| Atributo | Descrição |
|---|---|
| Informações armazenadas | Define o cookie da sessão. O AuthFilter integrado no IPS ImageServer (IS, IR e também os SWFs/capas e contextos de vídeo) usa o cookie para a autorização do acesso. Se estiver presente, permite que solicitações HTTP passem. Do contrário, retorna não autorizado. |
| Expiração | Este cookie é um cookie de sessão. A expiração da sessão atual está definida como 45 minutos no IPS [!DNL web.xml] do Scene7. |

**Nome do cookie: s7js.flyout.InfoMessage.displayed`assetId`.state**

<table id="table_6835D64C5D464A049F576621F2BE3FAD"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Atributo </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> Informações armazenadas </td> 
   <td colname="col2"> <p>&lt;assetId&gt; é o nome do ativo com o qual o visualizador está trabalhando. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Expiração </td> 
   <td colname="col2"> Este cookie é um cookie de sessão e expira quando o navegador é fechado. </td> 
  </tr> 
 </tbody> 
</table>

**Nome do cookie: s7js.flyout.InfoMessage.displayed`assetId`_idx`id`.ant**

Os cookies de navegador são usados por visualizadores DHTML herdados para armazenar informações de estado e dados de notas aderentes. Também são usado pelo menu DHTML multitela para tornar o indicador de mensagens em específico da sessão.

<table id="table_8F6CC83D32D54BEE99884318AD126C98"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Atributo </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> Informações armazenadas </td> 
   <td colname="col2"> <p> </p> <p> &lt;assetId&gt; é o nome do ativo com o qual o visualizador está trabalhando e &lt;id&gt; é o índice de nota aderente com base em 0. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Expiração </td> 
   <td colname="col2"> Este cookie é um cookie de sessão e expira quando o navegador é fechado. </td> 
  </tr> 
 </tbody> 
</table>

