---
description: Saiba mais sobre os cookies do Adobe Advertising para mapear eventos de envolvimento de anúncios em eventos de conversão e, possivelmente, usar essas informações para otimizar ofertas de anúncios.
title: Cookies do Adobe Advertising
uuid: 2eec48a3-3e81-488e-8e30-5fd62885de0b
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 6818edea-31b1-49fc-bca2-32828c7ca78d
TQID: 'https://experienceleague.adobe.com/jr9RwaF63elDUN-XewIdrPNsGb6T5wo98vktP5U6jIM'
product_v2: id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2: id: dab36b01-8bfa-48f3-8392-626455a058e6id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2: id: eb7e29b9-c5e9-4ed0-8e4b-6465dabb3cb1
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 9c2010694b8bb32c3922dd65f846375e43b2caac
workflow-type: tm+mt
source-wordcount: 309
ht-degree: 15%

---

# Cookies do Adobe Advertising

A Adobe Advertising (anteriormente Adobe Advertising Cloud) usa cookies para mapear eventos de envolvimento de anúncios a eventos de conversão e, possivelmente, para usar essas informações para otimizar ofertas de anúncios.

>[!NOTE]
>
>A tag beta do Javascript Adobe Advertising que usa o [Adobe CX Enterprise ID (ECID) Service](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html?lang=pt-BR) cria cookies próprios [CX Enterprise](experience-cloud.md) `s_ecid`, não cookies Adobe Advertising.

| Nome do cookie | Expiração | Tamanho | Localização | Descrição |
| --- | --- | --- | --- | --- |
| **`_lcc`** | 15 minutos | 52 bytes | `everesttech.net` | Armazena IDs e carimbos de data e hora de cliques de exibição. Determina se um evento de clique em um anúncio de exibição se aplica a uma ocorrência do Adobe Analytics. |
| **`_tmae`** | 1 ano | 1 KB | `everesttech.net` | Armazena IDs codificadas e carimbos de data e hora para envolvimento de anúncios usando o rastreamento do DSP. Inclui o engajamento do usuário com anúncios, como anúncios vistos pela última vez |
| **`_tmid`** | 1 ano | ~20 bytes | `everesttech.net` | Armazena a ID do Adobe Advertising Demand Side Platform (DSP). Corresponde à ID de visitante no cookie `everest_g_v2`. |
| **`adcloud`** | 1 ano | 50-150 bytes | Primários | Os carimbos de data e hora da última visita ao site e o último clique de pesquisa do visitante. Também armazena a `ef_id` que foi criada quando o visitante clicou em um anúncio. Vincula a ID de visitante a segmentos de público-alvo e conversões relevantes. Ajuda a otimizar os tempos de carregamento da página, evitando solicitações desnecessárias para o Adobe. |
| **`ev_sync_*`** |  | 8 bytes | `everesttech.net` | A data em que a sincronização é executada no formato `yyymmdd`. Sincroniza a ID de visitante do Adobe Advertising com a troca de anúncios do parceiro. Ele é criado para novos visitantes e envia uma solicitação de sincronização quando expira. Inclui os cookies `ev_sync_ax`, `ev_sync_bk`, `ev_sync_dd`, `ev_sync_fs`, `ev_sync_ix`, `ev_sync_nx`, `ev_sync_ox`, `ev_sync_pm`, `ev_sync_rc`, `ev_sync_tm` e `ev_sync_yh`. |
| **`everest_g_v2`** | 1 ano | ~27 bytes | `everesttech.net` | Armazena o navegador e a ID do visitante. Criada depois que um usuário clica inicialmente em um anúncio. Usado para mapear os cliques atuais e subsequentes com outros eventos em seu site. |
| **`everest_session_v2`** | Session | ~16 bytes | `everesttech.net` | Armazena a ID da sessão atual. |
| **`id_adcloud`** | 91 dias | 16 bytes | Primários | Armazena a ID do visitante. |

{style="table-layout:auto"}

