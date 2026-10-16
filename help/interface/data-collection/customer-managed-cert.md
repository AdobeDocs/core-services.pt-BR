---
title: Certificados gerenciados pelo cliente
description: Saiba quando usar um certificado gerenciado pelo cliente para a coleta de dados próprios e as responsabilidades de sua organização para renová-lo.
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
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: d3cdead0-685a-4489-9250-4bb709942f66
    internal-label: Data collection
source-git-commit: 18fd590d6f0fd1800e3d5c62851453aa91d9db5f
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 1%
---
# Certificados gerenciados pelo cliente

Com um certificado gerenciado pelo cliente, sua organização obtém o certificado para o nome de host da coleta de dados primária e o fornece à Adobe. O Adobe hospeda o certificado em seus servidores de coleta de dados. Sua organização é responsável por renovar o certificado e fornecer cada certificado renovado à Adobe antes que o certificado atual expire.

>[!TIP]
>
>A Adobe recomenda o [programa de certificados gerenciados pela Adobe](adobe-managed-cert.md) para a maioria das implementações primárias. É mais seguro e renova certificados automaticamente. Use um certificado gerenciado pelo cliente somente quando sua organização exigir.

## Quando usar um certificado gerenciado pelo cliente

* **Você encaminha a coleta de dados por meio de uma CDN com origem própria**: o [programa de certificados gerenciados pela Adobe](adobe-managed-cert.md) não oferece suporte a implementações de CDN. Consulte [Configurar um CDN com origem própria](cdn.md#first-party-origin).
* **Sua política de segurança requer o controle direto do certificado**: por exemplo, sua organização deve poder revogar o certificado por meio de sua própria autoridade de certificação, em vez de solicitar a revogação pelo Atendimento ao Cliente da Adobe.
* **Sua organização requer uma autoridade de certificação específica ou um tipo de certificado**: o programa de certificados gerenciados pela Adobe usa certificados emitidos pela DigiCert.

## Comparar métodos de certificado

| | Certificado gerenciado pela Adobe | Certificado gerenciado pelo cliente |
| --- | --- | --- |
| **Quem obtém o certificado** | Adobe, por meio da DigiCert | Sua organização, por meio de uma autoridade de certificação comercial de sua escolha |
| **Renovações** | O Adobe renova o certificado automaticamente | Sua organização renova o certificado e o fornece à Adobe antes de cada expiração |
| **Tipos de certificado** | A Adobe fornece certificados RSA e ECC | RSA é necessário; ECC é recomendado |
| **Compatível com um CDN** | Não | Sim, como origem própria |

## Configurar um certificado gerenciado pelo cliente

1. Entre em contato com o Atendimento ao cliente da Adobe para solicitar a coleta de dados primários com um certificado gerenciado pelo cliente. Inclua seu nome de host próprio, como `data.example.com`. Se sua organização tiver requisitos de residência ou conformidade de dados, especifique o [tipo de RDC](rdc.md) desejado em sua solicitação.
1. O Atendimento ao cliente da Adobe fornece uma solicitação de assinatura de certificado (CSR) para seu nome de host. O Adobe gera e mantém a chave privada, de modo que sua organização nunca lida com a chave privada. A Adobe exige um certificado RSA e recomenda um certificado ECC. Cada tipo de certificado exige seu próprio CSR. Portanto, se você quiser um certificado ECC, peça ao Atendimento ao cliente da Adobe um CSR ECC.
1. Envie cada CSR à autoridade de certificação comercial desejada para obter um certificado assinado. Os serviços de certificados gratuitos não são suportados. Forneça os certificados emitidos à Adobe, conforme instruído pelo Atendimento ao cliente.
1. Depois que o Adobe instalar seu certificado, direcione o tráfego do nome do host para o Adobe:
   * **Sem um CDN**: atualize os registros DNS da sua organização, conforme instruído pelo Atendimento ao Cliente da Adobe.
   * **Com um CDN**: defina sua origem de CDN como seu nome de host primário. Consulte [Configurar um CDN com origem própria](cdn.md#first-party-origin).
1. Se a sua implementação ainda não enviar dados para este nome de host, [atualize sua implementação](collection-domain.md#update-implementation).

## Renovar o certificado {#renewals}

Sua organização é responsável por renovar o certificado e fornecê-lo ao Atendimento ao cliente da Adobe antes que o certificado atual expire.

Se o certificado nos servidores da Adobe expirar, os navegadores e CDNs rejeitarão conexões com seu nome de host e os dados dessas solicitações serão perdidos. Um CDN pode descartar esses dados sem notificá-lo.

A duração máxima do certificado está diminuindo, o que torna as renovações mais frequentes. Consulte [6.3.2 Períodos operacionais do certificado e períodos de uso do par de chaves](https://cabforum.org/working-groups/server/baseline-requirements/requirements/#632-certificate-operational-periods-and-key-pair-usage-periods) nos Requisitos de Linha de Base do Certificado do Servidor do Fórum da CA/Navegador para obter mais informações. Para evitar lacunas na coleta de dados:

* Rastreie a data de expiração de cada certificado fornecido à Adobe.
* Atribua um proprietário para renovações e documente o processo de renovação para que ele continue por meio de alterações na equipe.

No momento, a Adobe está explorando um processo de renovação de certificado de autoatendimento.

## Parar de usar um certificado gerenciado pelo cliente

* **Para migrar para o programa de certificados gerenciados pela Adobe**: Entre em contato com o Atendimento ao Cliente da Adobe. O programa de certificado gerenciado pela Adobe exige que seu nome de host aponte diretamente para o Adobe, não para um CDN.
* **Para parar de usar seu nome de host próprio**: atualize todas as implementações que usam o nome de host e entre em contato com o Atendimento ao Cliente da Adobe para remover o certificado dos servidores da Adobe.
* **Para mover para uma CDN com origem de terceiros**: Consulte [Mover uma implementação própria existente para uma CDN](cdn.md#migrate).
