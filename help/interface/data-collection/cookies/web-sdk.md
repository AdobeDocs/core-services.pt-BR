---
title: Cookies do Adobe Experience Platform Web SDK
description: Saiba como o Web SDK usa cookies aplicáveis à sua implementação.
solution: Experience Cloud
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 14f06dc9-255e-4a6c-adec-471107cf202e
TQID: 'https://experienceleague.adobe.com/jysQ5m7o0cI3ECKz2RWZB4Kt3own7XAPm04pr4yLh-k'
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
    internal-label: CX Enterprise
feature_v2:
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
    internal-label: Administration
subfeature_v2:
  - id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
    internal-label: Support
  - id: fef08361-6ac5-460c-93fe-d063e40b6a49
    internal-label: Getting started
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 7b12d5debfccd62ab7b416e9a6fe278d251a4ca5
workflow-type: tm+mt
source-wordcount: '984'
ht-degree: 0%
---
# Cookies do Adobe Experience Platform Web SDK

O Adobe Experience Platform Web SDK usa cookies para armazenar valores específicos para sua implementação.

| Nome | Idade máxima | Tamanho | Descrição |
| --- | --- | --- | --- |
| **`AMCV_###@AdobeOrg`** | 33696000 (390 dias) quando escrito pelo Web SDK | 44 bytes quando gravado pelo Web SDK (`MCMID\|<ECID>`); maior quando gravado por `VisitorAPI.js` | Presente quando [`idMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/idmigrationenabled) está habilitado, que é o padrão. Ajuda na transição para o Web SDK enquanto algumas partes do site ainda usam o `VisitorAPI.js`. O Web SDK lê esse cookie para reutilizar uma ECID existente. Depois que o Edge Network retorna uma ECID, o Web SDK a grava neste cookie se o cookie estiver ausente ou contiver uma ECID diferente. |
| **`com.adobe.alloy.getTld`** | Nenhum (cookie de sessão, excluído imediatamente) | 22 bytes | Cookie auxiliar temporário usado internamente pelo Web SDK para determinar o domínio de nível superior do site atual. O Web SDK grava e exclui esse cookie quando a biblioteca é carregada, antes que o comando `configure` seja executado e antes que o consentimento seja avaliado, para que os verificadores de cookie possam relatá-lo como definido antes do consentimento. O cookie contém apenas seu próprio nome e não armazena dados comportamentais ou de perfil. |
| **`demdex`** | 15552000 (180 dias) | varia | Cookie de terceiros no domínio `demdex.net`. Presente quando [`thirdPartyCookiesEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/thirdpartycookiesenabled) estiver habilitado (o padrão) e o navegador permitir cookies de terceiros por padrão, como Chrome ou Edge. Nesse caso, o Web SDK envia solicitações de identidade para `adobedc.demdex.net`, que define esse cookie. O Audience Manager usa esse cookie para atribuir uma ID exclusiva e uma ID de suporte para sincronização, segmentação, modelagem e relatórios. Consulte `demdex` em [cookies do Audience Manager](audience-manager.md). |
| **`kndctr_<orgId>_identity`** | 34128000 (395 dias) | 100-120 bytes (variável) | Armazena a ECID e outras informações relacionadas desse dispositivo. |
| **`kndctr_<orgId>_cluster`** | 1800 (30 minutos) | 3 a 5 bytes | Armazena a região do Edge Network (dica de localização) que atende às solicitações do usuário atual. A região é usada no caminho do URL para que o Edge Network possa rotear a solicitação para a região correta. Se um usuário se conectar com um endereço IP diferente durante a vida útil do cookie, a solicitação será roteada novamente para a região mais próxima. |
| **`kndctr_<orgId>_consent`** | 15552000 (180 dias) | 10-11 bytes | Armazena as preferências de consentimento do visitante. Sempre defina independentemente do consentimento, pois armazena as próprias preferências de consentimento. |
| **`kndctr_<orgId>_consent_check`** | 7200 (2 horas) | | Auxiliar de escopo de sessão que sinaliza ao Edge Network para verificar novamente o consentimento do lado do servidor após a expiração do TTL. Ela impõe um TTL no consentimento em cache. |
| **`kndctr_<orgId>_personalization`** | 34128000 (395 dias) | | Armazena informações de sessão que o Adobe Target usa para personalizar o conteúdo. |
| **`kndctr_<orgId>_advertising`** | 31622400 (366 dias), renovado sempre que o cookie for atualizado | 80 bytes a 1 KB (variável) | Apresentar quando o componente do Adobe Advertising (beta) for incluído na sua compilação do Web SDK e o consentimento do visitante for `in`. O Web SDK grava este cookie quando a URL da página contém os parâmetros de clique do Adobe Advertising (`s_kwcid` ou `ef_id`), ou quando os anunciantes do [Adobe Advertising DSP](https://experienceleague.adobe.com/en/docs/experience-platform/tags/extensions/client/web-sdk/configure/advertising) estão configurados. Ele armazena JSON codificado em URL que pode incluir dados de cliques de pesquisa (`_les_lsc`), um endereço IP com hash, um envelope LiveRamp RampID (quando um caminho JavaScript RampID é configurado) e carimbos de data e hora de conversão usados para limitar conversões duplicadas. Em navegadores que permitem cookies de terceiros por padrão, ele também armazena a ID do surfer da Adobe Advertising e exibe dados de cliques (`ev_lcc`). Este cookie é definido somente no nome do host atual. O componente também carrega recursos de `pixel.everesttech.net`, `www.everestjs.net` (quando uma ID de parceiro ID5 está configurada) e seu caminho RampID `ats.js`. Esses recursos podem definir seus próprios cookies, que não estão listados nesta página. |
| **`kndctr_<orgId>_bc_session_id`** | Nenhum (cookie de sessão) | | Presente quando o componente do Brand Concierge (beta) é usado. Armazena a ID da sessão de chat do Brand Concierge. O Web SDK lê este cookie somente quando [`stickyConversationSession`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/conversation) está habilitado, para que as sessões de chat persistam entre os carregamentos de página. |
| **`mbox`** | 63072000 (2 anos) | | Presente quando [`targetMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/targetmigrationenabled) está habilitado. Ele permite que o [cookie da mbox](https://developer.adobe.com/target/implement/client-side/atjs/atjs-cookies/) do Target seja definido pelo Web SDK. |
| **`mboxEdgeCluster`** | 1800 (30 minutos) | | Presente quando [`targetMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/targetmigrationenabled) está habilitado. Ele permite que o Web SDK comunique o cluster de borda correto com `at.js` para que os perfis do Target possam permanecer sincronizados enquanto os usuários navegam em um site. Quando o cookie `kndctr_<orgId>_cluster` não está presente, o Web SDK também lê esse cookie para rotear solicitações para a região do Edge Network correspondente. |
| **`s_ecid`** | 63115200 (2 anos) | ~45 bytes | Contém uma cópia da CX Enterprise ID (ECID/MID) no formato `s_ecid=MCMID\|<ECID>`. Atua como um backup próprio da ECID, principalmente para cenários CNAME (primários). Quando [`idMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/idmigrationenabled) está habilitado, o Web SDK lê este cookie para reutilizar uma ECID existente. |
| **Destinos de cookies do Audience Manager** (o nome varia) | 864000 (10 dias), a menos que o destino especifique um tempo de vida diferente | varia | Presente quando a Edge Network retorna um [destino de cookie](https://experienceleague.adobe.com/en/docs/audience-manager/user-guide/features/destinations/custom-destinations/create-cookie-destination) do Audience Manager para o visitante. O Web SDK grava um cookie próprio usando o nome, o valor e o domínio do cookie definidos no destino. Os valores são codificados por URL, consistentes com o Audience Manager Data Integration Library (DIL). |

O Edge Network define todos os seus cookies com os atributos `secure` e `sameSite="none"`. Se você tiver seções seguras e não seguras em seu site, a identificação do usuário pode ser imprecisa. Quando um usuário navega de uma seção segura do site para uma seção não segura, o Edge Network gera um novo `ECID` com a solicitação.

Os cookies que o Web SDK cria por conta própria, em vez de na direção do Edge Network, usam atributos diferentes. Os destinos de cookies do Audience Manager e do cookie `AMCV_###@AdobeOrg` incluem os atributos `secure` e `sameSite="none"` somente em páginas HTTPS. Os cookies `com.adobe.alloy.getTld` e `kndctr_<orgId>_advertising` usam os atributos padrão do navegador.
