---
description: Saiba como as soluções e os serviços da Adobe Experience Cloud usam cookies.
title: Como os cookies são usados no Experience Cloud
uuid: 4255a13a-917b-4b5f-a7d4-4b2e7521d189
exl-id: 60f1a89e-d989-461b-a6a3-c1df022cd30b
source-git-commit: 2a80851c0a7d4ef7dbcc2565177b239f3e063164
workflow-type: tm+mt
source-wordcount: '890'
ht-degree: 58%

---

# Cookies usados no Experience Cloud

Vários serviços na Adobe Experience Cloud usam cookies. Um cookie é um pequeno pedaço de dados apresentado por um site a um navegador da Web. O navegador armazena esses dados, permitindo que um site referencie seus dados quando necessário. Esta ação é executada com cada solicitação subsequente para páginas e imagens.

Os cookies são fornecidos para manter informações durante e, às vezes, entre visitas a um site. Os cookies permitem que os dispositivos sejam diferenciados exclusivamente de outros navegadores que visualizaram o site.

Leis, regulamentos e princípios autorreguladores exigem que você obtenha o consentimento dos visitantes antes de armazenar ou recuperar informações em um computador ou outro dispositivo conectado à web. A Adobe sugere que você analise com o serviço jurídico de sua organização quais leis, regulamentos e princípios controlam seu uso de cookies.

## Sobre cookies próprios

Os serviços da Adobe Experience Cloud usam cookies para fornecer informações sobre variáveis e componentes que não persistem entre as solicitações de imagem e as sessões do navegador. Sempre que possível, o Adobe usa cookies primários para registrar atividades no site. Para registrar a atividade em sites diferentes, como em outros domínios pertencentes a você, são necessários cookies de terceiros.

Muitos navegadores e aplicativos antispyware foram projetados para rejeitar e excluir cookies de terceiros. O Adobe garante que os cookies sempre possam ser definidos, mesmo que os cookies de terceiros estejam bloqueados. O comportamento específico varia dependendo de você estar usando o Experience Platform Identity Service (serviço ECID) ou os identificadores herdados do Analytics (como o cookie `s_vi`):

* O [Experience Platform Identity Service (ECID Service)](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html?lang=pt-BR) define cookies primários de forma automática, independentemente de o domínio de coleção corresponder ao domínio do site. Se não corresponderem, o Identity Service usará o JavaScript para definir cookies no domínio do site.
* Se você usa [identificadores herdados do Analytics](analytics.md) (como o cookie `s_vi`), isso depende de como você configurou o servidor de coleção de dados. Se o servidor de coleção de dados corresponder ao domínio do site, os cookies serão definidos como primários. Se o servidor de coleção não corresponder ao seu domínio atual, os cookies serão definidos como de terceiros. Nesse caso, se os cookies de terceiros estiverem bloqueados, o Analytics definirá um id de fallback (`s_fid`) primário em vez do cookie `s_vi` padrão.

Se quiser garantir que o servidor de coleção corresponda ao domínio do site, você poderá usar uma implementação CNAME que permita o encaminhamento de um domínio personalizado especificado na implementação CNAME para servidores de coleção Adobe. Essa tarefa envolve alterações nas configurações de DNS da empresa para configurar um alias CNAME para apontar para um domínio hospedado em Adobe. Observe que, embora vários produtos da Adobe sejam compartíveis com o uso de um CNAME, em todos os casos o CNAME é usado para criar um endpoint de terceiros confiável para um cliente específico, e é de sua propriedade. Se você controlar vários domínios, eles poderão usar um único endpoint CNAME para rastrear usuários em seus domínios, mas sempre que o domínio do site não for correspondente ao CNAME, os cookies desse domínio serão definidos como de terceiros.

>[!NOTE]
>
>Independentemente de o domínio de coleção corresponder ao domínio do site, o programa de Prevenção de Rastreamento Inteligente (ITP) da Apple faz com que os cookies primários definidos pelo Adobe tenham vida curta em navegadores regidos pela ITP, que incluem o Safari no macOS e todos os navegadores no iOS e iPadOS. A partir de novembro de 2020, os cookies definidos por CNAME também terão a mesma expiração dos cookies definidos pelo JavaScript. Essa expiração está sujeita a alterações.

## Cookies e privacidade

A manutenção da privacidade do cliente e da segurança de dados são as principais prioridades da Adobe. A Adobe participa de várias organizações de privacidade e coopera com reguladores de privacidade e princípios autorreguladores. Essa cooperação inclui o programa Digital Advertising Alliance AdChoices para informar os clientes sobre como suas informações são usadas e quais são as opções sobre seu uso.

A maioria dos cookies definida pelos produtos da Experience Cloud não contém informações pessoalmente identificáveis. Esses cookies e dados associados são seguros e usados apenas para seus relatórios de empresa e para fornecer conteúdo e anúncios relevantes. Os dados não estão disponíveis para terceiros ou outros clientes da Adobe, a menos que sejam usados em relatórios agregados do setor. Por exemplo, a [!DNL Digital Marketing Insight Report] analisa dados agregados e anônimos entre varejistas.

A Adobe não combina informações a nível do navegador por meio de empresas. Para proteger a privacidade e a segurança dos dados dos clientes, alguns dos serviços na Experience Cloud oferecem às empresas a capacidade de usar um conjunto separado de cookies para cada site rastreado. Algumas ofertas também oferecem aos clientes a capacidade de usar seu próprio nome de domínio como proprietário do cookie. Esta prática cria uma camada extra de privacidade e segurança, já que transforma os cookies da Experience Cloud em *cookies primários*, pertencendo permanentemente ao site da empresa.

Os cookies podem armazenar e fornecer apenas as informações que foram depositadas neles anteriormente. Eles não podem executar código ou acessar outras informações armazenadas no computador. Além disso, os navegadores da web restringem o acesso aos dados de cookies. Os navegadores impõem uma política de segurança de cookie que disponibiliza todos os dados de cookie somente para o site que definiu as informações originalmente.

Por exemplo, os dados contidos em cookies definidos no site Adobe.com não podem ser exibidos por nenhum outro site que não o Adobe.com.

O diagrama a seguir ilustra o uso de cookies em uma solicitação de imagem padrão:

![Uso de cookies para uma solicitação de imagem padrão](assets/CookiesProcessGraphic-01.png)

O diagrama a seguir ilustra o uso de cookies em uma solicitação de imagem direta (usada em cenários nos quais um arquivo JS não é carregado):

![Uso de cookies para uma solicitação de imagem direta](assets/CookiesProcessGraphic2.png)
