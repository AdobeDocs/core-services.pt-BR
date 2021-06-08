---
description: Saiba como o Adobe Analytics usa cookies para fornecer informações sobre variáveis e componentes que não persistem entre as solicitações de imagem e as sessões do navegador.
keywords: cookies; privacidade
solution: Experience Cloud,Analytics
title: '"Cookies próprios "'
index: y
snippet: y
feature: Cookies
topic: Administração
role: Administrator
level: Experienced
exl-id: e15abde5-8027-4aed-a0c1-8a6fc248db5e
source-git-commit: 11b999ef0c0d4f258e8665eb9c5bf427f5d618c4
workflow-type: tm+mt
source-wordcount: '1576'
ht-degree: 55%

---

# Sobre cookies próprios

O Analytics usa cookies para fornecer informações sobre variáveis e componentes que não persistem entre as solicitações de imagem e as sessões do navegador. Sempre que possível, o Adobe usa cookies primários para registrar atividades no site. Para registrar a atividade em sites diferentes, como em outros domínios pertencentes a você, são necessários cookies de terceiros.

Muitos navegadores e aplicativos antispyware foram projetados para rejeitar e excluir cookies de terceiros, incluindo cookies usados na coleta de dados [!DNL Analytics]. Para ser compatível com o rastreamento de como seus visitantes interagem com o site, verifique se você configurou a coleta de dados para usar cookies primários:

Há duas opções disponíveis para implementar cookies próprios:

* Se você estiver usando o Experience Platform Identity Service (Serviço ECID), ele define cookies automaticamente no contexto primário usando JavaScript.
* Se estiver usando [!DNL Analytics] identificadores herdados (também conhecido como cookie `s_vi`), isso dependerá de como você configurou seu servidor de coleta de dados. Se o servidor de coleta de dados corresponder ao domínio do site, os cookies serão definidos como primários. Se o servidor de coleta não corresponder ao seu domínio atual, os cookies serão definidos como de terceiros. Nesse caso, se cookies de terceiros estiverem bloqueados, [!DNL Analytics] definirá um [id de fallback (s_fid)](cookies-analytics.md) próprio em vez do cookie &quot;s_vi&quot; padrão.

Para garantir que o servidor de coleta corresponda ao domínio do site, você pode usar uma implementação CNAME na qual os cookies sejam definidos em um contexto próprio. Isso envolve alterações nas configurações de DNS da empresa para configurar um alias CNAME para apontar para um domínio hospedado pelo Adobe. Observe que, embora vários produtos da Adobe sejam compartíveis com o uso de um CNAME, em todos os casos o CNAME é usado para criar um endpoint de terceiros confiável para um cliente específico, e é de sua propriedade. Se você controlar vários domínios, eles poderão usar um único endpoint CNAME para rastrear usuários em seus domínios, mas sempre que o domínio do site não corresponder aos cookies de domínio CNAME for definido como terceiros.

>[!NOTE]
>
>Para ambas as opções, o programa Intelligent Tracking Prevention (ITP) da Apple torna os cookies primários com vida curta em navegadores regidos pela ITP, que incluem o Safari no macOS e todos os navegadores no iOS e iPadOS. A partir de novembro de 2020, ambos os tipos de cookies têm um prazo de sete dias. Essa expiração está sujeita a alterações.

Na segunda opção usando um CNAME, se o site tiver páginas seguras usando o protocolo HTTPS, você poderá trabalhar com a Adobe para obter um certificado SSL para implementar cookies primários. O Adobe recomenda que você use exclusivamente HTTPS para coleta de dados, já que o Adobe está removendo o suporte para coleta HTTP na segunda metade de 2020.

Muitas vezes o processo de emissão do certificado SSL pode ser confuso e demorado. Como resultado, a Adobe estabeleceu uma parceria com a DigiCert, uma Autoridade de Certificação (CA) líder do setor, e desenvolveu um processo integrado pelo qual a compra e o gerenciamento desses certificados são automatizados.

Com sua permissão, trabalhamos com CA para emitir, implantar e gerenciar um novo certificado SSL SHA-2 para você. O Adobe continua a gerenciar esse certificado e garante que uma expiração, revogação ou preocupação de segurança inesperada não prejudique a disponibilidade da coleção segura de sua organização.

## Programa de certificado Adobe Managed

O Adobe Managed Certificate Program é o processo recomendado para implementar um novo certificado SSL próprio para cookies próprios.

