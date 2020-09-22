---
description: Perguntas frequentes e respostas para administradores na Experience Cloud.
keywords: core services, Experience Cloud, Experience Platform, Analytics, Target, user management.
seo-description: Perguntas frequentes e respostas para administradores na Experience Cloud.
seo-title: Perguntas frequentes sobre os serviços principais da Experience Cloud.
solution: Experience Cloud
title: Perguntas frequentes
index: true
translation-type: tm+mt
source-git-commit: 11ce83401a12c25853cd6412413b8abf98dd6612
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 100%

---


# Perguntas frequentes sobre a Experience Cloud

Perguntas frequentes e respostas para administradores na Experience Cloud.

## Como saber se minhas soluções estão habilitadas para os serviços principais?

Se a implementação foi provisionada para os serviços principais, consulte [Ativar as soluções para serviços principais](../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C), que descreve como:

1. [Associar-se à Experience Cloud e tornar-se um administrador](../core-services/core-services.md#section_2423F0BD3DF642658103310EE5EA6154)
1. [Implementar o Serviço da Experience Cloud ID usando o Experience Platform Launch](https://docs.adobe.com/content/help/pt-BR/launch/using/intro/get-started/quick-start.html).
1. [Mapear conjuntos de relatórios para uma organização da Experience Cloud](../core-services/core-services.md#concept_apg_zq2_rw)
1. [(Somente no Analytics) Modernizar o código do Analytics AppMeasurement](../core-services/core-services.md#section_1798D9D0F05C47E29816AC4EEB9A0913)
1. [(Somente no Adobe Target) Modernizar a implementação do Adobe Target](../core-services/core-services.md#section_C2F4493C7A36406DAE2266B429A4BD24)
1. [Verificar a implementação](../core-services/core-services.md#section_E641782A0F4F44AF8C9C91216BE330D5)
1. [Gerenciar usuários e produtos](../core-services/core-services.md#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF)
1. [Começar a usar os serviços principais](../core-services/core-services.md#section_960C06093623462E8EA247B3E97274A1)

Para obter mais ajuda, [entre em contato com o Suporte da Adobe](https://helpx.adobe.com/br/marketing-cloud/contact-support.html).

## A Adobe cobra minha empresa pelo acesso à Experience Cloud?

Não. A Experience Cloud está incluída sem custos adicionais. No entanto, certos serviços principais podem ter custos adicionais.

## Por que minha empresa precisa fazer logon na interface da Experience Cloud?

A funcionalidade fornecida pela interface da Experience Cloud agrega novo valor à empresa. Também é o caminho padrão para acessar as soluções avançadas, substituindo outros fluxos de logon da solução individual em algum momento. Fazer logon pela Experience Cloud facilitará uma transição mais suave posteriormente.

## Como resolver problemas sobre como migrar minha empresa?

[Entre em contato com o Suporte da Adobe](https://helpx.adobe.com/br/marketing-cloud/contact-support.html).

## O que é _provisionamento?_

O provisionamento na Experience Cloud significa que:

* Seus usuários podem começar a fazer logon na [!DNL Experience Cloud] e a vincular soluções.
* Eles podem começar a usar os recursos disponíveis na Experience Cloud, como People.
* Prepare-se para desativar o processo de logon específico da solução.
* Você pode manter o controle de acesso das soluções.

## Como faço para gerenciar perfis de usuários e produtos?

* Consulte o [Guia do usuário do Admin Console](https://helpx.adobe.com/br/enterprise/administering/user-guide.html) para obter ajuda.

* O gerenciamento de produtos e direitos do usuário é executado no [Adobe Admin Console](https://adminconsole.adobe.com/enterprise) (link do produto).

* **Importante:** administradores do Analytics, consultem [Gerenciar usuários do Analytics no Admin Console](https://docs.adobe.com/content/help/pt-BR/analytics/admin/user-product-management/user-management/migrate-users/c-migration-tool.html) sobre como migrar IDs de usuários das Ferramentas administrativas do Analytics para o Admin Console.

## Como proceder se alguém não conseguir fazer logon na Experience Cloud?

Os administradores do Admin Console podem conceder acesso aos usuários. Os usuários recebem emails com instruções de logon.

Talvez seja necessário [Entrar em contato com o suporte da Adobe](https://helpx.adobe.com/br/marketing-cloud/contact-support.html) para verificar se a empresa foi totalmente provisionada.

## Onde um usuário pode gerenciar a vinculação de contas?

Alguns usuários podem precisar vincular a conta da solução (Analytics) à Adobe ID ou à Enterprise ID.

Consulte [Vincular uma conta da solução a uma Adobe ID](../admin-getting-started/organizations.md#task_FD389E78640848919E247AC5E95B8369).

## Como faço para gerenciar organizações e perfis de contas de usuários?

Consulte [Gerenciar contas de usuário](../admin-getting-started/organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1).

## O que é uma organização?

Uma *organização* é a entidade que permite ao administrador configurar grupos e usuários, além de controlar o logon único na Experience Cloud. A organização funciona como uma empresa para logon que abrange os produtos e as soluções da Experience Cloud. Frequentemente, a organização é o nome da empresa. No entanto, uma empresa pode ter muitas organizações.

## Onde posso encontrar minha ID da organização de IMS?

Consulte [Localização da ID da organização](organizations.md).

A ID da organização é exibida na página de aterrissagem da Experience Cloud e na [página de aterrissagem do Admin Console](https://adminconsole.adobe.com).

Como alternativa, os administradores podem fazer logon no Admin Console (acesse [https://adminconsole.adobe.com](https://adminconsole.adobe.com#)) de uma organização específica e você será capaz de visualizar a ID da organização de IMS no URL.

Por exemplo, no URL a seguir:

`https://adminconsole.adobe.com/C538193582390300A495CC9@AdobeOrg/overview`

a ID é:

`C538193582390300A495CC9@AdobeOrg`

## O que devo fazer quando um dos meus usuários sair da empresa?

O acesso deles deverá ser removido da própria solução. Eles não poderão acessar o produto pela Experience Cloud nem por meio do logon direto. Você também deve removê-los no nível da Experience Cloud.

## O que é uma Adobe ID?

Consulte [Tipos de identidade](https://helpx.adobe.com/br/enterprise/help/identity.html).

## Posso vincular as contas da solução para meus usuários?

Não. Os usuários devem vincular suas próprias soluções com os nomes de usuário e senhas.

## Por que vejo Social se a minha empresa não o possui?

O Adobe Social é um produto que pode ser vendido com o Analytics. Portanto, se você tiver o Analytics, verá essa solução, mas não terá acesso a menos que tenha comprado.
