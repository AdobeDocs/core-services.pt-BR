---
description: Saiba mais sobre como o suporte a cookies de terceiros se tornou cada vez mais limitado nos navegadores.
keywords: cookies; privacidade
solution: Experience Cloud,Analytics,Target
title: 'Como as alterações no suporte a cookies de terceiros afetam os clientes '
uuid: 27332e0d-6932-4a6e-b97b-0adeced0b050
feature: Cookies
topic: Administração
role: Administrator
level: Experienced
exl-id: 3d12a1b1-c952-4b42-815d-f64b31429cec
source-git-commit: f720e37b693da2c657cb1efab45620c60bfa81a4
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 59%

---

# Como as alterações no suporte a cookies de terceiros afetam os clientes {#how-changes-to-third-party-cookie-support-impacts-customers}

O suporte a cookies de terceiros se tornou mais limitado em navegadores. Assim, o Adobe tem trabalhado em novas soluções que equilibram as necessidades do cliente com o direito do consumidor à privacidade nos aplicativos de Experience Cloud.

A lista a seguir descreve como o suporte a cookies de terceiros afeta as implementações atuais de aplicativos Experience Cloud:

## Adobe Analytics e Adobe Target

* O Analytics e o Target não são afetados, pois a mesma atividade do site depende apenas de cookies próprios. Cookies de terceiros são necessários para entender a atividade do usuário em vários domínios. Para navegadores onde cookies de terceiros são bloqueados, o rastreamento entre domínios não é possível usando cookies.

## Adobe Experience Manager

* Como o Adobe Experience Manager funciona integralmente no domínio do cliente, há uma interação mínima com cookies de terceiros e, portanto, impacto mínimo ou inexistente.

## Adobe Social

* O Social não é afetado, desde que o cliente tenha a versão mais recente do código.

## Adobe Advertising Cloud

* Pesquisa:

   * Quando a pesquisa for otimizada com base nos dados do Adobe Analytics, ela será afetada da mesma forma que o Adobe Analytics.
   * A coleta de dados de conversão não deve ser afetada.

* Exibir:

   * O remarketing de exibição hoje depende totalmente do uso de cookies de terceiros.
   * A exibição também depende muito da disponibilidade de vários cookies de rede de publicidade para sincronização.
   * O impacto geral é desconhecido. No entanto, de acordo com o primeiro ponto, a exibição é afetada mais do que outros serviços.
   * O Adobe está trabalhando internamente e com nossos parceiros de publicidade para avaliar a extensão total do impacto na entrega de anúncios.
