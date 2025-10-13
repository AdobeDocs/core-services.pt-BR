---
description: Saiba mais sobre os cookies do Adobe Analytics na Adobe Experience Cloud.
solution: Analytics
title: Cookies do Adobe Analytics
uuid: e2d3d61d-2708-48b2-a7e6-2331f2aed8e0
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: bc8ce894-f98c-4475-8a07-d74ae76f7451
source-git-commit: d3a559ca2f7963256d48a25cd51099edb5e3fe76
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 11%

---

# Cookies do Adobe Analytics

O Adobe Analytics usa cookies para diferenciar solicitações de navegadores diferentes e armazenar informações úteis que um aplicativo pode usar posteriormente. Eles também podem ser usados para associar informações de navegação a registros de clientes.

O Analytics usa cookies para definir novos visitantes anonimamente, ajudar a analisar dados de sequência de cliques e rastrear a atividade do histórico no site, como a resposta a campanhas específicas ou a duração do ciclo de vendas.

| Nome do cookie | Expiração | Tamanho | Localização | Descrição |
| --- | --- | --- | --- | --- |
| **`s_ecid`** | 13 meses | 45 bytes | Primários | Armazena a Experience Cloud ID (ECID) ou a MID. Definido por resposta HTTP. A MID está armazenada no formato `s_ecid=MCMID`. Definido depois que o cliente define o cookie AMCV. Ela permite o rastreamento persistente de ID primária e é usada como ID de referência se o cookie AMCV expirar. `SameSite` está definido como &quot;Lax&quot;. Se você usar o Web SDK para implementar o Adobe Analytics, a expiração do cookie será definida como 2 anos; no entanto, a maioria dos navegadores modernos trunca a expiração para 13 meses. |
| **`s_cc`** | Session | 4 bytes | Primários | Determina se os cookies estão ativados. Definido pelo JavaScript. |
| **`s_sq`** | Session | 100-200 bytes | Primários | Usado pelo Activity Map. Ele contém informações sobre o link anterior clicado pelo visitante. Definido pelo JavaScript. |
| **`s_vi`** | 2 anos | 44 bytes | Primário ou `*.omtrdc.net` (terceiro) | Armazena um identificador de visitante único e um carimbo de data e hora. Definido por resposta HTTP. Cada ID de visitante está associada a um perfil de visitante nos servidores da Adobe. Os perfis do visitante são excluídos após 1 ano de inatividade, independentemente de qualquer expiração de cookie da ID do visitante. O sinalizador `Secure` é definido quando `SameSite` é &quot;Nenhum&quot; e a conexão é HTTPS. `SameSite` é &quot;Lax&quot; por padrão para cookies próprios. `SameSite` é &quot;Nenhum&quot; ao usar cookies de terceiros, como em `omtrdc.net` ou `2o7.net`. Defina `SameSite` como &quot;Nenhum&quot; ao usar um único CNAME para rastrear vários domínios ou propriedades. |
| **`s_fid`** | 2 anos | 33 bytes | Primários | Armazena a ID de visitante exclusiva de fallback e o carimbo de data e hora. Definido pelo JavaScript se o cookie padrão `s_vi` não puder ser definido devido a restrições de cookies de terceiros. Não usado para implementações de cookies primários. |
| **`s_ac`** | Imediato | 1 byte | Primários | Ajuda a determinar o domínio correto para definir cookies do AppMeasurement. Contém o valor estático `"1"`. Depois que este cookie é configurado, ele é excluído imediatamente. |

## Cookies definidos por plug-ins

Algumas implementações usam plug-ins, que são trechos de código que fornecem funcionalidade adicional para o Analytics. Esses plug-ins podem definir cookies que não estão listados acima. Consulte [Visão geral dos plug-ins do Analytics](https://experienceleague.adobe.com/en/docs/analytics/implementation/vars/plugins/impl-plugins) para obter uma lista de plug-ins disponíveis e quais cookies eles definiram.

## Consequências da exclusão de cookies do Analytics

Se um visitante excluir os cookies do Analytics, considere o seguinte:

* **A identificação do visitante é perdida:** quando os cookies são excluídos, o Adobe Analytics não consegue reconhecer os visitantes recorrentes. Na próxima vez que o usuário visitar seu site, ele será contado como um novo visitante. [A Análise entre dispositivos](https://experienceleague.adobe.com/en/docs/analytics/components/cda/overview) pode ajudar a atenuar esse impacto.
* **A continuidade da sessão foi interrompida:** Qualquer análise baseada em sessão ou de várias visitas (como rastreamento de atribuição ou conversão) foi interrompida. Eventos e conversões que ocorrem após a exclusão do cookie não podem ser vinculados a atividades anteriores pelo mesmo usuário.
* **O Personalization e a segmentação são afetados:** Segmentos ou experiências personalizadas com base no histórico ou comportamento do visitante são redefinidos, pois os dados anteriores não são mais associados à visita atual.
* **O rastreamento entre domínios foi interrompido:** Em cookies de terceiros, a exclusão deles impede que o Adobe Analytics vincule as atividades dos usuários em vários domínios pertencentes a você.
