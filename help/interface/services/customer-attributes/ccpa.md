---
title: Suporte a atributos do cliente para a California Consumer Privacy Act
description: Saiba mais sobre o suporte a atributos do cliente para a California Consumer Privacy Act.
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 320defc7-2cd5-4481-955d-77cf6fbfef6d
source-git-commit: 361175f290d73f1637673420700874a2415e3fca
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 57%

---

# Suporte a atributos do cliente para a California Consumer Privacy Act

Esta página descreve o suporte de [!UICONTROL atributos do cliente] para a California Consumer Privacy Act (CCPA).

>[!IMPORTANT]
>
>O conteúdo deste documento não é um aconselhamento jurídico e não se destina a substituir tal aconselhamento. Consulte seu advogado para obter recomendações sobre a (CCPA).

A CCPA é a nova lei de privacidade da Califórnia, que entrou em vigor em 1º de janeiro de 2020. A CCPA fornece aos moradores da Califórnia novos direitos sobre suas informações pessoais e impõe responsabilidades de proteção de dados a determinadas entidades que exercem negócios na Califórnia. A CCPA dá aos consumidores o direito de acessar e apagar suas informações pessoais, bem como o direito de optar pela não participação em certas atividades qualificadas como &quot;venda&quot; de informações pessoais a terceiros.

Como empresa, você determinará os dados pessoais que a Adobe Experience Cloud processa e armazena em seu nome.

Como seu provedor de serviço, a Adobe Experience Cloud fornece suporte para que sua empresa cumpra as obrigações da CCPA aplicáveis ao uso de produtos e serviços da Experience Cloud. Isto inclui o gerenciamento de solicitações para acessar e excluir informações pessoais.

Este documento descreve como os [!UICONTROL atributos do cliente] oferecem suporte aos direitos de acesso e exclusão de dados da CCPA dos titulares de dados usando a API do Adobe Experience Platform Privacy Service e a interface do usuário do Privacy Service.

Para obter mais informações sobre os serviços de privacidade da Adobe para CCPA, consulte o [Centro de privacidade da Adobe](https://www.adobe.com/privacy/ccpa.html).

## Configuração necessária para enviar solicitações para [!UICONTROL atributos do cliente]

Para fazer solicitações de acesso e exclusão de dados para [!UICONTROL atributos do cliente], você deve:

1. Identificar o seguinte:

   * [ID da organização](../../administration/organizations.md)
   * ID de alias da Fonte de dados CRS na qual você deseja agir
   * ID do CRM do perfil no qual você deseja agir

   Sua ID da organização é uma sequência de 24 caracteres alfanuméricos anexada com @AdobeOrg. Você precisa da ID da organização para enviar solicitações à API de privacidade. Entre em contato com o Atendimento ao cliente da Adobe, em `gdprsupport@adobe.com`, caso não consiga localizar a ID.

1. No [!UICONTROL Privacy Service], você pode enviar solicitações de Acesso e Exclusão aos atributos do cliente e verificar o status das solicitações existentes.

## Valores de campo obrigatórios em [!UICONTROL solicitações JSON de atributos do cliente]

&quot;company context&quot;:

* &quot;namespace&quot;: **imsOrgID**
* &quot;value&quot;: &lt;*valor da ID da sua organização*>

&quot;users&quot;:

* &quot;key&quot;: &lt;*geralmente o nome do cliente*>
* &quot;ação&quot;: **acessar** ou **excluir**
* &quot;user IDs&quot;:
   * &quot;namespace&quot;: &lt;*ID de alias da fonte de dados CRS*>
   * &quot;type&quot;: **integrationCode**
   * &quot;value&quot;: &lt;*ID do CRM*>
* &quot;include&quot;: **CRS** (produto da Adobe que se aplica à solicitação)
* &quot;regulation&quot;: **ccpa** (regulamento de privacidade que se aplica à solicitação)

## Exemplo de solicitação JSON

```json
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

```json
attributes:
{
"value": "<*value*>",
"key": "<*key*>",
"displayName": "<*displayName*>"
}
```
