---
title: Coleta de dados regionais
description: Saiba mais sobre a coleta de dados regionais no Experience Cloud.
exl-id: 295e9736-2a58-48a8-9968-5dfa33b70d95
source-git-commit: 2a80851c0a7d4ef7dbcc2565177b239f3e063164
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# Coleta de dados regionais

A Adobe Experience Cloud usa a coleta de dados regionais (RDC) para que as interações entre seus visitantes e o Adobe aconteçam o mais próximo possível de seus visitantes. Os dados coletados localmente em um site de borda são encaminhados com segurança a um site principal para processamento. Após processados, os dados são disponibilizados para produtos e serviços da Adobe Experience Cloud.

O fluxo de trabalho de coleta de dados regional oferece vários benefícios:

* **Desempenho**: com a RDC, seus visitantes se conectam ao site de borda mais próximo. Essa otimização fornece o tempo de resposta mais rápido, resultando em rastreamento mais preciso e em tempos de carregamento mais rápidos.
* **Redundância**: se houver uma interrupção na comunicação entre qualquer site de borda e o site principal, a infraestrutura do Adobe salva os dados localmente e os encaminha para o site principal quando as comunicações forem restauradas. O Adobe também pode rotear o tráfego para outros sites de borda se um local específico sofrer interrupções.

Atualmente, a RDC inclui as seguintes localidades (sujeitas a alteração):

## Coleta de dados primários

| Tipo de RDC | Centros de coleta de dados |
| --- | --- |
| Global (padrão) | Oregon, Virgínia, Irlanda, Paris, Mumbai, Singapura, Tóquio, Sydney |
| Global + China* | Pequim*, Oregon, Virgínia, Irlanda, Paris, Mumbai, Singapura, Tóquio, Sydney |
| Somente Américas | Oregon, Virgínia |
| Somente Europa | Irlanda, Paris |
| Somente Pacífico Asiático | Mumbai, Singapura, Tóquio, Sydney |
| Somente China* | Pequim |

{style="table-layout:auto"}

_*A RDC da China exige o pacote complementar de Otimização de Desempenho da China e se aplica somente à Adobe Analytics usando a coleta de dados do AppMeasurement. Outros serviços Experience Cloud e coleção de dados do SDK da Web não são compatíveis. Entre em contato com a equipe de conta do Adobe para saber mais sobre o pacote complementar para Otimização de desempenho na China._

## Coleta de dados de terceiros

A coleção de dados de terceiros inclui domínios de cookies que não correspondem ao domínio do site. Os exemplos incluem `adobedc.net`, `omtrdc.net` e `2o7.net`.

| Tipo de RDC | Centros de coleta de dados |
| --- | --- |
| Padrão | Oregon, Virgínia, Irlanda, Paris, Mumbai, Singapura, Tóquio, Sydney |
| Padrão + China* | Pequim*, Oregon, Virgínia, Irlanda, Paris, Mumbai, Singapura, Tóquio, Sydney |

{style="table-layout:auto"}
