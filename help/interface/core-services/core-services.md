---
description: Implemente a Experience Cloud e torne-se um administrador. Esse processo moderniza suas soluções para recursos como atributos do cliente e públicos.
keywords: core services;Customer Attributes
seo-description: Implemente a Experience Cloud e torne-se um administrador. Esse processo moderniza suas soluções para recursos como atributos do cliente e públicos.
seo-title: Ativar as soluções da Experience Cloud para atributos e públicos-alvo do cliente
solution: Experience Cloud
title: Ativar as soluções dos serviços principais
index: true
translation-type: ht
source-git-commit: a47dc66b51758ed7e6b465f35375f979b479672f
workflow-type: ht
source-wordcount: '2402'
ht-degree: 100%

---


# Habilitar a implementação para serviços entre soluções

Se você implementou a Experience Cloud recentemente usando o Experience Platform Launch, você já configurou os atributos do cliente e os públicos-alvo da Experience Cloud. Você também pode gerenciar usuários e produtos no Admin Console.

Para clientes atuais, talvez seja necessário modernizar as implementações da solução e implementar a Experience Cloud. Dessa forma, você aproveitará os atributos do cliente e os recursos de público-alvo no Adobe Analytics, Audience Manager e Adobe Target. Para fazer isso, você deve:

1. [Associar-se à Experience Cloud e tornar-se um administrador](#section_2423F0BD3DF642658103310EE5EA6154)
1. [Implementar o Serviço da Experience Cloud ID](#section_3C9F6DF37C654D939625BB4D485E4354)
1. [Mapear conjuntos de relatórios para uma organização da Experience Cloud](#section_7B08516B01BA421681DF03D0E86CE3BA)
1. [Atualizar o código AppMeasurement do Analytics](#section_1798D9D0F05C47E29816AC4EEB9A0913)
1. [Atualizar a implementação do Adobe Target](#section_C2F4493C7A36406DAE2266B429A4BD24)
1. [Verificar a implementação](#section_E641782A0F4F44AF8C9C91216BE330D5)
1. [Gerenciar usuários e produtos](#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF)
1. [Começar a compartilhar dados de atributo e público-alvo](#section_960C06093623462E8EA247B3E97274A1)

## Etapa 1. Associar-se à Experience Cloud e tornar-se um administrador {#section_2423F0BD3DF642658103310EE5EA6154}

O que é necessário para entrar na Experience Cloud:

![](assets/step1_icon.png) Verifique se você tem as SKUs adequadas do Adobe Analytics ou Adobe Target.

* **Adobe Analytics:** Standard ou Premium (não o SKU do [!DNL SiteCatalyst] herdado).
* **Adobe Target:** Standard ou Premium.

>[!NOTE]
>
>No [!DNL Target], migre para at.js a partir do [!DNL mbox.js]. Consulte [Atualização do at.js 1.x para o at.js 2.x](https://docs.adobe.com/content/help/pt-BR/target/using/implement-target/client-side/upgrading-from-atjs-1x-to-atjs-20.html).

![](assets/step2_icon.png) Modernize sua implementação e consiga um administrador.

1. Siga as etapas abaixo em [Implantar o [!UICONTROL Serviço da Experience Cloud ID]](../core-services/core-services.md#section_3C9F6DF37C654D939625BB4D485E4354).
1. Entre em contato com o Gerente de contas e comece o processo de provisionamento da Experience Cloud.

![](assets/step3_icon.png) Gerenciar usuários e produtos no [!UICONTROL Admin Console].

### Logon do administrador

Depois de se tornar um administrador, faça logon em [experiencecloud.adobe.com](https://experiencecloud.adobe.com)

Você verá o link **[!UICONTROL Administração]** no menu de navegação da Experience Cloud.

Consulte [Administração de usuários e produtos da Experience Cloud](../admin-getting-started/admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909) para obter ajuda.

### Logon do usuário

Para fazer logon na Experience Cloud, os usuários devem:

1. Ter uma Adobe ID (ou Enterprise ID para sua empresa).
1. Faça logon em [experiencecloud.adobe.com](https://experiencecloud.adobe.com).
1. Pertencer a um grupo de soluções mapeado para um grupo corporativo.
1. Se necessário, vincule suas contas da solução à Adobe ID (descrito abaixo).

![](assets/step4_icon.png) Opcional: vincular contas de usuário existentes.

Provavelmente, há usuários que já são membros de grupos de soluções, como um grupo do Analytics gerenciado anteriormente em [!UICONTROL Analytics] > [!UICONTROL Ferramentas administrativas].

Quando você mapeia tais grupos para grupos corporativos da Experience Cloud, esses usuários devem vincular manualmente suas respectivas credenciais de conta da solução à Adobe ID.

Consulte [Vincular contas na Experience Cloud](../admin-getting-started/organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1)

>[!NOTE]
>
>Depois de mapear os grupos de solução e corporativos, os novos usuários são vinculados automaticamente. (As credenciais da solução são criadas e vinculadas automaticamente à Adobe ID.)

As seções a seguir descrevem como modernizar sua implementação. A modernização da implementação habilita os serviços principais na Experience Cloud.

## Etapa 2. Implemente o [!UICONTROL Serviço da Experience Cloud ID] usando o [!UICONTROL Experience Platform Launch] ou o [!UICONTROL Dynamic Tag Management] {#section_3C9F6DF37C654D939625BB4D485E4354}

O [!UICONTROL Serviço da Experience Cloud ID] fornece uma ID comum para integração entre soluções. Ele fornece identificação de visitantes entre domínios e um caminho para segmentação e personalização entre dispositivos/navegadores com base nos dados do CRM carregados pelos [!UICONTROL Atributos do cliente].

O método mais simples de habilitar os serviços principais da Experience Cloud é ativá-la automaticamente para o Analytics e o Adobe Target por meio da [extensão do Serviço da Experience Cloud ID](https://docs.adobe.com/content/help/en/launch/using/implement/solutions/idservice-save.html) no [!UICONTROL Experience Platform Launch] ou por meio da ferramenta ECID no [!UICONTROL Dynamic Tag Management]. (O Experience Platform Launch é altamente recomendado.)

Para obter a ajuda completa do Serviço da Experience Cloud ID (antiga ID de visitante), acesse [aqui](https://docs.adobe.com/content/help/pt-BR/id-service/using/home.html).

**Não está usando o [!UICONTROL Experience Platform Launch] ou o [!UICONTROL Dynamic Tag Management]?**

Se você não estiver usando o [!UICONTROL Experience Platform Launch] ou o [!UICONTROL Dynamic Tag Management], implemente o serviço de ID de forma manual pela implantação do JavaScript ([!DNL VisitorAPI.js]) da seguinte maneira:

| Tarefa | Descrição |
| -----------| ---------- |  
| [Implementar o serviço da Experience Cloud ID no Analytics](https://docs.adobe.com/content/help/pt-BR/id-service/using/implementation/setup-analytics.html) | A Adobe também recomenda configurar outras [IDs do cliente](https://docs.adobe.com/content/help/pt-BR/id-service/using/reference/authenticated-state.html). Essas IDs estão associadas a cada visitante e ativam a funcionalidade atual e futura da Experience Cloud. |
| Atualize seu [!DNL s_code] existente para a versão H.27.3 ou superior, ou seu [!DNL AppMeasurement.js] existente para a versão 1.4 ou superior. | Esses arquivos estão disponíveis para download no [Gerenciador de código](https://docs.adobe.com/content/help/pt-BR/analytics/admin/admin-tools/code-manager-admin.html) nas Ferramentas de administração do Analytics.  (O guia [Implementação do JavaScript](https://docs.adobe.com/content/help/pt-BR/analytics/implementation/js/overview.html) está disponível se você precisar de mais informações sobre o [!DNL AppMeasurement.js].) |
| Sincronizar a ID do cliente para o Analytics | Consulte [Analytics - sincronização da ID do cliente](../core-services/core-services.md#section_AD473A6A21C1446498E700363F9A8437) (abaixo) |

## Analytics &amp; Adobe Target - sincronização da ID do cliente {#section_AD473A6A21C1446498E700363F9A8437}

Como parte da configuração do Serviço da Experience Cloud ID, a Adobe recomenda para o Analytics e para o [!DNL Target] a sincronização das [IDs do cliente](https://docs.adobe.com/content/help/pt-BR/id-service/using/reference/authenticated-state.html) com a Experience Cloud.

No Adobe Target, o `mbox3rdpartyid` deve obter a ID do cliente e enviá-la para o [!DNL Target]. (Consulte [Trabalhar com atributos do cliente](https://docs.adobe.com/content/help/pt-BR/target/using/audiences/visitor-profiles/working-with-customer-attributes.html) em [!DNL Target].)

Quando um visitante é autenticado no seu site ou identificado de alguma forma, a implementação deve revelar a ID do cliente do CRM para a página ou aplicativo. Em seguida, você pode usar a chamada de função apropriada para sincronizar a ID do cliente com a Experience Cloud. Essa sincronização armazena a ID do cliente do CRM do visitante na Experience Cloud e ativa os atributos desse cliente para uso na Experience Cloud.

Por exemplo, digamos que Bob tenha a ID de cliente `52mc210tr42` em seu sistema do CRM. Quando Bob for autenticado no seu site, você deverá revelar essa ID na página e usar a ID para sincronizar por uma das seguintes maneiras:

* Chamar `visitor.setCustomerIDs({"crm_id":"52mc210tr42"})` usando o serviço de ID de visitante. Ou,
* Preencha o *`Customer ID (52mc210tr42)`* em uma prop ou eVar.

A ID do cliente deve ser definida em cada chamada do servidor do [!DNL Analytics] em que a ID do cliente seja conhecida.

### SDKs móveis

Consulte a seção *Serviço da Experience Cloud ID* para obter exemplos de sintaxe sobre como definir outras IDs do cliente em aplicativos móveis do [Android](https://docs.adobe.com/content/help/pt-BR/mobile-services/android/overview.html) e do [iOS](https://docs.adobe.com/content/help/pt-BR/mobile-services/ios/overview.html).

### Ativação de atributos para dados históricos

Os dados do atributo do cliente são disponibilizados depois que os visitantes fazem logon. Se você ainda não tiver implementado o Serviço da Experience Cloud ID e tiver um histórico de rastreamento de IDs do cliente em uma prop ou eVar, poderá solicitar um processo que envie logons do histórico para a Experience Cloud. Esse processo permite que você comece a usar os atributos do cliente imediatamente.

Entre em contato com o Atendimento ao cliente para ativar os dados históricos.

## Etapa 3. Mapear conjuntos de relatórios para uma organização da Experience Cloud {#section_7B08516B01BA421681DF03D0E86CE3BA}

Os serviços da Experience Cloud (como o Serviço da Experience Cloud ID e o [!UICONTROL serviço People]) estão associados a uma organização da Experience Cloud em vez de a um conjunto de relatórios individual do Analytics. Para garantir o funcionamento correto desses serviços, cada conjunto de relatórios do Analytics deve ser mapeado para uma organização da Experience Cloud.

Consulte [Mapear conjuntos de relatórios para uma organização](report-suite-mapping.md).

## Etapa 4. (Adobe Analytics) Atualizar o código do Analytics AppMeasurement {#section_1798D9D0F05C47E29816AC4EEB9A0913}

Verifique se você está na coleção de dados regionais (RDC). Se o domínio de coleta de dados for [!DNL omtrdc.net] ou se CNAME estiver mapeado para [!DNL omtrdc.net], você estará na RDC. Consulte [Transição para RDC](https://docs.adobe.com/content/help/pt-BR/analytics/technotes/rdc/regional-data-collection.html) para obter mais informações. Se você estiver usando cookies primários, consulte o [CNAME e o Serviço da Experience Cloud ID](https://docs.adobe.com/content/help/pt-BR/id-service/using/reference/analytics-reference/cname.html) para obter informações sobre coleta de dados CNAMEs e rastreamento entre domínios.

Recomenda-se modernizar sua implementação do Analytics ao atualizar suas bibliotecas do JavaScript, incluindo a API do visitante. A maneira simples de fazer isso é adicionar uma ferramenta do [!DNL Adobe Analytics] no Dynamic Tag Management, especificando *`Automatic`* como o método de configuração.

No [!UICONTROL Dynamic Tag Management], clique em **[!UICONTROL <Web Property Name>]** > **[!UICONTROL  Visão geral ]** > **[!UICONTROL  Adicionar uma ferramenta ]** > **[!UICONTROL  Adobe Analytics ]**. Consulte [Configurações do Adobe Analytics](https://docs.adobe.com/content/help/pt-BR/dtm/using/tools/analytics-dtm.html) no Dynamic Tag Management para obter informações sobre a implantação.

## Etapa 5. (Adobe Target) Atualizar a implementação do Adobe Target {#section_C2F4493C7A36406DAE2266B429A4BD24}

* É recomendável adicionar uma [Extensão do Adobe Target](https://docs.adobe.com/content/help/pt-BR/launch/using/extensions-ref/adobe-extension/targetv2-extension/adobe-target-extension-v2.html) ao [!UICONTROL Experience Platform Launch], para que a recuperação da biblioteca seja automática. Você também pode configurar a [extensão do Serviço da Experience Cloud ID](https://docs.adobe.com/content/help/pt-BR/launch/using/extensions-ref/adobe-extension/id-service-extension/overview.html) para o Adobe Target (e outras soluções) usando o [!UICONTROL Experience Platform Launch]. A atualização do [!UICONTROL Serviço da Experience Cloud ID] **é necessária** para que o Adobe Target use os serviços principais. (Se você usar o [!UICONTROL Dynamic Tag Management], adicione uma [ferramenta do Adobe Target](https://docs.adobe.com/content/help/pt-BR/dtm/using/tools/target.html). Além disso, você pode usar o [!UICONTROL Dynamic Tag Management] para implantar o Serviço da Experience Cloud ID para o Adobe Target.)
* Se não estiver usando o [!UICONTROL Experience Platform Launch] ou o [!UICONTROL Dynamic Tag Management], [atualize a biblioteca mbox](https://docs.adobe.com/content/help/pt-BR/target/using/implement-target/client-side/mbox-implement/target-download-config-mbox.html) manualmente.
* Solicite acesso para usar o Adobe Analytics como a fonte de relatórios para o [!DNL Adobe Target]. [!DNL Target] Os [!DNL Analytics] dados do e do são combinados na mesma chamada de servidor durante o processamento para que os visitantes sejam conectados entre as duas soluções. Consulte [Análise para implementação do Target](https://docs.adobe.com/content/help/pt-BR/target/using/integrate/a4t/a4t.html).

   >[!IMPORTANT]
   >
   >Todos os clientes do Analytics já foram provisionados com os serviços principais, como atributos do cliente. Se você não for um cliente do Analytics, entre em contato com o Atendimento ao cliente para solicitar o provisionamento.

## Etapa 6. Verificar a implementação {#section_E641782A0F4F44AF8C9C91216BE330D5}

Use o processo a seguir para garantir que o Serviço da Experience Cloud ID seja implementado corretamente no site.

1. Apague os cookies do site para que você possa ver a solicitação para o Serviço da Experience Cloud ID (a solicitação ocorre na primeira visita e, em seguida, aproximadamente uma vez por visitante, por semana).
1. Usando um analisador de pacote ou o painel de rede em um depurador de navegador da Web, procure por uma solicitação em [!DNL dpm.demdex.net].
1. Confira se a resposta possui `d_mid` e um valor, por exemplo: `_setMarketingCloudFields({"d_mid":"4235...`
1. Verifique se a solicitação do Analytics possui um parâmetro `mid` (a Experience Cloud ID). Durante o período de carência (se estiver ativado), você também deve ver um parâmetro `aid` (a ID do visitante do Analytics).

Resposta esperada contendo a Experience Cloud ID:

![](assets/mac_id_response.png)

Solicitação de imagem do Analytics que contém a Experience Cloud ID (também conhecida como `mid` ou _ID do visitante_):

![](assets/mid.png)

Experience Cloud ID na solicitação da mbox:

![](assets/mbox_request.png)

### Qual é o período de carência?

Depois de implantar o Serviço da Experience Cloud ID, os novos visitantes não receberão uma ID de visitante do Analytics de um servidor de coleta de dados. Se as seções no site ainda não implementaram o Serviço da Experience Cloud ID, quando os visitantes navegam até essas seções, a Experience Cloud ID não é reconhecida e os visitantes recebem uma ID de visitante herdada do Analytics. Isso pode causar possíveis problemas, incluindo visitas duplicadas e atribuições incorretas.

Por exemplo, se a seção de suporte do seu site for gerenciada em um CMS diferente, você terá um arquivo JavaScript do Analytics diferente para essa seção. Se você implantar a Experience Cloud ID no site principal antes de implantar o serviço de ID no site de suporte, os novos visitantes receberão uma ID do Analytics herdada quando visitarem a seção de suporte, e as visitas que abrangem ambas as seções do site serão relatadas como visitas diferentes.

Implantar o Serviço da Experience Cloud ID nos sites que usam vários arquivos JavaScript ou outras tecnologias (como o Flash) pode gerar problemas de coordenação, pois é necessário ativar o Serviço da Experience Cloud ID em todas as partes do site ao mesmo tempo. Ao configurar um período de carência, os novos visitantes continuam a receber uma ID de visitante do Analytics pelo serviço de ID, portanto, os visitantes podem ser identificados consistentemente em seções do site que não foram atualizadas para usar o serviço de ID de visitante.

## Etapa 7. Gerenciar usuários e produtos {#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF}

Quando tudo estiver funcionando, navegue até o [Admin Console](https://adminconsole.adobe.com/), onde é possível gerenciar usuários e perfis de produto.

![](assets/menu-administration-shell.png)

Consulte [Gerenciamento de usuários e produtos da Experience Cloud](../admin-getting-started/admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909).

### Atributos do cliente

Os usuários adicionados ao grupo [!UICONTROL Atributos do cliente] verão o item de menu [!UICONTROL Atributos do cliente] à esquerda da interface da Experience Cloud.

## Etapa 8. Começar a compartilhar dados de atributo e público-alvo {#section_960C06093623462E8EA247B3E97274A1}

Tire proveito dos seguintes recursos.

### [!UICONTROL People] > [!UICONTROL Atributos do cliente]

Se você capturar os dados de clientes de empresas em um banco de dados de gerenciamento de relacionamento com o cliente (CRM), poderá fazer upload dos dados em uma fonte de dados do atributo do cliente na Experience Cloud. Depois de enviado, aproveite os dados no [!DNL Adobe Analytics] e no [!DNL Adobe Target].

Consulte [Atributos do cliente](../attributes/attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1)

### [!UICONTROL People] > [!UICONTROL Biblioteca de público-alvo]

O [!UICONTROL Públicos-alvo] da Experience Cloud é a interface que permite criar públicos-alvo, combinar públicos-alvo existentes para criar públicos-alvo compostos e exibir todos os públicos-alvo compartilhados.

Consulte [Públicos-alvo](../audience-library/audience-library.md#topic_679810123CAA4E0CA4FA3417FB0100C7)

## Armazenamento de dados e divulgação de privacidade

Caso você use a definição de perfil do público-alvo em tempo real e outros serviços principais da Adobe [!DNL Experience Cloud], esses serviços podem afetar o data center (e país) em que estão seus dados. Especificamente, visto que os serviços principais do Adobe [!DNL Experience Cloud] usam o Adobe Audience Manager, os dados usados no serviço [!UICONTROL People] devem ficar nos servidores do Audience Manager nos Estados Unidos.

Ao aproveitar os serviços principais disponibilizados pelo serviço [!UICONTROL People], os tipos de dados enviados de outros produtos da Adobe para o gerenciamento de público-alvo são:

* Pares de valor/principais do [!DNL Analytics] (props, eVars, list vars e assim por diante). Por padrão, as linhas de log incluem endereço IP, inclusive o último octeto do IP (se o endereço IP não tiver sido modificado pelas configurações de ofuscação de IP no Adobe [!DNL Analytics]).
* Características e segmentos para os quais os visitantes se qualificam com base nas regras configuradas no Audience Manager.
* (Opcional) Uma ou mais IDs. Dependendo da implementação do serviço de ID, também é possível enviar uma ou mais IDs, como IDs CRM ou endereços de email em hash. Se os dados forem enviados para o Adobe [!DNL Analytics], serão transferidos para o gerenciamento de público-alvo da Adobe. A Adobe não recomenda fornecer dados pessoais ao Adobe [!DNL Analytics]. Em vez disso, use um hash unidirecional para mascarar os dados antes de enviá-los para a Adobe.
* Segmentos originados no [!DNL Analytics] através do segmento back-end que compartilha o recurso.
* O cookie demdex.net será configurado se os cookies de terceiros não estiverem bloqueados. O cookie próprio `AMCV_###@AdobeOrg` sempre está configurado com o Serviço da Experience Cloud ID.

Todos esses elementos de dados são fornecidos para o Adobe Audience Manager na forma de arquivos de log. O Audience Manager processa e armazena os dados nos Estados Unidos. O Audience Manager não fornece uma opção para armazenar ou processar esses dados fora dos Estados Unidos.

### Cookies e opções de não participação

Usar a definição de perfil do público-alvo em tempo real potencializa o cookie do Audience Manager, além dos cookies usados no [!DNL Analytics] e no [!DNL Target].

Se você desejar oferecer a capacidade de não participação adequada, os visitantes do seu site devem adicionar a opção de não participação do Audience Manager ao seu processo atual de não participação.

Consulte [Adobe Experience Cloud - Implementação das opções de não participação da Adobe](https://docs.adobe.com/content/help/pt-BR/analytics/implementation/js/opt-out.html) para obter instruções.

Consulte [Coletas de dados CNAMEs e Rastreamento entre domínios](https://docs.adobe.com/content/help/pt-BR/id-service/using/reference/analytics-reference/cname.html) para ativar o rastreamento entre domínios.
