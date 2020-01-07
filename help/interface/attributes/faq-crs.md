---
description: Perguntas frequentes e práticas recomendadas para atributos do cliente no Analytics e no Target.
keywords: customer attributes
seo-description: Perguntas frequentes e práticas recomendadas para atributos do cliente no Analytics e no Target.
seo-title: Perguntas frequentes, limitações e práticas recomendadas
solution: Experience Cloud
title: Perguntas frequentes, limitações e práticas recomendadas
uuid: e93eb531-23c7-4d75-92e8-75699f58546a
translation-type: tm+mt
source-git-commit: 12c3ac8bfa64b7c8708312576ac6dc4036c1b7d8

---


# Perguntas frequentes, limitações e práticas recomendadas

Perguntas frequentes e práticas recomendadas para atributos do cliente no Analytics e no Target.

## Práticas recomendadas e limitações {#section_7F5189B3DAA84EE6865B91D2026EE05A}

Orientações e limitações ao usar os Atributos do cliente.

| Problema | Descrição |
|--- |--- |
| Limitações de assinatura de atributo do cliente | Quando você atualiza para o Analytics Premium, há um atraso de 24 horas antes de os atributos adicionais estarem disponibilizados. Você pode observar um erro Máximo de assinatura de atributo emitido durante esse atraso. |
| Vários logons no mesmo dispositivo | Ao usar os atributos do cliente para fazer upload dos perfis do cliente em uma fonte de dados, a Adobe recomenda que os usuários compartilhem o mesmo dispositivo (ou seja, a mesma Experience Cloud ID). Isso pode fazer com que o serviço ECID, que persiste no dispositivo, vincule vários usuários na mesma Experience Cloud ID, resultando em resultados inesperados [!DNL Target]. **** Observação: Para o Mobile, o ECID é permanente depois que o aplicativo Mobile é instalado e você deve reinstalar o aplicativo para gerar um novo ECID. Para Web, um novo ECID é gerado depois que o cookie do navegador é limpo. |
| Limitação diária de carregamento de frequência | A Adobe recomenda que você atualize os atributos do cliente apenas uma vez por dia. Aguarde pelo menos 24 horas para carregar outro arquivo de dados de perfil do cliente para o mesmo conjunto de perfis. |
| Custom Analytics ID (`s.visitorID`) | Definir uma ID do cliente usando `s.visitorID` é um método para identificar usuários no Analytics. No entanto, as integrações nas quais os dados do Analytics são exportados ou importados usando o Serviço de ID não funcionarão quando um visitante for identificado usando `s.visitorID.`<br>Isso inclui, mas não está limitado a, públicos-alvo compartilhados, Analytics for Target (A4T) e Atributos do cliente.<br>Para essas integrações, não há suporte para uma ID personalizada do Analytics. |
| Limitações de caracteres no Analytics | Ao criar uma assinatura do Analytics, o tamanho do campo dos arquivos enviados por upload é truncado até 255. |

## Perguntas frequentes sobre atributos do cliente {#section_E47866EEA83348E09FE43CEC5E44C461}

