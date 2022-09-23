---
description: Perguntas frequentes sobre os atributos do cliente na Adobe Experience Cloud, no Adobe Analytics e no Adobe Target.
solution: Experience Cloud
title: Obtenha respostas para perguntas frequentes sobre os atributos do cliente
uuid: e93eb531-23c7-4d75-92e8-75699f58546a
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 6031e544-822b-4843-b3d8-98a36a3c40e8
source-git-commit: eb2ad8a8255915be47b6002a78cc810b522170d2
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 100%

---

# Perguntas frequentes sobre [!UICONTROL atributos do cliente]

Perguntas frequentes e práticas recomendadas para [!UICONTROL atributos do cliente] no Adobe Analytics e Adobe Target.

## Práticas recomendadas e limitações {#section_7F5189B3DAA84EE6865B91D2026EE05A}

Orientação e limitações ao usar [!UICONTROL atributos do cliente].

| Problema | Descrição |
|--- |--- |
| Limitações de assinatura do [!UICONTROL atributo do cliente] | Ao atualizar para o Analytics Premium, há um atraso de 24 horas antes da disponibilização de mais atributos. Você pode observar um erro de [!UICONTROL Máximo de assinatura de atributo] emitido durante esse atraso. |
| Vários logons no mesmo dispositivo | Ao usar [!UICONTROL atributos do cliente] para fazer upload de perfis de cliente em uma fonte de dados, a Adobe não recomenda que os usuários compartilhem dispositivos (ou seja, a mesma Experience Cloud ID). A Experience Cloud ID (ECID) persiste no dispositivo. O compartilhamento de dispositivos pode fazer com que a ECID vincule vários usuários à mesma ECID, resultando em resultados inesperados [!DNL Target]. **Observação:** em dispositivos móveis, a ECID é permanente depois que o aplicativo para dipositivos móveis é instalado, e você deve reinstalar o aplicativo para gerar uma nova ECID. Na Web, um novo ECID é gerado depois que o cookie do navegador é limpo. |
| Limitação diária de carregamento de frequência | A Adobe recomenda atualizar os atributos do cliente apenas uma vez por dia. Aguarde pelo menos 24 horas para carregar outro arquivo de dados de perfil do cliente para o mesmo conjunto de perfis. |
| ID personalizada do Analytics (`s.visitorID`) | Definir uma ID do cliente usando `s.visitorID` é um método para identificar usuários no Analytics. No entanto, as integrações nas quais os dados do [!DNL Analytics] são exportados ou importados usando o Serviço de ID não funcionarão quando um visitante for identificado usando `s.visitorID.`<br>Isso inclui, mas não se limita a, públicos-alvo compartilhados, [!DNL Analytics] para Adobe Target (A4T) e [!UICONTROL atributos do cliente].<br>Para essas integrações, não há suporte para uma ID personalizada do Analytics. |
| Limitações de comprimento de caracteres no [!DNL Analytics] | Ao criar uma assinatura do [!DNL Analytics], os comprimentos de campo dos arquivos de upload são truncados para 255. |

{style=&quot;table-layout:auto&quot;}

## Perguntas frequentes sobre atributos do cliente {#section_E47866EEA83348E09FE43CEC5E44C461}

