---
description: Saiba como configurar certificados seguros para usar com cookies primários do Adobe Experience Cloud.
solution: Experience Cloud,Analytics
title: Programa de certificado gerenciado pela Adobe
index: y
snippet: y
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: e15abde5-8027-4aed-a0c1-8a6fc248db5e
source-git-commit: 2a80851c0a7d4ef7dbcc2565177b239f3e063164
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 4%

---

# Programa de certificado gerenciado pela Adobe

O programa de certificados gerenciado por Adobe é o processo recomendado para configurar certificados primários necessários para uma implementação CNAME. O programa é totalmente automatizado depois de configurado. Ele renova certificados em tempo hábil para que não haja impacto na coleta de dados devido a certificados expirados. O programa é gratuito para os primeiros 100 CNAMEs.

Se você gerencia seus próprios certificados no momento, é responsável por comprar, manter e fornecer um certificado ao Adobe para uso de cookies próprios. Você pode entrar em contato com o Atendimento ao cliente do Adobe para discutir a migração para o programa de certificados gerenciados por Adobe.

## Implementação

Siga estas etapas para implementar um novo certificado para a coleção de dados próprios:

1. Baixe e preencha o [Formulário de solicitação de domínio próprio](cookies/assets/First_Party_Domain_Request_Form.xlsx)

1. Abra um tíquete no Atendimento ao cliente do Adobe solicitando a configuração da coleta de dados primários no programa de certificados gerenciados por Adobe.

1. Ao receber o tíquete, o representante da Adobe fornece um registro CNAME. Esses registros devem ser configurados no servidor DNS da empresa antes que a Adobe possa comprar o certificado em seu nome. Por exemplo, o nome de host `data.example.com` aponta para `hiodsibxvip01.data.adobedc.net`.

1. Quando o registro CNAME está em vigor nos servidores da sua organização, o Adobe trabalha com a DigiCert para comprar e instalar um certificado nos servidores de coleta de dados do Adobe.

## Validar o encaminhamento do nome do host {#validate}

Depois que o Adobe instalar o certificado, você poderá usar um dos métodos a seguir para validar se ele está funcionando.

+++**Validação do navegador**

Você pode usar qualquer navegador para validar se um certificado está instalado corretamente. Digite seu CNAME com `_check` como o caminho para a barra de endereços. Por exemplo:

`data.example.com/_check`

Se tudo funcionar, o navegador mostrará `SUCCESS`. Se o certificado não estiver instalado corretamente, você receberá um aviso de segurança.

+++

+++**Linha de comando (`curl`)**

