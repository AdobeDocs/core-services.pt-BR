---
description: O Target usa cookies para fornecer aos operadores de site a capacidade de testar quais conteúdos e ofertas online são mais relevantes para os visitantes.
keywords: cookies;privacy
seo-description: O Target usa cookies para fornecer aos operadores de site a capacidade de testar quais conteúdos e ofertas online são mais relevantes para os visitantes.
seo-title: Cookies do Target
solution: Experience Cloud,Analytics,Target,Social
title: Cookies do Target
uuid: 44f7e32e-8d99-4682-8b54-8364d001b403
translation-type: ht
source-git-commit: 11ce83401a12c25853cd6412413b8abf98dd6612
workflow-type: ht
source-wordcount: '285'
ht-degree: 100%

---


# Cookies do Adobe Target {#target-cookies}

O Adobe Target usa cookies para fornecer aos operadores de site a capacidade de testar quais conteúdos e ofertas online são mais relevantes para os visitantes.

Altere essas configurações, se necessário, com exceção da duração do cookie. Consulte seu representante de conta ao alterar as configurações de cookie.

>[!NOTE]
>
>Os usuários do Adobe Target também podem criar cookies de terceiros personalizados.

<table id="table_54B402C6E19C4A70B1E27BC9DFF776EB"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Configuração </th> 
   <th colname="col2" class="entry"> Informações </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Nome do cookie </p> </td> 
   <td colname="col2"> <p>mbox. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Domínio do cookie </p> </td> 
   <td colname="col2"> <p>Domínio de primeiro e segundo nível a partir de onde a mbox será disponibilizada. O cookie é sempre um cookie próprio porque é disponibilizado pelo domínio de sua companhia. Por exemplo: <span class="filepath">mycompany.com</span>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Domínio do servidor </p> </td> 
   <td colname="col2"> <p> <span class="filepath"> clientcode.tt.omtrdc.net</span>, utilizando o código de cliente da sua conta do Adobe Target. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Duração do cookie </p> </td> 
   <td colname="col2"> <p>O cookie permanece no navegador do visitante por dois anos após o último logon. Não é possível alterar a duração do cookie. </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Se qualquer um dos nomes de domínio incluir um código de país, como [!DNL mycompany.co.uk], trabalhe com os Serviços ao Cliente para configurar o [!DNL mbox.js] e suportar isto.

O cookie mantém vários valores para gerenciar a experiência dos visitantes nas campanhas do Adobe Target:

<table id="table_5245F72A2D5A4322B40ABB10B7DFB338"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Valor </th> 
   <th colname="col2" class="entry"> Definição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> session ID</span> </p> </td> 
   <td colname="col2"> <p>Uma ID exclusiva para uma sessão de usuário. Por padrão, leva 30 minutos. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> pc ID</span> </p> </td> 
   <td colname="col2"> <p>Um ID temporário para o navegador do visitante. Prolonga até que os cookies sejam excluídos manualmente. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> check</span> </p> </td> 
   <td colname="col2"> <p>Um valor de teste simples usado para determinar se um visitante suporta cookies. Defina toda vez que um visitante solicitar uma página. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> disable</span> </p> </td> 
   <td colname="col2"> <p>Configurado se o tempo de carga do visitante ultrapassar o tempo limite configurado no arquivo <span class="filepath">mbox.js</span>. A duração padrão é de uma hora. </p> </td> 
  </tr> 
 </tbody> 
</table>

