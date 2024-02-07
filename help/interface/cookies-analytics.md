---
description: Saiba mais sobre os cookies do Adobe Analytics na Adobe Experience Cloud.
solution: Experience Cloud,Analytics,Target
title: Cookies do Analytics
uuid: e2d3d61d-2708-48b2-a7e6-2331f2aed8e0
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: bc8ce894-f98c-4475-8a07-d74ae76f7451
source-git-commit: a20d51e6e7d5ec72d59e06e6a4951778a5828d9a
workflow-type: tm+mt
source-wordcount: '722'
ht-degree: 95%

---

# Cookies do Analytics {#analytics-cookies}

O Adobe Analytics usa cookies para diferenciar solicitações de navegadores diferentes e armazenar informações úteis que um aplicativo pode usar posteriormente. Eles também podem ser usados para associar informações de navegação a registros de clientes.

O Analytics utiliza cookies para definir novos visitantes anonimamente, além de ajudar a analisar dados de sequência de cliques e rastrear a atividade do histórico no site, como a resposta a campanhas específicas ou a duração do ciclo de vendas.

* [Nome do cookie: s_ecid](cookies-mc.md#section-32fd753c3fa54452acd62b021434919a)
* [Nome do cookie: AMCV_###@AdobeOrg](cookies-mc.md#section-a12aa2a9296940ae82d8921b381b8fb0)
* [Nome do cookie: s_cc](cookies-analytics.md#section-03aa90aa7e36427b8cb12dc4a0f0291e)
* [Nome do cookie: s_sq](cookies-analytics.md#section-8abfff3a302d494f81a3cfb91e3b09ff)
* [Nome do cookie: s_vi](cookies-analytics.md#section-5d50a078de444d12b7d927d68ff3b679)
* [Nome do cookie: s_fid](cookies-analytics.md#section-65e33f9bfc264959ac1513e2f4b10ac7)
* [Cookies definidos por plug-ins](cookies-analytics.md#section-a6b1cae8454945fab9eea5c7884c40fc)

Mais informações disponíveis na ajuda do Analytics sobre [Cookies primários](cookies-first-party.md).

## Nome do cookie: s_ecid {#section-32fd753c3fa54452acd62b021434919a}

| Atributo | Descrição |
|--- |--- |
| Informações armazenadas | Contém uma cópia da Experience Cloud ID (ECID) ou MID. A MID é armazenada em um par de valor principal que segue a sintaxe s_ecid=MCMID | `<ECID>` |
| Expiração | 2 anos |
| Uso | Esse cookie é definido pelo domínio do cliente depois que o cookie AMCV é definido pelo cliente. A finalidade deste cookie é permitir o rastreamento de ID persistente no estado próprio e ele é usado como ID de referência, se o cookie AMCV tiver expirado. Verifique o cookie AMCV aqui para obter mais detalhes. |
| Localização | Somente para clientes CNAME. Não aplicável para cenários de terceiros. O cookie é armazenado em seu domínio, o mesmo domínio usado pelo CNAME e pela solicitação de imagem do Analytics |
| Tamanho | 45 bytes |

{style="table-layout:auto"}

## Nome do cookie: s_cc {#section-03aa90aa7e36427b8cb12dc4a0f0291e}

| Atributo | Descrição |
|--- |--- |
| Informações armazenadas | Este cookie é definido e lido pelo código JavaScript para determinar se os cookies estão habilitados (definido como &quot;True&quot;) |
| Expiração | Este cookie é um cookie de sessão e expira quando o navegador é fechado |
| Uso | Somente um cookie para todas as contas |
| Localização | Esse cookie é armazenado no domínio da página. |
| Tamanho | 4 bytes |

{style="table-layout:auto"}

## Nome do cookie: s_sq {#section-8abfff3a302d494f81a3cfb91e3b09ff}

| Atributo | Descrição |
|--- |--- |
| Informações armazenadas | Esse cookie é definido e lido pelo código JavaScript quando a funcionalidade ClickMap ou Activity Map é ativada; ele contém informações sobre o link anterior que foi selecionado pelo usuário |
| Expiração | Este cookie é um cookie de sessão e expira quando o navegador é fechado |
| Uso | Somente um cookie para todas as contas |
| Localização | Esse cookie é armazenado no domínio da página. |
| Tamanho | Varia dependendo do tamanho do URL da página, mas normalmente entre 100 e 200 bytes |

{style="table-layout:auto"}

## Nome do cookie: s_vi {#section-5d50a078de444d12b7d927d68ff3b679}

| Atributo | Descrição |
|--- |--- |
| Informações armazenadas | Carimbo de data/hora do identificador de visitante único. |
| Expiração | 2 anos |
| Uso | Este cookie é usado para identificar um visitante único. |
| Localização | Este cookie é armazenado no domínio da solicitação de imagem - normalmente um subdomínio específico do cliente em 2o7.net ou omtrdc.net se você estiver usando cookies de terceiros ou se o domínio estiver usando cookies primários |
| Tamanho | 44 bytes |

{style="table-layout:auto"}

>[!NOTE]
>
>Cada ID de visitante do Analytics está associada a um perfil de visitante nos servidores da Adobe. Os perfis do visitante são excluídos depois de 1 ano de inatividade, independentemente de qualquer expiração de cookie da ID do visitante.

## Nome do cookie: s_fid {#section-65e33f9bfc264959ac1513e2f4b10ac7}

| Atributo | Descrição |
|--- |--- |
| Informações armazenadas | Carimbo de data/hora da ID do visitante único de fallback |
| Expiração | 2 anos |
| Uso | Este cookie é usado para identificar um visitante único se o cookie `s_vi` padrão não estiver disponível devido a restrições de cookies de terceiros. Não usado para implementações que usam cookies primários |
| Localização | Esse cookie é armazenado em seu domínio como um cookie primário |
| Tamanho | 33 bytes |

{style="table-layout:auto"}

## Sinalizadores de cookie

A tabela a seguir descreve os sinalizadores dos cookies do Analytics:

| Cookie (definido por) | httpOnly | Seguro | SameSite |
|--- |--- |--- |--- |
| s_vi (Resposta http) | Não | Sim quando SameSite for &quot;None&quot; e a conexão usar HTTPS | &quot;Lax&quot; por padrão ao usar CNAME. &quot;None&quot; ao usar 2o7.net ou omtrdc.net |
| s_ecid (Resposta http) | Não | Não | &quot;Lax&quot; |
| s_fid (Javascript) | Não | Não | Não definido |
| s_cc (Javascript) | Não | Não | Não definido |
| s_sq (Javascript) | Não | Não | Não definido |

{style="table-layout:auto"}

>[!NOTE]
>
>Se estiver usando um único CNAME para rastrear vários domínios ou propriedades, o SameSite deve ser definido como &quot;None&quot; para `s_vi`. Para obter ajuda sobre como alterar as configurações de cookies do Analytics, entre em contato com o Atendimento ao cliente.

## Cookies definidos por plug-ins {#section-a6b1cae8454945fab9eea5c7884c40fc}

{{plug-in}}

Cookies adicionais podem ser definidos dependendo do uso de plug-ins do Analytics. Esses cookies são fragmentos de código disponíveis ao cliente para uso em várias circunstâncias. Essas circunstâncias incluem: recuperar valores do URL; concatenar valores a serem transmitidos para o Analytics; capturar o abandono de formulário e assim por diante. Um exemplo seria o cookie [!DNL s_vh] usado com os plug-ins *Definir uma vez por* e *Definir e obter último valor*.

As variáveis de conversão (eVarX) passadas em uma solicitação de imagem sem JavaScript, como o código colocado em um email, serão atribuídos apropriadamente apenas se o cliente de email e o navegador compartilharem o mesmo espaço de cookie.
