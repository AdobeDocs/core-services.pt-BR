---
description: Como o Adobe Scene7 usa cookies para armazenar informações úteis que podem ser usadas para entrega de dynamic media ao navegador.
keywords: cookies; privacidade
solution: Experience Cloud,Analytics,Target
title: 'Cookies do Scene7 '
uuid: f9b9d13a-17e5-4139-8c84-6fe5d22c4196
feature: Cookies
topic: Administração
role: Administrator
level: Experienced
exl-id: ecb8d17f-f752-44ca-8877-44752c28dc70
source-git-commit: c7ed1324015beb7ebcf7a4ee21b05601e36e608f
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 85%

---

# Cookies do Scene7{#scene-cookies}

O Scene7 usa cookies para armazenar informações úteis que podem ser usadas para fornecer mídia dinâmica ao navegador.

O Scene7 armazena informações localmente para alguns visualizadores mais antigos baseados em AS2 Flash.

Em visualizadores AS2, os cookies:

* Rastreie o estado da sessão de um usuário, como a página atual e a imagem exibida, o nível de zoom atual e assim por diante.
* Determinam quanto tempo passou desde a sessão anterior do usuário. O visualizador usa essas informações para decidir se deseja continuar uma sessão anterior ou iniciar uma nova. Essas informações também são enviadas para os servidores do Scene7, mas não são usadas.

No visualizador AS2 Flash eCatalog, os cookies:

* Armazenam conteúdo gerado pelo usuário (principalmente o conteúdo inserido pelo usuário no recurso &quot;notas adesivas&quot; do visualizador de catálogo eletrônico). Esse conteúdo é restaurado quando o usuário retoma uma sessão.
* Quando o usuário cria um email para compartilhar o catálogo eletrônico com outro usuário, o conteúdo das notas adesivas do segundo marcador do visualizador AS2 é copiado para os servidores Adobe iniciantes para fornecê-lo ao destinatário. Quando o destinatário inicia a sessão do visualizador, o conteúdo das notas adesivas é recuperado do servidor e copiado em um cookie. Esse recurso é pouco utilizado, portanto, não expira e o conteúdo obsoleto não é removido. Atualmente, ela persiste nos servidores indefinidamente.

Os visualizadores AS3 mais recentes não implementam a persistência de sessão.

**Nome do cookie: VatLogin.jsp**

| Atributo | Descrição |
|---|---|
| Informações armazenadas | Define o cookie da sessão. O AuthFilter incorporado ao IPS ImageServer (IS, IR e também aos SWFs/capas e contextos de vídeo) usa o cookie para autorização de acesso. Se presente, permite que solicitações HTTP sejam transmitidas. Caso contrário, retorna não autorizado. |
| Expiração | Esse cookie é um cookie de sessão. A expiração da sessão atual está definida como 45 minutos no IPS [!DNL web.xml] do Scene7. |

**Nome do cookie: s7js.flyout.InfoMessage.displayed `assetId`.state**

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

Os cookies do navegador são usados por visualizadores DHTML herdados para armazenar informações de estado e dados de notas adesivas. Eles também são usados pelo menu DHTML multitela para tornar o indicador de mensagem específico da sessão.

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
   <td colname="col2"> <p> </p> <p> &lt;assetId&gt; é o nome do ativo com o qual o visualizador está trabalhando e &lt;id&gt; é o índice de nota adesiva com base em 0. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Expiração </td> 
   <td colname="col2"> Este cookie é um cookie de sessão e expira quando o navegador é fechado. </td> 
  </tr> 
 </tbody> 
</table>
