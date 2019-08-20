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
source-git-commit: 2bdc4b7287ccacfc4d968278b2c3ffdaeddfc105

---


# Sobre cookies primários

O Analytics usa cookies para fornecer informações sobre variáveis e componentes que não persistem entre as solicitações de imagem e as sessões do navegador. Esses cookies inofensivos são originários de um domínio hospedado pela Adobe, conhecidos como cookies de terceiros.

Muitos navegadores e aplicativos antispyware foram projetados para rejeitar e excluir cookies de terceiros, inclusive aqueles usados na coleta de dados do Analytics. Para contornar as limitações de rastreamento impostas por navegadores e programas, você pode implementar cookies primários.

Duas opções estão disponíveis para implementar cookies primários

* O Serviço de ID da plataforma Experience Platform. O serviço de ID pode definir o cookie no contexto primário usando javascript.
* Entradas DNS em seu servidor DNS de empresas.
* Se o site tem páginas seguras usando `https:` o protocolo e você não está usando o serviço de ID da Experience Platform, você pode trabalhar com a Adobe para obter um certificado SSL para implementar cookies primários.

O processo de emissão de certificado SSL geralmente pode ser confuso e demorado. Como resultado, a Adobe estabeleceu uma parceria com digicert, uma autoridade de certificação líder do setor (CA) e desenvolveu um processo integrado pelo qual a compra e o gerenciamento desses certificados são automatizados.

Com sua permissão, trabalharemos com a CA para emitir, implantar e gerenciar um novo certificado SSL de SHA -2 para você. A Adobe continuará a gerenciar esse certificado e garantirá que uma expiração, revogação ou preocupação de segurança inesperada não prejudique a disponibilidade de sua coleção segura de organizações.

## Programa Adobe Managed Certificate

O Adobe Managed Certificate Program é o processo recomendado para implementar um novo certificado SSL próprio para cookies primários.

O programa Adobe Managed Certificate permite implementar um novo certificado SSL próprio para cookies primários sem custo adicional. Se você possui o seu próprio certificado SSL gerenciado pelo cliente, fale com o Atendimento ao cliente da Adobe sobre a migração para o Adobe Managed Certificate Program.

### Implementação

A seguir, você implementa um novo certificado SSL próprio para cookies primários:

1. Preencha o [formulário de solicitação de cookie primário](/help/interface/cookies/assets/FPC_Request_Form.xlsx) e abra um ticket com o Atendimento ao cliente solicitando a configuração de cookies primários no programa Adobe Managed. Cada campo é descrito no documento com exemplos. 

1. Crie registros CNAME (consulte as instruções abaixo). Ao receber o bilhete, um especialista FPSSL deve fornecer um par de registros CNAME. Esses registros devem ser configurados no servidor DNS da sua empresa antes que a Adobe possa comprar o certificado em seu nome. Os CNAMES serão semelhantes ao seguinte: **Protegido** - por exemplo, o nome do host `smetrics.example.com` aponta para: `example.com.ssl.d1.omtrdc.net`. **Não seguro** - por exemplo, o nome do host `metrics.example.com` aponta para: `example.com.d1.omtrdc.net`.

1. Quando esses CNAMES estiverem em vigor, a Adobe trabalhará com digicert para comprar e instalar um certificado nos servidores de produção da Adobe. Se você tiver uma implementação existente, considere a Migração do visitante para manter os visitantes existentes. Depois que o certificado for enviado ao ambiente de produção da Adobe, você poderá atualizar as variáveis do servidor de rastreamento para os novos nomes de host. Ou seja, se o site não for seguro (https), atualize o `s.trackingServer`. Se o site for seguro (https), atualize as duas `s.trackingServer``s.trackingServerSecure` e as variáveis.

1. Ping do nome do host (veja abaixo).

1. Atualizar código de implementação (veja abaixo).

### Manutenção e Renovações

Os certificados SSL expiram anualmente, o que significa que a Adobe deve comprar um novo certificado para cada implementação anualmente. Todos os usuários suportados na organização receberão uma notificação por email sempre que uma implementação estiver próxima à expiração. Para que a Adobe renovar seu nome de host, um usuário suportado deverá responder ao email da Adobe e indicar que pretende continuar a usar o nome de host expandido para a coleta de dados. Nesse momento, a Adobe compra e instala automaticamente um novo certificado.

### Perguntas frequentes

