---
title: Endereços IP do Adobe Experience Cloud
description: Se o firewall da sua organização bloquear endereços IP originados da Adobe, use esta lista para atualizar as configurações do firewall.
exl-id: e24a70e4-9ed4-4b87-8bab-4ed0aebedd1f
source-git-commit: 2691f0dc91e48a8f817467e334d9028f2e506e70
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 27%

---

# Domínios e endereços IP do Adobe Experience Cloud

Algumas configurações de firewall bloqueiam endereços IP dos servidores de coleção de dados da Adobe ou dos servidores responsáveis por acessar os dados do Você pode usar essa lista de intervalos para alterar as configurações de firewall da sua organização para permitir acesso e enviar dados de dentro da organização. Esta página inclui sistemas de entrada (como a coleta de dados) e sistemas de saída (como feeds de dados no Adobe Analytics) que o Adobe usa.

>[!IMPORTANT]
>
>Embora o Adobe faça o possível para manter esse documento atualizado, não é possível garantir que a lista de intervalos IP permaneça a mesma. As possíveis alterações incluem o crescimento e a expansão dos negócios, um registro da Internet exige alterações no espaço de endereço IP do Adobe ou um provedor de serviços de Internet deixa de funcionar.

Além dos blocos de endereço IP listados abaixo, os produtos Adobe Experience Cloud individuais têm seus próprios domínios que usam:

* [Adobe Experience Cloud](domains.md)
* Adobe Analytics
* Customer Journey Analytics

## Todos os blocos de endereço IP da Adobe

A tabela a seguir abrange todos os endereços IP de propriedade de Adobe. Essa tabela inclui todos os escritórios de funcionários de Adobe e data centers executados pelo Adobe globalmente. Não inclui serviços hospedados em nuvens públicas.

| Bloco IP (Notação CIDR) |
| --- |
| `63.140.32.0/19` |
| `66.117.16.0/20` |
| `66.235.128.0/19` |
| `130.248.0.0/16` |
| `172.82.192.0/18` |
| `185.34.188.0/22` |
| `192.243.240.0/22` |

{style="table-layout:auto"}

## Coleta de dados do Adobe Experience Cloud e blocos de endereço IP de FTP

Se a empresa preferir permitir intervalos específicos de endereço IP, você pode consultar a tabela a seguir. O serviço inclui:

* Servidores de coleção de dados para todos os produtos Experience Cloud
* Servidores FTP para todos os produtos Experience Cloud

Todos os intervalos IP desta seção estão incluídos na tabela acima.

| Localização | Intervalo IP (Notação CIDR) |
| --- | --- |
| Austrália | `63.140.55.0/24` |
| Austrália | `63.140.56.0/23` |
| Califórnia | `63.140.32.0/23` |
| Califórnia | `63.140.34.0/24` |
| França | `63.140.62.0/23` |
| Índia | `66.117.20.0/24` |
| Índia | `66.117.22.0/23` |
| Japão | `130.248.169.0/23` |
| Japão | `63.140.50.0/23` |
| Japão | `66.117.31.0/24` |
| Londres | `66.235.156.0/24` |
| Londres | `185.34.188.0/22` |
| Londres | `130.248.152.0/22` |
| Londres | `130.248.244.0/23` |
| Oregon | `66.235.132.0/22` |
| Oregon | `130.248.130.0/23` |
| Oregon | `130.248.150.0/24` |
| Oregon | `130.248.160.0/21` |
| Oregon | `192.243.242.0/24` |
| Singapura | `130.248.170.0/23` |
| Singapura | `130.248.240.0/24` |
| Singapura | `63.140.44.0/22` |
| Singapura | `63.140.48.0/23` |
| Singapura | `66.117.30.0/24` |
| Singapura | `172.82.240.8/29` |
| Singapura | `172.82.240.88/29` |
| Virgínia | `63.140.38.0/23` |
| Virgínia | `63.140.54.0/24` |

{style="table-layout:auto"}

O Adobe Experience Cloud também oferece suporte ao IPv6 em capacidade limitada. Esses blocos IP atendem a objetivos de coleta de dados semelhantes aos de seus equivalentes IPv4 acima, mas não incluem FTP.

| Localização | Host |
| --- | --- |
| Austrália | `2406:da1c:406:1a00::/56` |
| Austrália | `2406:da1c:ce5:b400::/56` |
| Califórnia | `2600:1f1c:366:d900::/56` |
| França | `2a05:d012:706:d000::/56` |
| Índia | `2406:da1a:f34:6a00::/56` |
| Irlanda | `2a05:d018:309:600::/56` |
| Japão | `2406:da14:b07:ab00::/56` |
| Oregon | `2600:1f14:1eb:7d00::/56` |
| Oregon | `2600:1f14:9d3:2b00::/56` |
| Singapura | `2406:da18:6e8:1e00::/56` |
| Virgínia | `2600:1f18:1a20:e800::/56` |
| Virgínia | `2600:1f18:4fd:6000::/56` |
| Virgínia | `2600:1f18:b00:e100::/56` |
| Virgínia | `2600:1f18:d1f:bd00::/56` |

>[!TIP]
>
>As conexões FTP para recursos de exportação do Adobe Analytics (incluindo Data Warehouse e feeds de dados) são originadas apenas de endereços IPv4 nos locais de Londres, Oregon e Singapura.
