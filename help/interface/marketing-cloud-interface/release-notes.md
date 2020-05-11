---
description: Recursos, notas de versão e problemas conhecidos da interface da Experience Cloud.
keywords: core services
seo-description: Recursos, notas de versão e problemas conhecidos da interface da Experience Cloud.
seo-title: Notas de versão cumulativas
solution: Experience Cloud
title: Notas de versão cumulativas
uuid: fcff8cc6-e587-4bf2-9a75-261d4eabc7d4
translation-type: tm+mt
source-git-commit: 0bc7032d0052ba03beac1140dfbfd630e1802bfd
workflow-type: tm+mt
source-wordcount: '3809'
ht-degree: 68%

---


# Notas de versão cumulativas

Recursos, notas de versão e problemas conhecidos da interface da Experience Cloud.

Para obter uma lista de atualizações de documentação, consulte [Experience Cloud](../doc-updates.md#concept_4C8983FCD23848A4B1E4C2D99ED82784).

Para obter as notas de versão que abrangem todas as soluções, consulte Notas [de versão da](https://docs.adobe.com/content/help/pt-BR/release-notes/experience-cloud/current.html)Experience Cloud.

## Janeiro - 2020

* A página do Feed foi substituída em dezembro de 2019. Procure um aviso de desativação no produto. (MCUI-10039)

## Agosto - 2019

* Correção de um problema crítico no login da Experience Cloud que resultava no logout da sessão para alguns usuários. (MCUI-6908)
* Atualização do login da Experience Cloud para melhorar o desempenho e reduzir a latência. (MCUI-6854, MCUI-6869, MCUI-6883)
* Atualização da aparência da interface. (MCUI-6861, MCUI-6911, MCUI-6862)
* Correção de um problema com os [!UICONTROL Triggers] da Experience Cloud que resultava na interpretação incorreta da cláusula _Curtir_ na definição do [!UICONTROL Acionador]. (MCUI-6611)

## Abril - 2019

* Atualização do alternador de aplicativos para incluir o Marketing Cloud no conjunto de soluções da Experience Cloud e atualizações de marca na Experience Platform. (MCUI-6529)
* Página inicial da Experience Cloud atualizada para incluir links de navegação nas páginas Feed e Administração. (MCUI-6682)
* Correção de um problema na definição de [!UICONTROL Acionador] para um uso correto da cláusula “curtir”. (MCUI-6611)
* Melhorias nos atributos do cliente para melhor logon na Subscrição no serviço. (MCUI-6519)

## Versão 19.1.1 - 17 de janeiro de 2019

**Observação:** em março de 2019, a interface da Experience Cloud não será compatível com o Internet Explorer 11.

* Corrigido um problema que impedia que a pesquisa de ajuda retornasse os resultados. (MCUI-1670)
* O gerenciamento de eVar foi corrigido e aprimorado em Triggers. (MCUI-6400)

## Versão 16.5.1 - 26 de maio de 2016 {#section_3785F182BC13493F84903CA69EB6D0A8}

**Recursos e melhorias**

<table id="table_ABBCE1A66F534059BD728BC2B9AEFA80"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Recurso </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Configurações de produto pré-configuradas no Admin Console </p> </td> 
   <td colname="col2"> <p>Os administradores de clientes da Experience Cloud podem aproveitar as configurações de produto pré-criadas e mapeadas para grupos de permissões padrão do Analytics e do Gerenciamento dinâmico de tags. </p> <p>Essa otimização está disponível para organizações recentemente provisionadas e reduz a quantidade de tempo necessário para que as organizações gerenciem usuários no Admin Console. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Melhorias no feed </p> </td> 
   <td colname="col2"> <p> Ao criar uma nova publicação no Feed da Experience Cloud, a linha Para agora usa o tópico ativo no momento em vez de usar a organização por padrão.</p> </td> 
  </tr> 
 </tbody> 
</table>

**Correções**

* Corrigido um problema que evitava que miniaturas fossem exibidas em ativos compartilhados de Assets on Demand ao Feed da Experience Cloud. (MAC-29955)

## Versão 16.2 - 18 de fevereiro de 2016 {#section_D9610373116C4D77A38F67815C725EA3}

<table id="table_C9B288CF42034F329C3C72D95D22E515"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Recurso </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Melhorias nos ativos da Experience Cloud </p> </td> 
   <td colname="col2"> <p>No Experience Cloud Assets, você pode armazenar, compartilhar e sincronizar seus ativos digitais de um local central. O Experience Cloud Assets aproveita alguns dos recursos disponíveis no <span class="keyword">Adobe Experience Manager</span> (AEM). </p> <p>Consulte <a href="../experience-cloud-assets/experience-cloud-assets.md#concept_DDA5224C907D4A4F817D795DA0ED64D0" format="dita" scope="local">Experience Cloud</a></p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Melhorias na vinculação de contas </p> </td> 
   <td colname="col2"> <p>O fluxo de trabalho de interface foi aprimorado para vinculação de contas da solução com a Experience Cloud (Adobe ID). Esse novo fluxo de trabalho localiza todas as contas de usuário associadas a uma organização e permite que você escolha a qual conta vincular. Também simplificamos a experiência de vinculação de conta, para que você não precise mais acessar a página Gerenciar organizações para vincular contas manualmente. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Correções**

* Um problema que impedia a vinculação e o SSO para o Analytics foi corrigido. Esse problema exibia a mensagem &quot;Aviso: A mensagem de erro: ERRO IMS SSO Falha: Não é possível localizar a empresa vinculada.&quot;

**Problema conhecido**

If you access Dynamic Tag Management via the **[!UICONTROL Experience Cloud]** > **[!UICONTROL Activation]** interface, but your Dynamic Tag Management account is not linked to the Experience Cloud (Adobe ID), you will not be able to log in to Dynamic Tag Management. Para evitar esse problema, acesse diretamente [!DNL dtm.adobe.com] em uma nova guia do navegador.

## Versão 16.1 - 21 de janeiro de 2016 {#section_33B3F7DF6CA347E3AA93801BAC6232CE}

<table id="table_4223658257DA41C999AC710A10D26771"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Recurso </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> Mensagens da Biblioteca de Audiências </td> 
   <td colname="col2"> <p> Melhoramos a Biblioteca de público-alvo para incluir mensagens úteis ao criar públicos-alvo ou quando acontecer um tempo limite. </p> <p>Por exemplo, ao adicionar mais de cinco regras, uma mensagem é exibida indicando que você excedeu o máximo de regras permitido. (MAC-27376, MAC-27375) </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>a Microsoft [encerra o suporte](https://www.microsoft.com/en-us/WindowsForBusiness/End-of-IE-support) ao Internet Explorer 8, 9 e 10. Por esse motivo, nós deixaremos de corrigir problemas relatados nessas versões do Internet Explorer.

## Versão 15.10 - 14 de outubro de 2015 {#section_68123833D3634BD3A473C12862BF9606}

**Problemas conhecidos**

* Os clientes não conseguem fazer logon no Report Builder quando fazem SSO (logon único) no Analytics por meio da Experience Cloud. Esse problema não afeta os clientes que usam credenciais herdadas do Analytics.
* Problema conhecido na função “Vincular ao relatório” do Analytics. Os clientes que fazem logon no Analytics por meio da Experience Cloud são direcionados para uma página de logon não SSO do Analytics ao tentar compartilhar um relatório.

## Versão 15.9 - 10 de setembro de 2015 {#section_BCCE3E7DF62A4FF5A57B9C8FE2A5F37B}

* Correção de um problema de desempenho da API do Gerenciador de Audiências que causava tempos limite intermitentes ao carregar dados de Atributos do cliente. (MAC-26305)
* Correção de um problema que impedia os usuários de adicionar até 200 Atributos do cliente a uma subscrição. (MAC-26188)
* Corrigiu um problema da Biblioteca de público-alvo que evitou que o público-alvo compartilhasse da Segmentação de análise. Esse problema causou a exibição de “Dados de coleta” (0 públicos-alvo). Para evitar esse problema, a Adobe recomenda manter menos de 50 mil membros do público-alvo por segmento. (MAC-25788)
* Correção de um problema anterior dos atributos do cliente: a página Editar esquema causava o envio de um erro Sensível a conteúdo durante a alteração de um nome de exibição. (MAC-25589, AN-103834)

## Release 15.7 - July 22 2015 {#section_2683A152176944E48EF6C943892975B7}

* Correção de um problema que impedia que as descrições de atributos especificadas na página Visualização/Editar Schema (em Atributos do cliente) fossem atualizadas nos relatórios do Analytics. (MAC-25985)
* Correção de um problema que impedia a renderização de miniaturas em ativos que passaram por upload. (MAC-25863)
* Foi corrigido um problema que impedia a disponibilização de novos segmentos criados nos relatórios e análises da Experience Cloud Audiences. (MAC-25817)
* Correção de um problema que impedia o compartilhamento do público-alvo no Analytics quando o serviço de ID do visitante era usado. (MAC-25788, MAC-25747)
* Adicionado suporte para caracteres multibyte nos Atributos do cliente. (MAC-25552)

**Problema conhecido**

Um problema conhecido está causando a criação duplicada de contas geradas automaticamente no Audience Manager e vinculando-as automaticamente à identidade da Experience Cloud de um usuário. Esse problema ocorre ao tentar navegar para o Audience Manager antes de vincular as contas. A Adobe recomenda vincular suas contas do Audience Manager à Experience Cloud antes de navegar para o Audience Manager. (MAC-25640)

## Versão 15.6.1 - 11 de junho de 2015 {#section_AD2019F8D2F84C9EB2B0533FAACF7043}

Nenhuma informação disponível

## Versão 15.5.1 - 13 de maio de 2015 {#section_EF197410964E40D294D0D8024738CFBA}

<table id="table_14E7B35E06C84A258A21D09691B58354"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Recurso </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> </p> </td> 
   <td colname="col2"> <p>Os menus de navegação esquerdos foram atualizados e organizados para fornecer acesso a todos os serviços e soluções principais. As mudanças notáveis incluem: </p> 
    <ul id="ul_5BEBAB86B9234A239C4E2DAF8826D8E3"> 
     <li id="li_7FA9F64CE69144B8A8A92746BF40E5A1">The <span class="term"> Audience Library</span> and <span class="term"> Customer Attributes</span> menu selections are now located under <span class="term"> Audiences</span>. </li> 
     <li id="li_95D62A43AE6243DBB2A65EDB830D05C4">A seleção de menu <span class="term">Exchage </span>foi movida do menu suspenso Ajuda para o painel de navegação esquerdo. </li> 
     <li id="li_0443FD50C78446CD8AA27A4F272CAD31"> As <span class="term">soluções</span> do foram removidas. Agora, é possível iniciar todas as soluções na metade inferior do painel de navegação. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

* Correção de um problema que impedia a sincronização dos Atributos do cliente para alguns clientes.
* Correção de um problema que impedia a exibição da página [Documentação do produto do Adobe Target](https://docs.adobe.com/content/help/pt-BR/target/using/integrate/a4t/a4t.html) em japonês.
* Foi corrigido um problema que impedia o uso do texto em japonês nos comentários entre a [!DNL Creative Cloud] e a [!DNL Experience Cloud].

## Versão 15.4.1 - 8 de abril de 2015 {#section_75634120CC934B3381EDEA7F6F976F0A}

<table id="table_3A6FBAE36558425A803B078150862C92"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Recurso </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Melhorias na administração: </p> 
    <ul id="ul_7D5FCBEFA262435D865CA1018BFB792E"> 
     <li id="li_6E98974CCB094ABBAB57C51ED56C3F00"> <span class="wintitle"> Admin Console</span> </li> 
     <li id="li_8CDAB6301FD44C3999EE4EEB1A0A2FD6">Suporte para Enterprise ID e Federated ID </li> 
    </ul> </td> 
   <td colname="col2"> <p>A funcionalidade de gerenciamento de usuários e grupos foi transferida para o Admin Console. O novo caminho de navegação é: </p> <p> <span class="uicontrol"> Experience Cloud</span> &gt; <span class="uicontrol">Administração</span> &gt; <span class="uicontrol">Iniciar o Admin Console</span></p> <p> Além disso, foi incluído o suporte à Enterprise ID e às Federated ID. Você pode utilizar Enterprise ID, Federated ID e Adobe ID na mesma implantação corporativa. Por exemplo, utilize as Adobe IDs para usuários que podem usar outros produtos e serviços da Adobe. Use Enterprise ID ou Federated IDs para usuários nos quais você deseja gerenciar estritamente suas contas. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Correções**

* Correção de um problema que impedia o logon único entre o [!DNL Experience Cloud] e o [!DNL Media Optimizer].

**Problemas conhecidos**

* Vincular e desvincular a organização do Dynamic Tag Management com a Experience Cloud não funciona para as organizações recém-criadas na Experience Cloud. Estamos trabalhando para corrigir o problema e restaurar a funcionalidade normal na versão de maio. Em caso de problemas ao tentar efetuar o logon único no Dynamic Tag Management através da Experience Cloud, utilize o logon antigo em [!DNL dtm.adobe.com].
* Um problema conhecido impede que o público-alvo compartilhe conjuntos de relatórios que não são de propriedade da conta vinculada do Analytics. Estamos nos esforçando para solucionar os problemas

## Versão 15.3.2 - 19 de março de 2015 {#section_07760FD9CA43497FA8BDCCA990A24BFD}

<table id="table_54025DBE2D094FF1BE837BA60816C6DF"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Recurso </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Atributos do cliente </p> </td> 
   <td colname="col2"> <p>Se você capturar os dados de clientes de empresas em um banco de dados de gerenciamento de relacionamento com o cliente (CRM), poderá fazer upload dos dados em uma fonte de dados do atributo do cliente na Experience Cloud. Depois que os dados forem carregados, você poderá executar os relatórios <span class="uicontrol">Perfil do visitante</span> &gt; <span class="uicontrol">Atributos do cliente</span> no Analytics. </p> <p>Também é possível usar os dados carregados como um segmento do público-alvo no <span class="keyword">Adobe Target</span>. </p> <p>Consulte <a href="../attributes/attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1" format="dita" scope="local"> documentação do produto</a> Atributos do cliente. </p> <p> Para obter informações sobre como modernizar suas soluções para os, consulte <a href="../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C" format="dita" scope="local"> Ativar as soluções dos </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Versão 15.3.1 - 4 de março de 2015 {#section_57CB69C044DD47BDBC1A1BEC38957551}

<table id="table_EB3FFBA2DF904546A5185EC9A63BBA98"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Recurso </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Mapeamento de grupo </p> </td> 
   <td colname="col2"> <p>A página Gerenciamento de grupos foi reprojetada como uma interface administrativa que permite criar grupos, adicionar usuários a grupos e aplicar permissões nas soluções da Experience Cloud. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Mapeamento de um para muitos </p> </td> 
   <td colname="col2"> <p>Ao vincular contas da solução na Experience Cloud, se você tiver várias soluções e organizações, é possível mapear vários produtos e serviços para uma única organização. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Activation </p> </td> 
   <td colname="col2"> <p> <a href="../activation/activation.md#concept_EE756B6B0A0643DAB8CA3A00E665406C" format="dita" scope="local">Activation</a> agora é exibida na navegação à esquerda na <span class="keyword">Experience Cloud</span>. <span class="wintitle"> A Ativação</span> é um serviço da <span class="keyword"> Experience Cloud</span> que atualmente é composto pela tecnologia de gerenciamento dinâmico de tags e direciona você para lá quando clicado. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Atualizações de documentação - Principais serviços </p> </td> 
   <td colname="col2"> <p>Added the topic <a href="../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C" format="dita" scope="local"> Enable your solutions for core services</a> to assist you with implementing core services. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Versão 15.2.1 - 19 de fevereiro de 2015 {#section_BC694D5AE16A4E16B44B353ED67947F3}

Correções:

* O fluxo de trabalho do convite por email do usuário foi aprimorado para provisionamento de conta.
* Um problema da pasta de ativos, que impedia os ativos da [!DNL Experience Cloud] e do [!DNL Adobe Campaign] de exibir hierarquias idênticas de pastas, foi corrigido.
* Correção de um problema que impedia a exclusão de públicos-alvo que fizessem parte de atividades desativadas do [!DNL Target].
* Correção de um problema que impedia o ícone Adicionar (mais) de ser exibido em [!UICONTROL Regras] na página [!UICONTROL Criar um novo público-alvo].
* Aprimoramento do suporte à interface da Experience Cloud para o Internet Explorer 9.

## Release 15.1.1 - January 15 2015 {#section_F1A352E928AF432E94CC0A289C345184}

Novos recursos e correções na colaboração e interface de compartilhamento da [!DNL Adobe Experience Cloud].

<table id="table_AD0A8CA760E64227BB04BA6B0E425E80"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Recurso </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Acesso somente leitura. </p> </td> 
   <td colname="col2"> <p>Agora, os administradores podem conceder acesso somente leitura a usuários não administrativos. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Correções**

* Correção de um problema no qual os arquivos PNG não podiam ser renderizados em um cartão.
* Correção de um problema com o upload de arquivos para os Ativos da Experience Cloud por meio do arrastar e soltar.

**Problemas conhecidos**

* Os usuários não podem compartilhar arquivos PowerPoint em quadros.
* As alterações de grupo e de direito feitas no Gerenciamento de usuários só entram em vigor depois de um novo logon.
* Alguns usuários podem ter problemas quando fazem upload de arquivos grandes para os Ativos da Experience Cloud.
* Os usuários podem estar sem alguns links em seus cartões Experience Cloud do Media Optimizer.
* Alguns usuários administrativos podem enfrentar problemas quando vinculam suas contas depois de terem aceitado um convite para participarem da Experience Cloud.
* A interface da Experience Cloud pode ter seu desempenho reduzido se usada de modo paralelo por muitos usuários.
* Alguns usuários conseguem excluir um ativo antigo em vez de receberem uma notificação de erro.
* Alguns usuários podem enfrentar problemas ao fazer logon em dois navegadores com a mesma Adobe ID simultaneamente.
* Alguns usuários talvez não consigam adicionar novamente um usuário da Creative Cloud na pasta compartilhada se o usuário da Creative Cloud foi excluído.
* Alguns usuários podem perceber um atraso na notificação exibida quando uma pasta é compartilhada da Experience Cloud com a Creative Cloud.
* Alguns usuários podem enfrentar um problema ao compartilharem uma pasta entre a Experience Cloud e a Creative Cloud.
* Alguns usuários podem ter problemas para criar uma audiência em um conjunto de relatórios do Analytics depois que as audiências compartilhadas forem ativadas.
* Alguns usuários podem ter problemas para carregar ativos em um quadro.

## Versão 14.11.1 - 13 de novembro de 2014 {#section_A6CF1D4F27B9496892A89C983EB39102}

Problemas conhecidos:

* Alguns usuários conseguem excluir um ativo antigo em vez de receberem uma notificação de erro.
* Alguns arquivos [!DNL .png] não podem ser renderizados em um cartão.
* Alguns usuários podem ter problemas para carregar ativos em um quadro.
* Alterações de grupo e de direito realizadas no gerenciamento de usuários só têm efeito após um novo logon.
* Os administradores devem fazer logout e login novamente para ver as alterações feitas nas Configurações da conta.
* O usuário não pode compartilhar arquivos PowerPoint em quadros.
* A interface da [!DNL Experience Cloud] pode ter seu desempenho reduzido quando usada de modo paralelo por vários usuários.
* A sincronização do Adobe Experience Manager com a Creative Cloud não está funcionando.

## Versão 14.10.1 - 16 de outubro de 2014 {#section_E3A0F4423B814707AA3745E083500835}

Novos recursos e correções na colaboração e interface de compartilhamento da [!DNL Adobe Experience Cloud].

<table id="table_7C1ACE8108D54782AE128ACD35069DF5"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Recurso </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Editar permissões de usuário </p> </td> 
   <td colname="col2"> <p>Os proprietários de um quadro agora podem editar as permissões do usuário no quadro específico. </p> <p> 
     <ol id="ol_B12251C510744538AF9BCE60ACB04016"> 
      <li id="li_87B3EDE9542B47CEBE0BE7F2D1DE844D">No quadro, clique em <span class="uicontrol">Configurações</span>. </li> 
      <li id="li_0F4786B0E1E743069D082E7DC488A031">Ao lado de cada proprietário, especifique o <span class="uicontrol">Proprietário</span>, <span class="uicontrol">Visualizador</span> ou <span class="uicontrol">Editor</span>. </li> 
     </ol> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Correções**

* Criar um cartão a partir de um PDF e compartilhá-lo no quadro gerava uma mensagem de erro.

**Problemas conhecidos**

* Alguns usuários podem ter problemas para carregar ativos em um quadro.
* Alguns arquivos [!DNL .png] não podem ser renderizados em um cartão.
* Alterações de grupo e de direito realizadas no gerenciamento de usuários só têm efeito após um novo logon.
* É possível que alguns usuários não consigam criar um cartão a partir de um PDF e compartilhá-lo em um quadro.
* Alguns usuários conseguem excluir um ativo antigo em vez de receberem uma notificação de erro.
* O usuário não pode compartilhar arquivos PowerPoint em quadros.
* A interface da [!DNL Experience Cloud] pode ter seu desempenho reduzido quando usada de modo paralelo por vários usuários.
* A vinculação do [!DNL Search&Promote] não está disponível na página [!UICONTROL Organizations &amp; Product Access].

## Versão 14.9.1 - 18 de setembro de 2014 {#section_20F156A9CC2F4FC59C4970075C181D3A}

**Correções e melhorias**

* Ao entrar no [!DNL experiencecloud.adobe.com], você verá que a experiência de logon agora é compatível com o logon Creative Cloud da Adobe.
* Na página Gerenciar organizações, a experiência de vinculação (após o recebimento de um convite) agora é consistente para cada solução.

**Problemas conhecidos**

* Alterações de grupo e de direito realizadas no gerenciamento de usuários só têm efeito após um novo logon.
* É possível que alguns usuários não consigam criar um cartão a partir de um PDF e compartilhá-lo em um quadro.
* Alguns usuários podem ter problemas para carregar ativos em um quadro.
* Alguns usuários conseguem excluir um ativo antigo em vez de receberem uma notificação de erro.
* O usuário não pode compartilhar arquivos PowerPoint em quadros.
* Alguns arquivos [!DNL .png] não podem ser renderizados em um cartão.
* A interface da [!DNL Experience Cloud] pode ter seu desempenho reduzido quando usada de modo paralelo por vários usuários.
* A vinculação do [!DNL Search&Promote] não está disponível na página [!UICONTROL Organizations &amp; Product Access].
* É possível que os conteúdos [!DNL Creative Cloud] de alguns usuários sejam removidos da pasta se não estiverem compartilhados na [!DNL Experience Cloud].

## Versão 14.8.1 - 21 de agosto de 2014 {#section_03BF00F6A95A490C91BCC0A1988FA7AA}

Novos recursos e correções na colaboração e interface de compartilhamento da [!DNL Adobe Experience Cloud].

<table id="table_1E7DBEB5E83B4E4285B6FD1D718CD16D"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Recurso </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> </p> </td> 
   <td colname="col2"> <p>Agora você pode acessar os <span class="keyword">Adobe Mobile Services</span> no menu de navegação esquerdo. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Problemas conhecidos**

* Alterações de grupo e de direito realizadas no gerenciamento de usuários só têm efeito após um novo logon.
* É possível que alguns usuários não consigam criar um cartão a partir de um PDF e compartilhá-lo em um quadro.
* Alguns usuários podem ter problemas para carregar ativos em um quadro.
* É possível que alguns usuários não consigam fazer o logon do [!DNL Target] para a [!DNL Experience Cloud].
* Alguns usuários do Audience Manager não conseguem efetuar o logon na [!DNL Experience Cloud].
* Alguns usuários conseguem excluir um ativo antigo em vez de receberem uma notificação de erro.
* Os arquivos excluídos de [!DNL Experience Cloud] não estão sendo excluídos de [!DNL Digital Asset Management].
* O usuário não pode compartilhar arquivos PowerPoint em quadros.
* Alguns arquivos [!DNL .png] não podem ser renderizados em um cartão.
* A interface da [!DNL Experience Cloud] pode ter seu desempenho reduzido quando usada de modo paralelo por vários usuários.
* A vinculação do [!DNL Search&Promote] não está disponível na página [!UICONTROL Organizations &amp; Product Access].
* É possível que os conteúdos [!DNL Creative Cloud] de alguns usuários sejam removidos da pasta se não estiverem compartilhados na [!DNL Experience Cloud].

## Versão 14.7.1 - 24 de julho de 2014 {#section_B22D4F830756463DB27BB4D508D9ADD5}

Novos recursos e correções na colaboração e interface de compartilhamento da [!DNL Adobe Experience Cloud].

**Problemas conhecidos**

* Os arquivos excluídos de [!DNL Experience Cloud] não estão sendo excluídos de [!DNL Digital Asset Management].
* Alguns usuários do [!UICONTROL Exchange] podem ter seus nomes em forma de ID de sequência nos comentários em vez de seus nomes
* Alguns arquivos [!DNL .png] não podem ser renderizados em um cartão
* O carregamento de arquivos permite mais tipos de arquivos do que o método arrastar e soltar. Para obter melhores resultados, carregue usando [!UICONTROL Ativos].
* A vinculação do [!DNL Search&Promote] não está disponível na página [!UICONTROL Organizations &amp; Product Access].
* Usuários do [!DNL Exchange] devem limpar os cookies para melhorar o desempenho.
* A interface da [!DNL Experience Cloud] pode desacelerar caso seja usada de modo paralelo por muitos usuários.
* É possível que os conteúdos da [!DNL Creative Cloud] de alguns usuários sejam removidos da pasta caso não estejam compartilhados na [!DNL Experience Cloud].
* Sua sessão será encerrada após 15 minutos de inatividade. Além disso, encerrar a sessão em uma localização encerra a sua sessão da [!DNL Experience Cloud].
* Não será possível para alguns usuários vincular as contas do Audience Manager à [!DNL Experience Cloud].
* [!UICONTROL Os usuários do Exchange] só podem ver o inglês no seletor de idiomas.

**Correções**

Nenhum relatório.

## Versão 14.6.1 - 19 de junho de 2014 {#marketing_cloud_interface}

Novos recursos e correções na colaboração e interface de compartilhamento da [!DNL Adobe Experience Cloud].

**Melhoria**

<table id="table_C9BD63436BF0414B97B8D07387D1993B"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Recurso </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>  Botão <span class="wintitle">Salvar</span> nos Públicos-alvo </p> </td> 
   <td colname="col2"> <p>Ao criar um público-alvo, o botão <span class="wintitle">Salvar</span> da página <span class="wintitle">Criar novo público-alvo</span> será desabilitado até que os campos obrigatórios sejam preenchidos. 
     <!--MAC-19712 --></p> </td> 
  </tr> 
 </tbody> 
</table>

**Problemas conhecidos**

* Os arquivos excluídos de [!DNL Experience Cloud] não estão sendo excluídos de [!DNL Digital Asset Management].
* O carregamento de arquivos permite mais tipos de arquivos do que o método arrastar e soltar. Para obter melhores resultados, carregue usando Ativos.
* A vinculação do [!DNL Search&Promote] não está disponível na página [!UICONTROL Organizations &amp; Product Access].
* Os filtros aplicados aos relatórios de tendências do [!DNL Analytics] não se aplicam aos cartões na [!DNL Experience Cloud].
* Para alguns usuários, não é possível vincular a conta de gerenciamento de público-alvo à conta da [!DNL Experience Cloud].
* Sua sessão será encerrada após 15 minutos de inatividade. Além disso, encerrar a sessão em um local encerrá a sessão da Experience Cloud.
* Alguns usuários do Exchange podem ter seus nomes em forma de ID de sequência nos comentários em vez de seus nomes

**Correções**

* Correção de um problema que impedia o upload de vídeo em aplicativos.

## Versão 14.5.1 - 22 de maio de 2014 {#section_7E22B2CB3ABA4D6EAED8CA8EFDE5433E}

<table id="table_4E4B34EEE3D94D78BA1A1FBC62950559"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Recurso </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Experience Cloud Exchange </p> </td> 
   <td colname="col2"> <p> <span class="uicontrol"> Experience Cloud</span> &gt; <span class="uicontrol">Ajuda</span> &gt; <span class="uicontrol">Exchange</span></p> <p>O <span class="keyword">Experience Cloud</span><span class="wintitle">Exchange</span> é o único local onde você pode pesquisar, navegar, selecionar, pagar e baixar extensões de marketing digital através de aplicativos. </p> <p>Os aplicativos incluem Data Connectors, configurações personalizadas para o produto principal da Adobe, aplicativos de terceiros, relatórios e cartões da <span class="keyword">Experience Cloud</span>. </p> <p>Consulte <a href="../exchange.md#concept_E07F16F070544B82B56527A845C41D59" format="dita" scope="local"> Exchange Marketplace</a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Públicos-alvo da Experience Cloud </p> </td> 
   <td colname="col2"> <p> <span class="uicontrol"> Experience Cloud</span> &gt; <span class="uicontrol">Públicos-alvo</span></p> <p> <span class="wintitle">Públicos-alvo</span> é onde você pode criar, editar, gerenciar públicos-alvo de forma semelhante ao trabalho com segmentos. Por exemplo, você pode criar um segmento em relatórios e análises e, em seguida, compartilhá-lo nos <span class="wintitle">Públicos-alvo</span> da <span class="wintitle">Experience Cloud</span>. Depois de compartilhado, o público-alvo é disponibilizado no <span class="keyword">Adobe Target</span> para atividades de campanha e no Adobe Audience Manager para segmentação. </p> <p> <p>Observação: para solicitar a ativação no Target, visite <a href="https://www.adobe.com/go/audiences" format="http" scope="external">https://www.adobe.com/go/audiences</a>. </p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> </p> </td> 
   <td colname="col2"> <p>Os usuários que são mencionados nos cartões da <span class="keyword">Experience Cloud</span> agora têm permissões para esse cartão. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> </p> </td> 
   <td colname="col2"> <p>Os novos usuários da Adobe podem vincular suas contas do Scene7 à Adobe ID, bem como os membros da equipe. Os administradores também podem desvincular usuários de contas Scene7. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Sincronização de ativos. </p> </td> 
   <td colname="col2"> <p> Você pode compartilhar ativos no Adobe Experience Manager (AEM) Assets com a Adobe Experience Cloud e a Adobe Creative Cloud, de modo que quaisquer alterações nesses ativos sejam refletidas nas cópias compartilhadas dos ativos na Adobe Experience Cloud e na Adobe Creative Cloud. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Correções**

* A [!DNL Experience Cloud] não era vinculada ao [!DNL Adobe Target]. Esse problema ocorria se o login do [!DNL Adobe Target] pudesse ser usado em vários servidores do [!DNL Target].
* O [!DNL Adobe Media Optimizer] não criava automaticamente usuários quando eles eram criados na [!DNL Experience Cloud].
* As opções em caixas de combinação usadas para adicionar novos usuários temporariamente desapareceram durante a digitação.
* O link Comentários na visualização do cartão de ativos não era clicável.
* Após adicionar uma tag personalizada a um ativo, nenhuma outra alteração nos metadados persistiu.
* Ao deletar uma imagem, os Ativos não avisam se a imagem está sendo usada no Adobe Target Essentials.
* Desaceleração do desempenho da interface da [!UICONTROL Experience Cloud] quando usada em paralelo por muitos usuários.
* A exclusão de uma imagem no [!UICONTROL Experience Cloud Assets] não emitia um aviso se a imagem fosse usada no [!DNL Adobe Target Essentials].
* Quando a opção **[!UICONTROL Lembre-se de mim]** não estava selecionada durante o logon, o usuário era desconectado após 15 minutos.
* Os usuários deviam efetuar o logout e o logon novamente para que todas as permissões e alterações de direito tivessem efeito.
* Fazer logon na [!DNL Experience Cloud] demorava mais de um segundo.
* Para certos usuários, a exclusão dos arquivos do [!DNL Experience Cloud] não está sincronizando com [!DNL Digital Asset Management].
* Os usuários estavam sendo desconectados após apenas 15 minutos de inatividade do navegador.
* O usuário não pôde compartilhar arquivos PowerPoint em quadros.
* Alguns usuários apresentavam um layout visual ruim no Internet Explorer 10 em comparação a outros navegadores.

## Release 14.4.1 - April 22 2014 {#section_E2A699764E744D2E8D418E9A3D40AF6B}

<table id="table_D95C0DC64F2A4B47BAC83E504CFD6825"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Recurso </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Criar cartões a partir de tópicos de ajuda </p> </td> 
   <td colname="col2"> <p>Depois de ativar o recurso Compartilhar na Adobe Experience Cloud na barra de favoritos do seu navegador, você pode compartilhar páginas de ajuda do URL do microsite. </p> <p> <b>Para compartilhar um tópico de ajuda</b> </p> 
    <ol id="ol_F94B816121494B0FA16CC07B0E96AED8"> 
     <li id="li_F47187D4B5FE46D3A51D257DD569B4D6"> <p>Na <span class="keyword">Experience Cloud</span>, clique em <span class="uicontrol">Administração</span>. </p> </li> 
     <li id="li_94EF58E7A4974B63951E14F72A710183"> <p>Arraste o botão <span class="uicontrol">Compartilhar para a Adobe Experience Cloud</span> até a barra de marcadores. </p> </li> 
     <li id="li_69EEC4F25D8F4AD7AA106A10B7F50FF6"> <p>Navegue até uma página de ajuda (ou continue nessa), e então clique em <span class="uicontrol">Compartilhar para a Adobe Experience Cloud</span> na barra de marcadores do seu navegador. </p> <p>Essa etapa cria um cartão, que pode ser visto na <span class="wintitle">Experience Cloud</span>. </p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

**Correções**

* Após adicionar uma tag personalizada a um ativo, nenhuma outra alteração de metadados pode ser persistida.
* Os usuários precisam atualizar o quadro para que os cartões excluídos desapareçam da visualização.
* Quando a opção **[!UICONTROL Lembre-se de mim]** não está selecionada durante o logon, o usuário é desconectado após 15 minutos
* A página de aterrissagem de soluções [!DNL Analytics] exibe erros de formatação.
* Os usuários devem efetuar o logout e o logon novamente para que todas as permissões e alterações de direito tenham efeito.
* Ao deletar uma imagem, os [!UICONTROL Ativos] não avisam se a imagem está sendo usada no [!DNL Adobe Target Essentials].
* O link Comentários na visualização do cartão de ativos não é clicável.
* As opções para adicionar temporariamente novos usuários nas caixas de combo desaparecem enquanto você estiver digitando.
* Fazer logon na [!DNL Experience Cloud] demora mais de um segundo.
* Dados compartilhados pelo [!DNL Media Optimizer] são mal representados na [!DNL Experience Cloud].
* O Adobe [!DNL Media Optimizer] não cria usuários automaticamente quando o usuário foi criado na [!DNL Experience Cloud].
* A [!DNL Experience Cloud] não pode ser vinculada ao [!DNL Adobe Target] caso o logon do [!DNL Adobe Target] seja utilizado em vários servidores do [!DNL Target].
* A interface da [!DNL Experience Cloud] pode desacelerar caso seja usada de modo paralelo por muitos usuários.
* A vinculação do [!DNL Search&Promote] não está disponível na página [!UICONTROL Organizations &amp; Product Access].
* Os cartões de simulação do [!DNL Adobe Media Optimizer] não estão sendo renderizados corretamente.
* Os filtros aplicados aos relatórios de tendências do [!DNL Analytics] não se aplicam aos cartões na [!DNL Experience Cloud].
* Os filtros aplicados aos relatórios de tendências do Analytics não se aplicam aos cartões na Experience Cloud.
* Alguns arquivos Excel ou CSV não podem ser carregados para um quadro.
* Não será possível para alguns usuários vincular a conta de gerenciamento de público-alvo à [!DNL Experience Cloud].
* Um erro é exibido para alguns usuários ao compartilharem segmentos [!DNL Analytics] na [!DNL Experience Cloud].
* Não será possível para alguns usuários detalhar as subpastas no [!UICONTROL Seletor de ativo].
* Não será possível para alguns usuários compartilhar os gadgets AdLens na [!DNL Experience Cloud].

## Versão 14.3.1 - 13 de março de 2014 {#section_5D142E3225E3477A84DC01B8197D39BC}

A versão 14.3.1 é uma versão de manutenção com foco na agilidade, na estabilidade e na segurança. Não inclui novos recursos importantes.

**Correções**

* Foi adicionada a capacidade de remover a imagem do avatar.
* Correção de um problema que impedia a desvinculação das contas do [!DNL Adobe Media Optimizer].

**Problemas conhecidos**

* A exclusão de uma imagem nos Ativos da Experience Cloud não avisa se a imagem é usada no Adobe Público alvo Essentials.
* Atualizar um cartão do [!DNL Analytics] pode, às vezes, levar a um gráfico vazio no cartão expandido.
* Os usuários devem efetuar o logout e o logon novamente para que todas as permissões e alterações de direito tenham efeito.
* Quando *`Remember me`* não for selecionado durante o logon, a sessão do usuário será encerrada após 15 minutos.
* A página de aterrissagem de soluções [!DNL Analytics] exibe erros de formatação.
* O link Comentários não é clicável na exibição do cartão de ativos.
* A interface da Experience Cloud pode ficar lenta quando usada em paralelo por muitos usuários
* A Experience Cloud não pode ser vinculada ao [!DNL Adobe Target] caso o logon do [!DNL Adobe Target] seja utilizado em vários servidores do Target.
* Fazer logon na Experience Cloud demora mais de um segundo.
* Após adicionar uma tag personalizada a um ativo, nenhuma outra alteração de metadados pode ser persistida.
* O [!DNL Adobe Media Optimizer] não cria automaticamente usuários quando o usuário foi criado na Experience Cloud.
* As opções para adicionar temporariamente novos usuários nas caixas de combo desaparecem enquanto você estiver digitando.
* Dados compartilhados a partir do [!DNL Media Optimizer] são mal representados na Experience Cloud.
* Falha ao compartilhar imagens do Flickr.
* Os filtros aplicados aos relatórios de tendências do [!DNL Analytics] não se aplicam aos cartões na Experience Cloud.
* Alterações de grupo e de direito realizadas no gerenciamento de usuários só têm efeito após um novo logon.
* A vinculação do [!DNL Search&Promote] não está disponível em [!UICONTROL Organizations &amp; Product Access].
* O usuário precisa atualizar o quadro para que os cartões excluídos desapareçam da visualização.
* Alguns arquivos Excel ou CSV não podem ser carregados para um quadro.
* Os cartões de simulação do [!DNL Adobe Media Optimizer] não estão sendo renderizados corretamente.
* Alguns arquivos PNG não podem ser renderizados em um cartão.
* O feedback beta não pode ser enviado.

## Release 14.2.1 - February 24 2014 {#section_5AD81B0737C843AFB4BE9C4420D70EB3}

<table id="table_DFAB002358C94A17A7F91DAB323A488F"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Recurso </th> 
   <th colname="col2" class="entry"> Descrição </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>OEmbed </p> </td> 
   <td colname="col2"> <p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Atualizar dados </p> </td> 
   <td colname="col2"> <p> 
     <!--MAC-18174-->O ícone <span class="uicontrol">Atualizar dados</span> de um gráfico em um cartão agora está oculto, se a solução não permite atualização de dados. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Correções**

* Corrigido um problema que evitava que relatórios do [!DNL Analytics] compartilhados aplicassem filtros de segmento.
* Corrigido um problema que fazia com que as soluções fossem exibidas na página de [!UICONTROL Soluções da Experience Cloud] como vinculadas, mesmo se as contas de solução não estivessem vinculadas.
* Corrigido um problema que evitava que os clientes [!DNL Adobe Target] na Ásia pudessem clicar o botão **[!UICONTROL Seguir para a Experience Cloud]** na página de vinculação.
* Corrigido um problema que não permitia o compartilhamento de vídeos do YouTube.
