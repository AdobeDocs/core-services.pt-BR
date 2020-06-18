---
description: Como o suporte a cookies de terceiros se tornou cada vez mais limitado nos navegadores, a Adobe tem trabalhado em novas soluções que equilibram as necessidades do cliente com seu direito de privacidade nas soluções da Adobe Experience Cloud.
keywords: cookies;privacy
seo-description: Como o suporte a cookies de terceiros se tornou cada vez mais limitado nos navegadores, a Adobe tem trabalhado em novas soluções que equilibram as necessidades do cliente com seu direito de privacidade nas soluções da Adobe Experience Cloud.
seo-title: Como as alterações no suporte a cookies de terceiros afeta os clientes
solution: Marketing Cloud,Analytics,Adobe Target,Adobe Social
title: Como as alterações no suporte a cookies de terceiros afeta os clientes
uuid: 27332e0d-6932-4a6e-b97b-0adeced0b050
translation-type: tm+mt
source-git-commit: f65132e291ba925ded39d75e92b24cf707d520b5
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 91%

---


# Como as alterações no suporte a cookies de terceiros afetam os clientes {#how-changes-to-third-party-cookie-support-impacts-customers}

Como o suporte a cookies de terceiros se tornou cada vez mais limitado nos navegadores, a Adobe tem trabalhado em novas soluções que equilibram as necessidades do cliente com seu direito de privacidade nas soluções da Adobe Experience Cloud.

A seguinte lista descreve como o suporte a cookies de terceiros afeta as implementações atuais das soluções da Adobe Experience Cloud:

## Adobe Analytics e Adobe Target

* Clientes com uma [implementação própria](/help/interface/cookies/cookies-first-party.md) permaneceriam praticamente inalterados.
* Os clientes que não usam implementação própria podem implementar o [Serviço de ID da Experience Platform](https://docs.adobe.com/content/help/pt-BR/id-service/using/implementation/implementation-guides.html) para armazenar o cookie da ID como um cookie próprio, sem uma implementação própria.

## Adobe Experience Manager

* Como o Adobe Experience Manager funciona integralmente no domínio do cliente, há uma interação mínima com cookies de terceiros e, portanto, impacto mínimo ou inexistente.

## Adobe Social

* O Social não seria afetado, desde que o cliente tivesse a versão mais recente do código.

## Adobe Advertising Cloud

* Pesquisa:

   * Quando a pesquisa for otimizada com base nos dados do Adobe Analytics, ela será afetada da mesma forma que o Adobe Analytics.
   * A coleta de dados de conversão não deve ser afetada.

* Exibir:

   * O remarketing de exibição hoje depende totalmente do uso de cookies de terceiros.
   * A exibição também depende muito da disponibilidade de vários cookies de rede de publicidade para sincronização.
   * O impacto geral é desconhecido. No entanto, de acordo com o primeiro ponto, a exibição é afetada mais do que outros serviços.
   * Estamos trabalhando internamente e com nossos parceiros de publicidade para avaliar a extensão total do impacto na entrega de anúncios.

* Social:

   * Não há impacto nos anúncios do Facebook market-place.
   * O Facebook Exchange (FBX) será afetado da mesma forma que a entrega de anúncios de exibição.
