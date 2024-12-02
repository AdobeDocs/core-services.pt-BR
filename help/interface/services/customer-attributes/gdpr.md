---
title: '[!DNL Customer Attributes] Suporte ao Regulamento Geral sobre a Proteção de Dados'
description: Saiba mais sobre o Suporte a atributos do cliente para o Regulamento Geral sobre a Proteção de Dados
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 02417c0c-6780-4699-9470-f1685c3cd25d
source-git-commit: c39672f0d8a0fd353b275b2ecd095ada1e2bf744
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 98%

---

# Suporte a [!DNL Customer Attributes] para o Regulamento Geral sobre a Proteção de Dados

Esta página descreve como o [!DNL Customer Attributes] oferece suporte ao Regulamento Geral sobre a Proteção de Dados (RGPD).

>[!IMPORTANT]
>
>O conteúdo deste documento não é um aconselhamento jurídico e não se destina a substituir tal aconselhamento. Consulte seu advogado para obter recomendações sobre o GDPR.

O [Regulamento Geral sobre a Proteção de Dados](https://business.adobe.com/br/privacy/general-data-protection-regulation.html), uma lei em vigor desde 25 de maio de 2018 concede a todos os indivíduos (titulares de dados) dentro das fronteiras da União Europeia (UE) o controle de seus dados pessoais. Também simplifica o ambiente regulamentar para as empresas internacionais. Esta lei se aplica a todas as empresas (controladores de dados) que oferecem bens ou serviços para monitorar o comportamento ou coletar dados pessoais de indivíduos dentro das fronteiras da UE no momento em que seus dados pessoais são processados, independentemente da localização comercial do controlador de dados.

A Adobe Experience Cloud atua como um processador de dados para todos os dados pessoais que recebe e armazena em nome de seus clientes. Como o controlador de dados, você determinará os dados pessoais que a Adobe Experience Cloud processa e armazena em seu nome.

Este documento descreve como o [!DNL Customer Attributes] oferece suporte aos direitos de acesso e exclusão de dados de titulares do GDPR usando a Adobe Experience Platform Privacy Service API e a interface do Privacy Service.

Para obter mais informações sobre o que o GDPR significa para sua empresa, consulte [GDPR e sua empresa](https://business.adobe.com/br/privacy/general-data-protection-regulation.html).

## Configuração necessária para enviar solicitações para os [!DNL Customer Attributes]

Para fazer solicitações de acesso e exclusão de dados para [!DNL Customer Attributes], você deve:

1. Identificar o seguinte:

   * [ID da organização](../../administration/organizations.md)
   * ID de alias da Fonte de dados CRS na qual você deseja agir
   * ID do CRM do perfil no qual você deseja agir

   Sua [ID da organização](../../administration/organizations.md) é uma string de 24 caracteres alfanuméricos anexada com @AdobeOrg. Você precisa da ID da organização para enviar solicitações à API de privacidade. Entre em contato com o Atendimento ao cliente da Adobe, em `gdprsupport@adobe.com`, caso não consiga localizar a ID.

1. O [!UICONTROL Privacy Service] permite enviar solicitações de acesso e exclusão aos [!DNL Customer Attributes] e verificar o status das solicitações existentes.

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
* &quot;regulation&quot;: **GDPR** (regulamento de privacidade que se aplica à solicitação)

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
