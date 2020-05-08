---
title: Suporte a atributos do cliente para o Regulamento geral de proteção de dados
description: Suporte a atributos do cliente para o Regulamento geral de proteção de dados
translation-type: tm+mt
source-git-commit: 3a86aed0794c3e35cc028e5bfde5dafcb2285fc8
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 5%

---


# Suporte a atributos do cliente para o Regulamento geral de proteção de dados


>[!IMPORTANT]
>
>O conteúdo deste documento não é um aconselhamento jurídico e não se destina a substituir tal aconselhamento. Consulte o seu advogado para obter aconselhamento sobre o Regulamento Geral sobre Proteção de Dados.

O Regulamento [](https://www.adobe.com/privacy/general-data-protection-regulation/what-is-gdpr.html) Geral sobre a Proteção de Dados (RGPD), uma lei em vigor em 25 de maio de 2018, confere a todos os indivíduos (pessoas em causa) dentro das fronteiras da União Europeia (UE) o controlo dos seus dados pessoais e simplifica o ambiente regulamentar para as empresas internacionais. Esta lei aplica-se a todas as empresas (responsáveis pelo tratamento de dados) que ofertas bens ou serviços para, monitorizem o comportamento de pessoas singulares dentro das fronteiras da UE, ou recolhem dados pessoais, no momento em que os seus dados pessoais são tratados, independentemente da localização comercial do responsável pelo tratamento.

A Adobe Experience Cloud atua como um processador de dados para todos os dados pessoais que recebe e armazena em nome de seus clientes. Como controlador de dados, você determina os dados pessoais que a Adobe Experience Cloud processa e armazena em seu nome.

Este documento descreve como os Atributos do cliente suportam os direitos de acesso e exclusão de dados do RGPD das pessoas usando a API do Adobe Experience Platform Privacy Service e a interface do usuário do Privacy Service.

Para obter mais informações sobre o que o RGPD significa para sua empresa, consulte [RGPD e Sua empresa](https://www.adobe.com/br/privacy/general-data-protection-regulation.html).

## Configuração necessária para enviar solicitações para atributos do cliente

Para fazer solicitações de acesso e exclusão de dados para Atributos do cliente, é necessário:

1. Identifique o seguinte:

* ID da Org. de IMS
* ID de alias da Fonte de Dados CRS na qual você deseja agir
* ID do CRM do perfil no qual você deseja agir

Uma ID de organização IMS é uma sequência de 24 caracteres alfanuméricos anexada com @AdobeOrg. Se a sua equipe de marketing ou o administrador interno do sistema da Adobe não souber a ID da empresa IMS, entre em contato com o Atendimento ao cliente da Adobe em gdprsupport@adobe.com. Você precisará da ID de empresa IMS para enviar solicitações à API de privacidade.

2. Use a interface do usuário do Privacy Service para enviar acesso e excluir solicitações aos Atributos do cliente e verificar o status das solicitações existentes.

## Valores de campo obrigatórios em solicitações JSON de atributos do cliente

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

* &quot;Regulamento&quot;: **gdpr** (que é o regulamento de privacidade aplicável ao pedido)

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
