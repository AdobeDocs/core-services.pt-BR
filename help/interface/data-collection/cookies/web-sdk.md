---
title: Cookies do SDK da Web da Adobe Experience Platform
description: Saiba como o SDK da Web usa cookies aplicáveis à sua implementação.
solution: Experience Cloud
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 14f06dc9-255e-4a6c-adec-471107cf202e
source-git-commit: 2a80851c0a7d4ef7dbcc2565177b239f3e063164
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Cookies do Adobe Experience Platform Web SDK

O SDK da Web da Adobe Experience Platform usa cookies para armazenar valores específicos para a implementação.

| Nome | Idade máxima | Descrição |
|---|---|---|
| **kndct_orgid_identity** | 34128000 (395 dias) | Armazena a ECID, bem como outras informações relacionadas à ECID. |
| **kndctr_orgid_consent_check** | 7200 (2 horas) | Sinaliza ao servidor para procurar as preferências de consentimento no lado do servidor. |
| **kndctr_orgid_consent** | 15552000 (180 dias) | Armazena a preferência de consentimento do usuário para o site. |
| **kndctr_orgid_cluster** | 1800 (30 minutos) | Armazena a região do Edge Network que atende às solicitações do usuário atual. A região é usada no caminho do URL para que o Edge Network possa rotear a solicitação para a região correta. Se um usuário se conectar com um endereço IP diferente ou em uma sessão diferente, a solicitação será roteada novamente para a região mais próxima. |
| **mbox** | 63072000 (2 anos) | Presente quando a configuração de migração do Target estiver definida como verdadeira. Ele permite que o [cookie da mbox](https://developer.adobe.com/target/implement/client-side/atjs/atjs-cookies/) do Target seja definido pelo SDK da Web. |
| **mboxEdgeCluster** | 1800 (30 minutos) | Presente quando a configuração de migração do Target estiver definida como verdadeira. Ele permite que o SDK da Web comunique o cluster de borda correto com `at.js` para que os perfis do Target possam permanecer sincronizados enquanto os usuários navegam em um site. |
| **AMCV_###@AdobeOrg** | 34128000 (395 dias) | Presente quando [`idMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/web-sdk/commands/configure/idmigrationenabled) está habilitado. Ajuda na transição para o SDK da Web enquanto algumas partes do site ainda usam o `visitor.js`. |

O Edge Network define todos os cookies com os atributos `secure` e `sameSite="none"`. Se você tiver seções seguras e não seguras em seu site, a identificação do usuário pode ser imprecisa. Quando um usuário navega de uma seção segura do site para uma seção não segura, o Edge Network gera um novo `ECID` com a solicitação.