O programa Adobe Managed Certificate permite implementar um novo certificado SSL próprio para cookies próprios sem custo adicional (para os primeiros 100 CNAMEs). Caso tenha seu próprio certificado SSL gerenciado pelo cliente no momento, fale com o Atendimento ao cliente do Adobe sobre a migração para o Adobe-Managed Certificate Program.

### Implementação

A seguir, veja como implementar um novo certificado SSL próprio para cookies próprios:

1. Preencha o [Formulário de solicitação de cookie primário](/help/interface/cookies/assets/First_Part_Domain_Request_Form.xlsx) e abra um ticket no Atendimento ao cliente, solicitando a configuração de cookies próprios no programa Adobe-Managed. Cada campo é descrito no documento com exemplos.

2. Crie registros CNAME (consulte as instruções abaixo).

   Ao receber a solicitação, um representante do Atendimento ao cliente deve fornecer a você um registro CNAME. Esses registros devem ser configurados no servidor DNS da empresa antes que a Adobe possa comprar o certificado em seu nome. O CNAME é semelhante ao seguinte:

   **Seguro** - por exemplo, o nome de host `smetrics.example.com` aponta para: `example.com.adobedc.net`.

>[!NOTE]
> Anteriormente, o Adobe recomendava que os clientes configurassem dois CNAME um para HTTPS e outro para HTTP. Como é uma prática recomendada criptografar o tráfego e a maioria dos navegadores desencoraja expressamente o uso de HTTP, deixamos de recomendar a configuração de um CNAME para HTTP. Se precisar, seria assim:
>    **Não seguro** — o nome do host `metrics.example.com` aponta para: `example.com.adobedc.net`.

1. Quando o CNAME estiver em vigor, o Adobe funcionará com a DigiCert para comprar e instalar um certificado nos servidores de produção Adobe.

   Se tiver uma implementação existente, considere a Migração do visitante para manter os visitantes existentes. Depois que o certificado for enviado ao ambiente de produção da Adobe, você poderá atualizar as variáveis do servidor de rastreamento para os novos nomes de host. Ou seja, se o site não for seguro (HTTP), atualize o `s.trackingServer`. Se o site for seguro (HTTPS), atualize as variáveis `s.trackingServer` e `s.trackingServerSecure`.

