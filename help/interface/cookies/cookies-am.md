---
description: O Audience Manager depende de alguns cookies simples para realizar diferentes funções.  Estes incluem coisas como a atribuição de Ids, a gravação de chamadas de dados, o rastreamento de erros e os testes para ver se os cookies podem ser definidos. Esta seção lista e descreve os diferentes cookies definidos pelo Audience Manager.
keywords: cookies
seo-description: O Audience Manager depende de alguns cookies simples para realizar diferentes funções.  Estes incluem coisas como a atribuição de Ids, a gravação de chamadas de dados, o rastreamento de erros e os testes para ver se os cookies podem ser definidos.  Esta seção lista e descreve os diferentes cookies definidos pelo Audience Manager.
seo-title: Cookies do Audience Manager
solution: Experience Cloud,Audience Manager
title: Cookies do Audience Manager
uuid: 8b384c38-b85a-4e93-b00e-41a9d3ae2b21
translation-type: tm+mt
source-git-commit: 012283d79bda42f9dabb20b25903927b075f6d54

---


# Cookies do Audience Manager{#audience-manager-cookies}

O Audience Manager depende de alguns cookies simples para realizar diferentes funções.  Estes incluem coisas como a atribuição de Ids, a gravação de chamadas de dados, o rastreamento de erros e os testes para ver se os cookies podem ser definidos.  Esta seção lista e descreve os diferentes cookies definidos pelo Audience Manager.

**Cookie demdex**

<table id="table_1CCF7EA2BC9E421F8DEECA5F611E33F6"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Atributo </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <b>Propósito</b> </p> </td> 
   <td colname="col2"> <p> O <span class="keyword">Audience Manager</span> define este cookie para atribuir uma ID exclusiva a um visitante do site. O cookie <span class="wintitle">demdex</span> ajuda o <span class="keyword">Audience Manager</span> a executar funções básicas, como a identificação do visitante, a sincronização de ID, a segmentação, a modelagem, a geração de relatórios, etc. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Conteúdo</b> </p> </td> 
   <td colname="col2"> <p>O cookie <span class="wintitle">demdex</span> contém uma ID de usuário exclusiva (UUID), conforme mostrado no exemplo abaixo: </p> <p> <span class="codeph"> 06151304227769720433039235178204449977 </span> </p> <p>Consulte também <a href="https://marketing.adobe.com/resources/help/en_US/aam/ids-in-aam.html" format="https" scope="external">Índice de IDs no Audience Manager </a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Outros atributos</b> </p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_11291DA87C5045E880034E06C863BCDA"> 
      <li id="li_40C30A06A12449A4A8748621223CA71B">Duração: o cookie <span class="wintitle">demdex</span> tem um intervalo TTL (time-to-live) de 180 dias. O TTL é redefinido para 180 dias com cada interação do usuário com o site de um parceiro. O cookie expira se um usuário não voltar ao seu site dentro do intervalo TTL. </li> 
      <li id="li_A589EDA2198249829207A183872EF1FF">Rejeitar: o <span class="keyword">Audience Manager</span> redefine o cookie com uma string <span class="codeph">Não direcionar</span> se um usuário optar por rejeitar a coleta de dados. Nesse caso, o TTL do cookie é definido como 10 anos. </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Cookie dextp**

<table id="table_7343C9C9ADD24D3FA693ECC76E4A4045"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Atributo </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <b>Propósito</b> </p> </td> 
   <td colname="col2"> <p> O <span class="keyword">Audience Manager</span> define este cookie para registrar a última vez que fez uma chamada de sincronização de dados. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Conteúdo</b> </p> </td> 
   <td colname="col2"> <p>O cookie <span class="wintitle">dextp</span> contém o nome ou ID de um provedor de dados e um carimbo de data e hora UNIX UTC formatados como strings delimitadas por barra. Nos exemplos, <i>itálico</i> representa um espaço reservado para variável. </p> <p> 
     <ul id="ul_80D0BC3FCF06470991E12712401D784A"> 
      <li id="li_03747A433CEB4756A26CD866E716B89D">Old style: <span class="codeph"> <span class="varname"> data provider name here </span>-1490307822097| <span class="varname"> data provider name here </span>-1490307822038 </span> </li> 
      <li id="li_79E7000E82DB4ADA9E9887B017343B2D">Novo estilo: <span class="codeph">21-1-1490307821616|544-1-1490307821793|3-1-1490307821852|420-1-1490307822038| </span> </li> 
     </ul> </p> <p>Consulte também a seção de sintaxe dos dados abaixo. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Outros atributos</b> </p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_4922AC2CD55D4C888A6FBEB22F8B889B"> 
      <li id="li_91A68C44E53840379C2ACDED25468735">Duração: o cookie <span class="wintitle">dextp</span> tem um intervalo TTL (time-to-live) de 180 dias. </li> 
      <li id="li_6B8C674EFAAC4DABA0A640CF29247F99">Rejeitar: o <span class="keyword">Audience Manager</span> redefine o cookie com uma string <span class="codeph">Não direcionar</span> se um usuário optar por rejeitar a coleta de dados. Nesse caso, o TTL do cookie é definido como 10 anos. </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

