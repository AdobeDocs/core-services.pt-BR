---
description: '"Recursos, notas de versão e problemas conhecidos mais recentes dos serviços da Experience Cloud, como atributos do cliente, públicos e gerenciamento de usuários."'
keywords: principais serviços
solution: Experience Cloud
title: 'Notas de versão cumulativas '
uuid: fcff8cc6-e587-4bf2-9a75-261d4eabc7d4
feature: '"Atributos do cliente, Biblioteca de público-alvo, Admin Console"'
topic: Administração
role: Administrador
level: Experiente
translation-type: ht
source-git-commit: 61d60273e933c637dfe4400da78257e1c80015b3
workflow-type: ht
source-wordcount: '3973'
ht-degree: 100%

---


# Notas de versão cumulativas

Recursos, notas de versão e problemas conhecidos da interface da Experience Cloud.

Para obter uma lista de atualizações de documentação, consulte [Experience Cloud](../doc-updates.md#concept_4C8983FCD23848A4B1E4C2D99ED82784).

Para obter as notas de versão que abrangem todas as soluções, consulte [Notas de versão da Experience Cloud](https://docs.adobe.com/content/help/pt-BR/release-notes/experience-cloud/current.html).

## Agosto - 2020

| Recurso | Descrição |
| -----------| ---------- |
| Ferramenta administrativa - políticas | Esta página exibe a lista completa das políticas da Experience Cloud na sua organização. Ela fornece informações sobre produtos, instâncias, usuários e desenvolvedores. Pesquise, classifique e filtre exibições personalizadas da lista de políticas. Consulte a ajuda da [Ferramenta de administração da Experience Cloud](../admin-getting-started/admin-tool-experience-cloud.md) para obter detalhes. |

## Abril - 2020

* A página do [!UICONTROL Feed] da Experience Cloud foi substituída. (EXC-8505)
* A página de logon da Experience Cloud foi atualizada para refletir os novos elementos de marca. (EXC-10747)

## Fevereiro - 2020

| Recurso | Descrição |
| -----------| ---------- |
| Ferramenta de administração - exibir detalhes do usuário | Os administradores podem exibir uma lista classificável e filtrável de todos os usuários da Experience Cloud e seus detalhes na nova Ferramenta de administração. Os detalhes do usuário incluem o acesso ao produto, as funções e as últimas informações acessadas de um usuário. Consulte a ajuda da [Ferramenta de administração da Experience Cloud](../admin-getting-started/admin-tool-experience-cloud.md) para obter detalhes. |

**Correções**

* **Atributos do cliente:** a interface do usuário de atributos do cliente agora exibe status adicionais de perfis sincronizados no Target. (MCUI-10231)
* **Triggers de serviços principais:** devido à falta de uso, a pontuação de propensão &quot;Probabilidade de retorno em 30 dias&quot; ao criar um acionador do tipo Abandono foi removida. (MCUI-10056)

## Janeiro - 2020

* A página Feed foi desativada em dezembro de 2019. Procure um aviso de desativação no produto. (MCUI-10039)

## Agosto - 2019

* Correção de um problema crítico no login da Experience Cloud que resultava no logout da sessão para alguns usuários. (MCUI-6908)
* Atualização do login da Experience Cloud para melhorar o desempenho e reduzir a latência. (MCUI-6854, MCUI-6869, MCUI-6883)
* Atualização da aparência da interface. (MCUI-6861, MCUI-6911, MCUI-6862)
* Correção de um problema com os [!UICONTROL Triggers] da Experience Cloud que resultava na interpretação incorreta da cláusula _Curtir_ na definição do [!UICONTROL Acionador]. (MCUI-6611)

## Abril - 2019

* Atualização do alternador de aplicativo para incluir o Marketo no conjunto de soluções da Experience Cloud, além de atualizações de marca na plataforma do Experience. (MCUI-6529)
* Atualização da tela inicial da Experience Cloud para incluir links de navegação ao Feed e páginas de administração. (MCUI-6682)
* Correção de um problema na definição de [!UICONTROL Acionador] para um uso correto da cláusula “curtir”. (MCUI-6611)
* Melhorias nos atributos do cliente para um melhor logon no serviço de assinatura. (MCUI-6519)

## Versão 19.1.1 - 17 de janeiro de 2019

**Observação:** em março de 2019, a interface da Experience Cloud não será compatível com o Internet Explorer 11.

* Correção de um problema que impedia que a pesquisa na ajuda exibisse resultados. (MCUI-1670)
* Correção e melhora do gerenciamento eVar em Triggers. (MCUI-6400)

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
   <td colname="col1"> <p>Pré-configurações de produto no Admin Console </p> </td> 
   <td colname="col2"> <p>Os administradores de clientes da Experience Cloud podem aproveitar as configurações de produto pré-criadas e mapeadas a grupos de permissões padrão para o Analytics e Dynamic Tag Management. </p> <p>Essa otimização está disponível para organizações recentemente provisionadas e reduz a quantidade de tempo exigido por organizações para gerenciar usuários no Admin Console. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Melhorias no feed </p> </td> 
   <td colname="col2"> <p> Ao criar uma nova publicação no Feed da Experience Cloud, a linha Para agora usa o tópico ativo no momento como padrão, em vez de usar a organização.</p> </td> 
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
   <td colname="col1"> <p>Aprimoramentos no Experience Cloud Assets </p> </td> 
   <td colname="col2"> <p>No Experience Cloud Assets, você pode armazenar, compartilhar e sincronizar seus ativos digitais de um local central. O Experience Cloud Assets aproveita alguns dos recursos disponíveis no <span class="keyword">Adobe Experience Manager</span> (AEM). </p> <p>Consulte <a href="../experience-cloud-assets/experience-cloud-assets.md#concept_DDA5224C907D4A4F817D795DA0ED64D0" format="dita" scope="local">Experience Cloud</a></p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Melhorias na vinculação de contas </p> </td> 
   <td colname="col2"> <p>O fluxo de trabalho de interface foi aprimorado para vinculação de contas da solução com a Experience Cloud (Adobe ID). Esse novo fluxo de trabalho localiza todas as contas de usuário associadas a uma organização e permite que você escolha a qual conta vincular. Também simplificamos a experiência de vinculação de conta, para que você não precise mais acessar a página Gerenciar organizações para vincular contas manualmente. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Correções**

* Um problema que impedia a vinculação e o SSO para o Analytics foi corrigido. Esse problema exibia a mensagem &quot;Aviso: falha na mensagem de erro: ERRO IMS SSO: não é possível localizar a empresa vinculada.&quot;

**Problema conhecido**

Se você acessar o Dynamic Tag Management por meio da interface **[!UICONTROL Experience Cloud]** > **[!UICONTROL Activation]**, mas a conta do Dynamic Tag Management não estiver vinculada à Experience Cloud (Adobe ID), não será possível fazer logon no Dynamic Tag Management. Para evitar esse problema, acesse diretamente [!DNL dtm.adobe.com] em uma nova guia do navegador.

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
   <td colname="col1"> Mensagens da Biblioteca de públicos-alvo </td> 
   <td colname="col2"> <p> Melhoramos a Biblioteca de público-alvo para incluir mensagens úteis ao criar públicos-alvo ou quando acontecer um tempo limite. </p> <p>Por exemplo, ao adicionar mais de cinco regras, uma mensagem é exibida indicando que você excedeu o máximo de regras permitido. (MAC-27376, MAC-27375) </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>a Microsoft [encerra o suporte](https://www.microsoft.com/pt-br/WindowsForBusiness/End-of-IE-support) ao Internet Explorer 8, 9 e 10. Por esse motivo, nós deixaremos de corrigir problemas relatados nessas versões do Internet Explorer.

## Versão 15.10 - 14 de outubro de 2015 {#section_68123833D3634BD3A473C12862BF9606}

**Problemas conhecidos**

* Os clientes não conseguem fazer logon no Report Builder quando fazem SSO (logon único) no Analytics por meio da Experience Cloud. Esse problema não afeta os clientes que usam as credenciais mais antigas do Analytics.
* Problema conhecido na função “Vincular ao relatório” do Analytics. Os clientes que estão fazendo logon no Analytics por meio da Experience Cloud são direcionados a uma página sem logon único (SSO) do Analytics quando tentam compartilhar um relatório.

## Versão 15.9 - 10 de setembro de 2015 {#section_BCCE3E7DF62A4FF5A57B9C8FE2A5F37B}

* Correção de um problema de desempenho na API do Audience Manager que causava tempos limite intermitentes durante o upload dos dados de atributos do cliente. (MAC-26305)
* Correção de um problema que impedia os usuários de adicionarem até 200 atributos de cliente a uma assinatura. (MAC-26188)
* Corrigiu um problema da Biblioteca de público-alvo que evitou que o público-alvo compartilhasse da Segmentação de análise. Esse problema causou a exibição de “Dados de coleta” (0 públicos-alvo). Para evitar esse problema, a Adobe recomenda manter menos de 50 mil membros do público-alvo por segmento. (MAC-25788)
* Correção de um problema anterior dos atributos do cliente: a página Editar esquema causava o envio de um erro Sensível a conteúdo durante a alteração de um nome de exibição. (MAC-25589, AN-103834)

## Versão 15.7 - 22 de julho de 2015 {#section_2683A152176944E48EF6C943892975B7}

* Correção de um erro que evitou que as descrições de atributos especificadas na página Exibir/Editar esquema (nos atributos do cliente) fossem atualizadas nos Relatórios de análise. (MAC-25985)
* Correção de um problema que impedia a renderização de miniaturas em ativos que passaram por upload. (MAC-25863)
* Foi corrigido um problema que impedia a disponibilização de novos segmentos criados nos relatórios e análises da Experience Cloud Audiences. (MAC-25817)
* Correção de um problema que impedia o compartilhamento do público-alvo no Analytics quando o serviço de ID do visitante era usado. (MAC-25788, MAC-25747)
* Foi adicionado suporte para caracteres multibyte nos atributos do cliente. (MAC-25552)

**Problema conhecido**

Um problema conhecido está causando a criação duplicada de contas geradas automaticamente no Audience Manager e vinculando-as automaticamente à identidade da Experience Cloud de um usuário. Esse problema ocorre ao tentar navegar para o Audience Manager antes de vincular as contas. A Adobe recomenda vincular suas contas do Audience Manager à Experience Cloud antes de navegar para o Audience Manager. (MAC-25640)

## Versão 15.6.1 - 11 de junho de 2015 {#section_AD2019F8D2F84C9EB2B0533FAACF7043}

Nenhuma informação disponível.

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
   <td colname="col2"> <p>Os menus de navegação à esquerda foram atualizados e organizados para fornecer acesso a todos os serviços e soluções principais. As mudanças notáveis incluem: </p> 
    <ul id="ul_5BEBAB86B9234A239C4E2DAF8826D8E3"> 
     <li id="li_7FA9F64CE69144B8A8A92746BF40E5A1">As seleções de menu <span class="term">Biblioteca de públicos-alvo</span> e <span class="term">Atributos do cliente</span> agora estão localizadas em <span class="term">Públicos-alvo</span>. </li> 
     <li id="li_95D62A43AE6243DBB2A65EDB830D05C4">A seleção de menu <span class="term">Exchage </span>foi movida do menu suspenso Ajuda para o painel de navegação esquerdo. </li> 
     <li id="li_0443FD50C78446CD8AA27A4F272CAD31"> As <span class="term">soluções</span> do foram removidas. Agora, é possível iniciar todas as soluções na metade inferior do painel de navegação. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

* Correção de um problema que impedia a sincronização dos atributos do cliente para alguns clientes.
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
   <td colname="col2"> <p>A funcionalidade de gerenciamento de usuários e grupos foi transferida para o Admin Console. O novo caminho de navegação é: </p> <p> <span class="uicontrol"> Experience Cloud</span> &gt; <span class="uicontrol">Administração</span> &gt; <span class="uicontrol">Iniciar o Admin Console</span></p> <p> Além disso, foi incluído o suporte à Enterprise ID e às Federated ID. Você pode utilizar Enterprise ID, Federated ID e Adobe ID na mesma implantação corporativa. Por exemplo, utilize as Adobe IDs para usuários que podem usar outros produtos e serviços da Adobe. Use Enterprise ID ou Federated IDs para usuários nos quais você deseja gerenciar estritamente as contas. </p> </td> 
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
   <td colname="col2"> <p>A página Gerenciamento de grupo foi reprojetada como uma interface administrativa que permite criar grupos, adicionar usuários aos grupos e aplicar permissões nas soluções da Experience Cloud. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Mapeamento de um para muitos </p> </td> 
   <td colname="col2"> <p>Caso tenha várias soluções e empresas, poderá mapear vários produtos e serviços para uma única empresa ao vincular contas da solução na Experience Cloud. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Activation </p> </td> 
   <td colname="col2"> <p> <a href="../activation/activation.md#concept_EE756B6B0A0643DAB8CA3A00E665406C" format="dita" scope="local">Activation</a> agora é exibida na navegação à esquerda na <span class="keyword">Experience Cloud</span>. <span class="wintitle"> Activation</span> é um serviço da <span class="keyword"> Experience Cloud</span> e atualmente é composto pela tecnologia do Dynamic Tag Management, que direciona você ao clicar. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Atualizações de documentação - Serviços principais </p> </td> 
   <td colname="col2"> <p>Adição do tópico <a href="../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C" format="dita" scope="local"> Ativar as soluções dos serviços principais</a> para auxiliar com a implementação dos serviços principais. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Versão 15.2.1 - 19 de fevereiro de 2015 {#section_BC694D5AE16A4E16B44B353ED67947F3}

Correções:

* Melhoria do fluxo de trabalho de convite por email do usuário para provisionamento de conta.
* Um problema da pasta de ativos, que impedia os ativos da [!DNL Experience Cloud] e do [!DNL Adobe Campaign] de exibir hierarquias idênticas de pastas, foi corrigido.
* Correção de um problema que impedia a exclusão de públicos-alvo que fizessem parte de atividades desativadas do [!DNL Target].
* Correção de um problema que impedia o ícone Adicionar (mais) de ser exibido em [!UICONTROL Regras] na página [!UICONTROL Criar um novo público-alvo].
* Aprimoramento do suporte à interface da Experience Cloud para o Internet Explorer 9.

## Versão 15.1.1 - 15 de janeiro de 2015 {#section_F1A352E928AF432E94CC0A289C345184}

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
   <td colname="col2"> <p>Agora, os administradores podem conceder acesso de somente leitura a usuários não administrativos. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Correções**

* Correção de um problema em que os arquivos PNG não podiam ser renderizados em um cartão.
* Correção de um problema com o carregamento de arquivos para o Experience Cloud Assets por meio do arrastar e soltar.

**Problemas conhecidos**

* Os usuários não podem compartilhar arquivos PowerPoint em quadros.
* As alterações de grupo e de direito realizadas no Gerenciamento de usuários só têm efeito após um novo logon.
* Alguns usuários podem ter problemas quando fazem upload de arquivos grandes para os Ativos da Experience Cloud.
* Os usuários podem estar sem alguns links em seus cartões Experience Cloud do Media Optimizer.
* Alguns usuários administrativos podem enfrentar problemas quando vinculam suas contas depois de terem aceitado um convite para participarem da Experience Cloud.
* A interface da Experience Cloud pode ter seu desempenho reduzido se usada de modo paralelo por muitos usuários.
* Alguns usuários conseguem excluir um ativo antigo em vez de receberem uma notificação de erro.
* Alguns usuários podem enfrentar problemas ao fazer logon em dois navegadores com a mesma Adobe ID simultaneamente.
* Alguns usuários talvez não consigam adicionar novamente um usuário da Creative Cloud na pasta compartilhada se o usuário da Creative Cloud foi excluído.
* Alguns usuários podem perceber um atraso na notificação exibida quando uma pasta é compartilhada da Experience Cloud com a Creative Cloud.
* Alguns usuários podem enfrentar um problema ao compartilharem uma pasta entre a Experience Cloud e a Creative Cloud.
* Alguns usuários podem ter problemas ao criar um público-alvo em um conjunto de relatórios do Analytics depois que os públicos-alvo compartilhados forem ativados.
* Alguns usuários podem ter problemas ao carregar ativos em um quadro.

## Versão 14.11.1 - 13 de novembro de 2014 {#section_A6CF1D4F27B9496892A89C983EB39102}

Problemas conhecidos:

* Alguns usuários conseguem excluir um ativo antigo em vez de receberem uma notificação de erro.
* Alguns arquivos [!DNL .png] não podem ser renderizados em um cartão.
* Alguns usuários podem ter problemas ao carregar ativos em um quadro.
* Alterações de grupo e de direito realizadas no gerenciamento de usuários só têm efeito após um novo logon.
* Os administradores precisam fazer logoff e então, fazer logon novamente para ver alterações feitas nas Configurações da conta.
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
   <td colname="col2"> <p>Os proprietários de um quadro agora podem editar as permissões do usuário no determinado quadro. </p> <p> 
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

* Alguns usuários podem ter problemas ao carregar ativos em um quadro.
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
* Alguns usuários podem ter problemas ao carregar ativos em um quadro.
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
* Alguns usuários podem ter problemas ao carregar ativos em um quadro.
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
* Alguns usuários do [!UICONTROL Exchange] podem ter seus nomes em forma de ID de sequência nos comentários em vez de seus nomes.
* Alguns arquivos [!DNL .png] não podem ser renderizados em um cartão.
* O carregamento de arquivos permite mais tipos de arquivos do que o método arrastar e soltar. Para obter melhores resultados, carregue usando o [!UICONTROL Assets].
* A vinculação do [!DNL Search&Promote] não está disponível na página [!UICONTROL Organizations &amp; Product Access].
* Usuários do [!DNL Exchange] devem limpar os cookies para melhorar o desempenho.
* A interface da [!DNL Experience Cloud] pode desacelerar caso seja usada de modo paralelo por muitos usuários.
* É possível que os conteúdos da [!DNL Creative Cloud] de alguns usuários sejam removidos da pasta caso não estejam compartilhados na [!DNL Experience Cloud].
* Sua sessão será encerrada após 15 minutos de inatividade. Além disso, encerrar a sessão em uma localização encerra a sua sessão da [!DNL Experience Cloud].
* Não será possível para alguns usuários vincular as contas do Audience Manager à [!DNL Experience Cloud].
* Os usuários do [!UICONTROL Exchange] só veem inglês no seletor de idiomas.

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
   <td colname="col1"> <p> Botão <span class="wintitle">Salvar</span> nos Públicos-alvo </p> </td> 
   <td colname="col2"> <p>Ao criar um público-alvo, o botão <span class="wintitle">Salvar</span> da página <span class="wintitle">Criar novo público-alvo</span> será desabilitado até que os campos obrigatórios sejam preenchidos. 
     <!--MAC-19712 --></p> </td> 
  </tr> 
 </tbody> 
</table>

**Problemas conhecidos**

* Os arquivos excluídos de [!DNL Experience Cloud] não estão sendo excluídos de [!DNL Digital Asset Management].
* O carregamento de arquivos permite mais tipos de arquivos do que o método arrastar e soltar. Para obter melhores resultados, carregue usando o Assets.
* A vinculação do [!DNL Search&Promote] não está disponível na página [!UICONTROL Organizations &amp; Product Access].
* Os filtros aplicados aos relatórios de tendências do [!DNL Analytics] não se aplicam aos cartões na [!DNL Experience Cloud].
* Para alguns usuários, não é possível vincular a conta de gerenciamento de público-alvo à conta da [!DNL Experience Cloud].
* Sua sessão será encerrada após 15 minutos de inatividade. Além disso, encerrar a sessão em uma localização encerra a sessão na Experience Cloud.
* Alguns usuários do Exchange podem ter seus nomes em forma de ID de sequência nos comentários em vez de seus nomes.

**Correções**

* Correção de um problema que impedia o carregamento de vídeos em aplicativos.

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
   <td colname="col2"> <p>Os novos usuários da Adobe podem vincular suas contas do Scene7 à Adobe ID, bem como os membros da equipe. Os administradores também podem desvincular usuários de contas do Scene7. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Sincronização de ativos. </p> </td> 
   <td colname="col2"> <p> Compartilhe ativos no Adobe Experience Manager (AEM) Assets com a Adobe Experience Cloud e a Adobe Creative Cloud, de modo que as alterações nesses ativos sejam refletidas nas cópias compartilhadas dos ativos na Adobe Experience Cloud e na Adobe Creative Cloud. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Correções**

* A [!DNL Experience Cloud] não era vinculada ao [!DNL Adobe Target]. Esse problema ocorria se o login do [!DNL Adobe Target] pudesse ser usado em vários servidores do [!DNL Target].
* O [!DNL Adobe Media Optimizer] não criava automaticamente usuários quando eles eram criados na [!DNL Experience Cloud].
* As opções usadas para adicionar temporariamente novos usuários nas caixas de combo desaparecem enquanto você estiver digitando.
* O link Comentários não era clicável na exibição do cartão de ativos.
* Após adicionar uma tag personalizada a um ativo, nenhuma outra alteração nos metadados persiste.
* Ao deletar uma imagem, os Ativos não avisam se a imagem está sendo usada no Adobe Target Essentials.
* Desaceleração do desempenho da interface da [!UICONTROL Experience Cloud] quando usada em paralelo por muitos usuários.
* A exclusão de uma imagem no [!UICONTROL Experience Cloud Assets] não emitia um aviso se a imagem fosse usada no [!DNL Adobe Target Essentials].
* Quando a opção **[!UICONTROL Lembre-se de mim]** não estava selecionada durante o logon, o usuário era desconectado após 15 minutos.
* Os usuários deviam efetuar o logout e o logon novamente para que todas as permissões e alterações de direito tivessem efeito.
* Fazer logon na [!DNL Experience Cloud] demorava mais de um segundo.
* Para certos usuários, a exclusão dos arquivos do [!DNL Experience Cloud] não está sincronizando com [!DNL Digital Asset Management].
* Os usuários estavam sendo desconectados após apenas 15 minutos de inatividade do navegador.
* O usuário não podia compartilhar arquivos PowerPoint em quadros.
* Alguns usuários apresentavam um layout de exibição ruim no Internet Explorer 10 em comparação a outros navegadores.

## Versão 14.4.1 - 22 de abril de 2014 {#section_E2A699764E744D2E8D418E9A3D40AF6B}

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
   <td colname="col2"> <p>Depois de ativar o recurso Compartilhar na Adobe Experience Cloud na barra de favoritos do navegador, você pode compartilhar páginas de ajuda do URL do microsite. </p> <p> <b>Para compartilhar um tópico de ajuda</b> </p> 
    <ol id="ol_F94B816121494B0FA16CC07B0E96AED8"> 
     <li id="li_F47187D4B5FE46D3A51D257DD569B4D6"> <p>Na <span class="keyword">Experience Cloud</span>, clique em <span class="uicontrol">Administração</span>. </p> </li> 
     <li id="li_94EF58E7A4974B63951E14F72A710183"> <p>Arraste o botão <span class="uicontrol">Compartilhar para a Adobe Experience Cloud</span> até a barra de marcadores. </p> </li> 
     <li id="li_69EEC4F25D8F4AD7AA106A10B7F50FF6"> <p>Navegue até uma página de ajuda (ou continue nessa), e então clique em <span class="uicontrol">Compartilhar para a Adobe Experience Cloud</span> na barra de marcadores do seu navegador. </p> <p>Essa etapa cria um cartão, que pode ser visto na <span class="wintitle">Experience Cloud</span>. </p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

**Correções**

* Após adicionar uma tag personalizada a um ativo, nenhuma outra alteração nos metadados pode ser persistente.
* Os usuários precisam atualizar o quadro para que os cartões excluídos desapareçam da exibição.
* Quando a opção **[!UICONTROL Lembre-se de mim]** não está selecionada durante o logon, o usuário é desconectado após 15 minutos.
* A página de aterrissagem de soluções [!DNL Analytics] exibe erros de formatação.
* Os usuários devem efetuar o logout e o logon novamente para que todas as permissões e alterações de direito tenham efeito.
* Ao deletar uma imagem, os [!UICONTROL Ativos] não avisam se a imagem está sendo usada no [!DNL Adobe Target Essentials].
* O link Comentários não é clicável na exibição do cartão de ativos.
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

* Adição da capacidade de remover a imagem do avatar.
* Correção de um problema que impedia a desvinculação das contas do [!DNL Adobe Media Optimizer].

**Problemas conhecidos**

* Ao excluir uma imagem no Experience Cloud Assets não avisa se a imagem está sendo usada no Adobe Target Essentials.
* Atualizar um cartão do [!DNL Analytics] pode, às vezes, levar a um gráfico vazio no cartão expandido.
* Os usuários devem efetuar o logout e o logon novamente para que todas as permissões e alterações de direito tenham efeito.
* Quando *`Remember me`* não for selecionado durante o logon, a sessão do usuário será encerrada após 15 minutos.
* A página de aterrissagem de soluções [!DNL Analytics] exibe erros de formatação.
* O link Comentários não é clicável na exibição do cartão de ativos.
* A interface da Experience Cloud pode ficar lenta caso seja usada de modo paralelo por muitos usuários.
* A Experience Cloud não pode ser vinculada ao [!DNL Adobe Target] caso o logon do [!DNL Adobe Target] seja utilizado em vários servidores do Target.
* Fazer logon na Experience Cloud demora mais de um segundo.
* Após adicionar uma tag personalizada a um ativo, nenhuma outra alteração nos metadados pode ser persistente.
* O [!DNL Adobe Media Optimizer] não cria automaticamente usuários quando o usuário foi criado na Experience Cloud.
* As opções para adicionar temporariamente novos usuários nas caixas de combo desaparecem enquanto você estiver digitando.
* Dados compartilhados a partir do [!DNL Media Optimizer] são mal representados na Experience Cloud.
* Falha ao compartilhar imagens do Flickr.
* Os filtros aplicados aos relatórios de tendências do [!DNL Analytics] não se aplicam aos cartões na Experience Cloud.
* Alterações de grupo e de direito realizadas no gerenciamento de usuários só têm efeito após um novo logon.
* A vinculação do [!DNL Search&Promote] não está disponível em [!UICONTROL Organizations &amp; Product Access].
* O usuário precisa atualizar o quadro para que os cartões excluídos desapareçam da exibição.
* Alguns arquivos Excel ou CSV não podem ser carregados para um quadro.
* Os cartões de simulação do [!DNL Adobe Media Optimizer] não estão sendo renderizados corretamente.
* Alguns arquivos PNG não podem ser renderizados em um cartão.
* O feedback beta não pode ser enviado.

## Versão 14.2.1 - 24 de fevereiro de 2014 {#section_5AD81B0737C843AFB4BE9C4420D70EB3}

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
