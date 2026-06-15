---
description: Saiba como as soluções e os serviços da Adobe CX Enterprise usam cookies.
title: Como os cookies são usados na Experience Cloud
uuid: 4255a13a-917b-4b5f-a7d4-4b2e7521d189
exl-id: 60f1a89e-d989-461b-a6a3-c1df022cd30b
TQID: https://experienceleague.adobe.com/GH5WHcI9440NKYpUzizHlhOMlBSf-Y0WQ5GDBaSvqNI
product_v2:
  - id: e1971122-7081-4556-9222-8a31bd71800c
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: d3cdead0-685a-4489-9250-4bb709942f66
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 50012e2564e88e1a6e16578e3331136c7df0cb21
workflow-type: tm+mt
source-wordcount: 624
ht-degree: 8%

---

# Como os cookies são usados no CX Enterprise

O Adobe CX Enterprise usa cookies. Um cookie é um pequeno pedaço de dados que um site envia para o seu navegador, que o armazena para uso posterior. Os cookies ajudam o site a lembrar de coisas quando você visita novamente ou se move entre páginas. Os cookies ajudam a rastrear visitas e diferenciar um dispositivo de outro.

As leis geralmente exigem que você obtenha permissão antes de armazenar ou usar cookies no dispositivo de alguém. A Adobe recomenda consultar sua equipe jurídica para entender as regras aplicáveis.

## Sobre cookies próprios

O Adobe CX Enterprise usa cookies para rastrear informações que não duram entre exibições de página ou sessões do navegador. Quando possível, o Adobe usa cookies primários (vinculados ao seu próprio site). Para rastrear a atividade em vários sites ou domínios pertencentes a você, são necessários cookies de terceiros.

Alguns navegadores e ferramentas antisspyware bloqueiam cookies de terceiros. O Adobe tem maneiras de garantir que os cookies ainda funcionem mesmo que estejam bloqueados. O funcionamento depende do uso do Experience Platform Identity Service (ECID) ou de cookies mais antigos do Analytics (como o cookie `s_vi`):

* [CX Enterprise Identity Service](https://experienceleague.adobe.com/pt-br/docs/id-service/using/intro/overview): o ECID Service sempre define cookies próprios, quer o domínio de coleção corresponda ao domínio do site. Ele usa o JavaScript para colocar o cookie no domínio do site.

* [Identificadores herdados do Analytics](analytics.md) (como o cookie `s_vi`): a definição de cookies próprios ou de terceiros depende da sua configuração:

   * Se o servidor de coleção de dados corresponder ao domínio do site, os cookies são primários.
   * Se não corresponder, os cookies são de terceiros. Se cookies de terceiros estiverem bloqueados, o Adobe definirá um cookie de fallback (`s_fid`) em vez do habitual.

Para garantir que o servidor de coleção corresponda ao domínio do site, você pode usar uma **configuração de CNAME**. Isso envolve a atualização das configurações de DNS para apontar um domínio personalizado (seu) para os servidores da Adobe. Isso faz com que o cookie de rastreamento apareça como primário. Embora um CNAME possa funcionar em vários domínios, qualquer domínio que não corresponda ao CNAME ainda definirá cookies de terceiros.

>[!NOTE]
>
>A Prevenção de rastreamento inteligente (ITP) da Apple limita a duração dos cookies primários da Adobe, mesmo que o domínio de coleção corresponda ao domínio do site. O ITP afeta o Safari no macOS e todos os navegadores no iOS e iPadOS. Desde novembro de 2020, os cookies definidos com o CNAME expiram tão rapidamente quanto os definidos com o JavaScript. Este prazo pode ser alterado no futuro.

Esta é uma versão simplificada do texto:

## Cookies e privacidade

A Adobe leva a privacidade e a segurança dos dados muito a sério. Ele trabalha com organizações de privacidade, reguladores e programas como o AdChoices para fornecer às pessoas controle sobre como seus dados são usados.

A maioria dos cookies do Adobe CX Enterprise não armazena informações pessoais. Eles são seguros e usados apenas pela sua empresa para relatórios, conteúdo e anúncios. A Adobe não compartilha esses dados com outros clientes ou terceiros, exceto em relatórios anônimos em todo o setor (como Relatórios do Digital Marketing Insight).

A Adobe não combina dados de navegador em empresas diferentes. Para proteger a privacidade, algumas ferramentas do Adobe permitem que cada site use seu próprio conjunto de cookies. Alguns também permitem usar seu próprio domínio para cookies, tornando-os primários e mais seguros.

Os cookies só podem armazenar informações que foram salvas neles anteriormente. Eles não podem executar código ou ler outros dados em seu dispositivo. Além disso, os navegadores da Web só permitem que os cookies sejam lidos pelo site que os definiu. Por exemplo, somente Adobe.com pode ler cookies que ele define.

O diagrama a seguir ilustra o uso de cookies em uma solicitação de imagem padrão:

![Uso de cookies para uma solicitação de imagem padrão](assets/CookiesProcessGraphic-01.png)

O diagrama a seguir ilustra o uso de cookies em uma solicitação de imagem direta (usada em cenários nos quais um arquivo JS não é carregado):

![Uso de cookies para uma solicitação de imagem direta](assets/CookiesProcessGraphic2.png)

