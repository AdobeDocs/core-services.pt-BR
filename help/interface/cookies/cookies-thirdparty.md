---
description: Como o suporte a cookies de terceiros se tornou cada vez mais limitado nos navegadores, a Adobe tem trabalhado em novas soluções que equilibram as necessidades do cliente com seu direito de privacidade nas soluções da Adobe Experience Cloud.
keywords: cookies; privacidade
seo-description: Como o suporte a cookies de terceiros se tornou cada vez mais limitado nos navegadores, a Adobe tem trabalhado em novas soluções que equilibram as necessidades do cliente com seu direito de privacidade nas soluções da Adobe Experience Cloud.
seo-title: Como as alterações no suporte a cookies de terceiros afeta os clientes
solution: Experience Cloud,Analytics,Target,Social
title: Como as alterações no suporte a cookies de terceiros afeta os clientes
uuid: 27332e0d-6932-4a6e-b97b-0adeced0b050
index: y
internal: n
snippet: y
translation-type: ht
source-git-commit: f59badcd3423ada51a3fe0c605158a009d5b1d64

---


# Como as alterações no suporte a cookies de terceiros afetam os clientes{#how-changes-to-third-party-cookie-support-impacts-customers}

Como o suporte a cookies de terceiros se tornou cada vez mais limitado nos navegadores, a Adobe tem trabalhado em novas soluções que equilibram as necessidades do cliente com seu direito de privacidade nas soluções da Adobe Experience Cloud.

A seguinte lista descreve como o suporte a cookies de terceiros afeta as implementações atuais das soluções da Adobe Experience Cloud:

## Adobe Analytics e Adobe Target

* Clientes com uma [implementação própria](/help/interface/cookies/cookies-first-party.md) permaneceriam praticamente inalterados.
* Os clientes que não usam implementação própria podem implementar o [Serviço de ID da Experience Platform](https://docs.adobe.com/content/help/pt-BR/id-service/using/implementation-guides/implementation-guides.html) para armazenar o cookie da ID como um cookie próprio, sem uma implementação própria.

## Adobe Experience Manager

* Como o Adobe Experience Manager funciona integralmente no domínio do cliente, há uma interação mínima com cookies de terceiros e, portanto, impacto mínimo ou inexistente.

## Adobe Social

* O Social não é afetado, desde que o cliente tenha a versão mais recente do código.

## Adobe Advertising Cloud

* Pesquisa:

   * Quando a pesquisa é otimizada com base nos dados do Adobe Analytics, ela será afetada da mesma forma que o Adobe Analytics.
   * A coleta e dados de conversão não deve ser afetada.

* Exibir:

   * A exibição de remarketing hoje é totalmente dependente da utilização de cookies de terceiros.
   * A exibição também é altamente dependente da disponibilidade de diferentes cookies de rede de publicidade para sincronização.
   * O impacto geral é desconhecido. Entretanto, de acordo com o primeiro ponto, a exibição é afetada mais do que os serviços.
   * Estamos trabalhando internamente e com nossos parceiros de publicidade para avaliar a extensão total do impacto no fornecimento de anúncios.

* Social:

   * Não há impacto nos anúncios do Facebook marketplace.
   * O Facebook Exchange (FBX) será afetado da mesma forma que a exibição do fornecimento de anúncios.

