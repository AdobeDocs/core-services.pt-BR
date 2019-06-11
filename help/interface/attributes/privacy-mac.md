---
description: Considerações e práticas recomendadas relacionadas às informações de identificação pessoal (PII) carregadas e usadas na Adobe Experience Cloud.
keywords: atributos do cliente; principais serviços
seo-description: Considerações e práticas recomendadas relacionadas às informações de identificação pessoal (PII) carregadas e usadas na Adobe Experience Cloud.
seo-title: Considerações de privacidade - atributos do cliente
solution: Experience Cloud
title: Considerações de privacidade - atributos do cliente
uuid: 5666 dc 4 e -55 fa -4196-9985-cf 530 cfb 9247
translation-type: tm+mt
source-git-commit: 979b2202a70e2a5362aa86a65a17d7c4279b3a1a

---


# Considerações de privacidade - atributos do cliente

Considerações e práticas recomendadas relacionadas às informações de identificação pessoal (PII) carregadas e usadas na Adobe Experience Cloud.


<!-- <p>https://wiki.corp.adobe.com/display/omtrplatform/Visitor+Enrichment+and+privacy#VisitorEnrichmentandprivacy-INFORMATIONASSOCIATIONOPTIONS </p> -->


* Nome e sobrenome
* Endereço residencial ou outro endereço físico
* Endereço de email
* Telefone
* Número do seguro social
* Outro identificador que permite a contratação física ou online de um indivíduo. (Varia por localização. Confira e cumpra as leis e regulamentações locais relacionadas à privacidade e às PII para todos os locais em que você faz negócios.)


A Adobe oferece as ferramentas que permitem que os anunciantes reúnam informações comportamentais sobre os clientes que visitam seus sites ou usam seus aplicativos. A Adobe também fornece ferramentas que permitem que os anunciantes aprimorem essas informações com registros offline ou externos de clientes que o anunciante possa ter em outros sistemas de gerenciamento de informações.

Um motivo comum para os anunciantes fazerem isso é melhorar as informações disponíveis ao fazer o marketing adequado ao cliente e ao tomar decisões sobre a publicidade. O Adobe Analytics e o Target permitem que seus anunciantes façam upload de informações de identificação pessoal (PII), como endereços de email, somente quando estão com hash para impossibilitar que sejam usadas a fim de entrar em contato com o indivíduo. As informações com hash também podem ser usadas para fins de análise e marketing. Como lembrete, a Adobe proíbe que os anunciantes enviem informações pessoais confidenciais para a Adobe, como registros médicos, informações de conta bancária e informações sobre menores de idade.

A Adobe sabe que esses tipos de decisões de marketing e publicidade podem ter implicações de privacidade do cliente, que é o motivo de a Adobe criar controles de privacidade para ajudar os anunciantes a atender às expectativas dos seus clientes. A Adobe recomenda que os anunciantes considerem atentamente quais informações são apropriadas para usar para fins de marketing e em quais circunstâncias o anunciante tem permissão para usá-las.

**Práticas recomendadas**

Ao fazer upload das PII para o Adobe Analytics ou o Target, a Adobe recomenda que o cliente coloque as PII com hash antes de fazer upload dessas informações para a Adobe. As informações com hash também podem ser usadas para fins de análise e marketing. Como lembrete, a Adobe proíbe que os anunciantes enviem informações pessoais confidenciais para o Adobe Analytics e o Target, como registros médicos, informações de conta bancária e informações sobre menores de idade.

A Adobe recomenda que os anunciantes considerem atentamente quais informações são apropriadas para usar para fins de marketing e em quais circunstâncias o anunciante tem permissão para usá-las.

Como a legislação de privacidade do cliente permanece em curso, a Adobe recomenda que os anunciantes respeitem três princípios comuns:

1. Faça o que você disser (na política de privacidade).
1. Diga o que você fizer (na política de privacidade).
1. Não surpreenda seus clientes.

Com essas expectativas em mente, a Adobe recomenda que quando um anunciante associar as atividades de navegação com as PII, forneça avisos ou personalização indicando que o cliente está autenticado. Um exemplo disso inclui uma saudação no cabeçalho do site. A Adobe também recomenda que os anunciantes descrevam em sua política de privacidade o tipo de informações de navegação que ela associa com as PII e sob quais circunstâncias as informações de navegação se relacionam com as PII. Por fim, a Adobe recomenda firmemente que os anunciantes analisem as opções de não participação que eles oferecem aos clientes para entender se e como eles podem usar informações de perfil não autenticadas após a opção de não participação.

<!-- <p> <b>Vinay Geol</b> should help craft privacy regarding how all MAC uses privacy/cookies. Privacy implications around each part of the workflow. Moving from CRM to MAC. Can it include PII? What is PII? What isn't PII? </p> 
<p>CRM data is Known Data or Info. Going to combine with activity that occurs when visitor was not authenticated. PII wiki: </p> 
<p>https://wiki.corp.adobe.com/display/omtrplatform/Visitor+Enrichment+and+privacy#VisitorEnrichmentandprivacy-INFORMATIONASSOCIATIONOPTIONS </p> 
<p>Refactoring of implementation docs as it relates to privacy and cookies. </p> 
<p>Add content to https://marketing.adobe.com/resources/help/en_US/mcloud/t-publish-audience-segment.html, as follows: </p> 
<p> Audiences are not filtered based on the authentication state of a visitor. If a visitor can browse your site in un-authenticated and authenticated states, actions that occur when a visitor is un-authenticated can still cause a visitor to be included in an audience. Please review <link> to understand the full privacy implications of audience sharing. </p> 
<p>That "link" goes to a topic dedicated to PII, with this text: </p> 
<p> - Adobe Analytics allows its advertisers to upload personally identifiable information (PII) such as email addresses. When uploading PII to Adobe Analytics, Adobe recommends that the customer should hash PII prior to uploading it to Adobe. Hashed information can still be used for analysis and for marketing purposes. As a reminder, Adobe prohibits advertisers from sending sensitive personal information to Adobe Analytics, such as medical records, financial account information, and information about minors. </p> 
<p> - Adobe recommends its advertisers carefully consider which information is appropriate to use for marketing purposes and in which circumstances the advertiser has permission to use such information. </p> 
<p> - As consumer privacy law remains in flux, Adobe recommends that advertisers respect three common tenets: 1) Do what you say (in your privacy policy); 2) Say what you do (in your privacy policy); and 3) Don't surprise your consumers. </p> 
<p> - With these expectations in mind, Adobe recommends that when an advertiser associates browsing activities to PII, the advertiser provide notices/personalization indicating that the consumer is authenticated. An example of this is including a 'Hello, Jane' greeting within the header of the website. Adobe also recommends that advertisers describe in its privacy policy what type of browsing information it associates with PII and under what circumstances browsing information is associated with PII. Lastly, Adobe strongly recommends advertisers review the opt out choices they provide their consumers to understand whether and how they can use unauthenticated profile information post opt out. </p> 
<p>Possibly revamp the cookies to include privacy, with best practices: https://marketing.adobe.com/resources/help/en_US/whitepapers/cookies/ </p> -->
