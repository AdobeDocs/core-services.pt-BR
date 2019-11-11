---
description: O Analytics usa cookies para fornecer informações sobre variáveis e componentes que não persistem entre as solicitações de imagem e as sessões do navegador.
keywords: cookies; privacidade
seo-description: O Analytics usa cookies para fornecer informações sobre variáveis e componentes que não persistem entre as solicitações de imagem e as sessões do navegador.
seo-title: Cookies próprios
solution: Experience Cloud, Analytics
title: Cookies próprios
index: y
snippet: y
translation-type: tm+mt
source-git-commit: 90123ac9194d180a6a8ae59a273a6a6154ea8d96

---


# Sobre cookies próprios

O Analytics usa cookies para fornecer informações sobre variáveis e componentes que não persistem entre as solicitações de imagem e as sessões do navegador. Esses cookies inofensivos são originários de um domínio hospedado pela Adobe, conhecidos como cookies de terceiros.

Muitos navegadores e aplicativos antispyware foram projetados para rejeitar e excluir cookies de terceiros, inclusive aqueles usados na coleta de dados do Analytics. Para contornar as limitações de rastreamento impostas por navegadores e programas, você pode implementar cookies próprios.

Há duas opções disponíveis para implementar cookies próprios

* O Serviço de ID da Experience Platform. O serviço de ID pode definir o cookie no contexto próprio usando JavaScript.
* Entradas DNS no servidor DNS de empresas.
* Se o site tem páginas seguras usando o `https:` protocolo e você não está usando o serviço de ID da Experience Platform, você pode trabalhar com a Adobe para obter um certificado SSL a fim de implementar cookies próprios.

Muitas vezes o processo de emissão do certificado SSL pode ser confuso e demorado. Como resultado, a Adobe estabeleceu uma parceria com a DigiCert, uma Autoridade de certificação (CA) líder do setor, e desenvolveu um processo integrado pelo qual a compra e o gerenciamento desses certificados são automatizados.

Com sua permissão, trabalharemos com a CA para emitir, implantar e gerenciar um novo certificado SSL de SHA-2 para você. A Adobe continuará a gerenciar esse certificado e garantirá que uma expiração, revogação ou preocupação de segurança inesperada não prejudique a disponibilidade da coleção segura de suas organizações.

## Programa Adobe Managed Certificate

O Adobe Managed Certificate Program é o processo recomendado para implementar um novo certificado SSL próprio para cookies próprios.

O programa Adobe Managed Certificate permite implementar um novo certificado SSL próprio para cookies próprios sem custo adicional. Se você tem seu próprio certificado SSL gerenciado pelo cliente no momento, fale com o Atendimento ao cliente da Adobe sobre a migração para o Adobe Managed Certificate Program.

### Implementação

A seguir, veja como implementar um novo certificado SSL próprio para cookies próprios:

1. Preencha o [Formulário de solicitação de cookies próprios](/help/interface/cookies/assets/FPC_Request_Form.xlsx) e abra um ticket no Atendimento ao cliente, solicitando a configuração de cookies próprios no programa Adobe Managed. Cada campo é descrito no documento com exemplos.

1. Crie registros CNAME (consulte as instruções abaixo). Ao receber o ticket, um representante do Atendimento ao cliente deve fornecer um par de registros CNAME. Esses registros devem ser configurados no servidor DNS da empresa antes que a Adobe possa comprar o certificado em seu nome. Os CNAMES serão semelhantes ao seguinte: **Protegido** - por exemplo, o nome de host `smetrics.example.com` aponta para: `example.com.ssl.d1.omtrdc.net`. **Não seguro** - por exemplo, o nome de host `metrics.example.com` aponta para: `example.com.d1.omtrdc.net`.

1. Quando esses CNAMES estiverem em vigor, a Adobe trabalhará com a DigiCert para comprar e instalar um certificado nos servidores de produção da Adobe. Se você tiver uma implementação existente, considere a Migração do visitante para manter os visitantes existentes. Depois que o certificado for enviado ao ambiente de produção da Adobe, você poderá atualizar as variáveis do servidor de rastreamento para os novos nomes de host. Ou seja, se o site não for seguro (https), atualize o `s.trackingServer`. Se o site for seguro (https), atualize as duas variáveis `s.trackingServer` e `s.trackingServerSecure`.

1. Execute o ping do nome de host (veja abaixo).

1. Atualize o código de implementação (veja abaixo).

### Manutenção e Renovações

Os certificados SSL expiram todo ano, o que significa que a Adobe deve comprar um novo certificado para cada implementação anualmente. Todos os usuários suportados na organização receberão uma notificação por email, sempre que uma implementação estiver próxima à expiração. Para que a Adobe renove o nome de host, um usuário suportado deverá responder ao email da Adobe e indicar que pretende continuar a usar o nome de host que está expirando para a coleta de dados. Nesse momento, a Adobe compra e instala automaticamente um novo certificado.

### Perguntas frequentes

