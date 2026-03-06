---
description: Saiba como configurar certificados seguros para usar com cookies primários do Adobe Experience Cloud.
solution: Experience Cloud,Analytics
title: Programa de certificado gerenciado pela Adobe
index: true
snippet: y
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: e15abde5-8027-4aed-a0c1-8a6fc248db5e
TQID: https://experienceleague.adobe.com/LWbjh-jXKmY6mcl047uzA1ZkhZlAmeNpt9JRg3Ynt9E
product_v2: id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87id: e55547f1-a1ff-40c6-8978-026e40ab7fa4
feature_v2: id: b3f03848-ae12-48b2-8aab-cad18567eb32id: e9dbdbc5-3e52-40f0-a7bc-e18542967b7aid: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2: id: b75843fa-0a67-4a44-a6b1-cc627b0481dcid: c8add8f2-4250-4fd9-9cde-9707036c567did: d2311670-43bd-4c2e-bc98-1da2aaba9cefid: e992d880-33bc-4949-a648-aa7d410276cdid: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: c1579802-ddd4-4214-8a91-97b2066abe11id: c2be0313-b3ae-45e0-b454-d20bf54b23f2id: d095671a-1355-40aa-8b5f-06c33c68080bid: d3cdead0-685a-4489-9250-4bb709942f66id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 5354e3c8a48184315ca4eaa8c8de1d12493cc227
workflow-type: tm+mt
source-wordcount: 1106
ht-degree: 3%

---

# Programa de certificado gerenciado pela Adobe

O programa de certificados gerenciados pela Adobe é o processo recomendado para configurar certificados primários necessários para uma implementação CNAME. O programa é totalmente automatizado depois de configurado. Ele renova certificados em tempo hábil para que não haja impacto na coleta de dados devido a certificados expirados. O programa é gratuito para os primeiros 100 CNAMEs.

Se você gerencia seus próprios certificados no momento, é responsável por comprar, manter e fornecer um certificado à Adobe para uso de cookies próprios. Você pode entrar em contato com o Atendimento ao cliente da Adobe para discutir a migração para o programa de certificados gerenciados pela Adobe.

## Implementação

Siga estas etapas para implementar um novo certificado para a coleção de dados próprios:

1. Baixe e preencha o [Formulário de solicitação de domínio próprio](cookies/assets/First_Party_Domain_Request_Form.xlsx)
1. Abra um tíquete no Atendimento ao cliente da Adobe solicitando a configuração da coleta de dados primários no programa de certificados gerenciados pela Adobe.
1. Ao receber o tíquete, o representante da Adobe fornece um registro CNAME. Esses registros devem ser configurados no servidor DNS da empresa antes que a Adobe possa comprar o certificado em seu nome. Por exemplo, o nome de host `data.example.com` aponta para `hiodsibxvip01.data.adobedc.net`.
1. Quando o registro CNAME estiver em vigor nos servidores da organização, a Adobe trabalhará com a DigiCert para comprar e instalar um certificado nos servidores de coleta de dados da Adobe.

## Validar o encaminhamento do nome do host

Depois que o Adobe tiver instalado o certificado, você poderá usar um dos métodos a seguir para validar se ele está funcionando.

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

Se tudo funcionar corretamente, os servidores de coleta de dados da Adobe serão retornados:

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

## Atualizar código de implementação

Depois de validar que o certificado funciona corretamente, você pode atualizar a implementação do Adobe para usar esses valores.

