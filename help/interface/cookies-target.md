---
description: Saiba como o Adobe Target usa cookies para fornecer aos operadores de site a capacidade de testar quais conteúdos e ofertas online são mais relevantes para os visitantes.
solution: Experience Cloud,Analytics,Target,Social
title: Cookies do Adobe Target
uuid: 44f7e32e-8d99-4682-8b54-8364d001b403
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: c4399cc0-8333-47b8-b830-2ba7359f464a
source-git-commit: 65e4b6739568ea06b86744e891d30c3917f02bcc
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 92%

---

# Cookies do Adobe Target {#target-cookies}

O Adobe Target usa cookies para fornecer aos operadores de site a capacidade de testar quais conteúdos e ofertas online são mais relevantes para os visitantes.

É possível alterar essas configurações, se necessário, exceto pela duração do cookie. Consulte seu representante de conta ao alterar as configurações de cookie.

>[!NOTE]
>
>Os usuários do Adobe Target também podem criar cookies de terceiros personalizados.

| Configuração | Informações |
| --- | --- |
| Nome do cookie | mbox. |
| Domínio do cookie | Domínio de primeiro e segundo nível a partir de onde a mbox será disponibilizada. O cookie é sempre um cookie próprio porque é disponibilizado pelo domínio de sua companhia. Exemplo: `mycompany.com`. |
| Domínio do servidor | `clientcode.tt.omtrdc.net`, utilizando o código de cliente de sua [!DNL Adobe Target] conta. |
| Duração do cookie | O cookie permanece no navegador do visitante por dois anos a contar de seu último logon. Não é possível alterar a duração do cookie. |

{style=&quot;table-layout:auto&quot;}

>[!NOTE]
>
>Se qualquer um dos nomes de domínio incluir um código de país, como `mycompany.co.uk`, trabalhe com os Serviços ao cliente para configurar o seu `at.js` para ter suporte a este código.

O cookie mantém alguns valores para gerenciar a experiência dos visitantes nas campanhas do Adobe Target:

| Valor | Definição |
| --- | --- |
| session ID | Um identificador exclusivo para uma sessão de usuário. Por padrão, a sessão expira após 30 minutos de inatividade. Se estiver gerando um sessionId (por exemplo, para implementações no lado do servidor), verifique o seguinte:<ul><li>A ID de sessão pode ser qualquer string imprimível, exceto um espaço, um ponto de interrogação ( ?  ) ou uma barra ( / ).</li><li>A ID da sessão deve ter entre 1 e 128 caracteres.</li><li>Para uma sessão específica, o valor deve permanecer o mesmo em diferentes solicitações</li><li>Você nunca deve ter sessões paralelas (sessionIds distintas) para determinado visitante em qualquer momento.</li></ul>O roteamento para um nó específico no cluster de borda é feito usando a ID de sessão.<ul><li>A sessão fica ativa por 30 minutos no lado do servidor. Portanto, você não deve usar uma ID de sessão diferente para um determinado `tntId/thirdPartyId` no prazo de 30 minutos a contar da última solicitação feita com o `tntId/thirdPartyId`. Caso contrário, as alterações no perfil podem ser inconsistentes e imprevisíveis.</li><li>Uma nova ID de sessão deve ser usada após trinta minutos de inatividade de um visitante.</li><li>Usar a mesma ID de sessão com vários `tntIds/thirdPartyIds` pode causar alterações imprevisíveis nos perfis identificados pelo `tntId/thirdPartyIDs`.</li></ul>**Observação**: consulte [Limite de número de solicitações simultâneas](https://experienceleague.adobe.com/docs/target/using/troubleshoot/target-limits.html?lang=pt-BR#content-delivery) para uma ID de sessão específica. |
| pc ID | Um ID temporário para o navegador do visitante. Prolonga até que os cookies sejam excluídos manualmente. |
| check | Um valor de teste simples usado para determinar se um visitante suporta cookies. Defina toda vez que um visitante solicitar uma página. |
| disable | Definido se o tempo de carregamento do visitante exceder o tempo limite configurado no arquivo at.js. A duração padrão é de uma hora. |

{style=&quot;table-layout:auto&quot;}
