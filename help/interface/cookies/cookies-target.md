---
description: O Target usa cookies para fornecer aos operadores de site a capacidade de testar quais conteúdos e ofertas online são mais relevantes para os visitantes.
keywords: cookies; privacidade
seo-description: O Target usa cookies para fornecer aos operadores de site a capacidade de testar quais conteúdos e ofertas online são mais relevantes para os visitantes.
seo-title: Cookies do Target
solution: Experience Cloud,Analytics,Target,Social
title: Cookies do Target
uuid: 44f7e32e-8d99-4682-8b54-8364d001b403
index: y
internal: n
snippet: y
translation-type: tm+mt
source-git-commit: 426c1fecf16e1cf83cd28971e4de6fdb66b0e10d

---


# Cookies do Target{#target-cookies}

O Target usa cookies para fornecer aos operadores de site a capacidade de testar quais conteúdos e ofertas online são mais relevantes para os visitantes.

Você pode alterar essas configurações, se necessário, exceto a duração do cookie. Entre em contato com seu representante de contas ao modificar as configurações de cookie.

>[!NOTE]
>
>Os usuários do Target também podem criar cookies de terceiros personalizados.

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
   <td colname="col2"> <p> <span class="filepath"> clientcode.tt.omtrdc.net</span>, utilizando o código de cliente da sua conta Target. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Duração do cookie </p> </td> 
   <td colname="col2"> <p>O cookie permanece no navegador do visitante por dois anos a partir do último logon. Não é possível alterar a duração do cookie. </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Se qualquer um dos nomes de domínio incluir um código de país, como [!DNL mycompany.co.uk], trabalhe com os Serviços ao Cliente para configurar o [!DNL mbox.js] e suportar isto.

O cookie mantém um número de valores para gerenciar a experiência de seus visitantes nas campanhas do Target:

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
   <td colname="col2"> <p>ID único para a sessão do usuário. A duração padrão é de 30 minutos. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> pc ID</span> </p> </td> 
   <td colname="col2"> <p>Um ID temporário para o navegador do visitante. Dura até o cookie ser removido manualmente. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> check</span> </p> </td> 
   <td colname="col2"> <p>Um simples valor de teste utilizado para determinar se o navegador do visitante tem suporte a cookies. Definido sempre que o usuário solicita uma página. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> disable</span> </p> </td> 
   <td colname="col2"> <p>Configurado se o tempo de carga do visitante ultrapassar o tempo limite configurado no arquivo <span class="filepath">mbox.js</span>. A duração padrão é de uma hora. </p> </td> 
  </tr> 
 </tbody> 
</table>

