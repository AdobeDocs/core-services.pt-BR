---
description: Implemente a Experience Cloud e torne-se um administrador. Esse processo moderniza suas soluções para os recursos dos principais serviços, como atributos do cliente e públicos-alvo.
keywords: serviços principais, customer attributes
seo-description: Implemente a Experience Cloud e torne-se um administrador. Esse processo moderniza suas soluções para os recursos dos principais serviços, como atributos do cliente e públicos-alvo.
seo-title: Ativar as soluções Experience Cloud dos serviços principais
solution: Experience Cloud
title: Ativar as soluções dos principais serviços
uuid: 5820060f-9b18-4339-81e0-401d964f7a03
translation-type: tm+mt
source-git-commit: b4809ff0b4546f105ac6270eca1bfce2b6467876

---


# Ativar as soluções dos principais serviços

Implemente a Experience Cloud e torne-se um administrador. Esse processo moderniza suas soluções para os recursos dos principais serviços, como atributos do cliente e públicos-alvo.

<!-- <p>https://marketing-beta.adobe.com/resources/help/core/core-services.html </p> 
<p>https://adobe.sharepoint.com/sites/AGSConsulting/CoreServices/PA/_layouts/15/start.aspx#/ </p> -->

<!-- Core services architecture and data flow wiki: https://wiki.corp.adobe.com/pages/viewpage.action?pageId=1004285689 -->

## Etapa 1. Associar-se à Experience Cloud e tornar-se um administrador {#section_2423F0BD3DF642658103310EE5EA6154}

O que é necessário para entrar na Experience Cloud:

![](assets/step1_icon.png) Verifique se você tem as SKUs adequadas do Adobe Analytics ou Adobe Target.

* **Adobe Analytics:** Standard ou Premium (não o SKU do SiteCatalyst antigo).
* **Adobe Target:** Standard ou Premium.



