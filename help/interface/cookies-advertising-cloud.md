---
description: Saiba mais sobre os cookies da Adobe Ad Cloud para mapear eventos de envolvimento de anúncios em eventos de conversão e, potencialmente, usar essas informações para otimizar ofertas de anúncios.
title: 'Cookies da Advertising Cloud  '
uuid: 2eec48a3-3e81-488e-8e30-5fd62885de0b
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 6818edea-31b1-49fc-bca2-32828c7ca78d
source-git-commit: 854a2b298db4fab3339e2b2ea03701dc6511af8d
workflow-type: ht
source-wordcount: '569'
ht-degree: 100%

---

# Cookies da Advertising Cloud {#advertising-cloud-cookies}

A Advertising Cloud usa cookies para mapear eventos de envolvimento de anúncios a eventos de conversão e, possivelmente, para usar essas informações para otimizar ofertas de anúncios.

>[!NOTE]
>
>A tag beta do JavaScript Advertising Cloud que usa o [Adobe Experience Cloud ID (ECID) Service](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html?lang=pt-BR) cria [cookies próprios s_ecid da Experience Cloud](cookies-first-party.md), não cookies da Advertising Cloud.

## Nome do cookie: _lcc

<table id="table_821F8EBE91F244CBA72B0975B961B908"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Atributo </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Informações armazenadas </p> </td> 
   <td colname="col2"> <p>IDs e carimbos de data e hora (no formato aaaammdd) dos cliques de exibição</p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Expiração </p> </td> 
   <td colname="col2"> <p>15 minutos</p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Uso </p> </td> 
   <td colname="col2"> <p>Um cookie de terceiros usado para determinar se um evento de cliques em um anúncio de exibição se aplica a uma ocorrência do Adobe Analytics </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Localização </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Tamanho </p> </td> 
   <td colname="col2"> <p>52 bytes </p> </td> 
  </tr> 
 </tbody> 
</table>

## Nome do cookie: _tmae

<table id="table_28C2B62595E240D5A3C3E0BE147748C1"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Atributo </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Informações armazenadas </p> </td> 
   <td colname="col2"> <p>IDs codificadas e carimbos de data e hora para envolvimento de anúncios usando o rastreamento DSP da Advertising Cloud </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Expiração </p> </td> 
   <td colname="col2"> <p>1 ano </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Uso </p> </td> 
   <td colname="col2"> <p>Um cookie de terceiros que armazena os envolvimentos do usuário com anúncios, como "último anúncio xyz123 visto em 30 de junho de 2016" </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Localização </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Tamanho </p> </td> 
   <td colname="col2"> <p>Variável; os dados são codificados e geralmente menos que 1 KB </p> </td> 
  </tr> 
 </tbody> 
</table>

## Nome do cookie: adcloud

<table id="table_D7CD238736BC4571883F92F47673F57C"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Atributo </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Informações armazenadas </p> </td> 
   <td colname="col2"> <p>Os carimbos de data e hora da última visita ao site do anunciante e o último clique de pesquisa, e a ef_id criada quando o usuário clicou em um anúncio</p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Expiração </p> </td> 
   <td colname="col2"> <p>Os cookies definidos em 24 de fevereiro de 2021 ou antes expiram após 730 dias. Os cookies definidos em 25 de fevereiro de 2021 ou depois expiram após 364 dias.</p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Uso </p> </td> 
   <td colname="col2"> <p>Um cookie próprio que associa a ID do surfer aos segmentos e conversões relevantes do público-alvo </p> <p> As informações sobre a última visita são usadas para otimizar os tempos de carregamento da página, evitando solicitações desnecessárias para os servidores da Adobe. </p> <p>As informações sobre o último clique de pesquisa ajudam a determinar se um evento de conversão foi o resultado de um clique ou de uma visualização (conversão resultante de impressões, mas sem cliques). </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Localização </p> </td> 
   <td colname="col2"> <p>O domínio de nível superior do anunciante (como example.com) </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Tamanho </p> </td> 
   <td colname="col2"> <p>Variável, mas normalmente entre 50 e 150 bytes </p> </td> 
  </tr> 
 </tbody> 
