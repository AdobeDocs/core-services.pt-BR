---
description: Saiba mais sobre a compatibilidade com o navegador e consulte perguntas e respostas comuns para administradores na Adobe Experience Cloud.
keywords: serviços principais, Experience Cloud, Experience Platform, Analytics, Target, User Management.
solution: Experience Cloud
title: 'Perguntas frequentes sobre a Experience Cloud '
index: true
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: 062576da-328e-4b46-9e71-5a25733d607a
source-git-commit: 00a6aa791dd08c2907cd09c17b7e2a1e62b060c1
workflow-type: ht
source-wordcount: '775'
ht-degree: 100%

---

# Perguntas frequentes sobre a Experience Cloud

Saiba mais sobre a compatibilidade com o navegador e consulte perguntas e respostas comuns para administradores no Experience Cloud.

## Quais navegadores são compatíveis com a Experience Cloud?

* Microsoft® Edge (versão atual e as duas anteriores)
* Google Chrome (versão atual e duas posteriores)
* Mozilla Firefox (versão atual e duas posteriores)
* Safari (versão atual e duas posteriores)
* Opera (versão atual e duas posteriores)

## Como saber se meus aplicativos estão habilitados para os serviços principais?

Se a implementação não foi provisionada para os serviços principais, consulte [Habilitar os aplicativos para serviços principais](core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C), que descreve como:

1. [Associar-se à Experience Cloud e tornar-se um administrador](core-services.md#section_2423F0BD3DF642658103310EE5EA6154)
1. [Implementar o Serviço da Experience Cloud ID usando o Experience Platform Launch](https://experienceleague.adobe.com/docs/experience-platform/tags/get-started/quick-start.html?lang=pt-BR).
1. [Mapear conjuntos de relatórios para uma organização da Experience Cloud](core-services.md#concept_apg_zq2_rw)
1. [(Somente no Analytics) Modernizar o código do Analytics AppMeasurement](core-services.md#section_1798D9D0F05C47E29816AC4EEB9A0913)
1. [(Somente no Adobe Target) Modernizar a implementação do Adobe Target](core-services.md#section_C2F4493C7A36406DAE2266B429A4BD24)
1. [Verifique a implementação](core-services.md#section_E641782A0F4F44AF8C9C91216BE330D5)
1. [Gerenciar usuários e produtos](core-services.md#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF)
1. [Começar a usar os serviços principais](core-services.md#section_960C06093623462E8EA247B3E97274A1)

Para obter mais ajuda, [entre em contato com o Suporte da Adobe](https://experienceleague.adobe.com/?support-solution=General&amp;lang=pt-BR#support).

## A Adobe cobra minha empresa pelo acesso à Experience Cloud?

Não. A Experience Cloud está incluída sem custos adicionais. No entanto, certos serviços principais podem ter custos adicionais.

## Por que minha empresa deve fazer logon por meio da interface da Experience Cloud?

A funcionalidade fornecida pela interface da Experience Cloud agrega novo valor à empresa. Também é o caminho padrão para acessar aplicativos daqui em diante, e eventualmente substituirá outros fluxos individuais de logon para aplicativos. Fazer logon pela Experience Cloud possibilitará uma transição mais suave posteriormente.

## Como resolver problemas sobre como migrar minha empresa?

[Entre em contato com o Suporte da Adobe](https://experienceleague.adobe.com/?support-solution=General&amp;lang=pt-BR#support).

## Como o [!DNL Adobe Support] pode acessar o meu ambiente de nuvem da Adobe para solucionar um problema?

O [!DNL Adobe Support] pode enviar uma solicitação de representação para a qual você recebe um e-mail da marca Adobe (exemplo abaixo) que solicita a sua autorização explícita. O acesso é concedido por um período limitado. Depois de concedido, o acesso pode ser revogado por você a qualquer momento. A Adobe registra todas as ações tomadas por representantes da Adobe.

![Caso de suporte da Adobe](assets/support-email.png)

## O que é _provisionamento?_

O provisionamento na Experience Cloud significa que:

* Seus usuários podem começar a fazer logon na [!DNL Experience Cloud] e a vincular aplicativos.
* Eles podem começar a usar os recursos disponíveis na Experience Cloud, como o Pessoas.
* Você pode preparar-se para desativar o processo de logon específico do aplicativo.
* É possível manter o controle de acesso dos aplicativos.

## Como faço para gerenciar perfis de usuários e produtos?

* Consulte o [Guia do usuário do Admin Console](https://helpx.adobe.com/br/enterprise/admin-guide.html) para obter ajuda.

* O gerenciamento de produtos e direitos do usuário é executado no [Adobe Admin Console](https://adminconsole.adobe.com/enterprise) (link do produto).

* **Importante:** administradores do Analytics, consultem [Gerenciar usuários do Analytics no Admin Console](https://experienceleague.adobe.com/docs/analytics/admin/user-product-management/migrate-users/c-migration-tool.html?lang=pt-BR) sobre como migrar IDs de usuários das Ferramentas administrativas do Analytics para o Admin Console.

## Como proceder se alguém não conseguir fazer logon na Experience Cloud?

Os administradores do Admin Console podem conceder acesso aos usuários. Os usuários recebem emails com instruções de logon.

Talvez seja necessário [entrar em contato com o suporte da Adobe](https://experienceleague.adobe.com/?support-solution=General&amp;lang=pt-BR#support) para verificar se a empresa foi totalmente provisionada.

## Onde um usuário pode gerenciar a vinculação de contas?

Alguns usuários podem precisar vincular a conta do aplicativo (Analytics) à Adobe ID ou à Enterprise ID.

Consulte [Vincular a conta de um aplicativo a uma Adobe ID](organizations.md#task_FD389E78640848919E247AC5E95B8369).

## Como faço para gerenciar organizações e perfis de contas de usuários?

Consulte [Gerenciar contas de usuário](organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1).

## O que é uma organização?

Uma [organização](organizations.md) é a entidade que permite ao administrador configurar grupos e usuários, além de controlar o logon único na Experience Cloud. A organização funciona como uma empresa para logon que abrange todos os produtos e os aplicativos da Experience Cloud. Frequentemente, a organização é o nome da empresa. No entanto, uma empresa pode ter muitas organizações.

## Onde posso encontrar minha ID da organização IMS?

Consulte [Visualizar a ID da organização](organizations.md) para obter detalhes.

## O que devo fazer quando um dos meus usuários sair da empresa?

O acesso dele deve ser removido do próprio aplicativo. Eles não poderão acessar o produto pela Experience Cloud nem por meio do logon direto. Você também deve removê-los no nível da Experience Cloud.

## O que é uma Adobe ID?

Consulte [Tipos de identidade](https://helpx.adobe.com/br/enterprise/using/identity.html).

## Posso vincular contas do aplicativo para meus usuários?

Não. Os usuários devem vincular seus próprios aplicativos com seus respectivos nomes de usuário e senhas.

## Por que vejo Social se a minha empresa não o possui?

O Adobe Social é um produto que pode ser vendido com o Analytics. Portanto, se tiver o Analytics, você verá esse aplicativo, mas só poderá acessá-lo após a compra.