* **Extensão de marca do Web SDK**: atualize o campo [[!UICONTROL Edge domain]](https://experienceleague.adobe.com/en/docs/experience-platform/tags/extensions/client/web-sdk/web-sdk-extension-configuration) ao configurar a extensão.
* **Web SDK (liga)**: atualize a propriedade [`edgeDomain`](https://experienceleague.adobe.com/en/docs/experience-platform/web-sdk/commands/configure/edgedomain) no comando [`configure`](https://experienceleague.adobe.com/en/docs/experience-platform/web-sdk/commands/configure/overview).
* **Extensão do Adobe Analytics**: atualize o campo [[!UICONTROL SSL Tracking Server]](https://experienceleague.adobe.com/en/docs/experience-platform/tags/extensions/client/analytics/overview) ao configurar a extensão. Verifique se você também tem a [extensão de tag do Serviço de ID de visitante](https://experienceleague.adobe.com/en/docs/experience-platform/tags/extensions/client/id-service/overview) instalada. Consulte [Identificação do visitante usando a extensão de tag do Analytics](https://experienceleague.adobe.com/en/docs/analytics/implementation/id/analytics-extension) para obter mais informações.
* **AppMeasurement**: atualize a variável de configuração [`trackingServerSecure`](https://experienceleague.adobe.com/en/docs/analytics/implementation/vars/config-vars/trackingserversecure). Verifique se você também implementou o [Serviço de ID de Visitante](https://experienceleague.adobe.com/pt-br/docs/id-service/using/home) usando o `VisitorAPI.js`. Consulte [Identificação do visitante usando o AppMeasurement](https://experienceleague.adobe.com/en/docs/analytics/implementation/id/analytics-extension) para obter mais informações.

Se o site usar vários métodos de implementação e você não puder atualizar todos eles simultaneamente, considere configurar um período de carência. Consulte [Considerações sobre a migração do Serviço de ID de visitante](https://experienceleague.adobe.com/en/docs/analytics/implementation/id/migration) para obter etapas adicionais sobre como evitar que os visitantes sejam contados como novos visitantes em seu site.

## Manutenção e renovações

Trinta dias antes do certificado próprio expirar, a Adobe valida se o CNAME ainda é válido e está em uso. Em caso afirmativo, a Adobe presume que você deseja continuar usando o serviço e renova automaticamente o certificado em seu nome.

>[!IMPORTANT]
>
>Se o registro CNAME da sua organização for removido ou não mapear mais para o nome de host seguro fornecido pela Adobe, a Adobe não poderá renovar o certificado. A entrada no sistema do Adobe está marcada para remoção sem comunicação adicional.

## Perguntas frequentes

+++Esse processo é seguro?

Sim. O programa de certificados gerenciado pela Adobe é mais seguro do que a organização que fornece um certificado à Adobe. Nenhum certificado ou chave privada muda de mãos fora do Adobe e da autoridade de certificação emissora.

+++

+++Como a Adobe pode comprar um certificado para o nosso domínio?

O certificado só pode ser comprado quando você aponta o nome de host especificado para um nome de host da Adobe. Você basicamente delega esse nome de host à Adobe e permite que a Adobe compre o certificado em seu nome.

+++

+++Posso solicitar que o certificado seja revogado?

Sim. Como proprietário do domínio, você está autorizado a solicitar que o certificado seja revogado. Entre em contato com o Atendimento ao cliente da Adobe para iniciar esse processo.

+++

+++Que tipo de criptografia é usado?

A Adobe trabalha com a DigiCert para emitir um certificado SHA-2.

+++

+++Esse programa gera custo adicional?

Não. A Adobe oferece esse serviço a todos os clientes da Adobe Experience Cloud sem custo adicional.

+++

+++Quais níveis de segurança de criptografia o Adobe oferece?

A Adobe oferece dois níveis de segurança de criptografia para atender às diversas necessidades de segurança do cliente na coleta de dados primários. Esses níveis determinam quais algoritmos de criptografia são compatíveis com conexões HTTPS com servidores do Adobe. A Adobe revisa e atualiza regularmente o conjunto de algoritmos compatíveis com base nas práticas atuais de segurança. Se você quiser alterar as configurações de segurança de criptografia, entre em contato com o Atendimento ao cliente.

* **Standard** requer TLS 1.2 ou mais recente e criptografia de pelo menos 128 bits. Ele foi projetado para fornecer a mais ampla compatibilidade de dispositivos, mantendo a criptografia segura.
* **Alto** nível de segurança de criptografia requer TLS 1.2 ou mais recente e remove o suporte para cifras mais fracas. Ele foi projetado para clientes que desejam a criptografia mais forte e não estão preocupados com o suporte para dispositivos mais antigos.

Os seguintes clientes são conhecidos por não conseguirem se conectar com a segurança de criptografia definida como **Alta**:

* Windows 8.1 e anterior (última atualização em 2018)
* Windows Phone 8.1 e anterior (última atualização em 2016)
* OS X 10.10 e anterior (última atualização em 2017)
* iOS 8.4 e anterior (última atualização em 2015)

+++

+++Quais tipos de certificado HTTPS são compatíveis?

A Adobe oferece suporte aos tipos de certificado RSA e ECC para atender às diversas necessidades dos clientes. Os certificados RSA têm suporte mais amplo para clientes, mas os certificados ECC usam menos processamento no servidor e no cliente. Para certificados gerenciados pela Adobe, são fornecidos RSA e ECC. Para certificados gerenciados pelo cliente, é necessário RSA e recomenda-se ECC. Clientes modernos são compatíveis com RSA e ECC. Os seguintes clientes geralmente só oferecem suporte a certificados RSA:

* Windows Vista e anteriores (última atualização em 2012)
* Windows Phone 8.0 e anterior (última atualização em 2014)
* OS X 10.8 e anterior (última atualização em 2013)
* iOS 5.1 e anterior (última atualização em 2012)
* Android 4.3 e anterior (última atualização em 2013)

+++

+++Posso gerenciar meus próprios certificados?

Sim. No entanto, se você gerenciar seus próprios certificados, será responsável por renová-los e fornecê-los à Adobe sempre que renová-los. Esse processo é menos seguro e pode causar perda de dados se sua organização esquecer de renovar um certificado a tempo. A Adobe recomenda usar o programa de certificado gerenciado em vez de gerenciar certificados por conta própria, especialmente devido a reduções na duração máxima do certificado TLS. Consulte [6.3.1 Arquivamento de chave pública](https://cabforum.org/working-groups/server/baseline-requirements/requirements/#632-certificate-operational-periods-and-key-pair-usage-periods) nos Requisitos de linha de base de certificado do servidor de fórum da autoridade de certificação/navegador para obter mais informações.
+++

