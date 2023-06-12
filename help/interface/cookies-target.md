---
description: Saiba como o Adobe Target usa cookies para fornecer aos operadores de site a capacidade de testar quais conteúdos e ofertas online são mais relevantes para os visitantes.
solution: Experience Cloud,Analytics,Target
title: Cookies do Adobe Target
uuid: 44f7e32e-8d99-4682-8b54-8364d001b403
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: c4399cc0-8333-47b8-b830-2ba7359f464a
source-git-commit: a1d24f95b1ac567686d58af8adf0132e5beb8f2a
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 23%

---

# Cookies do Adobe Target

[!DNL Adobe Target]O usa cookies para fornecer aos operadores de site a capacidade de testar quais conteúdos e ofertas online são mais relevantes para os visitantes.

>[!NOTE]
>
>As informações deste artigo se aplicam à [[!DNL Target] Biblioteca JavaScript at.js](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html?lang=pt-BR){target=_blank} somente.
>
>Para obter informações sobre cookies usados em uma [!DNL Target] implementação usando o [[!DNL Adobe Experience Platform Web SDK]](https://experienceleague.adobe.com/docs/experience-platform/edge/home.html?lang=pt-BR){target=_blank}, see "Does the [!DNL Adobe Experience Platform Web SDK] use cookies? If so, what cookies does it use?" in [Frequently Asked questions in the DNL Platform Web SDK overview guide](https://experienceleague.adobe.com/docs/experience-platform/edge/web-sdk-faq.html){target=_blank}.
>
>Você pode alterar as configurações discutidas neste artigo, se necessário, exceto pela duração do cookie. [Consulte seu representante de conta ao alterar as configurações de cookie.](https://experienceleague.adobe.com/docs/target/using/cmp-resources-and-contact-information.html){target=_blank}
>
>[!DNL Target]Os usuários do também podem criar cookies de terceiros personalizados.

## Cookies próprios

Os seguintes cookies primários são armazenados no domínio do cliente:

| Cookie | Detalhes |
| --- | --- |
| mbox | Armazena identificadores anônimos sobre o visitante.<P>**Domínio do cookie**: o domínio do qual você fornece a mbox. Como esse cookie é disponibilizado pelo domínio de sua empresa, o cookie é um cookie próprio. Exemplo: `mycompany.com`. Se qualquer um dos nomes de domínio incluir um código de país, como `mycompany.co.uk`, trabalhe com os Serviços ao cliente para configurar o at.js para ter suporte a esse código. Para obter informações sobre como personalizar o domínio do cookie, se necessário, consulte &quot;`cookieDomain`&quot; em [targetGlobalSettings](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html?lang=pt-BR){target=_blank} no *[!DNL Adobe Target]Guia do desenvolvedor*.<P>**Domínio do servidor**: `clientcode.tt.omtrdc.net`, utilizando o código de cliente do [!DNL Target] conta.<P>**Duração do cookie**: o cookie permanece no navegador do visitante por dois anos a partir do último logon. Não é possível alterar a duração do cookie.<P>O cookie mantém alguns valores para gerenciar a experiência dos visitantes [!DNL Target] atividades:<P>**session ID**: um identificador exclusivo para uma determinada sessão de usuário. Por padrão, a sessão expira após 30 minutos de inatividade. Se você estiver gerando `sessionId` você mesmo (por exemplo, para [implementações do lado do servidor](https://experienceleague.adobe.com/docs/target-dev/developer/server-side/server-side-overview.html){target=_blank}), verifique o seguinte:<ul><li>A ID da sessão pode ser qualquer string imprimível, exceto um espaço, um ponto de interrogação ( ? ) ou uma barra ( / ).</li><li>A ID da sessão deve ter entre 1 e 128 caracteres.</li><li>Para uma sessão específica, o valor do cookie deve permanecer o mesmo em várias solicitações.</li><li>Você nunca deve ter sessões paralelas (distintas `sessionIds`) para um determinado visitante em qualquer momento.</li></ul>O roteamento para um nó específico no cluster de borda é feito usando a ID da sessão.<ul><li>A sessão fica ativa por 30 minutos no lado do servidor. Portanto, você não deve usar uma ID de sessão diferente para um `tntId/thirdPartyId` no prazo de 30 minutos a contar da última solicitação `tntId/thirdPartyId`. Caso contrário, as alterações no perfil podem ser inconsistentes e imprevisíveis.</li><li>Uma nova ID de sessão deve ser usada após trinta minutos de inatividade de um visitante.</li><li>Usar a mesma ID de sessão com vários `tntIds/thirdPartyIds` pode causar alterações imprevisíveis nos perfis identificados pelo `tntId/thirdPartyIDs`.</li></ul>OBSERVAÇÃO: consulte [limite de número de solicitações simultâneas](https://experienceleague.adobe.com/docs/target/using/troubleshoot/target-limits.html?lang=pt-BR#content-delivery){target=_blank} para uma ID de sessão específica.<P>**pc ID**: uma ID semipermanente para o navegador de um visitante. Prolonga até que os cookies sejam excluídos manualmente.<P>**check**: um valor de teste simples usado para determinar se um visitante suporta cookies. Defina toda vez que um visitante solicitar uma página.<P>**disable**: definido se o tempo de carregamento de um visitante exceder o tempo limite configurado no arquivo at.js. Por padrão, esse tempo limite dura uma hora. |
| at_check | Cookie temporário para verificar se o recurso de leitura/gravação de cookie está ativado no navegador. |
| mboxEdgeCluster | Estes cookies só estão presentes quando/se [configuração overrideMboxEdgeServer](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html?lang=pt-BR){target=_blank} está definida como `true`. |

Não é possível usar HTTPOnly nesses cookies primários. A biblioteca JavaScript at.js do precisa ler/gravar nesses cookies. Esses cookies são criados pela at.js e não são definidos no servidor.

A variável `secure` a configuração pode ser ativada em todos esses cookies usando o `secureOnly: true` na implementação da at.js.

## Cookies de terceiros

Os seguintes cookies de terceiros são armazenados em `tt.omtrdc.net`:

| Cookie | Detalhes |
| --- | --- |
| customerclientcode!mboxPC | Este cookie estará presente se o domínio cruzado estiver ativado. |
| customerclientcode!mboxSession | Este cookie estará presente se o domínio cruzado estiver ativado. |

Esses cookies de terceiros estão prontos para uso imediato e são definidos pelo [!DNL Target] servidores de borda.

A variável `secure` pode ser ativada em todos os cookies usando a variável `secureOnly: true` na implementação da at.js.