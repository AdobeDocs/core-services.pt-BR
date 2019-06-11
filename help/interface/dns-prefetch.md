---
description: Implemente a pré-busca DNS para ajudar a reduzir o tempo de carregamento da página com soluções e serviços diferentes.
seo-description: Implemente a pré-busca DNS para ajudar a reduzir o tempo de carregamento da página com soluções e serviços diferentes.
seo-title: Uso da pré-busca DNS com diferentes soluções e serviços
solution: Experience Cloud
title: Uso da pré-busca DNS com diferentes soluções e serviços
uuid: 4220 e 223-e 00 e -46 b 1-8 bde -52248913 bea 1
translation-type: tm+mt
source-git-commit: af5339fe58ce884345804574c209907d6504a483

---


# Uso da pré-busca DNS com diferentes soluções e serviços

Implemente a pré-busca DNS para ajudar a reduzir o tempo de carregamento da página com soluções e serviços diferentes.

## Noções básicas da pré-busca DNS {#section_772BF9CB7C4141DE9B0355146E2CD962}

Os navegadores usam a pré-busca DNS para resolver automaticamente os nomes de domínio vinculados em uma página da Web aos endereços IP correspondentes. O processo de pré-busca inicia quando o navegador carrega uma página da Web. Como exemplo, considere que sua página contém um link clicável para `www.adobe.com`. Quando um navegador carrega essa página, ele usa o [sistema DNS](https://www.networksolutions.com/support/what-is-a-domain-name-server-dns-and-how-does-it-work/) para buscar o nome do domínio vinculado e resolvê-lo em um endereço IP numérico correspondente. A pré-busca DNS ajuda a melhorar o desempenho da página, pois o nome do domínio já foi resolvido em um endereço IP antes de um visitante do site clicar nesse link ou botão. O processo da pré-busca DNS é transparente para os usuários.

## Pré-busca DNS e soluções da Adobe Experience Cloud {#section_202A07F9F79F4ABDA44B98BA1DDCD516}

A pré-busca DNS funciona automaticamente com links estáticos e incorporados em uma página. Isso significa que a pré-busca DNS automática não funciona com soluções e serviços da [!UICONTROL Experience Cloud], pois:

* Cada solução ou serviço da Experience Cloud gera chamadas DNS dinamicamente à medida que a página é carregada.
* O navegador não pode resolver nomes de domínio para um endereço IP antes de efetuar essas chamadas.

Entretanto, você pode implementar a pré-busca DNS manualmente com as soluções da Experience Cloud. Você faz isso adicionando a tag HTML `<dns-prefetch>` à `<head>` seção do código da página, como mostrado abaixo. Quando implementado adequadamente, a pré-busca DNS pode ajudar a economizar alguns milissegundos de tempo de carregamento da página.

## Amostras de código pré-busca DNS {#section_E886F7B2861E48BA9EF3D8B3CE32B345}

Os seguintes exemplos mostram como fazer chamadas de pré-busca DNS para soluções e serviços diferentes da [!DNL Experience Cloud]. Algumas chamadas de pré-busca exigem a ID da organização da [!DNL Adobe] ou as informações do servidor de rastreamento. Nesses exemplos, o código em *itálico* representa um espaço reservado de variável. Você pode substituir esse código pela sua ID de parceiro da [!DNL Adobe], pelo código do cliente ou pelas informações do servidor de rastreamento etc.

* **Analytics:** `<link rel="dns-prefetch" href="//insert tracking server name here">`.

   Adicione uma tag separada para cada nome DNS se você usar servidores de rastreamento protegidos e não protegidos.

* **Audience Manager:** `<link rel="dns-prefetch" href="//dpm.demdex.net">`

* **Serviço da Experience Cloud ID:**`<link rel="dns-prefetch" href="//fast. *`inserir ID do parceiro aqui`*.demdex.net">`

* **Gerenciador dinâmico de tags** (DTM): Não obrigatório. Os links de DTM estão disponíveis assim que a página é carregada.

* **Media Optimizer (Ad Cloud):**

   * `<link rel="dns-prefetch" href="//pixel.everesttech.net">`
   * `<link rel="dns-prefetch" href="//cm.everesttechnet">`


* **Target:** `<link rel="dns-prefetch" href="//insert customer code here.tt.omtrdc.net">`

>[!MORE_ LIKE_ THIS]
>
>* [Busca prévia no DNS](https://www.chromium.org/developers/design-documents/dns-prefetching)

