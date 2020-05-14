---
title: Suporte aos atributos do cliente para a Lei de privacidade do consumidor da Califórnia
description: Suporte aos atributos do cliente para a Lei de privacidade do consumidor da Califórnia
translation-type: tm+mt
source-git-commit: 4223f9260865756842ad43b99d2509908f4d6572
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 4%

---


# Suporte aos Atributos do cliente para a Lei de Privacidade do Consumidor da Califórnia

Esta página descreve o suporte dos Atributos do  cliente para o California Consumer Privacy Act (CCPA).

>[!IMPORTANT]
>
>O conteúdo deste documento não é um aconselhamento jurídico e não se destina a substituir tal aconselhamento. Consulte o seu advogado para obter conselhos sobre o (CCPA).

A CCPA é a nova lei de privacidade da Califórnia, que entrará em vigor em 1º de janeiro de 2020. A CCPA fornece aos moradores da Califórnia novos direitos sobre suas informações pessoais e impõe responsabilidades de proteção de dados a determinadas entidades que exercem negócios na Califórnia. A CCPA dá aos consumidores o direito de acessar e apagar suas informações pessoais, bem como o direito de opt out certas atividades qualificadas como &quot;vendendo&quot; informações pessoais a terceiros.

Como empresa, você determinará os dados pessoais que a Adobe Experience Cloud processa e armazena em seu nome.

Como seu provedor de serviço, a Adobe Experience Cloud oferece suporte para que sua empresa cumpra suas obrigações no CCPA, aplicáveis ao uso de produtos e serviços da Experience Cloud, incluindo o gerenciamento de solicitações para acessar e excluir informações pessoais.

Este documento descreve como os Atributos [!UICONTROL do] cliente oferecem suporte aos direitos de acesso e exclusão de dados CCPA das pessoas usando a API do Adobe Experience Platform Privacy Service e a interface do usuário do Privacy Service.

Para obter mais informações sobre os serviços de privacidade da Adobe para CCPA, consulte o Centro [de privacidade da](https://www.adobe.com/privacy/ccpa.html)Adobe.

## Configuração necessária para enviar solicitações de atributos [!UICONTROL do cliente]

Para fazer solicitações de acesso e exclusão de dados para Atributos [!UICONTROL do]cliente, é necessário:

1. Identifique o seguinte:

   * ID da Org. de IMS
   * ID de alias da Fonte de Dados CRS na qual você deseja agir
   * ID do CRM do perfil no qual você deseja agir
   Uma ID de organização IMS é uma sequência de 24 caracteres alfanuméricos anexada com @AdobeOrg. Se a sua equipe de marketing ou o administrador interno do sistema da Adobe não souber a ID da empresa IMS, entre em contato com o Atendimento ao cliente da Adobe em gdprsupport@adobe.com. Você precisará da ID de empresa IMS para enviar solicitações à API de privacidade.

1. No [!UICONTROL Privacy Service], você pode enviar solicitações de Acesso e Excluir aos Atributos do cliente e verificar o status das solicitações existentes.

## Valores de campo obrigatórios em solicitações JSON de atributos [!UICONTROL do] cliente

&quot;Contexto de empresa&quot;:

* &quot;namespace&quot;: **imsOrgID**
* &quot;value&quot;: &lt;*seu valor* de ID de organização IMS>

&quot;usuários&quot;:

* &quot;key&quot;: &lt;*geralmente o nome do cliente*>

* &quot;Ação&quot;: **acessar** ou **excluir**

* &quot;IDs de usuário&quot;:

   * &quot;namespace&quot;: &lt;ID de *alias da fonte* de dados CRS>

   * &quot;Tipo&quot;: **integrationCode**

   * &quot;value&quot;: &lt;ID ** CRM>

* &quot;Incluir&quot;: **CRS** (que é o produto da Adobe que se aplica à solicitação)

* &quot;Regulamento&quot;: **ccpa** (que é a regra de privacidade que se aplica à solicitação)

## Exemplo de solicitação JSON

```
{
  "companyContexts": [
    {
      "namespace": "imsOrgID",
      "value": "<IMS_ORG_ID>"
    }
  ],
  "users": [
    {
      "key": "<KEY>",
      "action": [
        "<access/delete>"
      ],
      "userIDs": [
        {
          "namespace": "<Alias ID of CRS Data Source>",
          "type": "integrationCode",
          "value": "<CRM ID>"
        }
      ]
    }
  ],
  "regulation": "<gdpr/ccpa/pdpa>",
  "include": [
    "CRS"
  ]
}
```

## Campos de dados retornados para solicitações de acesso

```
attributes:
{
"value”:<*value*>,
"key”:<*key*>,
"displayName”:<*displayName*>
}
```