>[!NOTE]
>
>For Target, [migrate to at.js from mbox.js](https://marketing.adobe.com/resources/help/en_US/target/ov2/t_target-migrate-atjs.html).


![](assets/step2_icon.png) Modernize sua implementação e consiga um administrador.


1. Siga as etapas abaixo em [Implantar o serviço da Experience Cloud ID](../core-services/core-services.md#section_3C9F6DF37C654D939625BB4D485E4354).
1. Entre em contato com o gerente da conta e inicie o processo de provisionamento da Experience Cloud.

![](assets/step3_icon.png) Gerenciar usuários e produtos no Admin Console.

**Acesso de administrador**

Depois de se tornar um administrador, faça logon em [marketing.adobe.com](https://marketing.adobe.com)

Você verá o link **[!UICONTROL Administração]** no menu de navegação da Experience Cloud.

Consulte [Administração de usuários e produtos da Experience Cloud](../admin-getting-started/admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909) para obter ajuda.

**Acesso do usuário**

Para fazer logon na Experience Cloud, os usuários devem:


1. Ter uma Adobe ID.
1. Fazer logon em [!DNL marketing.adobe.com].
1. Pertencer a um grupo de soluções mapeado para um grupo corporativo.
1. Caso necessário, vincular as contas da solução à Adobe ID (descrito abaixo).

![](assets/step4_icon.png) Opcional: vincular contas de usuário existentes.

Provavelmente, há usuários que já são membros de grupos de soluções, como um grupo do Analytics gerenciado em Analytics &gt; Ferramentas administrativas.

Quando você mapeia tais grupos para grupos corporativos da Experience Cloud, esses usuários devem vincular manualmente suas respectivas credenciais de conta da solução à Adobe ID.

Consulte [Vincular contas na Experience Cloud](../admin-getting-started/organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1)

> [!NOTE]
> 
> Depois de mapear os grupos de solução e corporativos, os novos usuários são vinculados automaticamente. (As credenciais da solução são criadas e vinculadas automaticamente à Adobe ID.)

As seções a seguir descrevem como modernizar sua implementação. A modernização da implementação habilita os principais serviços na Experience Cloud.

## Etapa 2: Implementar o serviço da Experience Cloud ID usando o Gerenciador dinâmico de tags ou o Experience Platform Launch {#section_3C9F6DF37C654D939625BB4D485E4354}

O método mais simples de habilitar os principais serviços da Experience Cloud é ativá-la automaticamente para o Analytics e o Target com a [ferramenta de serviço da Experience Cloud ID](https://marketing.adobe.com/resources/help/en_US/mcvid/mcvid-dtm-implement.html) no Gerenciador dinâmico de tags. (ou Experience Platform Launch.)

![](assets/menu-activation-shell.png)

Para obter o serviço completo da Experience Cloud ID (anteriormente, ID de visitante), acesse [este link](https://marketing.adobe.com/resources/help/en_US/mcvid/).

Além disso, o gerenciamento de tags de próxima geração é o [Launch da Adobe](https://marketing.adobe.com/resources/help/en_US/experience-cloud/launch/)

**Não está usando o Dynamic Tag Management ou o Launch?**

Se você não estiver usando o Dynamic Tag Management, implemente o serviço de ID de forma manual pela implantação de JavaScript ([!DNL VisitorAPI.js]) da seguinte maneira:

1. Execute as etapas descritas em [Implementação do serviço da Experience Cloud ID para o Analytics](https://marketing.adobe.com/resources/help/en_US/mcvid/mcvid-setup-analytics.html).

   A Adobe também recomenda configurar outras [IDs de cliente](https://marketing.adobe.com/resources/help/en_US/mcvid/mcvid-authenticated-state.html). Essas IDs estão associadas a cada visitante e ativam a funcionalidade atual e futura nos principais serviços da Experience Cloud.

1. Atualize seu [!DNL s_code] existente para a versão H.27.3 ou superior, ou seu [!DNL AppMeasurement.js] existente para a versão 1.4 ou superior.

   Esses arquivos estão disponíveis para download no [Gerenciador de código](https://marketing.adobe.com/resources/help/en_US/reference/index.html?f=code_manager_admin) nas Ferramentas administrativas do Analytics.

   (O guia [Implementação do JavaScript](https://marketing.adobe.com/resources/help/en_US/sc/implement/js_implementation.html) está disponível se você precisar de mais informações sobre [!DNL AppMeasurement.js].)

1. Sincronize a ID do cliente para Analytics. Consulte [Analytics - sincronização da ID do cliente](../core-services/core-services.md#section_AD473A6A21C1446498E700363F9A8437) (abaixo).

## Analytics &amp; Target - sincronização da ID do cliente {#section_AD473A6A21C1446498E700363F9A8437}

Como parte da configuração do serviço da Experience Cloud ID, a Adobe recomenda para o Analytics e Target a sincronização das [IDs do cliente](https://marketing.adobe.com/resources/help/en_US/mcvid/mcvid-authenticated-state.html) com a Experience Cloud.

No Target, o [!DNL mbox3rdpartyid] deve obter a ID do cliente e enviá-la para o Target. (Consulte [Trabalhar com atributos do cliente](https://marketing.adobe.com/resources/help/en_US/target/target/c_working-with-customer-attributes.html) no Target.)

Quando um visitante é autenticado no seu site ou identificado de alguma forma, a implementação deve revelar a ID do cliente do CRM para a página ou aplicativo. Em seguida, você pode usar a chamada de função apropriada para sincronizar a ID do cliente com a Experience Cloud. Essa sincronização armazena a ID do cliente do CRM do visitante na Experience Cloud e ativa os atributos desse cliente para uso na Experience Cloud.

Por exemplo, digamos que Bob tenha a ID de cliente `52mc210tr42` em seu sistema do CRM. Quando Bob for autenticado no seu site, você deverá revelar essa ID na página e usar a ID para sincronizar por uma das seguintes maneiras:

* Chamar `visitor.setCustomerIDs({"crm_id":"52mc210tr42"})` usando o serviço de ID de visitante. Ou,
* Preencher a *`Customer ID (52mc210tr42)`* em uma prop ou eVar.


A ID do cliente deve ser definida em cada chamada do servidor do [!DNL Analytics] em que a ID do cliente seja conhecida.

**SDKs móveis**

Consulte a seção do serviço *da* Experience Cloud ID para obter exemplos de sintaxe sobre como definir outras IDs do cliente em aplicativos [Android](https://marketing.adobe.com/resources/help/en_US/mobile/android/?f=methods) e [iOS](https://marketing.adobe.com/resources/help/en_US/mobile/ios/?f=methods) Mobile.

**Ativação de atributos para dados históricos**

Os dados do atributo do cliente são disponibilizados depois que os visitantes fazem logon. Se você ainda não tiver implementado o serviço da Experience Cloud ID e tiver um histórico de rastreamento de IDs do cliente em uma prop ou eVar, será possível solicitar um processo que envie logons do histórico para a Experience Cloud. Esse processo permite começar a usar os atributos do cliente imediatamente.

Entre em contato com o Atendimento ao cliente para ativar dados históricos.

## Etapa 3. Mapear conjuntos de relatórios para uma organização da Experience Cloud {#section_7B08516B01BA421681DF03D0E86CE3BA}

Os serviços da Experience Cloud (como o serviço da Experience Cloud ID e Pessoas) estão associados à organização da Experience Cloud em vez de um conjunto de relatórios individual. Para garantir a operação correta desses serviços, cada conjunto de relatórios do Analytics deve ser mapeado para uma organização da Experience Cloud.

Consulte [Mapear conjuntos de relatórios para uma organização](report-suite-mapping.md).

## Etapa 4. (Adobe Analytics) Modernizar o código do Analytics AppMeasurement {#section_1798D9D0F05C47E29816AC4EEB9A0913}

Verifique se você está na coleção de dados regionais (RDC). Se o domínio de coleta de dados for [!DNL omtrdc.net] ou se CNAME estiver mapeado para [!DNL omtrdc.net], você estará na RDC. Consulte [Transição para a RDC](https://marketing.adobe.com/resources/help/en_US/whitepapers/rdc/?f=rdc_transition) para obter mais informações. Se estiver usando cookies próprios, consulte [CNAME e o serviço de ID de visitante](https://marketing.adobe.com/resources/help/en_US/mcvid/?f=mcvid_cname) para obter informações sobre os CNAMEs de coleta de dados e o rastreamento entre domínios.

Recomenda-se modernizar sua implementação do Analytics ao atualizar suas bibliotecas do JavaScript, incluindo a API do visitante. A maneira simples de fazer isso é adicionar uma ferramenta do [!DNL Adobe Analytics] no Dynamic Tag Management, especificando *`Automatic`* como o método de configuração.

No Dynamic Tag Management, clique em **[!UICONTROL <Web Property Name>]**&gt;**[!UICONTROL Visão geral]**&gt;**[!UICONTROL Adicionar uma ferramenta]**&gt;**[!UICONTROL Adobe Analytics]**. Consulte[Configurações do Adobe Analytics](https://marketing.adobe.com/resources/help/en_US/dtm/?f=analytics_dtm)no Dynamic Tag Management para obter informações sobre a implementação.

## Etapa 5. (Adobe Target) Modernizar a implementação do Adobe Target {#section_C2F4493C7A36406DAE2266B429A4BD24}

* Recomenda-se adicionar uma [ferramenta do Adobe Target](https://marketing.adobe.com/resources/help/en_US/dtm/target.html) no Dynamic Tag Management, de modo que a recuperação da biblioteca seja automática. No Dynamic Tag Management, clique em **[!UICONTROL <Web Property Name>]**&gt;**[!UICONTROL Visão geral]**&gt;**[!UICONTROL Adicionar uma ferramenta]**&gt;**[!UICONTROL Adobe Target]**.** Observação:**você também pode usar o Dynamic Tag Management para implantar o serviço da Experience Cloud ID no Target (e outras soluções). A atualização do serviço da Experience Cloud ID**&#x200B;é necessária **para usar os principais serviços do Target.
* Se você não estiver usando o Dynamic Tag Management, [atualize a biblioteca mbox](https://marketing.adobe.com/resources/help/en_US/target/ov/?f=t_mbox_download) de forma manual.
* Solicite acesso para usar o Adobe Analytics como a fonte de relatórios para o Adobe Target. Os dados do Target e do Analytics são combinados na mesma chamada de servidor durante o processamento para que os visitantes sejam conectados entre as duas soluções. Consulte [Analytics para a implementação do Target](https://marketing.adobe.com/resources/help/en_US/target/a4t/?f=a4t).
* 
   >[!IMPORTANT]
   >
   >Todos os clientes do Analytics já foram provisionados com os serviços principais, como atributos do cliente. Se você não for um cliente do Analytics, entre em contato com o Atendimento ao cliente para solicitar o provisionamento.

## Etapa 6. Verificar a implementação dos principais serviços {#section_E641782A0F4F44AF8C9C91216BE330D5}

Use o processo a seguir para verificar se o serviço da Experience Cloud ID foi implementado corretamente em seu site.

1. Apague os cookies do site para visualizar a solicitação do serviço da Experience Cloud ID (a solicitação ocorre na primeira visita e, depois, aproximadamente uma vez a cada visitante, toda semana).1. Usando um analisador de pacote ou o painel de rede em um depurador de navegador da Web, procure por uma solicitação em [!DNL dpm.demdex.net].
1. Confira se a resposta possui `d_mid` e um valor, por exemplo: `_setMarketingCloudFields({"d_mid":"4235...`
1. Verifique se a solicitação do Analytics possui um parâmetro mid (a Experience Cloud ID). Durante o período de carência (se ativado), você também deve visualizar um parâmetro de auxílio (a ID de visitante do Analytics).

Resposta esperada contendo a Experience Cloud ID:

![](assets/mac_id_response.png)

A solicitação de imagem do Analytics contendo a Experience Cloud ID (mid):

![](assets/mid.png)

Experience Cloud ID na solicitação de mbox:

![](assets/mbox_request.png)

**O que é o período de carência?**

Após implantar o serviço de ID de visitante, os novos visitantes não receberão mais uma ID de visitante do Analytics no seu servidor de coleção de dados. Se as seções do seu site ainda não tiverem implementado o serviço de ID de visitante, a Experience Cloud ID não será reconhecida e os visitantes receberão uma ID de visitante antiga do Analytics quando navegarem para essas seções. Isso pode causar problemas, incluindo visitas duplicadas e atribuições incorretas.

Por exemplo, se a seção de suporte do seu site for gerenciada em um CMS diferente, você terá um arquivo JavaScript do Analytics diferente para essa seção. Se você implantar uma ID de visitante no seu site principal antes de implantar o serviço de ID de visitante para o site de suporte, os novos visitantes receberão uma ID do Analytics antiga quando visitarem a seção de suporte, e as visitas que tratam das duas seções do site serão contadas como visitas diferentes.

Implantar o serviço de ID de visitante nos sites que usam vários arquivos JavaScript ou outras tecnologias (como Flash) pode gerar problemas de coordenação, pois é necessário ativar o serviço de ID de visitante em todas as partes do seu site ao mesmo tempo. Ao configurar um período de carência, os novos visitantes continuam recebendo uma ID de visitante do Analytics no serviço de ID de visitante, de modo que os visitantes possam ser continuamente identificados nas seções do seu site que não tenham sido atualizadas para usar o serviço de ID de visitante.

## Etapa 7. Gerenciar usuários e produtos {#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF}

Quando tudo estiver funcionando, navegue até **[!UICONTROL Administração]** &gt; **[!UICONTROL Iniciar o Admin Console]**, onde é possível gerenciar usuários e perfis de produto.

![](assets/menu-administration-shell.png)

Consulte [Gerenciamento de usuários e produtos da Experience Cloud](../admin-getting-started/admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909).

**Atributos do cliente**

<!-- <p> 
 <note type="important">
  To use the Customer Attributes feature, users must belong to the 
  <span class="term"> Adobe Customer Attributes</span> group, and to solution-level groups (Analytics or Target). 
 </note> </p> 
 -->

Os usuários adicionados ao grupo Atributos do cliente visualizarão o item de menu [!UICONTROL Atributos do cliente] à esquerda da interface da Experience Cloud

## Etapa 8. Começar a usar os principais serviços {#section_960C06093623462E8EA247B3E97274A1}

Tire proveito dos seguintes recursos do serviço principal.

![](assets/menu-audiences-shell.png)

**Pessoas &gt; Atributos dos clientes**

Se você capturar os dados de clientes de empresas em um banco de dados de gerenciamento de relacionamento com o cliente (CRM), poderá fazer upload dos dados em uma fonte de dados do atributo do cliente na Experience Cloud. Depois de enviado, aproveite os dados no [!DNL Adobe Analytics] e no [!DNL Adobe Target].

Consulte [Atributos do cliente](../attributes/attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1)

**Pessoas &gt; Biblioteca de público-alvo**

A Experience Cloud Audiences é a interface que permite criar públicos-alvo, combinar públicos-alvo existentes para criar públicos-alvo compostos e exibir todos os públicos-alvo compartilhados.

Consulte [Públicos-alvo](../audience-library/audience-library.md#topic_679810123CAA4E0CA4FA3417FB0100C7)

<!-- aam_mc.xml -->

## Informações sobre armazenamento de dados e divulgação de privacidade

Caso você use a definição de perfil do público-alvo em tempo real e outros principais serviços da Adobe [!DNL Experience Cloud], esses serviços podem afetar o data center (e país) em que estão seus dados. Especificamente, visto que os principais serviços da Adobe [!DNL Experience Cloud] usam o Adobe Audience Manager, os dados usados no serviço principal Pessoas devem ficar nos servidores do Audience Manager nos Estados Unidos.

Ao aproveitar os principais serviços disponibilizados pelo serviço principal Pessoas, os tipos de dados enviados de outros produtos da Adobe para o gerenciamento de público-alvo são:

* Pares de valor/principais do [!DNL Analytics] (props, eVars, list vars e assim por diante). Por padrão, as linhas de log incluem endereço IP, inclusive o último octeto do IP (se o endereço IP não tiver sido modificado pelas configurações de ofuscação de IP no Adobe [!DNL Analytics]).
* Características e segmentos para os quais os visitantes se qualificam com base nas regras definidas no Audience Manager.
* (Opcional) Uma ou mais IDs. Dependendo da implementação do serviço de ID, também é possível enviar uma ou mais IDs, como IDs CRM ou endereços de email em hash. Se os dados forem enviados para o Adobe [!DNL Analytics], serão transferidos para o gerenciamento de público-alvo da Adobe. A Adobe não recomenda fornecer dados pessoais ao Adobe [!DNL Analytics]. Em vez disso, use um hash unidirecional para apresentar os dados sob pseudônimo antes de enviá-los para a Adobe.
* Segmentos originados no [!DNL Analytics] através do segmento back-end que compartilha o recurso.
* O cookie demdex.net será configurado se os cookies de terceiros não estiverem bloqueados. O cookie próprio `AMCV_###@AdobeOrg` sempre está configurado com a Experience Cloud ID (antigo serviço de ID de visitante).


Todos esses elementos de dados são fornecidos para o Adobe Audience Manager na forma de arquivos de log. O Audience Manager processa e armazena os dados nos Estados Unidos. O Audience Manager não oferece uma opção para armazenar ou processar esses dados fora dos Estados Unidos.

**Cookies e opções de não participação**

Usar a definição de perfil do público-alvo em tempo real potencializa o cookie do Audience Manager, além dos cookies usados no [!DNL Analytics] e no [!DNL Target].

Se você desejar oferecer a capacidade de não participação adequada, os visitantes do seu site devem adicionar a opção de não participação do Audience Manager ao seu processo atual de não participação.

Consulte [Adobe Experience Cloud - Implementação das opções de não participação da Adobe](https://marketing.adobe.com/resources/help/en_US/sc/implement/opt_out.html) para obter instruções.

Consulte [CNAMEs de coleta de dados e rastreamento entre domínios](https://marketing.adobe.com/resources/help/en_US/mcvid/?f=mcvid_cname) para habilitar o rastreamento entre domínios.
