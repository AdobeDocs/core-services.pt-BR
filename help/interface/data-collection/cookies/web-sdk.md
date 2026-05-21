---
title: Cookies do Adobe Experience Platform Web SDK
description: Saiba como o Web SDK usa cookies aplicáveis à sua implementação.
solution: Experience Cloud
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 14f06dc9-255e-4a6c-adec-471107cf202e
TQID: https://experienceleague.adobe.com/jysQ5m7o0cI3ECKz2RWZB4Kt3own7XAPm04pr4yLh-k
product_v2: id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2: id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2: id: b75843fa-0a67-4a44-a6b1-cc627b0481dcid: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 50012e2564e88e1a6e16578e3331136c7df0cb21
workflow-type: tm+mt
source-wordcount: 484
ht-degree: 1%

---

# Cookies do Adobe Experience Platform Web SDK

O Adobe Experience Platform Web SDK usa cookies para armazenar valores específicos para sua implementação.

| Nome | Idade máxima | Tamanho | Descrição |
| --- | --- | --- | --- |
| **`AMCV_###@AdobeOrg`** | 34128000 (395 dias) | 100-120 bytes (variável) | Presente quando [`idMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/idmigrationenabled) está habilitado. Ajuda na transição para o Web SDK enquanto algumas partes do site ainda usam o `visitor.js`. O Web SDK lê e grava neste cookie durante a migração. |
| **`com.adobe.alloy.getTld`** | Nenhum (excluído imediatamente) | N/D | Cookie auxiliar temporário usado internamente pelo Web SDK para determinar o domínio de nível superior do site atual. Depois que o domínio de nível superior é estabelecido, o cookie é excluído. Ele não armazena dados comportamentais ou de perfil. |
| **`demdex`** | 15552000 (180 dias) | varia | Apresentar se a sincronização da Audience Manager ID estiver habilitada. O Audience Manager define esse cookie para atribuir uma ID exclusiva e uma ID de suporte para sincronização, segmentação, modelagem e relatórios. Consulte `demdex` em [cookies do Audience Manager](audience-manager.md). |
| **`kndctr_<orgId>_identity`** | 34128000 (395 dias) | 100-120 bytes (variável) | Armazena a ECID e outras informações relacionadas desse dispositivo. |
| **`kndctr_<orgId>_cluster`** | 1800 (30 minutos) | 3 a 5 bytes | Armazena a região do Edge Network (dica de localização) que atende às solicitações do usuário atual. A região é usada no caminho do URL para que o Edge Network possa rotear a solicitação para a região correta. Se um usuário se conectar com um endereço IP diferente durante a vida útil do cookie, a solicitação será roteada novamente para a região mais próxima. |
| **`kndctr_<orgId>_consent`** | 15552000 (180 dias) | 10-11 bytes | Armazena as preferências de consentimento do visitante. Sempre defina independentemente do consentimento, pois armazena as próprias preferências de consentimento. |
| **`kndctr_<orgId>_consent_check`** | 7200 (2 horas) | | Auxiliar de escopo de sessão que sinaliza ao Edge Network para verificar novamente o consentimento do lado do servidor após a expiração do TTL. Ela impõe um TTL no consentimento em cache. |
| **`kndctr_<orgId>_personalization`** | 34128000 (395 dias) | | Armazena informações de sessão que o Adobe Target usa para personalizar o conteúdo. |
| **`mbox`** | 63072000 (2 anos) | | Presente quando [`targetMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/targetmigrationenabled) está habilitado. Ele permite que o [cookie da mbox](https://developer.adobe.com/target/implement/client-side/atjs/atjs-cookies/) do Target seja definido pelo Web SDK. |
| **`mboxEdgeCluster`** | 1800 (30 minutos) | | Presente quando [`targetMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/targetmigrationenabled) está habilitado. Ele permite que o Web SDK comunique o cluster de borda correto com `at.js` para que os perfis do Target possam permanecer sincronizados enquanto os usuários navegam em um site. |
| **`s_ecid`** | 63115200 (2 anos) | ~45 bytes | Contém uma cópia do CX Enterprise ID (ECID/MID) no formato `s_ecid=MCMID\|<ECID>`. Atua como um backup próprio da ECID, principalmente para cenários CNAME (primários). |

O Edge Network define todos os cookies com os atributos `secure` e `sameSite="none"`. Se você tiver seções seguras e não seguras em seu site, a identificação do usuário pode ser imprecisa. Quando um usuário navega de uma seção segura do site para uma seção não segura, o Edge Network gera um novo `ECID` com a solicitação.