2. [Validar o encaminhamento do nome do host](#validate) (veja abaixo).

3. [Atualizar o código de implementação](#update) (veja abaixo).

### Manutenção e Renovações

Os certificados SSL expiram todo ano, o que significa que a Adobe deve comprar um novo certificado para cada implementação anualmente. Todos os usuários suportados em sua organização recebem uma notificação por email sempre que uma implementação estiver próxima à expiração. Para que a Adobe renove o nome de host, um usuário suportado deverá responder ao email da Adobe e indicar que pretende continuar a usar o nome de host que está expirando para a coleta de dados. Nesse momento, a Adobe compra e instala automaticamente um novo certificado.

### Perguntas frequentes

| Pergunta | Resposta |
|---|---|
| **Esse processo é seguro?** | Sim, o programa Adobe-Managed é mais seguro do que nosso método herdado, pois nenhum certificado ou chave privada muda de mãos fora do Adobe e da autoridade de certificação emissora. |
| **Como a Adobe pode comprar um certificado para o nosso domínio?** | O certificado só pode ser comprado quando você aponta o nome de host especificado (por exemplo, `telemetry.example.com`) para um nome de host da Adobe. Essa ação basicamente delega esse nome de host à Adobe e permite que a Adobe compre o certificado em seu nome. |
| **É possível solicitar que o certificado seja revogado?** | Sim, como proprietário do domínio, você está autorizado a solicitar a revogação do certificado. Você só precisará abrir um ticket no Atendimento ao cliente para que isso seja concluído. |
| **Esse certificado usará a criptografia SHA-2?** | Sim, a Adobe trabalhará com a DigiCert para emitir um certificado SHA-2. |
| **Isso gera custo adicional?** | Não, a Adobe disponibiliza esse serviço para todos os clientes atuais da Adobe Digital Experience sem custo adicional. |

## Criar registros CNAME

A equipe de operações de rede da organização deve configurar os servidores DNS criando registros CNAME. Cada nome de host encaminha os dados para os servidores de coleta de dados da Adobe.

O especialista em FPC fornece o nome de host configurado e o CNAME para o qual ele deve ser apontado. Por exemplo:

* **Nome de host SSL**: `smetrics.mysite.com`
* **CNAME SSL**: `mysite.com.adobedc.net`

>[!NOTE]
> Se você ainda usar o não seguro, ele terá esta aparência:
> * **Nome de host não SSL**: `metrics.mysite.com`
> * **CNAME não SSL**: `mysite.com.adobedc.net`


Contanto que o código de implementação não seja alterado, esta etapa não afetará a coleta de dados e poderá ser feita a qualquer momento após a atualização do código de implementação.

>[!NOTE]
>
>O serviço de ID de visitante da Experience Cloud oferece uma alternativa para configurar um CNAME para ativar cookies primários.

## Validar o encaminhamento do nome do host {#validate}

Os seguintes métodos estão disponíveis para validação:

### Validar usando um navegador

Se você tiver um CNAME configurado e o certificado instalado, poderá usar o navegador para validação:

`https://smetrics.adobe.com/_check`

>[!NOTE]
>
>Você recebe um aviso de segurança se um certificado não estiver instalado.

### Validar usando o [!DNL curl]

A Adobe recomenda usar [[!DNL curl]](https://curl.se/) na linha de comando. (os usuários do [!DNL Windows] podem instalar [!DNL curl] de: <https://curl.se/windows/>)

Se você tiver um CNAME mas nenhum certificado estiver instalado, execute:
`curl -k https://smetrics.adobe.com/_check`
Resposta: `SUCCESS`

(O valor `-k` desativa o aviso de segurança.)

Se você tiver um CNAME configurado e o certificado estiver instalado, execute:
`curl https://smetrics.adobe.com/_check`
Resposta: `SUCCESS`

### Validar usando o [!DNL nslookup]

Você pode usar `nslookup` para validação. Usando `smetrics.adobe.com` como exemplo, abra um prompt de comando e digite `nslookup smetrics.adobe.com`

Se tudo for configurado com êxito, você verá um retorno semelhante a:

```
nslookup smetrics.adobe.com
Server:             10.30.7.247
Address:     10.30.7.247#53

smetrics.adobe.com    canonical name = adobe.com.ssl.d1.sc.omtrdc.net.
Name:  adobe.com.ssl.d1.sc.omtrdc.net
Address: 54.218.180.161
Name:  adobe.com.ssl.d1.sc.omtrdc.net
Address: 52.39.8.230
Name:  adobe.com.ssl.d1.sc.omtrdc.net
Address: 54.187.216.46
```

## Atualizar código de implementação {#update}

Antes de editar o código no site para usar cookies primários, conclua estes pré-requisitos:

* Solicite um certificado SSL seguindo as etapas descritas acima, na seção *Implementar* do [Programa de certificado Adobe-gerenciado](#adobe-managed-certificate-program).
* Criar registros CNAME (veja acima).
* Valide os nomes de host (veja acima).

Após verificar que os nomes de host estão respondendo e encaminhando para os servidores de coleta de dados do Adobe, é possível alterar a implementação para apontar para seus próprios nomes de host da coleta de dados.

1. Abra seu arquivo JavaScript principal (`s_code.js/AppMeasurement.js`).
1. Se quiser atualizar a versão de seu código, substitua o arquivo`s_code.js/AppMeasurement.js` completo pela versão mais nova e substitua todos os plug-ins ou personalizações (se houver). **Ou**, se quiser atualizar o código pertinente somente a cookies próprios, localize as variáveis s.trackingServer e s.trackingServerSecure (se estiver usando o SSL) e aponte-as para os novos nomes de host da coleta de dados. Usando o mysite.com como exemplo: `s.trackingServer = "metrics.mysite.com"` `s.trackingServerSecure = "smetrics.mysite.com"`

1. Carregue o arquivo JavaScript principal atualizado em seu site.

1. Se você estiver mudando de uma implementação antiga para cookies próprios ou mudando para um nome de host de coleção própria diferente, o Adobe recomenda migrar os visitantes do domínio anterior para o novo domínio.

Consulte [Migração de visitantes](https://experienceleague.adobe.com/docs/analytics/implementation/javascript-implementation/visitor-migration.html?lang=en) no Guia de implementação do Analytics.

Após carregar o arquivo JavaScript, tudo é configurado para a coleta de dados de cookie próprio. O Adobe recomenda monitorar os relatórios do Analytics das próximas horas para garantir que a coleta de dados continue normalmente. Caso contrário, verifique se todas as etapas acima foram concluídas e peça para um dos usuários suportados da organização entrar em contato com o Atendimento ao cliente.
