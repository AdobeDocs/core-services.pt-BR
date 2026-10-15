---
title: Escolha um domínio de coleção de dados
description: Saiba mais sobre os domínios que você pode usar para enviar dados para o Adobe e como encontrar a ID de locatário da sua organização.
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
    internal-label: CX Enterprise
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
  - id: d3cdead0-685a-4489-9250-4bb709942f66
    internal-label: Data collection
source-git-commit: e1185eeafc809b036b10955880536db7a576ca0b
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 3%
---
# Escolha um domínio de coleta de dados

O domínio de coleta de dados é o nome do host para o qual a implementação envia dados. Todos os produtos da Adobe CX Enterprise que usam a coleta de dados do Adobe (como Adobe Analytics, Customer Journey Analytics, Adobe Experience Platform, Adobe Target e Adobe Journey Optimizer) dependem desse domínio.

## Opções de domínio para coleta de dados

| Opção | Domínio de implementação | [RDC](rdc.md) bloqueada por região | Manutenção do certificado |
| --- | --- | --- | --- |
| [Domínio de terceiros](#third-party) | `example.data.adobedc.net` | Incompatível | Nenhum |
| Domínio próprio com um [certificado gerenciado pela Adobe](adobe-managed-cert.md) | `data.example.com` | Suportado | Nenhum (o Adobe renova o certificado automaticamente) |
| Domínio próprio com um [certificado gerenciado pelo cliente](customer-managed-cert.md) | `data.example.com` | Suportado | Sua organização renova o certificado e o fornece à Adobe |
| [Rede de entrega de conteúdo (CDN) com origem de terceiros](cdn.md#third-party-origin) | `data.example.com` | Incompatível | Nenhum |
| [CDN com origem própria](cdn.md#first-party-origin) | `data.example.com` | Suportado | Sua organização renova o certificado e o fornece à Adobe |

## Domínio de coleção de dados de terceiros {#third-party}

Se você não usa um domínio próprio, envie dados para um subdomínio de `data.adobedc.net`. A Adobe recomenda usar a [ID de locatário](#tenant-id) da sua organização como subdomínio. Por exemplo, `example.data.adobedc.net`. Este domínio também é a origem recomendada quando você [roteia a coleta de dados por meio de uma CDN](cdn.md).

* Domínios de terceiros sempre usam o [tipo de RDC](rdc.md#third-party-data-collection) padrão.
* Não use subdomínios mais profundos do que `example.data.adobedc.net`. Por exemplo, `custom.example.data.adobedc.net` não é um domínio de coleção de dados válido.
* Implementações mais antigas podem usar domínios como `sc.omtrdc.net` ou `2o7.net`. Embora esses domínios ainda sejam válidos, a Adobe recomenda usar o `data.adobedc.net` quando possível.

### Encontrar a ID do locatário {#tenant-id}

1. Faça logon no [Adobe CX Enterprise](https://experience.adobe.com) usando suas credenciais do Adobe ID.
1. Em qualquer lugar na interface do CX Enterprise, pressione `[Cmd]` + `[I]` (macOS) ou `[Ctrl]` + `[I]` (Windows).
1. Um **[!UICONTROL Depurador de dados do usuário]** é exibido. Selecione a guia **[!UICONTROL Organizações atribuídas]**.
1. Expanda a organização IMS desejada.
1. Localize o campo **[!UICONTROL Locatário]**. Esse valor é a ID do locatário.

Sua ID de locatário é diferente da ID de organização IMS, que termina em `@AdobeOrg`. Cada organização IMS tem uma ID de locatário. Se sua empresa usa várias organizações IMS, cada organização tem sua própria ID de locatário.

## Atualizar a implementação {#update-implementation}

Ao alterar o domínio de coleta de dados, atualize cada implementação que envia dados para a Adobe:

* **Extensão de marca do Web SDK**: atualize o campo [[!UICONTROL Domínio do Edge]](https://experienceleague.adobe.com/en/docs/experience-platform/tags/extensions/client/web-sdk/configure/general) ao configurar a extensão.
* **Web SDK (liga)**: atualize a propriedade [`edgeDomain`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/edgedomain) no comando `configure`.
* **Extensão do Adobe Analytics**: atualize o campo [[!UICONTROL Servidor de Rastreamento SSL]](https://experienceleague.adobe.com/en/docs/experience-platform/tags/extensions/client/analytics/overview) ao configurar a extensão. Verifique se você também tem a [extensão de tag do Serviço de ID de visitante](https://experienceleague.adobe.com/en/docs/experience-platform/tags/extensions/client/id-service/overview) instalada. Consulte [Identificação do visitante usando a extensão de tag do Analytics](https://experienceleague.adobe.com/en/docs/analytics/implementation/id/analytics-extension) para obter mais informações.
* **AppMeasurement**: atualize a variável de configuração [`trackingServerSecure`](https://experienceleague.adobe.com/en/docs/analytics/implementation/vars/config-vars/trackingserversecure). Verifique se você também implementou o [Serviço de ID de Visitante](https://experienceleague.adobe.com/pt-br/docs/id-service/using/home) usando o `VisitorAPI.js`. Consulte [Identificação do visitante usando o AppMeasurement](https://experienceleague.adobe.com/en/docs/analytics/implementation/id/appmeasurement) para obter mais informações.
* **Outras implementações**: atualize o domínio de coleta de dados em qualquer outra implementação que envie dados para a Adobe, como aplicativos móveis ou implementações do lado do servidor.

Se sua implementação não usar o Serviço de ID de visitante ou o Web SDK, a alteração do domínio de coleta de dados alterará o domínio dos cookies do visitante e os visitantes recorrentes poderão ser contados como novos visitantes.

Se o site usar vários métodos de implementação e você não puder atualizar todos eles simultaneamente, considere configurar um período de carência. Consulte [Considerações sobre a migração do Serviço de ID de visitante](https://experienceleague.adobe.com/en/docs/analytics/implementation/id/migration) para obter etapas adicionais sobre como evitar que os visitantes sejam contados como novos visitantes em seu site.
