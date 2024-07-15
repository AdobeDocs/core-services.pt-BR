---
description: Saiba como o serviço de ID é armazenado e usado nos aplicativos do Experience Cloud.
solution: Experience Cloud,Analytics,Target
title: Cookies da Experience Cloud
uuid: a4788c1c-0402-4fc8-b894-cd24fa794f4f
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: bd9bea58-9987-40d6-84e0-da185388bbbb
source-git-commit: c39672f0d8a0fd353b275b2ecd095ada1e2bf744
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 91%

---

# Cookies da Experience Cloud 

O Adobe Experience Cloud usa cookies para armazenar uma ID de visitante usada em aplicativos Experience Cloud. Esses cookies se aplicam especificamente ao acesso aos aplicativos do Adobe Experience Cloud em [experience.adobe.com](https://experience.adobe.com).

**Nome do cookie: s_ecid**

<table id="table_FF4C70D3D4CC425BA65162D5A9504F7D"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> <p>Atributo </p> </th> 
   <th colname="col2" class="entry"> <p>Descrição </p> </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Informações armazenadas </p> </td> 
   <td colname="col2"> <p> Contém uma cópia da Experience Cloud ID (ECID) ou MID. A MID é armazenada em um par de valor principal que segue a sintaxe s_ecid=MCMID|&lt;ECID&gt; </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Expiração </p> </td> 
   <td colname="col2"> <p>2 anos </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Uso </p> </td> 
   <td colname="col2"> <p>Esse cookie é definido pelo domínio do cliente depois que o cookie AMCV é definido pelo cliente. A finalidade desse cookie é permitir o rastreamento de ID persistente no estado próprio e ele é usado como ID de referência, se o cookie AMCV tiver expirado. Verifique o cookie AMCV aqui para obter mais detalhes. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Localização </p> </td> 
   <td colname="col2"> <p>Somente para clientes CNAME. Não aplicável para cenários de terceiros. O cookie é armazenado em seu domínio, o mesmo domínio usado pelo CNAME e pela solicitação de imagem do Analytics </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Tamanho </p> </td> 
   <td colname="col2"> <p>45 bytes </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> SameSite=Lax </p> </td> 
   <td colname="col2"> <p>Os cookies com essa configuração só são enviados quando o domínio exibido no URL do navegador corresponde ao domínio do cookie. Este é o novo padrão para cookies no Chrome.</p> </td> 
  </tr> 
 </tbody> 
</table>

**Nome do cookie: AMCV_###@AdobeOrg**

O [Serviço de ID da Experience Platform](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=pt-BR) usa o JavaScript para armazenar um identificador de visitante único em um cookie `AMCV_###@AdobeOrg` no domínio do site atual, onde `###` representa uma string aleatória de caracteres, como `AMCV_1FD6776A524453CC0A490D44%40AdobeOrg.`

Consulte [Cookies e o serviço da ID](https://experienceleague.adobe.com/docs/id-service/using/intro/cookies.html).

<table id="table_1883C0836C1E4AF5A262FBF5000C1B11"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> <p>Atributo </p> </th> 
   <th colname="col2" class="entry"> <p>Descrição </p> </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Informações armazenadas </p> </td> 
   <td colname="col2"> <p> Identificadores de visitante único usados pelas Soluções da Experience Cloud. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Expiração </p> </td> 
   <td colname="col2"> <p> 2 anos </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Uso </p> </td> 
   <td colname="col2"> <p> Este cookie é usado para identificar um visitante único. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Localização </p> </td> 
   <td colname="col2"> <p> Este cookie é armazenado no domínio do site (não no domínio da solicitação de imagem). </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Tamanho </p> </td> 
   <td colname="col2"> <p> Varia, a maioria dos clientes pode esperar que esse cookie tenha cerca de 200 bytes de comprimento. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Nenhum valor adicionado. O padrão do Chrome é o Lax. </p> </td> 
   <td colname="col2"> <p> Os cookies com essa configuração só são enviados quando o domínio exibido no URL do navegador corresponde ao domínio do cookie. Este é o novo padrão para cookies no Chrome. </p> </td> 
  </tr> 
 </tbody> 
</table>
