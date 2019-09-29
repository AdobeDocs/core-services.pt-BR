---
description: O Adobe Analytics usa cookies para diferenciar solicitações de navegadores diferentes e armazenar informações úteis que um aplicativo pode usar posteriormente. Também podem ser usados para associar informações de navegação a registros do cliente.
keywords: cookies; privacidade
seo-description: O Adobe Analytics usa cookies para diferenciar solicitações de navegadores diferentes e armazenar informações úteis que um aplicativo pode usar posteriormente. Também podem ser usados para associar informações de navegação a registros do cliente.
seo-title: Cookies do Analytics
solution: Experience Cloud,Analytics,Target,Social
title: Cookies do Analytics
uuid: e2d3d61d-2708-48b2-a7e6-2331f2aed8e0
index: y
internal: n
snippet: y
translation-type: tm+mt
source-git-commit: f59badcd3423ada51a3fe0c605158a009d5b1d64

---


# Cookies do Analytics{#analytics-cookies}

O Adobe Analytics usa cookies para diferenciar solicitações de navegadores diferentes e armazenar informações úteis que um aplicativo pode usar posteriormente. Também podem ser usados para associar informações de navegação a registros do cliente.

Particularmente, o Analytics usa cookies para definir novos visitantes anonimamente, para ajudar a analisar dados de sequência de cliques e para rastrear atividades do histórico no site, como respostas a campanhas específicas ou a duração do ciclo de vendas.

* [Nome do cookie: s_ecid](../cookies/cookies-mc.md#section-32fd753c3fa54452acd62b021434919a)
* [Nome do cookie: AMCV_###@AdobeOrg](../cookies/cookies-mc.md#section-a12aa2a9296940ae82d8921b381b8fb0)
* [Nome do cookie: s_cc](../cookies/cookies-analytics.md#section-03aa90aa7e36427b8cb12dc4a0f0291e)
* [Nome do cookie: s_cc](../cookies/cookies-analytics.md#section-03aa90aa7e36427b8cb12dc4a0f0291e)
* [Nome do cookie: s_sq](../cookies/cookies-analytics.md#section-8abfff3a302d494f81a3cfb91e3b09ff)
* [Nome do cookie: s_vi](../cookies/cookies-analytics.md#section-5d50a078de444d12b7d927d68ff3b679)
* [Nome do cookie: s_fid](../cookies/cookies-analytics.md#section-65e33f9bfc264959ac1513e2f4b10ac7)
* [Cookies definidos por plug-ins](../cookies/cookies-analytics.md#section-a6b1cae8454945fab9eea5c7884c40fc)

Mais informações estão disponíveis na ajuda do Analytics sobre [Cookies primários](/help/interface/cookies/cookies-first-party.md).

## Nome do cookie: s_ecid {#section-32fd753c3fa54452acd62b021434919a}

| Atributo | Descrição |
|--- |--- |
| Informações armazenadas | Contém uma cópia da Experience Cloud ID (ECID) ou MID. A MID é armazenada em um par de valor principal que segue a sintaxe s_ecid=MCMID | <ECID> |
| Expiração | 2 anos |
| Uso | Esse cookie é definido pelo domínio do cliente depois que o cookie AMCV é definido pelo cliente. A finalidade deste cookie é permitir o rastreamento de ID persistente no estado próprio e ele é usado como ID de referência, se o cookie AMCV tiver expirado. Verifique o cookie AMCV aqui para obter mais detalhes. |
| Localização | Somente para clientes CNAME. Não aplicável para cenários de terceiros. O cookie é armazenado em seu domínio, o mesmo domínio usado pelo CNAME e pela solicitação de imagem do Analytics. |
| Tamanho | 45 bytes |

## Nome do cookie: s_cc {#section-03aa90aa7e36427b8cb12dc4a0f0291e}

| Atributo | Descrição |
|--- |--- |
| Informações armazenadas | Este cookie é definido e lido pelo código JavaScript para determinar se os cookies estão ativados (definir como "True") |
| Expiração | Este cookie é um cookie de sessão e expira quando o navegador é fechado |
| Uso | Apenas um cookie para todas as contas |
| Localização | Este cookie é armazenado no domínio da página |
| Tamanho | 4 bytes |

## Nome do cookie: s_sq {#section-8abfff3a302d494f81a3cfb91e3b09ff}

| Atributo | Descrição |
|--- |--- |
| Informações armazenadas | Este cookie é definido e lido pelo código JavaScript quando as funcionalidades ClickMap e Activity Map são ativadas; ele contém as informações sobre o link anterior que foi clicado pelo usuário |
| Expiração | Este cookie é um cookie de sessão e expira quando o navegador é fechado |
| Uso | Apenas um cookie para todas as contas |
| Localização | Este cookie é armazenado no domínio da página |
| Tamanho | Varia dependendo do tamanho do URL da página, mas normalmente entre 100 e 200 bytes |

## Nome do cookie: s_vi {#section-5d50a078de444d12b7d927d68ff3b679}

| Atributo | Descrição |
|--- |--- |
| Informações armazenadas | Carimbo único de hora/data da ID do visitante |
| Expiração | 2 anos |
| Uso | Este cookie é usado para identificar um visitante único |
| Localização | Este cookie é armazenado no domínio de solicitação da imagem, normalmente 2O7.net se você está usando cookies de terceiros ou se o domínio está usando cookies primários. |
| Tamanho | 44 bytes |

>[!NOTE]
>
>Cada ID de visitante do Analytics está associada a um perfil de visitante nos servidores da Adobe. Os perfis do visitante são excluídos depois de 1 ano de inatividade, independentemente de qualquer expiração de cookie da ID do visitante.

## Nome do cookie: s_fid {#section-65e33f9bfc264959ac1513e2f4b10ac7}

| Atributo | Descrição |
|--- |--- |
| Informações armazenadas | Recuar carimbo de data/hora da ID de visitante único |
| Expiração | 5 anos |
| Uso | Este cookie é usado para identificar um visitante único se o cookie s_vi padrão estiver indisponível devido a restrições de cookies de terceiros. Não usado para implementações que usam cookies primários. |
| Localização | Este cookie é armazenado no seu domínio como um cookie primário. |
| Tamanho | 33 bytes |

## Cookies definidos por plug-ins {#section-a6b1cae8454945fab9eea5c7884c40fc}

Cookies adicionais são definidos dependendo do uso dos plugins do Analytics. Esses cookies são trechos de código à disposição do cliente para uso em várias circunstâncias. Essas circunstâncias incluem: recuperar valores do URL; concatenar valores para passar ao Analytics; capturar abandono de formulário, etc. Para obter detalhes específicos sobre cookies definidos por cada plug-in, entre em contato com ClientCare. Um exemplo seria o cookie [!DNL s_vh] usado com os plug-ins *Definir uma vez por* e *Definir e obter último valor*.

As variáveis de conversão (eVarX) passadas em uma solicitação de imagem sem JavaScript, como o código colocado em um email, são atribuídos apropriadamente apenas se o cliente de email e o navegador compartilharem o mesmo espaço de cookie.
