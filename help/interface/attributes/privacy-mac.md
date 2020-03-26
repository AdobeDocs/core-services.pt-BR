---
description: Considerações e práticas recomendadas relacionadas às informações de identificação pessoal (PII) carregadas e usadas na Adobe Experience Cloud.
keywords: customer attributes;core services
seo-description: Considerações e práticas recomendadas relacionadas às informações de identificação pessoal (PII) carregadas e usadas na Adobe Experience Cloud.
seo-title: Considerações de privacidade - Atributos do cliente
solution: Experience Cloud
title: Considerações de privacidade - Atributos do cliente
uuid: 5666dc4e-55fa-4196-9985-cf530cfb9247
translation-type: tm+mt
source-git-commit: f7ec8bf6087a18be41c9efbf05f60e6cfd24e566

---


# Considerações de privacidade - Atributos do cliente

Considerações e práticas recomendadas relacionadas às informações de identificação pessoal (PII) carregadas e usadas na Adobe Experience Cloud.


<!-- <p>https://wiki.corp.adobe.com/display/omtrplatform/Visitor+Enrichment+and+privacy#VisitorEnrichmentandprivacy-INFORMATIONASSOCIATIONOPTIONS </p> -->


* Nome e sobrenome
* Endereço residencial ou outro endereço físico
* Endereço de email
* Telefone
* Número da Segurança Social
* Outro identificador que permite a contratação física ou online de um indivíduo. (Varia por localização. Verifique e cumpra as leis e regulamentos locais relacionados à privacidade e às PII para todos os locais onde você faz negócios.)


A Adobe oferece as ferramentas que permitem que os anunciantes reúnam informações comportamentais sobre os clientes que visitam seus sites ou usam seus aplicativos. A Adobe também fornece ferramentas que permitem aos anunciantes aprimorar essas informações com registros de clientes offline ou externos que o anunciante possa ter em outros sistemas de gerenciamento de informações.

Um motivo comum para os anunciantes fazerem isso é melhorar as informações disponíveis ao fazer o marketing adequado ao cliente e ao tomar decisões sobre a publicidade. O Adobe Analytics e o Target permitem que seus anunciantes façam upload de informações de identificação pessoal (PII), como endereços de email, somente quando estão com hash para impossibilitar que sejam usadas a fim de entrar em contato com o indivíduo. As informações com hash também podem ser usadas para fins de análise e marketing. Como lembrete, a Adobe proíbe que os anunciantes enviem informações pessoais confidenciais para a Adobe, como registros médicos, informações de conta financeira e informações sobre menores.

A Adobe sabe que esses tipos de decisões de marketing e publicidade podem ter implicações de privacidade do cliente, que é o motivo de a Adobe criar controles de privacidade para ajudar os anunciantes a atender às expectativas dos seus clientes. A Adobe recomenda que seus anunciantes considerem cuidadosamente quais informações são apropriadas para uso para fins de marketing e em quais circunstâncias o anunciante tem permissão para usar essas informações.

**Práticas recomendadas**

Ao fazer upload das PII para o Adobe Analytics ou o Adobe Público alvo, a Adobe recomenda que o cliente coloque as PII em hash antes de fazer upload para a Adobe. As informações com hash também podem ser usadas para fins de análise e marketing. Como lembrete, a Adobe proíbe que os anunciantes enviem informações pessoais confidenciais para o Adobe Analytics e o Adobe Público alvo, como registros médicos, informações de conta financeira e informações sobre menores.

A Adobe recomenda que seus anunciantes considerem cuidadosamente quais informações são apropriadas para uso para fins de marketing e em quais circunstâncias o anunciante tem permissão para usar essas informações.

Como a legislação de privacidade do consumidor permanece em constante mudança, a Adobe recomenda que os anunciantes respeitem três princípios comuns:

1. Faça o que você disser (na sua política de privacidade).
1. Diga o que você faz (em sua política de privacidade).
1. Não surpreenda seus consumidores.

Com essas expectativas em mente, a Adobe recomenda que quando um anunciante associar as atividades de navegação com as PII, forneça avisos ou personalização indicando que o cliente está autenticado. Um exemplo disso inclui uma saudação no cabeçalho do site. A Adobe também recomenda que os anunciantes descrevam em sua política de privacidade o tipo de informações de navegação que ela associa com as PII e sob quais circunstâncias as informações de navegação se relacionam com as PII. Por fim, a Adobe recomenda enfaticamente que os anunciantes analisem as opções de não participação que eles oferecem aos seus consumidores para entender se e como eles podem usar o opt out de publicação de informações de perfil não autenticado.

<!-- <p> <b>Vinay Geol</b> should help craft privacy regarding how all MAC uses privacy/cookies. Privacy implications around each part of the workflow. Moving from CRM to MAC. Can it include PII? What is PII? What isn't PII? </p> 
<p>CRM data is Known Data or Info. Going to combine with activity that occurs when visitor was not authenticated. PII wiki: </p> 
<p>https://wiki.corp.adobe.com/display/omtrplatform/Visitor+Enrichment+and+privacy#VisitorEnrichmentandprivacy-INFORMATIONASSOCIATIONOPTIONS </p> 
<p>Refactoring of implementation docs as it relates to privacy and cookies. </p> 
<p>Add content to t-publish-audience-segment, as follows: </p> 
<p> Audiences are not filtered based on the authentication state of a visitor. If a visitor can browse your site in un-authenticated and authenticated states, actions that occur when a visitor is un-authenticated can still cause a visitor to be included in an audience. Please review <link> to understand the full privacy implications of audience sharing. </p> 
<p>That "link" goes to a topic dedicated to PII, with this text: </p> 
<p> - Adobe Analytics allows its advertisers to upload personally identifiable information (PII) such as email addresses. When uploading PII to Adobe Analytics, Adobe recommends that the customer should hash PII prior to uploading it to Adobe. Hashed information can still be used for analysis and for marketing purposes. As a reminder, Adobe prohibits advertisers from sending sensitive personal information to Adobe Analytics, such as medical records, financial account information, and information about minors. </p> 
<p> - Adobe recommends its advertisers carefully consider which information is appropriate to use for marketing purposes and in which circumstances the advertiser has permission to use such information. </p> 
<p> - As consumer privacy law remains in flux, Adobe recommends that advertisers respect three common tenets: 1) Do what you say (in your privacy policy); 2) Say what you do (in your privacy policy); and 3) Don't surprise your consumers. </p> 
<p> - With these expectations in mind, Adobe recommends that when an advertiser associates browsing activities to PII, the advertiser provide notices/personalization indicating that the consumer is authenticated. An example of this is including a 'Hello, Jane' greeting within the header of the website. Adobe also recommends that advertisers describe in its privacy policy what type of browsing information it associates with PII and under what circumstances browsing information is associated with PII. Lastly, Adobe strongly recommends advertisers review the opt out choices they provide their consumers to understand whether and how they can use unauthenticated profile information post opt out. </p> 
<p>Possibly revamp the cookies to include privacy, with best practices: https://docs.adobe.com/content/help/en/core-services/interface/ec-cookies/cookies-privacy.html </p> -->
