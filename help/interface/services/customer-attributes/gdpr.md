---
title: '[!DNL Customer Attributes] Suporte ao Regulamento Geral sobre a Proteção de Dados'
description: Saiba mais sobre o suporte de Atributos do cliente para o Regulamento Geral sobre a Proteção de Dados
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 02417c0c-6780-4699-9470-f1685c3cd25d
TQID: https://experienceleague.adobe.com/wU6Y5XK5Fs9-w7Jl7THXjturzTVrsB7eh7GdExsS2TQ
product_v2:
  - id: e1971122-7081-4556-9222-8a31bd71800c
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: a42153ba5a885509e7735e7407e38586fcabb0ad
workflow-type: tm+mt
source-wordcount: 407
ht-degree: 82%

---

# Suporte a [!DNL Customer Attributes] para o Regulamento Geral sobre a Proteção de Dados

Esta página descreve como o [!DNL Customer Attributes] oferece suporte ao Regulamento Geral sobre a Proteção de Dados (RGPD).

>[!IMPORTANT]
>
>O conteúdo deste documento não é um aconselhamento jurídico e não se destina a substituir tal aconselhamento. Consulte seu advogado para obter recomendações sobre o RGPD.

O [Regulamento Geral sobre a Proteção de Dados](https://business.adobe.com/br/privacy/general-data-protection-regulation.html), uma lei em vigor desde 25 de maio de 2018 concede a todos os indivíduos (titulares de dados) dentro das fronteiras da União Europeia (UE) o controle de seus dados pessoais. Também simplifica o ambiente regulamentar para os negócios internacionais. Esta lei se aplica a todos os negócios (controladores de dados) que oferecem bens ou serviços para monitorar o comportamento ou coletar dados pessoais de indivíduos dentro das fronteiras da UE no momento em que seus dados pessoais são processados, independentemente da localização comercial do controlador de dados.

A Adobe CX Enterprise atua como um processador de dados para todos os dados pessoais que recebe e armazena em nome de seus clientes. Como controlador de dados, você determinará os dados pessoais que a Adobe CX Enterprise processa e armazena em seu nome.

Este documento descreve como o [!DNL Customer Attributes] oferece suporte aos direitos de acesso e exclusão de dados de titulares do RGPD usando a Adobe Experience Platform Privacy Service API e a interface do Privacy Service.

Para obter mais informações sobre o que o RGPD significa para sua empresa, consulte [RGPD e sua empresa](https://business.adobe.com/br/privacy/general-data-protection-regulation.html).

## Configuração necessária para enviar solicitações para os [!DNL Customer Attributes]

Para fazer solicitações de acesso e exclusão de dados para [!DNL Customer Attributes], você deve:

1. Identificar o seguinte:

   * [ID da organização](../../administration/organizations.md)
   * ID de alias da Fonte de dados CRS na qual você deseja agir
   * ID do CRM do perfil no qual você deseja agir

   Sua [ID da organização](../../administration/organizations.md) é uma string de 24 caracteres alfanuméricos anexada com @AdobeOrg. Você precisa da ID da organização para enviar solicitações à API de privacidade. Entre em contato com o Atendimento ao cliente da Adobe, em `gdprsupport@adobe.com`, caso não consiga localizar a ID.

1. Em [!UICONTROL Privacy Service], você pode enviar solicitações de Acesso e Exclusão para [!DNL Customer Attributes] e verificar o status das solicitações existentes.

## Valores de campo obrigatórios em solicitações JSON de [!DNL Customer Attributes]

&quot;company context&quot;:

* &quot;namespace&quot;: **imsOrgID**
* &quot;value&quot;: &lt;*valor da ID de org IMS*>

&quot;users&quot;:

* &quot;key&quot;: &lt;*geralmente o nome do cliente*>
* &quot;ação&quot;: **acessar** ou **excluir**
* &quot;user IDs&quot;:
   * &quot;namespace&quot;: &lt;*ID de alias da fonte de dados CRS*>
   * &quot;type&quot;: **integrationCode**
   * &quot;value&quot;: &lt;*ID do CRM*>
* &quot;include&quot;: **CRS** (produto da Adobe que se aplica à solicitação)
* &quot;regulation&quot;: **RGPD** (regulamento de privacidade que se aplica à solicitação)

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
