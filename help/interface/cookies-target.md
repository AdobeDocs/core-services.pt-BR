---
description: Saiba como o [!DNL Adobe Target] usa cookies para fornecer aos operadores de site a capacidade de testar quais conteúdos e ofertas online são mais relevantes para os visitantes.
solution: Experience Cloud,Analytics,Target
title: Cookies do Adobe Target
uuid: 44f7e32e-8d99-4682-8b54-8364d001b403
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: c4399cc0-8333-47b8-b830-2ba7359f464a
source-git-commit: 3ca021a0a2e6b0b6e265d35084d89d7720c28908
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 8%

---

# Cookies do Adobe Target

O [!DNL Adobe Target] usa cookies para fornecer aos operadores de site a capacidade de testar quais conteúdos e ofertas online são mais relevantes para os visitantes.

>[!NOTE]
>
>As informações deste artigo se aplicam somente à [[!DNL Target] biblioteca at.js de JavaScript](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html){target=_blank}.
>
>Para obter informações sobre cookies usados em uma implementação do [!DNL Target] usando o [[!DNL Adobe Experience Platform Web SDK]](https://experienceleague.adobe.com/docs/experience-platform/edge/home.html){target=_blank}, consulte &quot;O [!DNL Adobe Experience Platform Web SDK] usa cookies? Em caso afirmativo, quais cookies ele usa?&quot; em [Perguntas frequentes no guia de visão geral do DNL Platform Web SDK](https://experienceleague.adobe.com/docs/experience-platform/edge/web-sdk-faq.html){target=_blank}.
>
>Você pode alterar as configurações discutidas neste artigo, se necessário, exceto pela duração do cookie. [Consulte seu representante de conta](https://experienceleague.adobe.com/docs/target/using/cmp-resources-and-contact-information.html){target=_blank} ao alterar as configurações de cookie.
>
>[!DNL Target] usuários também podem criar cookies de terceiros personalizados.

## Cookies próprios

Os seguintes cookies primários são armazenados no domínio do cliente:

| Cookie | Detalhes |
| --- | --- |
| mbox | Armazena identificadores anônimos sobre o visitante.<P>**Domínio de cookie**: o domínio do qual você fornece a mbox. Como esse cookie é disponibilizado pelo domínio de sua empresa, o cookie é um cookie próprio. Exemplo: `mycompany.com`. Se qualquer um dos nomes de domínio incluir um código de país, como `mycompany.co.uk`, trabalhe com os Serviços ao Cliente para configurar a at.js para ter suporte a esse código. Para obter informações sobre como personalizar o domínio do cookie, se necessário, consulte &quot;`cookieDomain`&quot; em [targetGlobalSettings](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html){target=_blank} no *[!DNL Adobe Target]Guia do Desenvolvedor*.<P>**Domínio do servidor**: `clientcode.tt.omtrdc.net`, usando o código de cliente da sua conta do [!DNL Target].<P>**Duração do cookie**: o cookie permanece no navegador do visitante por dois anos a partir do último logon. Não é possível alterar a duração do cookie.<P>O cookie mantém alguns valores para gerenciar a experiência dos visitantes nas atividades de [!DNL Target]:<P>**identificação de sessão**: um identificador exclusivo para uma determinada sessão de usuário. Por padrão, a sessão expira após 30 minutos de inatividade. Se estiver gerando `sessionId` você mesmo (por exemplo, para [implementações do lado do servidor](https://experienceleague.adobe.com/docs/target-dev/developer/server-side/server-side-overview.html){target=_blank}), verifique o seguinte:<ul><li>A ID da sessão pode ser qualquer string imprimível, exceto um espaço, um ponto de interrogação ( ? ), chaves ( { } ) ou uma barra ( / ).</li><li>A ID da sessão deve ter entre 1 e 128 caracteres.</li><li>Para uma sessão específica, o valor do cookie deve permanecer o mesmo em várias solicitações.</li><li>Você nunca deve ter sessões paralelas (`sessionIds` distintas) para um determinado visitante em nenhum momento.</li></ul>O roteamento para um nó específico no cluster de borda é feito usando a ID da sessão.<ul><li>A sessão fica ativa por 30 minutos no lado do servidor. Portanto, você não deve usar uma ID de sessão diferente para um `tntId/thirdPartyId` específico dentro de 30 minutos após a última solicitação feita com o `tntId/thirdPartyId`. Caso contrário, as alterações no perfil podem ser inconsistentes e imprevisíveis.</li><li>Uma nova ID de sessão deve ser usada após trinta minutos de inatividade de um visitante.</li><li>Usar a mesma ID de sessão com vários `tntIds/thirdPartyIds` pode causar alterações imprevisíveis nos perfis identificados pelo `tntId/thirdPartyIDs`.</li></ul>OBSERVAÇÃO: consulte [limite de número de solicitações simultâneas](https://experienceleague.adobe.com/docs/target/using/troubleshoot/target-limits.html?lang=pt-BR#content-delivery){target=_blank} para uma ID de sessão específica.<P>**pc ID**: uma ID semipermanente para o navegador de um visitante. Prolonga até que os cookies sejam excluídos manualmente.<P>**verificação**: um valor de teste simples usado para determinar se um visitante suporta cookies. Defina toda vez que um visitante solicitar uma página.<P>**disable**: definido se o tempo de carregamento de um visitante exceder o tempo limite configurado no arquivo at.js. Por padrão, esse tempo limite dura uma hora. |
| at_check | Cookie temporário para verificar se o recurso de leitura/gravação de cookie está ativado no navegador. |
| mboxEdgeCluster | Estes cookies só estão presentes quando/se a configuração [overrideMboxEdgeServer](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html){target=_blank} estiver definida como `true`. |

Não é possível usar HTTPOnly nesses cookies primários. A biblioteca JavaScript at.js do precisa ler/gravar nesses cookies. Esses cookies são criados pela at.js e não são definidos no servidor.

A configuração `secure` pode ser ativada em todos esses cookies usando a configuração `secureOnly: true` na implementação da at.js.

## Cookies de terceiros

Os seguintes cookies de terceiros são armazenados em `tt.omtrdc.net`:

| Cookie | Detalhes |
| --- | --- |
| customerclientcode!mboxPC | Este cookie estará presente se o domínio cruzado estiver ativado. |
| customerclientcode!mboxSession | Este cookie estará presente se o domínio cruzado estiver ativado. |

Esses cookies de terceiros são HTTPOnly prontos para uso e são definidos pelos servidores de borda [!DNL Target].

A configuração `secure` pode ser ativada em todos os cookies usando a configuração `secureOnly: true` na implementação da at.js.