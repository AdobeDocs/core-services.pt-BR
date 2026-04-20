---
title: Coleta de dados regionais
description: Saiba mais sobre a coleta de dados regionais na CX Enterprise.
exl-id: 295e9736-2a58-48a8-9968-5dfa33b70d95
TQID: https://experienceleague.adobe.com/hjHQDRoNOP2e6pKhKHB9DZaII2o8eJVzL5wjRzaMFwM
product_v2:
  - id: e1971122-7081-4556-9222-8a31bd71800c
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
  - id: d3cdead0-685a-4489-9250-4bb709942f66
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 1a77ef8d31211fb11c790152e78037a8c3b238a2
workflow-type: tm+mt
source-wordcount: 299
ht-degree: 0%

---

# Coleta de dados regionais

A Adobe CX Enterprise usa a coleta de dados regionais (RDC) para que as interações entre seus visitantes e o Adobe ocorram o mais próximo possível de seus visitantes. Os dados coletados localmente em um site de borda são encaminhados com segurança a um site principal para processamento. Após processados, os dados são disponibilizados para produtos e serviços da Adobe CX Enterprise.

O fluxo de trabalho de coleta de dados regional oferece vários benefícios:

* **Desempenho**: com a RDC, seus visitantes se conectam ao site de borda mais próximo. Essa otimização fornece o tempo de resposta mais rápido, resultando em rastreamento mais preciso e em tempos de carregamento mais rápidos.
* **Redundância**: se houver uma interrupção na comunicação entre qualquer site de borda e o site principal, a infraestrutura da Adobe salvará os dados localmente e os encaminhará para o site principal quando as comunicações forem restauradas. O Adobe também pode rotear o tráfego para outros sites de borda se um local específico sofrer interrupções.

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

_*A RDC da China exige o pacote complementar de Otimização de Desempenho da China e se aplica somente à Adobe Analytics que usa a coleta de dados da AppMeasurement. Outros serviços da CX Enterprise e coleta de dados do Web SDK não são compatíveis. Entre em contato com a equipe de conta da Adobe para saber mais sobre o pacote complementar para Otimização de desempenho na China._

## Coleta de dados de terceiros

A coleção de dados de terceiros inclui domínios de cookies que não correspondem ao domínio do site. Os exemplos incluem `adobedc.net`, `omtrdc.net` e `2o7.net`.

| Tipo de RDC | Centros de coleta de dados |
| --- | --- |
| Padrão | Oregon, Virgínia, Irlanda, Paris, Mumbai, Singapura, Tóquio, Sydney |
| Padrão + China* | Pequim*, Oregon, Virgínia, Irlanda, Paris, Mumbai, Singapura, Tóquio, Sydney |

{style="table-layout:auto"}