<table id="table_88631069013B408EBB0A810657662B36"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Pergunta </th> 
   <th colname="col2" class="entry"> Resposta </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>É possível receber notificações sobre o status do upload para atributos do cliente? </p> </td> 
   <td colname="col2"> <p>Sim. Consulte <a href="../admin-getting-started/organizations.md#concept_0105453AD71847B8BFCAF4A40915F157" format="dita" scope="local">Gerenciar notificações</a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> O que devo fazer para começar a usar os atributos do cliente? </p> </td> 
   <td colname="col2"> 
    <ol id="ol_1FACEF0990B6486B8DE86245D17695A8"> 
     <li id="li_F0C1542853684F8591FDC1B441D31A56"> <p>Ser provisionado. </p> <p>Se você for um cliente do <b>Analytics</b>, a Adobe está provisionando para os atributos do cliente. Se você usar somente o <b>Target</b> e não tiver o Analytics, é necessário solicitar o provisionamento para os principais serviços ao contatar o Atendimento ao cliente. </p> </li> 
     <li id="li_444FEDEE4B7244F79BA847662F5B17CB"> <p>Conversar com a equipe de CRM. Descubra o tipo de dados do cliente que está disponível e poderia ser usado no Analytics e em toda a Experience Cloud. </p> </li> 
     <li id="li_32D4AAF8C29748A78801A0E1BFB37AF5"> <p>Implementar os principais serviços. </p> <p>Consulte <a href="../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C" format="dita" scope="local"> Introdução - ativar as soluções dos serviços principais</a> para obter as etapas sobre como modernizar a implementação dos serviços principais. (consulte a sessão sobre como sincronizar as IDs do cliente para obter informações importantes.) </p> </li> 
    </ol> <p> <b>Observação:</b> há perguntas frequentes do administrador para implementar os principais serviços da <a href="../admin-getting-started/faq.md#concept_13219B4E51784577B6FF78AAA203DE91" format="dita" scope="local"> aqui</a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Quantos atributos do cliente eu posso usar? </p> </td> 
   <td colname="col2"> <p>Você pode fazer upload de centenas de colunas de <span class="filepath">.csv</span> para o serviço de atributos do cliente. No entanto, ao configurar assinaturas e selecionar atributos, os seguintes limites se aplicam (por conjunto de relatórios), dependendo das soluções que você possui:</p> <p> 
     <ul>
     <li>Foundation: 0</li>
     <li>Select: 3</li>
     <li>Prime: 15</li>
     <li>Ultimate: 200</li>
     <li>Standard: total de 3</li>
     <li>Premium: 200</li>
     <li>Target Standard: 5</li>
     <li>Target Premium: 200</li></ul>
     </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>É necessário migrar para o serviço da Experience Cloud ID? </p> </td> 
   <td colname="col2"> <p>A migração depende das soluções usadas. </p> <p> 
     <ul id="ul_9C473434B5DA4C6299AAB209DEDFCDE7"> 
      <li id="li_8BC10EB2825F4ADF8CA61F71D4994A28"> <b>Adobe Analytics</b>: recomendado </li> 
      <li id="li_56F518E3F3DF4C93B6F7EF3B40ACC52F"> <b>Adobe Target:</b> obrigatório. </li> 
     </ul> </p> <p>Usar o serviço da ID melhora a funcionalidade e abre as portas para usar a funcionalidade mais recente da Experience Cloud, incluindo públicos-alvo em tempo real, a modernização do Target, a integração do Analytics e o rastreamento de heartbeat de vídeo. </p> <p>Para obter mais detalhes, consulte <a href="../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C" format="dita" scope="local">Principais serviços - Ativação das soluções</a>. </p> <p> <b>Observação</b>: O serviço da <span class="term">Experience Cloud ID</span> é a implementação modernizada do que era conhecido como o <span class="term"> serviço de ID de visitante do Analytics</span>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Como a funcionalidade do atributo do cliente está relacionada ao Adobe Audience Manager? </p> </td> 
   <td colname="col2"> <p>Embora o Audience Manager possa receber dados para executar a identificação do público-alvo, não é possível executar a funcionalidade de análise que vincula os atributos aos dados comportamentais históricos ou oferecer os recursos de relatório, análise e segmentação que estão disponíveis no Adobe Analytics. O serviço principal Pessoas permite que dados avançados nas soluções sejam reunidos e associados a uma única ID para uso na Experience Cloud. </p> <p> No Adobe Target, os atributos do cliente aparecem como atributos individuais que podem ser combinados com outras regras para construir públicos-alvo. Os públicos-alvo compartilhados no serviço principal Pessoas são públicos completos que não podem ser modificados. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>(Somente para Analytics) </b>Como essa funcionalidade é diferente do que é oferecido no Analytics premium? </p> </td> 
   <td colname="col2"> <p>Antes, os clientes interessados em combinar os dados de atributo do cliente com os dados do Analytics dependiam muito da ferramenta de Data Workbench para essa funcionalidade. Os atributos do cliente expõem essa funcionalidade para um público-alvo maior por fornecer atributos do cliente como dimensões e métricas nos relatórios e análises, Ad Hoc Analysis e construtor de relatórios. Os clientes do Analytics Standard terão acesso aos atributos do cliente, mas com recursos limitados. O recurso completo está disponível para os clientes do Analytics Premium. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>(Somente para Target)</b> É possível pré-carregar ou fazer upload dos dados para clientes desconhecidos para o Target? </p> </td> 
   <td colname="col2"> <p> Sim. Quando o visitante faz a primeira solicitação para o Target, o sistema coleta as informações existentes sobre ele nos Atributos do cliente e utiliza os dados para o direcionamento. </p> <p> <p>Observação: a recuperação desses dados pode demorar até 20 minutos a partir da primeira interação com o Target. </p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>(Somente para Target)</b> É possível criar um super público-alvo ao combinar dados de atributos do cliente com dados de público-alvo compartilhados? </p> </td> 
   <td colname="col2"> <p>Não. Os dados de público-alvo compartilhados compõem um público-alvo completo. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>(Somente para Target) </b>Como a funcionalidade de atributos do cliente se compara à API do perfil em massa do Target? </p> </td> 
   <td colname="col2"> <p> A <a href="https://www.adobe.io/apis/experiencecloud/target.html" format="https" scope="external">API de perfil em massa</a> permite que os perfis do Target sejam atualizados diretamente pela API, para um perfil individual ou em massa. O recurso é semelhante aos atributos do cliente, com estas diferenças: </p> 
    <ul id="ul_5AAA4A8497C04F50A8AAA9F776BB868E"> 
     <li id="li_B20AEA397F3B4C86A1140CDA61ABD575">A API do perfil é uma chamada de API REST e os atributos do cliente usam FTP. </li> 
     <li id="li_7FBE428EF5D34B6AA09B6368E8210344">A API de perfil do Target envia dados apenas para o Target, e não para a Experience Cloud. </li> 
     <li id="li_CBB4D3FAF53944E0A066A4AD9F9C8760">Os atributos do cliente fornecem uma interface simples para criar e gerenciar os dados externos. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>(Somente para Target)</b> O envio de dados de atributos do cliente para o Adobe Target prolonga a vida útil do perfil de visitante do Target? </p> </td> 
   <td colname="col2"> <p>Sim. Consulte <a href="https://docs.adobe.com/content/help/en/target/using/audiences/visitor-profiles/visitor-profile.html" format="https" scope="external">Vida útil do perfil do visitante</a> na ajuda do Adobe Target. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b> (Somente para Target)</b> É possível direcionar os dados enviados em atributos do cliente imediatamente depois que o visitante é identificado pela ID do cliente? </p> </td> 
   <td colname="col2"> <p>Sim. </p> <p>Na chamada de servidor do Target, que inclui a ID de terceiros da mbox, todos os dados de atributos do cliente estarão disponíveis. </p> </td> 
  </tr> 
 </tbody> 
</table>
