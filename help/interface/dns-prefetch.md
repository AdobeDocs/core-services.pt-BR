---
description: Saiba como implementar a pré-busca DNS para ajudar a reduzir o tempo de carregamento de página com diferentes aplicativos e serviços no Experience Cloud.
solution: Experience Cloud
title: 'Uso da pré-busca DNS com diferentes aplicativos e serviços '
uuid: 4220e223-e00e-46b1-8bde-52248913bea1
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: caf2ff76-2076-436d-a5a7-aff531464480
source-git-commit: ae14748aa7b0f0d803d48fe980a6743f53d996ab
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 69%

---

# Uso da pré-busca DNS com diferentes aplicativos e serviços

Implemente a pré-busca DNS para ajudar a reduzir o tempo de carregamento da página com diferentes aplicativos e serviços.

## Noções básicas da pré-busca DNS {#section_772BF9CB7C4141DE9B0355146E2CD962}

Os navegadores usam a pré-busca DNS para resolver automaticamente os nomes de domínio vinculados em uma página da Web aos endereços IP correspondentes. O processo de pré-busca é inciado quando o navegador carrega uma página da Web. Como exemplo, considere que sua página contém um link que pode ser selecionado para `www.adobe.com`. Quando um navegador carrega essa página, ele usa o [sistema DNS](https://www.networksolutions.com/support/what-is-a-domain-name-server-dns-and-how-does-it-work/) para buscar o nome do domínio vinculado e resolvê-lo em um endereço IP numérico correspondente. A pré-busca DNS ajuda a melhorar o desempenho da página porque o nome do domínio já está resolvido a um endereço IP antes que um visitante do site clique nesse link ou botão. O processo de pré-busca DNS é transparente para os usuários.

## Pré-busca DNS e aplicativos Adobe Experience Cloud {#section_202A07F9F79F4ABDA44B98BA1DDCD516}

A pré-busca DNS funciona automaticamente com links estáticos e incorporados em uma página. Isso também significa que a pré-busca DNS automática não funciona com diferentes [!UICONTROL Experience Cloud] Aplicações e serviços porque:

* Cada aplicativo ou serviço de Experience Cloud gera chamadas DNS dinamicamente à medida que a página é carregada.
* O navegador não pode resolver nomes de domínio para endereço IP antes que essas chamadas sejam feitas.

No entanto, é possível implementar a pré-busca DNS manualmente com seus aplicativos Experience Cloud. Para isso, adicione a tag HTML `<dns-prefetch>` à seção `<head>` do código da página, como mostrado abaixo. Quando implementado adequadamente, a pré-busca DNS pode ajudar a economizar alguns milissegundos de tempo de carregamento da página.

## Amostras de código de pré-busca DNS {#section_E886F7B2861E48BA9EF3D8B3CE32B345}

Os exemplos a seguir mostram como fazer chamadas de pré-busca DNS para diferentes [!DNL Experience Cloud] aplicativos e serviços. Algumas chamadas de pré-busca exigem a ID da organização da [!DNL Adobe] ou as informações do servidor de rastreamento. Nesses exemplos, o código em *itálico* representa um espaço reservado de variável. Você pode substituir esse código pela sua ID de parceiro do [!DNL Adobe], pelo código do cliente, pelas informações do servidor de rastreamento e assim por diante.

* **Analytics:** `<link rel="dns-prefetch" href="//insert tracking server name here">`.

   Adicione uma tag separada para cada nome DNS se você usar servidores de rastreamento protegidos e não protegidos.

* **Audience Manager:** `<link rel="dns-prefetch" href="//dpm.demdex.net">`

* **Serviço da Experience Cloud ID:** `<link rel="dns-prefetch" href="//fast. *`insira a ID do parceiro aqui`*.demdex.net">`

* **Gerenciador dinâmico de tags** (DTM): Não obrigatório. Os links do DTM ficam disponíveis quando a página é carregada.

* **Media Optimizer (Advertising Cloud):**

   * `<link rel="dns-prefetch" href="//pixel.everesttech.net">`
   * `<link rel="dns-prefetch" href="//cm.everesttechnet">`


* **[!DNL Target]:** `<link rel="dns-prefetch" href="//insert customer code here.tt.omtrdc.net">`

>[!MORELIKETHIS]
>
>* [Pré-busca DNS](https://www.chromium.org/developers/design-documents/dns-prefetching)