| Pergunta | Resposta |
|---|---|
| **Esse processo está protegido?** | Sim, o programa Adobe Managed é mais seguro do que o nosso método legado, pois nenhum certificado ou chave privada muda para fora da Adobe e da autoridade de certificação emissora. |
| **Como a Adobe pode comprar um certificado para o nosso domínio?** | O certificado só pode ser comprado quando você apontou o nome do host especificado (por exemplo, smetrics.example.com) para um nome de host da Adobe. Isso basicamente delega esse nome de host à Adobe e permite que a Adobe comprem o certificado em seu nome. |
| **É possível solicitar que o certificado seja revogado?** | Sim, como proprietário do domínio, você está autorizado a solicitar o certificado revogado. Você só precisará abrir um ticket com o Atendimento ao cliente para que isso seja concluído. |
| **Esse certificado estará usando a criptografia SHA -2?** | Sim, a Adobe trabalhará com digicert para emitir um certificado SHA -2. |
| **Isso gera custo adicional?** | Não, a Adobe disponibiliza esse serviço para todos os clientes atuais do Analytics sem custo adicional. |

## Criar registros CNAME

A equipe de operações de rede de sua organização deve configurar seus servidores DNS criando novo (s) registro (s) CNAME. Cada nome de host encaminhar dados para os servidores de coleta de dados da Adobe.

O especialista FPC fornece os nomes de hosts configurados e os cnames aos quais eles devem ser apontados. Por exemplo:

* **Nome do host SSL**:`smetrics.mysite.com`
* **CNAME SSL**:`mysite.com.ssl.d1.sc.omtrdc.net`
* **Nome do host não SSL**:`metrics.mysite.com`
* **CNAME não SSL**:`mysite.com.d1.sc.omtrdc.net`

Desde que o código de implementação não seja alterado, essa etapa não afetará a coleção de dados e poderá ser feita a qualquer momento depois de atualizar o código de implementação.

>[!Note:] O serviço de ID de visitante da Experience Cloud fornece uma alternativa para configurar um CNAME para ativar cookies primários.

## Ping do nome do host

Ping o nome do host para garantir o encaminhamento correto. Todos os nomes de host devem responder a um ping para evitar perda de dados.

Depois que os registros CNAME forem configurados corretamente, e a Adobe tiver confirmado a instalação do certificado, abra um prompt de comando e faça ping do (s) nome (s) do host. Using `mysite.com` as an example: `ping metrics.mysite.com`

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

>[!Note:] Se estiver usando `https:// protocol`, o ping só responderá depois da data de upload especificada pelo especialista FPC. Além disso, verifique se o nome do host seguro e o nome do host não seguro estão funcionando corretamente antes de atualizar a implementação.

## Atualização do código de implementação

Antes de editar o código em seu site para utilizar cookies primários, preencha estes pré-requisitos:

* Solicite um certificado SSL, conforme descrito acima nas Etapas de implementação para o Adobe Managed Certificate Program.
* Crie registros CNAME (veja acima).
* Ping do nome do host (veja acima).

Depois de verificar se os nomes do host estão respondendo e encaminhando para os servidores de coleta de dados da Adobe, você pode alterar sua implementação para apontar para seus próprios nomes de host de coleção de dados.

1. Open your core JavaScript file (`s_code.js/AppMeasurement.js`).
1. Se quiser atualizar a versão de seu código, substitua o arquivo`s_code.js/AppMeasurement.js`   completo pela versão mais nova e substitua todos os plug-ins ou personalizações (se houver). **Ou**, se quiser atualizar o código pertinentes a cookies primários, localize as variáveis s. trackingserver e s. trackingserversecure (se estiver usando o SSL) e aponte-as para os novos nomes de host da coleção de dados. Using mysite.com as an example:`s.trackingServer = "metrics.mysite.com"` `s.trackingServerSecure = "smetrics.mysite.com"`

1. Carregue o arquivo javascript principal atualizado em seu site.

1. Se você estiver mudando para cookies primários a partir de uma implementação longa ou mudando para um nome de host de coleção primário diferente, recomendamos migrar os visitantes do domínio anterior para o novo domínio.

Consulte [Migração de visitante](https://docs.adobe.com/help/en/analytics/implementation/javascript-implementation/visitor-migration.html) no Guia de implementação do Analytics.

Depois de carregar o arquivo javascript, tudo é configurado para a coleta de dados do cookie primário. Recomendamos que você monitore os relatórios do Analytics das próximas horas para garantir que a coleta de dados continue como normal. Caso contrário, verifique se todas as etapas acima foram concluídas e faça com que um dos usuários suportados da organização entre em contato com o Atendimento ao cliente.
