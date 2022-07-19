---
description: Saiba como o Adobe Analytics usa cookies para fornecer informações sobre variáveis e componentes que não persistem entre as solicitações de imagem e as sessões do navegador.
keywords: cookies; privacidade
solution: Experience Cloud,Analytics
title: '"Cookies próprios "'
index: y
snippet: y
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: e15abde5-8027-4aed-a0c1-8a6fc248db5e
source-git-commit: 00a6aa791dd08c2907cd09c17b7e2a1e62b060c1
workflow-type: tm+mt
source-wordcount: '1604'
ht-degree: 91%

---

# Sobre cookies próprios

O Analytics usa cookies para fornecer informações sobre variáveis e componentes que não persistem entre as solicitações de imagem e as sessões do navegador. Sempre que possível, a Adobe usa cookies primários para registrar atividades no site. Para registrar a atividade em sites diferentes, como em outros domínios pertencentes a você, são necessários cookies de terceiros.

Muitos navegadores e aplicativos antispyware foram projetados para rejeitar e excluir cookies de terceiros. O Adobe garante que os cookies sempre possam ser definidos, mesmo que os cookies de terceiros estejam bloqueados. O comportamento específico varia dependendo de você estar usando o Experience Platform Identity Service (serviço ECID) ou os identificadores herdados do Analytics (também conhecidos como o cookie s_vi):