A maioria dos sistemas operacionais modernos já tem o [`curl`](https://curl.se) instalado.

Digite o seguinte na linha de comando:

```sh
curl data.example.com/_check
```

Se tudo funcionar corretamente, o console retornará `SUCCESS`.

>[!TIP]
>
>Você pode usar o sinalizador `-k` para desabilitar o aviso de segurança para ajudar na solução de problemas.

+++

+++**Linha de comando (`nslookup`)**

Digite o seguinte na linha de comando:

```sh
nslookup data.example.com
```

Se tudo funcionar corretamente, os servidores de coleta de dados do Adobe são retornados:

```text
Server: hiodsibxvip01.corp.adobe.com
Address: 10.50.112.247

Name: example.com.ssl.d1.sc.omtrdc.net
Addresses: 63.140.37.126
    63.140.37.206
    63.140.36.51
    63.140.36.145
Aliases: smetrics.example.com
```

+++

## Atualizar código de implementação {#update}

Depois de validar que seu certificado funciona corretamente, você pode atualizar sua implementação de Adobe para usar esses valores.

* Para implementações do Adobe Analytics AppMeasurement, atualize a variável de configuração [`trackingServer`](https://experienceleague.adobe.com/en/docs/analytics/implementation/vars/config-vars/trackingserver). Se você tiver uma implementação existente, consulte [Migração de visitante](https://experienceleague.adobe.com/en/docs/analytics/technotes/visitor-migration) para obter etapas adicionais sobre como impedir que visitantes existentes sejam contados como novos visitantes.
* Para implementações do SDK da Web, atualize a propriedade [`edgeDomain`](https://experienceleague.adobe.com/en/docs/experience-platform/web-sdk/commands/configure/edgedomain) no comando [`configure`](https://experienceleague.adobe.com/en/docs/experience-platform/web-sdk/commands/configure/overview).

## Manutenção e renovações

Trinta dias antes do certificado próprio expirar, o Adobe valida se o CNAME ainda é válido e está em uso. Em caso afirmativo, o Adobe presume que você deseja continuar usando o serviço e renova automaticamente o certificado em seu nome.

>[!IMPORTANT]
>
>Se o registro CNAME da sua organização for removido ou não mapear mais para o nome de host seguro do Adobe fornecido, o Adobe não poderá renovar o certificado. A entrada no sistema Adobe é marcada para remoção sem outras comunicações.

## Perguntas frequentes

+++Este processo é seguro?

Sim. O programa de certificados gerenciado por Adobe é mais seguro do que a organização que fornece um certificado para o Adobe. Nenhum certificado ou chave privada muda de mãos fora do Adobe e da autoridade de certificação emissora.

+++

+++Como o Adobe pode comprar um certificado para o nosso domínio?

O certificado só pode ser comprado quando você aponta o nome de host especificado para um nome de host de propriedade de Adobe. Você basicamente delega esse nome de host ao Adobe e permite que o Adobe compre o certificado em seu nome.

+++

+++É possível solicitar que o certificado seja revogado?

Sim. Como proprietário do domínio, você está autorizado a solicitar que o certificado seja revogado. Entre em contato com o Atendimento ao cliente do Adobe para iniciar esse processo.

+++

+++Que tipo de criptografia é usado?

O Adobe funciona com DigiCert para emitir um certificado SHA-2.

+++

+++Este programa implica algum custo adicional?

Não. A Adobe oferece esse serviço a todos os clientes da Adobe Experience Cloud sem custo adicional.

+++

+++Quais níveis de segurança de criptografia o Adobe oferece?

O Adobe oferece dois níveis de segurança de criptografia para atender às diversas necessidades de segurança do cliente na coleta de dados primários. Esses níveis determinam quais algoritmos de criptografia são compatíveis com as conexões HTTPS com servidores Adobe. O Adobe revisa e atualiza regularmente o conjunto de algoritmos compatíveis com base nas práticas atuais de segurança. Se você quiser alterar as configurações de segurança de criptografia, entre em contato com o Atendimento ao cliente.

* **Standard** requer TLS 1.2 ou mais recente e criptografia de pelo menos 128 bits. Ele foi projetado para fornecer a mais ampla compatibilidade de dispositivos, mantendo a criptografia segura.
* **Alto** nível de segurança de criptografia requer TLS 1.2 ou mais recente e remove o suporte para cifras mais fracas. Ele foi projetado para clientes que desejam a criptografia mais forte e não estão preocupados com o suporte para dispositivos mais antigos.

Os seguintes clientes são conhecidos por não conseguirem se conectar com a segurança de criptografia definida como **Alta**:

* Windows 8.1 e anterior (última atualização em 2018)
* Windows Phone 8.1 e anterior (última atualização em 2016)
* OS X 10.10 e anterior (última atualização em 2017)
* iOS 8.4 e anterior (última atualização em 2015)

+++

+++Quais tipos de certificados HTTPS são compatíveis?

O Adobe oferece suporte aos tipos de certificado RSA e ECC para atender às diversas necessidades dos clientes. Os certificados RSA têm suporte mais amplo para clientes, mas os certificados ECC usam menos processamento no servidor e no cliente. Para certificados gerenciados por Adobe, são fornecidos RSA e ECC. Para certificados gerenciados pelo cliente, é necessário RSA e recomenda-se ECC. Clientes modernos são compatíveis com RSA e ECC. Os seguintes clientes geralmente só oferecem suporte a certificados RSA:

* Windows Vista e anteriores (última atualização em 2012)
* Windows Phone 8.0 e anterior (última atualização em 2014)
* OS X 10.8 e anterior (última atualização em 2013)
* iOS 5.1 e anterior (última atualização em 2012)
* Android 4.3 e anterior (última atualização em 2013)

+++
