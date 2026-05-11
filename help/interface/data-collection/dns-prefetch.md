---
description: Saiba como implementar a pré-busca de DNS para ajudar a reduzir os tempos de carregamento de página de diferentes aplicativos e serviços no CX Enterprise.
solution: Experience Cloud
title: Usar pré-busca DNS
uuid: 4220e223-e00e-46b1-8bde-52248913bea1
topic: Administration
role: Admin
level: Experienced
exl-id: caf2ff76-2076-436d-a5a7-aff531464480
TQID: 'https://experienceleague.adobe.com/uTXtbHEccwB-Nog-AJ282p59hHCppAsAyg5pgNRreR4'
product_v2: id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2: id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2: id:id:
role_v2: id:
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: f01d85af42b8f2c27dbada8f73546bc6fe4bf710
workflow-type: tm+mt
source-wordcount: 350
ht-degree: 77%

---

# Usar pré-busca de DNS

Implemente a pré-busca de DNS para ajudar a reduzir os tempos de carregamento de página de diferentes aplicativos e serviços.

## Noções básicas da pré-busca DNS

Os navegadores usam a pré-busca DNS para resolver automaticamente os nomes de domínio vinculados em uma página da Web aos endereços IP correspondentes. O processo de pré-busca é inciado quando o navegador carrega uma página da Web. Como exemplo, considere que sua página contém um link que pode ser selecionado para `www.adobe.com`. Quando um navegador carrega essa página, ele usa o _sistema DNS_ para buscar o nome do domínio vinculado e resolvê-lo em um endereço IP numérico correspondente. A pré-busca DNS ajuda a melhorar o desempenho da página porque o nome do domínio já está resolvido a um endereço IP antes que um visitante do site clique nesse link ou botão. O processo de pré-busca DNS é transparente para os usuários.

## Pré-busca DNS e aplicativos corporativos do Adobe CX

A pré-busca de DNS funciona automaticamente com links estáticos e incorporados em uma página. Isso também significa que a pré-busca de DNS automática não funciona com diferentes aplicativos e serviços do [!UICONTROL CX Enterprise] porque:

* Cada aplicativo ou serviço corporativo CX gera chamadas DNS dinamicamente à medida que a página é carregada.
* O navegador não pode resolver nomes de domínio para o endereço IP antes que essas chamadas sejam feitas.

No entanto, você pode implementar a pré-busca de DNS manualmente com os aplicativos corporativos do CX. Para isso, adicione a tag HTML `<dns-prefetch>` à seção `<head>` do código da página, como mostrado abaixo. Quando implementado adequadamente, a pré-busca DNS pode ajudar a economizar alguns milissegundos de tempo de carregamento da página.

## Amostras de código de pré-busca DNS

Os seguintes exemplos mostram como fazer chamadas de pré-busca de DNS para diferentes aplicativos e serviços da [!DNL CX Enterprise]. Algumas chamadas de pré-busca exigem a ID da organização da [!DNL Adobe] ou as informações do servidor de rastreamento. Nesses exemplos, o código em *itálico* representa um espaço reservado de variável. Você pode substituir esse código pela sua ID de parceiro do [!DNL Adobe], pelo código do cliente, pelas informações do servidor de rastreamento e assim por diante.

* **Analytics:** `<link rel="dns-prefetch" href="//data.example.com">`.

  Adicione uma tag separada para cada nome DNS se você usar servidores de rastreamento protegidos e não protegidos.

* **Audience Manager:** `<link rel="dns-prefetch" href="//dpm.demdex.net">`

* **Serviço CX Enterprise ID:** `<link rel="dns-prefetch" href="//fast.examplepartnerid.demdex.net">`

* **Advertising Cloud:**

   * `<link rel="dns-prefetch" href="//pixel.everesttech.net">`
   * `<link rel="dns-prefetch" href="//cm.everesttech.net">`

* **[!DNL Target]:** `<link rel="dns-prefetch" href="//example.tt.omtrdc.net">`

>[!MORELIKETHIS]
>
>* [Pré-busca DNS](https://www.chromium.org/developers/design-documents/dns-prefetching) no Chromium