Sintaxe de dados do cookie dextp:

A tabela a seguir lista e define os elementos de um cookie [!DNL dextp] por localização na string de dados.

<table id="table_BE00604B97F24F5A94AA4F566063D785"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Posição variável </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <b>Primeiro ou segundo</b> </p> </td> 
   <td colname="col2"> <p>A posição do nome ou ID do provedor de dados varia dependendo se o cookie usa o estilo de formatação novo ou antigo. </p> <p> <b>Estilo antigo de formatação:</b> </p> <p> 
     <ul id="ul_5BFBF40E3FE849CA859030F2D070FDF6"> 
      <li id="li_E8F4DC0CB15B472ABE9892B3A61D7F77">Syntax: <span class="codeph"> <span class="varname"> data provider name </span> - <span class="varname"> UNIX UTC timestamp </span> </span> </li> 
      <li id="li_7CD8B101156140F49EA97B18E9591402">Exemplo: <span class="codeph"> dataProvider1 - 1490307822038 </span> </li> 
     </ul> </p> <p>O cookie de estilo antigo identifica o provedor de dados com um nome legível. </p> <p> <b>Novo estilo de formatação:</b> </p> <p> 
     <ul id="ul_AC6225CA781746148C125F21DFED1ED9"> 
      <li id="li_29C4B52E398B4EA28944980A15B05A57">Sintaxe: <span class="codeph"> <span class="varname"> ID do provedor de dados </span> - 1 2 - <span class="varname"> Carimbo de data e hora UNIX UTC </span> </span> </li> 
      <li id="li_3BF30CA5FED242DF96E0B54AFC64B06F">Exemplo: <span class="codeph"> 123345 - 1 - 1490307822038 </span> </li> 
     </ul> </p> <p>O novo cookie de estilo: </p> <p> 
     <ul id="ul_F05A91A455FA44C7A71186C0C9E31630"> 
      <li id="li_A8C9638173684359BABC4207845A4F48">Substitui o nome do provedor de dados legível por uma ID numérica. </li> 
      <li id="li_28F1E2DB24904E53BE9718AD788CE61E">Identifica o tipo de chamada com ID 1 ou ID 2. A ID 1 representa uma chamada de sincronização de ID. A ID 2 representa uma chamada obsoleta que não é mais usada. Você não deve ver muitos (caso veja algum) cookies dextp com ID 2. </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Última</b> </p> </td> 
   <td colname="col2"> <p>A última posição contém um carimbo de data e hora UNIX UTC. </p> </td> 
  </tr> 
 </tbody> 
</table>

**dst Cookie**

<table id="table_83AE9B6350C6408BAECD9FCF33022B98"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Atributo </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <b>Propósito</b> </p> </td> 
   <td colname="col2"> <p> O <span class="keyword">Audience Manager</span> define este cookie quando ocorre um erro ao enviar dados para um <a href="https://marketing.adobe.com/resources/help/en_US/aam/c_destinations.html" format="https" scope="external">destino </a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Conteúdo</b> </p> </td> 
   <td colname="col2"> <p> O cookie <span class="wintitle">DST</span> contém conjuntos de IDs de destino e carimbos de data e hora UNIX formatados como strings delimitadas por barra. Nos exemplos, <i>itálico</i> representa um espaço reservado para variável. </p> <p> 
     <ul id="ul_CE98076A02DA413486C1D341E9806889"> 
      <li id="li_850209D956644749B98C7A208C825C15">Sintaxe: <span class="codeph"> <span class="varname"> ID de destino </span> - <span class="varname"> Carimbo de data e hora UNIX UTC </span> </span> </li> 
      <li id="li_4A22152C70844733982230EBF7B9EB78">Exemplo: <span class="codeph">067797-1490349684|1010788-1490349692|1067797-1490349692 </span> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Outros atributos</b> </p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_5D13DD701B484B51BF2808A69A919106"> 
      <li id="li_4E665114C63246FBA32A4E19984D2693">Duração: o cookie <span class="wintitle">dst</span> tem um intervalo TTL (time-to-live) de 180 dias. </li> 
      <li id="li_A682B566704F43D2AB72487EFF212474">Rejeitar: o <span class="keyword">Audience Manager</span> redefine o cookie com uma string <span class="codeph">Não direcionar</span> se um usuário optar por rejeitar a coleta de dados. </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Cookie _dp**

Este é um cookie temporário. O [!DNL Audience Manager] tenta definir o cookie [!DNL _dp] para determinar se ele pode definir outros cookies no domínio demdex.net em um contexto de terceiros. Quando [!DNL _dp] é definido, ele contém um valor igual a 1. O [!DNL Audience Manager] lê este valor e remove imediatamente o cookie. Se o cookie [!DNL _dp] não estiver presente, o [!DNL Audience Manager] sabe que não pode definir cookies.