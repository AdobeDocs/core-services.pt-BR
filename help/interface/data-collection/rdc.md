---
title: Coleta de dados regionais
description: Saiba mais sobre a coleta de dados regionais no CX Enterprise.
exl-id: 295e9736-2a58-48a8-9968-5dfa33b70d95
TQID: 'https://experienceleague.adobe.com/0thWRpu2KT2EFomB1hkgehjHfVrXMeKD-K0VN-fvfrM'
product_v2:
  - id: e1971122-7081-4556-9222-8a31bd71800c
role_v2: id:id:
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
  - id: d3cdead0-685a-4489-9250-4bb709942f66
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: f01d85af42b8f2c27dbada8f73546bc6fe4bf710
workflow-type: tm+mt
source-wordcount: 361
ht-degree: 0%

---

# Coleta de dados regionais

O Adobe CX Enterprise usa a coleta de dados regionais (RDC) para que as interações entre seus visitantes e o Adobe ocorram o mais próximo possível de seus visitantes. Os dados coletados localmente em um site de borda são encaminhados com segurança a um site principal para processamento. Depois de processados, os dados são disponibilizados para os produtos e serviços da Adobe CX Enterprise.

O fluxo de trabalho de coleta de dados regional oferece vários benefícios:

* **Desempenho**: com a RDC, seus visitantes se conectam ao site de borda mais próximo. Essa otimização fornece o tempo de resposta mais rápido, resultando em rastreamento mais preciso e em tempos de carregamento mais rápidos.
* **Redundância**: se houver uma interrupção na comunicação entre qualquer site de borda e o site principal, a infraestrutura da Adobe salvará os dados localmente e os encaminhará para o site principal quando as comunicações forem restauradas. O Adobe também pode rotear o tráfego para outros sites de borda se um local específico sofrer interrupções.

## Coleta de dados primários

A coleta de dados primários usa uma implementação CNAME para rotear dados para a Adobe por meio de seu próprio domínio. Seu tipo de RDC está selecionado como parte do processo de instalação do [Programa de Certificados Gerenciados pela Adobe](adobe-managed-cert.md). Para verificar ou atualizar o tipo de RDC, entre em contato com a equipe de conta da Adobe. Os seguintes tipos de RDC e data centers associados estão disponíveis:

| Tipo de RDC | Centros de coleta de dados |
| --- | --- |
| Global (padrão) | Oregon, Virgínia, Irlanda, Paris, Mumbai, Singapura, Tóquio, Sydney |
| Global + China* | Pequim*, Oregon, Virgínia, Irlanda, Paris, Mumbai, Singapura, Tóquio, Sydney |
| Somente Américas | Oregon, Virgínia |
| Somente Europa | Irlanda, Paris |
| Somente Pacífico Asiático | Mumbai, Singapura, Tóquio, Sydney |
| Somente China* | Pequim |

_*A RDC da China exige o pacote complementar de Otimização de Desempenho da China e se aplica somente à Adobe Analytics que usa a coleta de dados da AppMeasurement. Outros serviços CX Enterprise e coleta de dados do Web SDK não são compatíveis. Entre em contato com a equipe de conta da Adobe para saber mais sobre o pacote complementar para Otimização de desempenho na China._

## Coleta de dados de terceiros

A coleta de dados de terceiros usa domínios de cookies que não correspondem ao domínio do site. Os exemplos incluem `adobedc.net`, `omtrdc.net` e `2o7.net`.

| Tipo de RDC | Centros de coleta de dados |
| --- | --- |
| Padrão | Oregon, Virgínia, Irlanda, Paris, Mumbai, Singapura, Tóquio, Sydney |
| Padrão + China* | Pequim*, Oregon, Virgínia, Irlanda, Paris, Mumbai, Singapura, Tóquio, Sydney |

_*Requer o pacote complementar para Otimização de desempenho da China. Consulte a seção de coleta de dados próprios acima para obter detalhes._
