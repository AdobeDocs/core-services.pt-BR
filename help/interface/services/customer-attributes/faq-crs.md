---
description: Perguntas frequentes sobre  [!DNL customer attributes]  na Adobe Experience Cloud, no Adobe Analytics e no Adobe Target.
solution: Experience Cloud
title: Perguntas frequentes sobre  [!DNL customer attributes]
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 6031e544-822b-4843-b3d8-98a36a3c40e8
source-git-commit: 2f126877f6a5f090884ebe093f35e4f6d90b4df6
workflow-type: tm+mt
source-wordcount: '1033'
ht-degree: 81%

---

# Perguntas frequentes sobre [!DNL customer attributes]

Perguntas frequentes e práticas recomendadas para [!DNL customer attributes] no Adobe Analytics e Adobe Target.

## Práticas recomendadas e limitações {#best_practices}

Orientação e limitações ao usar [!DNL customer attributes].

| Problema | Descrição |
|--- |--- |
| Limitações de assinatura do [!UICONTROL atributo do cliente] | Ao atualizar para o Analytics Premium, há um atraso de 24 horas antes da disponibilização de mais atributos. Você pode ver um erro de [!UICONTROL Máximo de Assinatura de atributo] emitido durante esse atraso. |
| Vários logons no mesmo dispositivo | Ao usar [!DNL customer attributes] para fazer upload de perfis de cliente em uma fonte de dados, a Adobe não recomenda que usuários compartilhem dispositivos (ou seja, a mesma Experience Cloud ID). A Experience Cloud ID (ECID) persiste no dispositivo. O compartilhamento de dispositivos pode fazer com que a ECID vincule vários usuários à mesma ECID, resultando em resultados inesperados [!DNL Target]. **Observação:** em dispositivos móveis, a ECID é permanente depois que o aplicativo para dipositivos móveis é instalado, e você deve reinstalar o aplicativo para gerar uma nova ECID. Na Web, um novo ECID é gerado depois que o cookie do navegador é limpo. |
| Limitação diária de carregamento de frequência | A Adobe recomenda atualizar [!DNL customer attributes] apenas uma vez por dia. Aguarde pelo menos 24 horas para carregar outro arquivo de dados de perfil do cliente para o mesmo conjunto de perfis. |
| ID personalizada do Analytics (`s.visitorID`) | Definir uma ID do cliente usando `s.visitorID` é um método para identificar usuários no Adobe Analytics. No entanto, as integrações nas quais os dados do [!DNL Analytics] são exportados ou importados usando o serviço de ID não funcionam se for detectado que o(a) visitante utiliza `s.visitorID.`<br>. Isso inclui, mas não se limita a, serviços de públicos-alvo compartilhados, [!DNL Analytics] para Adobe Target (A4T) e [!DNL customer attributes].<br>Para essas integrações, não há suporte para uma ID personalizada do Analytics. |
| Limitações de comprimento de caracteres no [!DNL Analytics] | Ao criar uma assinatura do [!DNL Analytics], os comprimentos de campo dos arquivos de upload são truncados para 255. |

{style="table-layout:auto"}

## Perguntas frequentes sobre [!DNL customer attributes] {#section_E47866EEA83348E09FE43CEC5E44C461}