</table>

## Nome do cookie: ev_sync_*

(ev_sync_ax, ev_sync_bk, ev_sync_dd, ev_sync_fs, ev_sync_ix, ev_sync_nx, ev_sync_ox, ev_sync_pm, ev_sync_rc, ev_sync_tm, ev_sync_yh)

<table id="table_A05C02AB261946E0AABAD78259392D81"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Atributo </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Informações armazenadas </p> </td> 
   <td colname="col2"> <p>A data em que a sincronização será realizada, no formato aaaammdd </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Expiração </p> </td> 
   <td colname="col2"> <p>A data em que a sincronização será realizada, no formato aaaammdd </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Uso </p> </td> 
   <td colname="col2"> <p>Um cookie de terceiros específico da troca de anúncios que sincroniza a ID do surfer da Advertising Cloud, com a troca de anúncios do parceiro. Ele é criado para novos surfers e envia uma solicitação de sincronização quando expira. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Localização </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Tamanho </p> </td> 
   <td colname="col2"> <p>8 caracteres </p> </td> 
  </tr> 
 </tbody> 
</table>

## Nome do cookie: everest_g_v2

<table id="table_04043292A43B41B69EAF17AF4E217C69"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Atributo </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Informações armazenadas </p> </td> 
   <td colname="col2"> <p>O navegador e a ID do surfer </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Expiração </p> </td> 
   <td colname="col2"> <p>2 anos </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Uso </p> </td> 
   <td colname="col2"> <p>Criada depois que um usuário clica inicialmente em um anúncio do cliente e usada para mapear os cliques atuais e subsequentes com outros eventos no site do cliente </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Localização </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Tamanho </p> </td> 
   <td colname="col2"> <p>~27 caracteres </p> </td> 
  </tr> 
 </tbody> 
</table>

## Nome do cookie: everest_session_v2

<table id="table_1A3AE4CA71304ADB943CB1F64BE695F5"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Atributo </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Informações armazenadas </p> </td> 
   <td colname="col2"> <p>A ID da sessão </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Expiração </p> </td> 
   <td colname="col2"> <p>Quando o navegador é fechado </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Uso </p> </td> 
   <td colname="col2"> <p>Um cookie de terceiros da sessão do navegador; um cookie é usado para todas as contas </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Localização </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Tamanho </p> </td> 
   <td colname="col2"> <p>~16 caracteres </p> </td> 
  </tr> 
 </tbody> 
</table>

## Nome do cookie: ev_tm

<table id="table_6C4D9DCFA4BF4FB2BD445E027550955F"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Atributo </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Informações armazenadas </p> </td> 
   <td colname="col2"> <p>ID da Advertising Cloud DSP (Demand Side Platform) </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Expiração </p> </td> 
   <td colname="col2"> <p>2 anos </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Uso </p> </td> 
   <td colname="col2"> <p>Um cookie de terceiros que armazena a DSP ID que corresponde à ID do surfer no cookie everest_g_v2 </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Localização </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Tamanho </p> </td> 
   <td colname="col2"> <p>~20 bytes </p> </td> 
  </tr> 
 </tbody> 
</table>

## Nome do cookie: id_adcloud

<table> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Atributo </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Informações armazenadas </p> </td> 
   <td colname="col2"> <p>A ID do surfer </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Expiração </p> </td> 
   <td colname="col2"> <p>91 dias </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Uso </p> </td> 
   <td colname="col2"> <p>O cookie é definido no domínio próprio, mas ainda não é usado </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Localização </p> </td> 
   <td colname="col2"> <p>O domínio de nível superior do anunciante (como example.com) </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Tamanho </p> </td> 
   <td colname="col2"> <p>16 bytes </p> </td> 
  </tr> 
 </tbody> 
</table>