| Pergunta | Resposta |
|--- |--- |
| É possível receber notificações sobre o status de upload de atributos do cliente? | Sim. |
| O que devo fazer para começar a usar os atributos do cliente? | <ol><li>Seja provisionado. Se você for um cliente do Analytics, a Adobe está provisionando para os atributos do cliente. Se você usar somente o Adobe Target e não tiver o Analytics, solicite o provisionamento para os serviços principais entrando em contato com o Atendimento ao cliente.</li> <li>Conversar com a equipe de CRM. Descubra que tipo de dados do cliente estão disponíveis e que você gostaria de usar no Analytics e em toda a Experience Cloud.</li><li>Implementar os serviços principais. Consulte [Habilitar os aplicativos para os serviços principais](core-services.md) para obter etapas sobre como modernizar a implementação. (Consulte a seção sobre sincronização de IDs de clientes para obter informações importantes.)</li></ol> **Observação:** as perguntas frequentes do administrador para implementar os serviços principais estão disponíveis [aqui](faq.md). |
| Quantos atributos do cliente eu posso usar? | Você pode fazer upload de centenas de colunas de `.csv` para o serviço de atributos do cliente. No entanto, ao configurar assinaturas e selecionar atributos, os seguintes limites poderão ser aplicados (por conjunto de relatórios), dependendo dos aplicativos que possui:  <ul><li>Foundation: 0</li><li>Select: 3</li><li>Prime: 15</li><li>Ultimate: 200</li><li>Standard: total de 3</li><li>Premium: 200</li><li>Adobe Target Standard: 5</li><li>Adobe Target Premium: 200</li></ul> |
| É necessário migrar para o Serviço da Experience Cloud ID? | A migração depende dos aplicativos que você usa. <ul><li>Adobe Analytics: recomendado </li><li>Adobe Target: obrigatório. </li></ul><br>O uso do serviço da Experience Cloud ID permite a funcionalidade mais recente da Experience Cloud, incluindo públicos em tempo real, a modernização do Adobe Target, a integração do Analytics e o rastreamento de pulsação de vídeo. <br> Para obter mais detalhes, consulte [Habilitar os aplicativos para os serviços principais](core-services.md). <br>**Observação:** o [Serviço da Experience Cloud ID](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html?lang=pt-BR) é a implementação modernizada do que era conhecido como _Serviço de ID de visitante do Analytics._ |
| Como a funcionalidade de atributo do cliente está relacionada ao Adobe Audience Manager? | Embora o Audience Manager possa receber dados para identificar o público, ele não pode executar a funcionalidade de análise que vincula os atributos aos dados comportamentais históricos. Ele também não fornece os recursos de relatórios, análise e segmentação disponíveis no Adobe Analytics. O recurso [!UICONTROL Pessoas] permite que dados avançados de vários aplicativos sejam vinculados e associados a uma única ID para uso na Experience Cloud. <br>No Adobe Target, os atributos do cliente aparecem como atributos individuais que podem ser combinados com outras regras para construir públicos. Os públicos-alvo compartilhados com o serviço [!UICONTROL People] são públicos-alvo completos que não podem ser modificados. |
| **(Somente no Analytics)** Como essa funcionalidade difere do que é fornecido no Analytics Premium? | Antes, os consumidores interessados em combinar os dados de atributo do cliente com os dados do Analytics dependiam muito da ferramenta Data Workbench para essa funcionalidade. Os [!UICONTROL atributos do cliente] expõem essa funcionalidade para um público-alvo maior fornecendo atributos do cliente como dimensões e métricas no Reports &amp; Analytics, no Ad Hoc Analysis e no Report Builder. Os clientes do Analytics Standard terão acesso aos atributos do cliente, mas com recursos limitados. O recurso completo está disponível para os clientes do Analytics Premium. |
| **(Somente no Adobe Target)** É possível pré-carregar ou carregar dados para clientes que o Adobe Target nunca viu? | Sim. Quando o visitante faz sua primeira solicitação ao Adobe Target, o sistema busca as informações existentes sobre ele nos atributos do cliente e utiliza esses dados para o direcionamento. **Observação:** a recuperação desses dados pode demorar até 20 minutos a partir da primeira interação com o Adobe Target. |
| **(Somente no Adobe Target)** É possível criar um super público-alvo combinando dados de atributos do cliente com dados de público-alvo compartilhados? | Não. Os dados de público-alvo compartilhados são um público-alvo concluído. |
| **(Somente no Adobe Target)** Como a funcionalidade de [!UICONTROL atributos do cliente] se compara à API de perfil em massa do Adobe Target? | A API de perfil em massa permite que os perfis do Adobe Target sejam atualizados diretamente pela API, para um perfil individual ou em massa. O recurso é semelhante aos atributos do cliente, com estas diferenças:<ul><li>A API do perfil é uma chamada de API REST e os atributos do cliente usam FTP.</li><li>A API do perfil do Adobe Target envia dados somente para o Adobe Target em vez de para toda a Experience Cloud.</li><li>Os atributos do cliente fornecem uma interface simples para criar e gerenciar esses dados externos.</li></ul> |
| **(Somente no Adobe Target)** O upload de dados dos atributos do cliente para o Adobe Target estende a duração do perfil do visitante do Adobe Target? | Sim. Consulte [Vida útil do perfil do visitante](https://experienceleague.adobe.com/docs/target/using/audiences/visitor-profiles/visitor-profile.html?lang=pt-BR) na ajuda do Adobe Target. |
| **(Somente no Adobe Target)** É possível segmentar os dados carregados nos atributos do cliente imediatamente após o visitante ser identificado pela ID do cliente? | Sim. Na chamada do servidor para o Adobe Target, que inclui a ID de terceiros da mbox, todos os dados de atributos do cliente ficam disponíveis. |
| **(Somente no Adobe Target)** O que a coluna **[!UICONTROL Status de sincronização]** representa para os arquivos carregados na fonte de atributo do cliente? | Para ver o número de registros publicados e sincronizados pelo Adobe Target, selecione o ícone Sincronizar status de um arquivo de atributo específico. `Sync %` é uma métrica em tempo real que especifica a % de perfis que foram sincronizados no Adobe Target.<br> **Observação:** pode levar até 24 horas para que os atributos sincronizem com o Adobe Target. |
| O que as métricas de carregamento de arquivo representam na Fonte de atributos do cliente? | Verifique o status dos atributos carregados nos Atributos do cliente com a ajuda das seguintes métricas: <ul><li>Registros: número de registros no arquivo de atributos.</li><li>**Novos registros:** número de novos registros presentes no arquivo de atributos.</li> <li>**Registros atualizados:** número de registros já existentes nos atributos do cliente com valores atualizados no arquivo.</li><li>**Todos os dados (registros):** número total de registros carregados com êxito nos Atributos do cliente.</li></ul> |

{style=&quot;table-layout:auto&quot;}