* O [Experience Platform Identity Service (ECID Service)](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html?lang=pt-BR) definirá cookies primários de forma automática, independentemente de o domínio de coleção corresponder ao domínio do site. Se não corresponderem, o Identity Service usará o JavaScript para definir cookies no domínio do site.
* Se estiver usando [identificadoes herdados do Analytics](https://experienceleague.adobe.com/docs/core-services/interface/administration/ec-cookies/cookies-analytics.html?lang=pt-BR) (também conhecidos como cookies `s_vi`), dependerá de como você configurou o servidor de coleção de dados. Se o servidor de coleção de dados corresponder ao domínio do site, os cookies serão definidos como primários. Se o servidor de coleção não corresponder a seu domínio atual, os cookies serão definidos como de terceiros. Nesse caso, se os cookies de terceiros estiverem bloqueados, o Analytics definirá um cookie primário [fallback id (s_fid)](cookies-analytics.md) em vez do cookie padrão &quot;s_vi&quot;.

Se quiser garantir que o servidor de coleção corresponda ao domínio do site, você poderá usar uma implementação CNAME que habilitará o encaminhamento de um domínio personalizado especificado na implementação CNAME para os servidores de coleção da Adobe. Isso envolve alterações nas configurações de DNS da empresa para configurar um alias CNAME para apontar para um domínio hospedado pela Adobe. Observe que, embora vários produtos da Adobe sejam compartíveis com o uso de um CNAME, em todos os casos o CNAME é usado para criar um endpoint de terceiros confiável para um cliente específico, e é de sua propriedade. Se você controlar vários domínios, eles poderão usar um único endpoint CNAME para rastrear usuários em seus domínios, mas sempre que o domínio do site não for correspondente ao CNAME, os cookies desse domínio serão definidos como de terceiros.

>[!NOTE]
>
>Independentemente de o domínio de coleta corresponder ao domínio do site, o programa de Prevenção de Rastreamento Inteligente (ITP) da Apple faz com que os cookies primários definidos pelo Adobe tenham curta duração em navegadores regidos pela ITP, que incluem o Safari no macOS e todos os navegadores no iOS e iPadOS. A partir de novembro de 2020, os cookies definidos por CNAME também terão a mesma expiração dos cookies definidos pelo JavaScript. Essa expiração está sujeita a alterações.

Se você quiser estabelecer um CNAME para a coleção de dados e se o site tiver páginas seguras que usem o protocolo HTTPS, será possível trabalhar com a Adobe para obter um certificado SSL.

Muitas vezes o processo de emissão do certificado SSL pode ser confuso e demorado. Como resultado, a Adobe estabeleceu uma parceria com a DigiCert, uma Autoridade de certificação (CA) que é líder do setor, e desenvolveu um processo integrado pelo qual a compra e o gerenciamento desses certificados são automatizados.

Com sua permissão, trabalharemos com a CA para emitir, implantar e gerenciar um novo certificado SSL SHA-2 para você. A Adobe continuará a gerenciar esse certificado e garantirá que uma expiração, uma revogação ou uma preocupação de segurança inesperada não prejudiquem a disponibilidade da coleção segura de suas organizações.

## Programa de certificado gerenciado pela Adobe

O Adobe Managed Certificate Program é o processo recomendado para configurar o certificado SSL próprio necessário para uma implementação CNAME, o que garante que o servidor de coleção da Adobe corresponde ao domínio do site.

O Adobe Managed Certificate Program permite implementar um novo certificado SSL próprio sem custo adicional (para os primeiros 100 CNAMEs). Se você tem seu próprio certificado SSL gerenciado pelo cliente no momento, consulte o Atendimento ao cliente da Adobe sobre a migração para o Adobe Managed Certificate Program.

### Implementação

A seguir, veja como implementar um novo certificado SSL próprio para coleção de dados próprios.

1. Preencha o [Formulário de solicitação de domínio própri](/help/interface/cookies/assets/First_Part_Domain_Request_Form.xlsx) e abra um tíquete para o Atendimento ao cliente solicitando a configuração da coleção de dados próprios no programa gerenciado pela Adobe.
Category: Adobe checklist 
Cada campo é descrito no documento com exemplos.

2. Crie registros CNAME (consulte as instruções abaixo).

   Ao receber a solicitação, um representante do Atendimento ao cliente deve fornecer a você um registro CNAME. Esses registros devem ser configurados no servidor DNS da empresa antes que a Adobe possa comprar o certificado em seu nome. O CNAME é semelhante ao seguinte:

   **Seguro** - por exemplo, o nome de host `smetrics.example.com` aponta para: `example.com.adobedc.net`.

>[!NOTE]
> Anteriormente, o Adobe recomendava que os clientes configurassem dois CNAME, um para HTTPS e outro para HTTP. Como é uma prática recomendada criptografar o tráfego e a maioria dos navegadores está desencorajando o HTTP, não recomendamos mais configurar um CNAME para HTTP. Entre em contato com o Atendimento ao cliente do Adobe para configurar o CNAME para HTTP.

1. Quando o CNAME estiver em vigor, a Adobe trabalhará com a DigiCert para comprar e instalar um certificado nos servidores de produção da Adobe.

   Se tiver uma implementação existente, considere a Migração do visitante para manter os visitantes existentes. Depois que o certificado for enviado ao ambiente de produção da Adobe, você poderá atualizar as variáveis do servidor de rastreamento para os novos nomes de host. Ou seja, se o site não for seguro (HTTP), atualize o `s.trackingServer`. Se o site for seguro (HTTPS), atualize as variáveis `s.trackingServer` e `s.trackingServerSecure`.

2. [Validar o encaminhamento do nome do host](#validate) (veja abaixo).

3. [Atualizar o código de implementação](#update) (veja abaixo).

### Manutenção e Renovações

Os certificados SSL expiram todo ano, o que significa que a Adobe deve comprar um novo certificado para cada implementação anualmente. Todos os usuários com suporte na organização receberão uma notificação por email sempre que uma implementação estiver próxima de expirar. Para que a Adobe renove o nome de host, um usuário suportado deverá responder ao email da Adobe e indicar que pretende continuar a usar o nome de host que está expirando para a coleta de dados. Nesse momento, a Adobe compra e instala automaticamente um novo certificado.

### Perguntas frequentes

| Pergunta | Resposta |
|---|---|
| **Esse processo é seguro?** | Sim, o programa Adobe Managed é mais seguro que nosso método antigo, pois nenhum certificado ou chave privada muda de mãos fora da Adobe e da autoridade de certificação emissora. |
| **Como a Adobe pode comprar um certificado para o nosso domínio?** | O certificado só pode ser comprado quando você aponta o nome de host especificado (por exemplo, `telemetry.example.com`) para um nome de host da Adobe. Essa ação basicamente delega esse nome de host à Adobe e permite que a Adobe compre o certificado em seu nome. |
| **É possível solicitar que o certificado seja revogado?** | Sim, como proprietário do domínio, você tem direito a solicitar que o certificado seja revogado. Abra um ticket no Atendimento ao cliente para fazer com que isso seja concluído. |
| **Esse certificado usará a criptografia SHA-2?** | Sim, o Adobe trabalha com a DigiCert para emitir um certificado SHA-2. |
| **Isso gera custo adicional?** | Não, a Adobe disponibiliza esse serviço para todos os clientes atuais da Adobe Digital Experience sem custo adicional. |

{style=&quot;table-layout:auto&quot;}

## Criar registros CNAME

A equipe de operações de rede da organização deve configurar os servidores DNS criando novos registros CNAME. Cada nome de host encaminha os dados para os servidores de coleta de dados da Adobe.

O especialista em FPC fornece o nome de host configurado e o CNAME para o qual ele deve ser apontado. Por exemplo:

* **Nome de host SSL**: `smetrics.mysite.com`
* **CNAME SSL**: `mysite.com.adobedc.net`

>[!NOTE]
> Se você ainda usar um não seguro, ele será assim:
> * **Nome de host não SSL**: `metrics.mysite.com`
> * **CNAME não SSL**: `mysite.com.adobedc.net`


Contanto que o código de implementação não seja alterado, esta etapa não afetará a coleta de dados e poderá ser feita a qualquer momento após a atualização do código de implementação.

## Validar o encaminhamento do nome do host {#validate}

Os seguintes métodos estão disponíveis para validação:

### Validar usando um navegador

Se você tiver um CNAME configurado e o certificado instalado, poderá usar o navegador para validação:

`https://smetrics.adobe.com/_check`

>[!NOTE]
>
>Você verá um aviso de segurança se um certificado não estiver instalado.

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

Você pode usar `nslookup` para validação. Usando `smetrics.adobe.com`como exemplo, abra um prompt de comando e digite `nslookup smetrics.adobe.com`

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

Antes de editar o código no site para utilizar a coleção de dados próprios, conclua estes pré-requisitos:

* Solicite um certificado SSL seguindo as etapas descritas acima, na seção *Implementação* do [Adobe-Managed Certificate Program](#adobe-managed-certificate-program).
* Criar registros CNAME (veja acima).
* Validar os nomes de host (veja acima).

Após verificar que os nomes de host estão respondendo e encaminhando para os servidores de coleta de dados da Adobe, você pode alterar a implementação para apontar para seus próprios nomes de host de coleção de dados.

1. Abra seu arquivo JavaScript principal (`s_code.js/AppMeasurement.js`).
1. Se quiser atualizar a versão de seu código, substitua o arquivo`s_code.js/AppMeasurement.js` completo pela versão mais nova e substitua todos os plug-ins ou personalizações (se houver). **Ou**, se quiser atualizar o código pertinente somente à coleção de dados próprios, localize as variáveis s.trackingServer e s.trackingServerSecure (se estiver usando o SSL) e aponte-as para os novos nomes de host da coleção de dados. Usando o mysite.com como exemplo:`s.trackingServer = "metrics.mysite.com"` `s.trackingServerSecure = "smetrics.mysite.com"`

1. Carregue o arquivo JavaScript principal atualizado em seu site.

1. Se você está mudando de uma implementação de longa data para a coleção de dados próprios ou mudando para um nome de host de coleção própria diferente, a Adobe recomenda migrar os visitantes do domínio anterior para o novo domínio.

Consulte [Migração de visitantes](https://experienceleague.adobe.com/docs/analytics/technotes/visitor-migration.html?lang=pt-BR) no Guia de implementação do Analytics.

Após carregar o arquivo JavaScript, tudo é configurado para a coleta de dados de próprio. A Adobe recomenda monitorar os relatórios do Analytics das próximas horas, para garantir que a coleção de dados continue normalmente. Caso contrário, verifique se todas as etapas acima foram concluídas e peça para um dos usuários suportados da organização entrar em contato com o Atendimento ao cliente.
