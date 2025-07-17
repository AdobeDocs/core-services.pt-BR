---
description: Saiba como as soluções e os serviços da Adobe Experience Cloud usam cookies.
title: Como os cookies são usados no Experience Cloud
uuid: 4255a13a-917b-4b5f-a7d4-4b2e7521d189
exl-id: 60f1a89e-d989-461b-a6a3-c1df022cd30b
source-git-commit: d6dc659104b3b24b60495cd97adb21ebb3962fc7
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 10%

---

# Cookies usados no Experience Cloud

O Adobe Experience Cloud usa cookies. Um cookie é um pequeno pedaço de dados que um site envia para o seu navegador, que o armazena para uso posterior. Os cookies ajudam o site a lembrar de coisas quando você visita novamente ou se move entre páginas. Os cookies ajudam a rastrear visitas e diferenciar um dispositivo de outro.

As leis geralmente exigem que você obtenha permissão antes de armazenar ou usar cookies no dispositivo de alguém. A Adobe recomenda consultar sua equipe jurídica para entender as regras aplicáveis.

## Sobre cookies próprios

O Adobe Experience Cloud usa cookies para rastrear informações que não duram entre exibições de página ou sessões do navegador. Quando possível, o Adobe usa cookies primários (vinculados ao seu próprio site). Para rastrear a atividade em vários sites ou domínios pertencentes a você, são necessários cookies de terceiros.

Alguns navegadores e ferramentas antisspyware bloqueiam cookies de terceiros. O Adobe tem maneiras de garantir que os cookies ainda funcionem mesmo que estejam bloqueados. O funcionamento depende do uso do Experience Platform Identity Service (ECID) ou de cookies mais antigos do Analytics (como o cookie `s_vi`):

* [Experience Cloud Identity Service](https://experienceleague.adobe.com/pt-br/docs/id-service/using/intro/overview): o ECID Service sempre define cookies próprios, quer o domínio de coleção corresponda ao domínio do site. Ele usa o JavaScript para colocar o cookie no domínio do site.

* [Identificadores herdados do Analytics](analytics.md) (como o cookie `s_vi`): a definição de cookies próprios ou de terceiros depende da sua configuração:

   * Se o servidor de coleção de dados corresponder ao domínio do site, os cookies são primários.
   * Se não corresponder, os cookies são de terceiros. Se cookies de terceiros estiverem bloqueados, o Adobe definirá um cookie de fallback (`s_fid`) em vez do habitual.

Para garantir que o servidor de coleção corresponda ao domínio do site, você pode usar uma **configuração de CNAME**. Isso envolve a atualização das configurações de DNS para apontar um domínio personalizado (seu) para os servidores da Adobe. Isso faz com que o cookie de rastreamento apareça como primário. Embora um CNAME possa funcionar em vários domínios, qualquer domínio que não corresponda ao CNAME ainda definirá cookies de terceiros.

>[!NOTE]
>
>A Prevenção de rastreamento inteligente (ITP) da Apple limita a duração dos cookies primários da Adobe, mesmo que o domínio de coleção corresponda ao domínio do site. O ITP afeta o Safari no macOS e todos os navegadores no iOS e iPadOS. Desde novembro de 2020, os cookies definidos com o CNAME expiram tão rapidamente quanto os definidos com o JavaScript. Este prazo pode ser alterado no futuro.

Esta é uma versão simplificada do texto:

## Cookies e privacidade

A Adobe leva a privacidade e a segurança dos dados muito a sério. Ele trabalha com organizações de privacidade, reguladores e programas como AdChoices para fornecer às pessoas controle sobre como seus dados são usados.

A maioria dos cookies da Adobe Experience Cloud não armazena informações pessoais. Eles são seguros e usados apenas pela sua empresa para relatórios, conteúdo e anúncios. A Adobe não compartilha esses dados com outros clientes ou terceiros, exceto em relatórios anônimos em todo o setor (como Relatórios do Digital Marketing Insight).

A Adobe não combina dados de navegador em empresas diferentes. Para proteger a privacidade, algumas ferramentas do Adobe permitem que cada site use seu próprio conjunto de cookies. Alguns também permitem usar seu próprio domínio para cookies, tornando-os primários e mais seguros.

Os cookies só podem armazenar informações que foram salvas neles anteriormente. Eles não podem executar código ou ler outros dados em seu dispositivo. Além disso, os navegadores da Web só permitem que os cookies sejam lidos pelo site que os definiu. Por exemplo, somente Adobe.com pode ler cookies que ele define.

O diagrama a seguir ilustra o uso de cookies em uma solicitação de imagem padrão:

![Uso de cookies para uma solicitação de imagem padrão](assets/CookiesProcessGraphic-01.png)

O diagrama a seguir ilustra o uso de cookies em uma solicitação de imagem direta (usada em cenários nos quais um arquivo JS não é carregado):

![Uso de cookies para uma solicitação de imagem direta](assets/CookiesProcessGraphic2.png)