| Pergunta | Resposta |
|--- |--- |
| Posso receber notificações sobre o status de upload de [!DNL customer attributes]? | Sim. |
| O que devo fazer para começar a usar [!DNL customer attributes]? | <ol><li>Seja provisionado. Se você for um cliente do Adobe Analytics, a Adobe está provisionando para [!DNL customer attributes]. Se você usar somente o Adobe Target e não tiver o Analytics, solicite o provisionamento para os serviços principais entrando em contato com o Atendimento ao cliente.</li> <li>Conversar com a equipe de CRM. Descubra que tipo de dados de clientes estão disponíveis e quais você deseja usar no Analytics e em toda a Experience Cloud.</li><li>Implementar os serviços principais.</li></ol> |
| Quantos [!DNL customer attributes] posso usar? | Você pode fazer upload de centenas de colunas de `.csv` para o serviço de atributos do cliente. No entanto, ao configurar assinaturas e selecionar atributos, os seguintes limites poderão ser aplicados (por conjunto de relatórios), dependendo dos aplicativos que possui:  <ul><li>Foundation: 0</li><li>Select: 3</li><li>Prime: 15</li><li>Ultimate: 200</li><li>Standard: total de 3</li><li>Premium: 200</li><li>Adobe Target Standard: 5</li><li>Adobe Target Premium: 200</li></ul> |
| É necessário migrar para o Serviço da Experience Cloud ID? | A migração depende dos aplicativos que você usa. <ul><li>Adobe Analytics: recomendado </li><li>Adobe Target: obrigatório. </li></ul><br>O uso do serviço da Experience Cloud ID permite a funcionalidade mais recente do Experience Cloud, incluindo públicos em tempo real, a modernização do Adobe Target, a integração do Analytics e o rastreamento de pulsação de vídeo. |
| Como a funcionalidade de atributo do cliente está relacionada ao Adobe Audience Manager? | Embora o Audience Manager possa receber dados para identificar o público, ele não pode executar a funcionalidade de análise que vincula os atributos aos dados comportamentais históricos. Ele também não fornece os recursos de relatórios, análise e segmentação disponíveis no Adobe Analytics. [!UICONTROL Atributos do cliente] permite que dados avançados de vários aplicativos sejam vinculados e associados a uma única ID para uso na Experience Cloud. <br>No Adobe Target, [!DNL customer attributes] aparecem como atributos individuais que podem ser combinados com outras regras para criar públicos-alvo. Os públicos-alvo compartilhados com o serviço [!UICONTROL People] são públicos-alvo completos que não podem ser modificados. |
| **(Somente Adobe Analytics)** Como essa funcionalidade difere do que é fornecido no Analytics Premium? | Anteriormente, os clientes interessados em combinar os dados de atributo do cliente com os dados do Analytics dependiam muito da ferramenta do Data Workbench para essa funcionalidade. O [!DNL customer attributes] expõe essa funcionalidade para um público maior fornecendo [!DNL customer attributes] como dimensões e métricas no Report Builder. Clientes do Analytics Standard têm acesso a [!DNL customer attributes], mas com recursos limitados. O recurso completo está disponível para os clientes do Analytics Premium. |
| **(Somente no Adobe Target)** É possível pré-carregar ou carregar dados para clientes que o Adobe Target nunca viu? | Sim. Quando o(a) visitante faz sua primeira solicitação ao Adobe Target, o sistema busca as informações existentes que a Adobe tem sobre ele(a) nos [!DNL customer attributes] e usa esses dados para o direcionamento. **Observação:** a recuperação desses dados pode demorar até 20 minutos a partir da primeira interação com o Adobe Target. |
| **(Somente no Adobe Target)** É possível criar um super público-alvo combinando dados de atributos do cliente aos dados de público-alvo compartilhados? | Não. Os dados de público-alvo compartilhados são um público-alvo concluído. |
| **(Somente Adobe Target)** Como a funcionalidade de [!DNL customer attributes] se compara à API de perfil em massa do Adobe Target? | A API de perfil em massa permite que os perfis do Adobe Target sejam atualizados diretamente pela API, para um perfil individual ou em massa. O recurso é semelhante aos [!DNL customer attributes], com estas principais diferenças:<ul><li>A API de perfil é uma chamada de API REST e o serviço de [!DNL customer attributes] usa FTP.</li><li>A API de perfil do Adobe Target envia dados somente para o Adobe Target em vez de para toda a Experience Cloud.</li><li>O serviço de [!DNL customer attributes] fornece uma interface simples para criar e gerenciar esses dados externos.</li></ul> |
| **(Somente Adobe Target)** O upload de dados de [!DNL customer attributes] para o Adobe Target prolonga a vida útil do perfil de visitante do Adobe Target? | Sim. Consulte [Vida útil do perfil do visitante](https://experienceleague.adobe.com/docs/target/using/audiences/visitor-profiles/visitor-profile.html?lang=pt-BR) na ajuda do Adobe Target. |
| **(Somente Adobe Target)** Posso direcionar os dados enviados a [!DNL customer attributes] imediatamente após o(a) visitante ser identificado(a) pela ID do cliente? | Sim. Na chamada do servidor para o Adobe Target, que inclui a ID de terceiros da mbox, todos os dados de atributos do cliente ficam disponíveis. |
| **(Somente no Adobe Target)** O que a coluna **[!UICONTROL Status de sincronização]** representa para os arquivos carregados na fonte de atributo do cliente? | Para ver o número de registros publicados e sincronizados pelo Adobe Target, selecione o ícone Sincronizar status de um arquivo de atributo específico. `Sync %` é uma métrica em tempo real que especifica a % de perfis que foram sincronizados no Adobe Target.<br> **Observação:** pode levar até 24 horas para que os atributos sincronizem com o Adobe Target. |
| O que as métricas de upload de arquivo representam na origem de [!DNL customer attributes]? | É possível verificar o status dos atributos enviados para [!DNL customer attributes] com a ajuda das seguintes métricas: <ul><li>Registros: número de registros no arquivo de atributos.</li><li>**Novos registros:** número de novos registros presentes no arquivo de atributos.</li> <li>**Registros atualizados:** número de registros já existentes em [!DNL customer attributes] com valores atualizados no arquivo.</li><li>**Todos os dados (registros):** número total de registros enviados com êxito para [!DNL customer attributes].</li></ul> |

{style="table-layout:auto"}
