---
description: Implemente a Experience Cloud e torne-se um administrador. Esse processo moderniza suas soluções para os principais recursos do serviço, como atributos do cliente e audiências.
keywords: core services;customer attributes
seo-description: Implemente a Experience Cloud e torne-se um administrador. Esse processo moderniza suas soluções para os principais recursos do serviço, como atributos do cliente e audiências.
seo-title: Ativar as soluções Experience Cloud dos serviços principais
solution: Experience Cloud
title: Ativar as soluções dos principais serviços
uuid: 5820060f-9b18-4339-81e0-401d964f7a03
translation-type: tm+mt
source-git-commit: 979520e2f0e015180a3b51d4b0b88b96b72301a3

---


# Ativar as soluções dos principais serviços

Para clientes existentes, saiba como modernizar suas implementações de solução e implementar a Experience Cloud para que você possa usar recursos como atributos do cliente e audiências. Para fazer isso, você:

1. [Associar-se à Experience Cloud e tornar-se um administrador](#section_2423F0BD3DF642658103310EE5EA6154)
1. [Implementação do serviço da Experience Cloud ID](#section_3C9F6DF37C654D939625BB4D485E4354)
1. [Mapear conjuntos de relatórios para uma organização da Experience Cloud](#section_7B08516B01BA421681DF03D0E86CE3BA)
1. [Atualizar seu código do AppMeasurement do Analytics](#section_1798D9D0F05C47E29816AC4EEB9A0913)
1. [Atualize sua implementação de Públicos alvos da Adobe](#section_C2F4493C7A36406DAE2266B429A4BD24)
1. [Verificar a implementação dos principais serviços](#section_E641782A0F4F44AF8C9C91216BE330D5)
1. [Gerenciar usuários e produtos](#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF)
1. [Começar a usar os principais serviços](#section_960C06093623462E8EA247B3E97274A1)

## Etapa 1. Associar-se à Experience Cloud e tornar-se um administrador {#section_2423F0BD3DF642658103310EE5EA6154}

O que é necessário para entrar na Experience Cloud:

![](assets/step1_icon.png) Verifique se você tem as SKUs adequadas do Adobe Analytics ou Adobe Target.

* **Adobe Analytics:** Standard ou Premium (não o [!DNL SiteCatalyst] SKU herdado).
* **Público alvo da Adobe:** Padrão ou Premium.

>[!NOTE]
>
>Por exemplo, [!DNL Target]migre para at.js a partir de [!DNL mbox.js]. See [Upgrading from at.js 1. x to at.js 2. x](https://docs.adobe.com/content/help/en/target/using/implement-target/client-side/upgrading-from-atjs-1x-to-atjs-20.html).

![](assets/step2_icon.png) Modernize sua implementação e consiga um administrador.

1. Siga as etapas abaixo em [Implantar o serviço [!UICONTROL da]](../core-services/core-services.md#section_3C9F6DF37C654D939625BB4D485E4354)Experience Cloud ID.
1. Entre em contato com seu Gerente de contas e start o processo de provisionamento da Experience Cloud.

![](assets/step3_icon.png)[!UICONTROL  Gerenciar usuários e produtos no Admin Console].

### Logon do administrador

After you are an administrator, you can log in at [experiencecloud.adobe.com](https://experiencecloud.adobe.com).

Você verá o link **[!UICONTROL Administração]** no menu de navegação da Experience Cloud.

Consulte [Administração de usuários e produtos da Experience Cloud](../admin-getting-started/admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909) para obter ajuda.

### Login do usuário

Para fazer logon na Experience Cloud, os usuários devem:

1. Tenha uma Adobe ID (ou Enterprise ID para sua empresa).
1. Sign in at [experiencecloud.adobe.com](https://experiencecloud.adobe.com).
1. Pertencer a um grupo de soluções mapeado para um grupo corporativo.
1. Se necessário, vincule suas contas da solução à Adobe ID (descrito abaixo).

![](assets/step4_icon.png) Opcional: vincular contas de usuário existentes.

Provavelmente, você tem usuários que já são membros de grupos de soluções, como um grupo do Analytics gerenciado anteriormente em [!UICONTROL Analytics] > Ferramentas administrativas.

Quando você mapeia esses grupos para grupos corporativos da Experience Cloud, esses usuários devem vincular manualmente suas credenciais de conta da solução à Adobe ID.

Consulte [Vincular contas na Experience Cloud](../admin-getting-started/organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1)

>[!NOTE]
>
>Depois de mapear os grupos de solução e corporativos, os novos usuários são vinculados automaticamente. (As credenciais da solução são criadas e vinculadas automaticamente à Adobe ID.)

As seções a seguir descrevem como modernizar sua implementação. A modernização da implementação habilita os principais serviços na Experience Cloud.

## Etapa 2: Implemente o serviço [!UICONTROL da] Experience Cloud ID usando o [!UICONTROL Experience Platform Launch]ou o Gerenciamento  dinâmico de tags {#section_3C9F6DF37C654D939625BB4D485E4354}

O serviço [!UICONTROL da] Experience Cloud ID fornece uma ID comum para a integração entre soluções. Fornece identificação de visitantes entre domínios e um caminho para definição de metas e personalização entre dispositivos/navegadores com base nos dados do CRM carregados pelos Atributos [!UICONTROL do]cliente.

O método mais simples de habilitar os principais serviços da Experience Cloud é ativá-la automaticamente para o Analytics e o Público alvo da Adobe por meio da extensão [do Serviço da](https://docs.adobe.com/content/help/en/launch/using/implement/solutions/idservice-save.html) Experience Cloud ID no [!UICONTROL Experience Platform Launch]ou por meio da ferramenta ECID no Gerenciamento dinâmico de tags. (O Experience Platform Launch é altamente recomendado.)

![](assets/menu-activation-shell.png)

Para obter a ajuda completa do Serviço da Experience Cloud ID (anteriormente, ID do visitante), acesse [aqui](https://docs.adobe.com/content/help/en/id-service/using/home.html).

**Não está usando o Launch[!UICONTROL da plataforma]Experience ou o Gerenciamentodinâmico de tags?**

If you are not using [!UICONTROL Experience Platform Launch] or [!UICONTROL Dynamic Tag Management], manually implement the ID service via the JavaScript Deployment ([!DNL VisitorAPI.js]), as follows:

| Tarefa | Descrição |
| -----------| ---------- |  
| [Implementar o serviço da Experience Cloud ID no Analytics](https://docs.adobe.com/content/help/en/id-service/using/implementation/setup-analytics.html) | A Adobe também recomenda configurar outras IDs [do](https://docs.adobe.com/content/help/en/id-service/using/reference/authenticated-state.html)cliente. Essas IDs estão associadas a cada visitante e ativam a funcionalidade atual e futura na Experience Cloud. |
| Atualize seu [!DNL s_code] existente para a versão H.27.3 ou superior, ou seu [!DNL AppMeasurement.js] existente para a versão 1.4 ou superior. | Esses arquivos estão disponíveis para download no Gerenciador [de](https://docs.adobe.com/content/help/en/analytics/admin/admin-tools/code-manager-admin.html) código nas Ferramentas administrativas do Analytics.  (O guia Implementação [do](https://docs.adobe.com/content/help/en/analytics/implementation/javascript-implementation/javascript-implementation-overview.html) JavaScript está disponível se você precisar de mais informações sobre [!DNL AppMeasurement.js].) |
| Sincronizar a ID do cliente para o Analytics | See [Analytics - synching the customer ID](../core-services/core-services.md#section_AD473A6A21C1446498E700363F9A8437) (below). |

## Analytics &amp; Adobe Target - synching the customer ID {#section_AD473A6A21C1446498E700363F9A8437}

As a part of setting up the Experience Cloud ID Service, Adobe recommends for Analytics and [!DNL Target] that you synchronize your [customer IDs](https://docs.adobe.com/content/help/en/id-service/using/reference/authenticated-state.html) with the Experience Cloud.

In Adobe Target, the `mbox3rdpartyid` needs to get the customer ID and send it to [!DNL Target]. (Consulte [Trabalhar com atributos](https://docs.adobe.com/content/help/en/target/using/audiences/visitor-profiles/working-with-customer-attributes.html) do cliente em [!DNL Target].)

Quando um visitante é autenticado no seu site ou identificado de alguma forma, a implementação deve revelar a ID do cliente do CRM para a página ou aplicativo. Em seguida, você pode usar a chamada de função apropriada para sincronizar a ID do cliente com a Experience Cloud. Essa sincronização armazena a ID do cliente do CRM do visitante na Experience Cloud e ativa os atributos desse cliente para uso na Experience Cloud.

Por exemplo, digamos que Bob tenha a ID de cliente `52mc210tr42` em seu sistema do CRM. Quando Bob for autenticado no seu site, você deverá revelar essa ID na página e usar a ID para sincronizar por uma das seguintes maneiras:

* Chamar `visitor.setCustomerIDs({"crm_id":"52mc210tr42"})` usando o serviço de ID de visitante. Ou,
* Preencha o *`Customer ID (52mc210tr42)`* em uma prop ou eVar.

A ID do cliente deve ser definida em cada chamada do servidor do [!DNL Analytics] em que a ID do cliente seja conhecida.

### SDKs móveis

Consulte a seção Serviço *da* Experience Cloud ID para obter exemplos de sintaxe sobre como definir outras IDs do cliente em aplicativos [Android](https://docs.adobe.com/content/help/en/mobile-services/android/overview.html) e [iOS](https://docs.adobe.com/content/help/en/mobile-services/ios/overview.html) Mobile.

### Ativação de atributos para dados históricos

Os dados do atributo do cliente são disponibilizados depois que os visitantes fazem logon. Se você ainda não tiver implementado o serviço da Experience Cloud ID mais recente e tiver rastreado historicamente as IDs do cliente em uma prop ou eVar, poderá solicitar um processo que envie logons históricos para a Experience Cloud. Esse processo permite que você comece a usar os atributos do cliente imediatamente.

Entre em contato com o Atendimento ao cliente para ativar os dados históricos.

## Etapa 3. Map report suites to an Experience Cloud Organization {#section_7B08516B01BA421681DF03D0E86CE3BA}

Os serviços da Experience Cloud (como o Serviço da Experience Cloud ID e o serviço Pessoas) estão associados a uma organização da Experience Cloud em vez de a um conjunto de relatórios individual do Analytics. Para garantir que esses serviços funcionem corretamente, cada conjunto de relatórios do Analytics deve ser mapeado para uma organização da Experience Cloud.

Consulte [Mapear conjuntos de relatórios para uma organização](report-suite-mapping.md).

## Etapa 4. (Adobe Analytics) Update your Analytics AppMeasurement code {#section_1798D9D0F05C47E29816AC4EEB9A0913}

Verifique se você está na coleção de dados regionais (RDC). Se o domínio de coleta de dados for [!DNL omtrdc.net] ou se CNAME estiver mapeado para [!DNL omtrdc.net], você estará na RDC. Consulte [Transição para RDC](https://docs.adobe.com/content/help/en/analytics/technotes/rdc/regional-data-collection.html) para obter mais informações. Se você estiver usando cookies primários, consulte o [CNAME e o Serviço](https://docs.adobe.com/content/help/en/id-service/using/reference/analytics-reference/cname.html) da Experience Cloud ID para obter informações sobre coleta de dados CNAMEs e rastreamento entre domínios.

Recomenda-se modernizar sua implementação do Analytics ao atualizar suas bibliotecas do JavaScript, incluindo a API do visitante. A maneira simples de fazer isso é adicionar uma ferramenta do [!DNL Adobe Analytics] no Dynamic Tag Management, especificando *`Automatic`* como o método de configuração.

In [!UICONTROL Dynamic Tag Management], click **[!UICONTROL <Web Property Name>]**>**[!UICONTROL  Visão geral ]**>**[!UICONTROL  Adicionar uma ferramenta ]**>**[!UICONTROL  Adobe Analytics ]**. Consulte Configurações[do](https://docs.adobe.com/content/help/en/dtm/using/tools/analytics-dtm.html)Adobe Analytics no Gerenciamento dinâmico de tags para obter informações sobre implantação.

## Etapa 5. (Adobe Target) Update your Adobe Target implementation {#section_C2F4493C7A36406DAE2266B429A4BD24}

* É recomendável adicionar uma Extensão do target [da](https://docs.adobe.com/content/help/en/launch/using/extensions-ref/adobe-extension/targetv2-extension/adobe-target-extension-v2.html) Adobe no [!UICONTROL Experience Platform Launch], para que a recuperação da biblioteca seja automática. Você também pode configurar a extensão [do serviço da](https://docs.adobe.com/content/help/en/launch/using/extensions-ref/adobe-extension/id-service-extension/overview.html) Experience Cloud ID para o Público alvo da Adobe (e outras soluções) usando o [!UICONTROL Experience Platform Launch]. A atualização do serviço [!UICONTROL da] Experience Cloud ID **é necessária** para que o Público alvo da Adobe use os principais serviços. (Se você usar o Gerenciamento [!UICONTROL dinâmico de tags, adicione uma ferramenta]de Público alvo [](https://docs.adobe.com/content/help/en/dtm/using/tools/target.html)da Adobe. Você também pode usar o Gerenciamento  dinâmico de tags para implantar o Serviço da Experience Cloud ID para o Público alvo da Adobe.)
* Se você não estiver usando o [!UICONTROL Experience Platform Launch] ou o Gerenciamento dinâmico de tags, [atualize a biblioteca](https://docs.adobe.com/content/help/en/target/using/implement-target/client-side/mbox-implement/target-download-config-mbox.html) mbox manualmente.
* Solicite acesso para usar o Adobe Analytics como a fonte de relatórios para o [!DNL Adobe Target]. [!DNL Target]Os dados do e do são combinados na mesma chamada de servidor durante o processamento para que os visitantes sejam conectados entre as duas soluções. [!DNL Analytics] See [Analytics for Target Implementation](https://docs.adobe.com/content/help/en/target/using/integrate/a4t/a4t.html).

   >[!IMPORTANT]
   >
   >Todos os clientes do Analytics já foram provisionados para os principais serviços, como atributos do cliente. Se você não for um cliente do Analytics, entre em contato com o Atendimento ao cliente para solicitar o provisionamento.

## Etapa 6. Verificar a implementação dos principais serviços {#section_E641782A0F4F44AF8C9C91216BE330D5}

Use o processo a seguir para garantir que o Serviço da Experience Cloud ID seja implementado corretamente em seu site.

1. Apague os cookies do seu site para que você possa ver a solicitação para o serviço da Experience Cloud ID (a solicitação ocorre na primeira visita e, em seguida, aproximadamente uma vez por visitante, por semana).
1. Usando um analisador de pacote ou o painel de rede em um depurador de navegador da Web, procure por uma solicitação em [!DNL dpm.demdex.net].
1. Confira se a resposta possui `d_mid` e um valor, por exemplo: `_setMarketingCloudFields({"d_mid":"4235...`
1. Verify that the Analytics request contains the `mid` parameter (the Experience Cloud ID). Durante o período de carência (se estiver ativado), você também deve ver um `aid` parâmetro (a ID do visitante do Analytics).

Resposta esperada contendo a Experience Cloud ID:

![](assets/mac_id_response.png)

Solicitação de imagem do Analytics que contém a Experience Cloud ID (também conhecida como `mid` ou ID _do_ visitante):

![](assets/mid.png)

Experience Cloud ID na solicitação da mbox:

![](assets/mbox_request.png)

### Qual é o período de carência?

Após implantar o serviço da Experience Cloud ID, os novos visitantes não receberão mais uma Experience Cloud ID do servidor de coleta de dados. Se as seções do site ainda não tiverem implementado o Serviço da Experience Cloud ID, quando os visitantes navegarem para essas seções, a Experience Cloud ID não será reconhecida e os visitantes receberão uma ID de visitante herdada do Analytics. Isso pode causar possíveis problemas, incluindo visitas de duplicados e atribuições incorretas.

Por exemplo, se a seção de suporte do seu site for gerenciada em um CMS diferente, você terá um arquivo JavaScript do Analytics diferente para essa seção. Se você implantar a Experience Cloud ID no seu site principal antes de implantar o serviço de ID no site de suporte, os novos visitantes receberão uma ID do Analytics herdada quando visitarem a seção de suporte e as visitas que abrangem ambas as seções do site serão relatadas como visitas diferentes.

A implantação do Serviço da Experience Cloud ID em sites que usam vários arquivos JavaScript ou outras tecnologias (como Flash) pode causar problemas de coordenação, pois é necessário ativar o Serviço da Experience Cloud ID em todas as partes do site ao mesmo tempo. Ao configurar um período de carência, os novos visitantes continuam recebendo uma ID de visitante do Analytics a partir do serviço de ID, para que os visitantes possam ser continuamente identificados nas seções do site que não foram atualizadas para usar o serviço de ID de visitante.

## Etapa 7. Gerenciar usuários e produtos {#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF}

Once you are up and running, navigate to the [Admin Console](https://adminconsole.adobe.com/), where you can manage users and product profiles.

![](assets/menu-administration-shell.png)

Consulte [Gerenciamento de usuários e produtos da Experience Cloud](../admin-getting-started/admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909).

### Atributos do cliente

<!-- <p> 
 <note type="important">
  To use the Customer Attributes feature, users must belong to the 
  <span class="term"> Adobe Customer Attributes</span> group, and to solution-level groups (Analytics or Adobe Target). 
 </note> </p> 
 -->

Users that are added to the [!UICONTROL Customer Attributes] group will see the [!UICONTROL Customer Attributes] menu item on the left side of the Experience Cloud interface.

## Etapa 8. Begin using core services {#section_960C06093623462E8EA247B3E97274A1}

Tire proveito dos seguintes recursos do serviço principal.

![](assets/menu-audiences-shell.png)

### [!UICONTROL Pessoas] > Atributos [!UICONTROL do cliente]

Se você capturar os dados de clientes de empresas em um banco de dados de gerenciamento de relacionamento com o cliente (CRM), poderá fazer upload dos dados em uma fonte de dados do atributo do cliente na Experience Cloud. Depois de enviado, aproveite os dados no [!DNL Adobe Analytics] e no [!DNL Adobe Target].

Consulte [Atributos do cliente](../attributes/attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1)

### [!UICONTROL Pessoas] > Biblioteca [!UICONTROL de Audiências]

Experience Cloud [!UICONTROL Audiences] is the interface that lets you create audiences, combine existing audiences to create composite audiences, and view all shared audiences.

Consulte [Públicos-alvo](../audience-library/audience-library.md#topic_679810123CAA4E0CA4FA3417FB0100C7)

## armazenamento de dados e divulgação de privacidade

Caso você use a definição de perfil do público-alvo em tempo real e outros principais serviços da Adobe [!DNL Experience Cloud], esses serviços podem afetar o data center (e país) em que estão seus dados. Specifically, because the core services of the Adobe [!DNL Experience Cloud] leverage Adobe Audience Manager, data used within the [!UICONTROL People] service must reside within Audience Manager servers in the United States.

When leveraging core services made available via the [!UICONTROL People] service, the types of data sent from other Adobe products to audience management are:

* Pares de valor/principais do [!DNL Analytics] (props, eVars, list vars e assim por diante). Por padrão, as linhas de log incluem endereço IP, inclusive o último octeto do IP (se o endereço IP não tiver sido modificado pelas configurações de ofuscação de IP no Adobe [!DNL Analytics]).
* Características e segmentos para os quais os visitantes se qualificam com base nas regras configuradas no Gerenciador de Audiências.
* (Opcional) Uma ou mais IDs. Dependendo da implementação do serviço de ID, também é possível enviar uma ou mais IDs, como IDs CRM ou endereços de email em hash. Se os dados forem enviados para o Adobe [!DNL Analytics], serão transferidos para o gerenciamento de público-alvo da Adobe. A Adobe não recomenda fornecer dados pessoais ao Adobe [!DNL Analytics]. Em vez disso, use um hash unidirecional para mascarar os dados antes de enviá-los para a Adobe.
* Segmentos originados no [!DNL Analytics] através do segmento back-end que compartilha o recurso.
* O cookie demdex.net será configurado se os cookies de terceiros não estiverem bloqueados. The `AMCV_###@AdobeOrg` first-party cookie is always set with the Experience Cloud ID Service.

Todos esses elementos de dados são fornecidos para o Adobe Audience Manager na forma de arquivos de log. O Audience Manager processa e armazena os dados nos Estados Unidos. O Gerenciador de Audiências não fornece uma opção para armazenar ou processar esses dados fora dos Estados Unidos.

### Cookies e opções de não participação

Usar a definição de perfil do público-alvo em tempo real potencializa o cookie do Audience Manager, além dos cookies usados no [!DNL Analytics] e no [!DNL Target].

Se você desejar oferecer a capacidade de não participação adequada, os visitantes do seu site devem adicionar a opção de não participação do Audience Manager ao seu processo atual de não participação.

Consulte [Adobe Experience Cloud - Implementação das opções de não participação](https://docs.adobe.com/content/help/en/analytics/implementation/javascript-implementation/data-collection/opt-out.html) da Adobe para obter instruções.

Consulte Coletas de [dados CNAMEs e Rastreamento](https://docs.adobe.com/content/help/en/id-service/using/reference/analytics-reference/cname.html) entre domínios para ativar o rastreamento entre domínios.