| Pergunta | Resposta |
|---|---|
| **Esse processo é seguro?** | Sim, o programa Adobe Managed é mais seguro que nosso método antigo, pois o certificado ou a chave privada não muda de mãos fora da Adobe e da autoridade de certificação emissora. |
| **Como a Adobe pode comprar um certificado para o nosso domínio?** | O certificado só pode ser comprado quando você aponta o nome de host especificado (por exemplo, smetrics.example.com) para um nome de host da Adobe. Essa ação basicamente delega esse nome de host à Adobe e permite que a Adobe compre o certificado em seu nome. |
| **É possível solicitar que o certificado seja revogado?** | Sim, como proprietário do domínio, você está autorizado a solicitar a revogação do certificado. Você só precisará abrir um ticket no Atendimento ao cliente para que isso seja concluído. |
| **Esse certificado usará a criptografia SHA-2?** | Sim, a Adobe trabalhará com a DigiCert para emitir um certificado SHA-2. |
| **Isso gera custo adicional?** | Não, a Adobe disponibiliza esse serviço para todos os clientes atuais do Analytics sem custo adicional. |

## Criar registros CNAME

A equipe de operações de rede da organização deve configurar os servidores DNS criando novos registros CNAME. Cada nome de host encaminha os dados para os servidores de coleta de dados da Adobe.

O especialista FPC fornece os nomes de host configurados e os CNAMEs para os quais eles devem ser apontados. Por exemplo:

* **Nome de host SSL**:`smetrics.mysite.com`
* **CNAME SSL**:`mysite.com.ssl.sc.omtrdc.net`
* **Nome de host não SSL**:`metrics.mysite.com`
* **CNAME não SSL**:`mysite.com.sc.omtrdc.net`

Contanto que o código de implementação não seja alterado, esta etapa não afetará a coleta de dados e poderá ser feita a qualquer momento após a atualização do código de implementação.

>[!NObservação:] o serviço de ID de visitante da Experience Cloud oferece uma alternativa para configurar um CNAME para ativar cookies próprios.

## Execute o ping do nome de host

Execute o ping do nome de host para garantir o encaminhamento correto. Todos os nomes de host devem responder a um ping para evitar a perda de dados.

Depois que os registros CNAME forem configurados corretamente e a Adobe tiver confirmado a instalação do certificado, abra um prompt de comando e execute o ping dos nomes de host. Usando o `mysite.com` como exemplo: `ping metrics.mysite.com`

Se tudo for configurado com êxito, retornará algo semelhante ao exposto a seguir:

```Pinging mysite.com.112.2o7.net [66.235.132.232] with 32 bytes of data:
Reply from 66.235.132.232: bytes=32 time=19ms TTL=246
Reply from 66.235.132.232: bytes=32 time=19ms TTL=246
Reply from 66.235.132.232: bytes=32 time=19ms TTL=246
Reply from 66.235.132.232: bytes=32 time=19ms TTL=246

Ping statistics for 66.235.132.232: Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds: Minimum = 19ms, Maximum = 19ms, Average = 19ms
```

Se os registros CNAME não foram configurados ou ativados corretamente, retornará o seguinte:

`Ping request could not find the host. Please check the name and try again.`

>[!NObservação:] Se você estiver usando `https:// protocol`, o ping só responderá após a data de upload especificada pelo especialista FPC. Além disso, execute o ping no nome de host seguro e não seguro para garantir que ambos estejam funcionando corretamente, antes da atualização da implementação.

## Atualizar código de implementação

Antes de editar o código no site para utilizar cookies próprios, preencha estes pré-requisitos:

* Solicite um certificado SSL, conforme descrito acima nas Etapas de implementação do Programa Adobe Managed Certificate.
* Crie registros CNAME (veja acima).
* Execute o poing do nome de host (veja acima).

Após verificar que o nome de host está respondendo e encaminhando para os servidores de coleta de dados da Adobe, você pode alterar a implementação para apontar para seus próprios nomes de host da coleta de dados.

1. Abra seu arquivo JavaScript principal (`s_code.js/AppMeasurement.js`).
1. Se quiser atualizar a versão de seu código, substitua o arquivo`s_code.js/AppMeasurement.js` completo pela versão mais nova e substitua todos os plug-ins ou personalizações (se houver). **Ou**, se quiser atualizar o código pertinente somente a cookies próprios, localize as variáveis s.trackingServer e s.trackingServerSecure (se estiver usando o SSL) e aponte-as para os novos nomes de host da coleta de dados. Usando o mysite.com como exemplo:`s.trackingServer = "metrics.mysite.com"` `s.trackingServerSecure = "smetrics.mysite.com"`

1. Carregue o arquivo JavaScript principal atualizado em seu site.

1. Se você estiver mudando de uma implementação que existe a muito tempo para cookies próprios ou mudando para um nome de host de coleção própria diferente, é recomendável migrar os visitantes do domínio anterior para o novo domínio.

Consulte Migração [de](https://docs.adobe.com/help/en/analytics/implementation/javascript-implementation/visitor-migration.html) visitantes no Guia de implementação do Analytics.

Após carregar o arquivo JavaScript, tudo é configurado para a coleta de dados de cookie próprio. É recomendável monitorar os relatórios do Analytics das próximas horas, para garantir que a coleta de dados continue normalmente. Caso contrário, verifique se todas as etapas acima foram concluídas e peça para um dos usuários suportados da organização entrar em contato com o Atendimento ao cliente.
