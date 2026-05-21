---
title: '[!DNL Audience Library]'
description: Saiba como gerenciar a conversão dos dados do visitante em segmentação de público no CX Enterprise [!DNL Audience Library].
solution: Experience Cloud
type: Documentation
uuid: 92faf3a8-1375-4e32-905b-74cad48144d3
feature: Audience Library
topic: Administration
role: Admin
level: Experienced
exl-id: 1c6e54ac-4886-46ed-9df7-201d2df31847
TQID: https://experienceleague.adobe.com/QEAfCWPNI-JhDw-HjZwBGv0TlqyctIqSwz8eVQqS6Gg
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2:
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2:
  - id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
  - id: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
  - id: ff2b9b37-92e0-45fc-b853-379d44c08c89
source-git-commit: 50012e2564e88e1a6e16578e3331136c7df0cb21
workflow-type: tm+mt
source-wordcount: 745
ht-degree: 48%

---

# Públicos-alvo da CX Enterprise

[!DNL Audience Library] exibe públicos-alvo na CX Enterprise. Os públicos-alvo são coleções de visitantes (uma lista de IDs da [!DNL CX Enterprise]). Você pode gerenciar a conversão de dados de visitante em uma segmentação de público-alvo. Assim, criar e gerenciar públicos-alvo é como criar e usar segmentos. Você também pode compartilhar o segmento de público-alvo com produtos e serviços na [!DNL CX Enterprise].

![Públicos-alvo da CX Enterprise](assets/audiences.png)

Os públicos-alvo podem ser criados ou derivados de várias fontes, como:

* Novos, criados em [!DNL CX Enterprise]
* [!DNL Analytics] segmentos publicados em [!DNL CX Enterprise]
* [!DNL Audience Manager]

**Públicos-alvo em tempo real vs. históricos**

Todos os públicos-alvo, independentemente de sua fonte, podem ser acessados para casos de uso de direcionamento em tempo real. No entanto, os públicos-alvo compartilhados do Analytics para o Audience Manager não estão acessíveis para o direcionamento em tempo real. O sistema avalia os públicos-alvo de duas maneiras:

* Os públicos-alvo históricos do Analytics são avaliados a cada quatro horas. O tempo total para processar e compartilhar pode levar até oito horas. Os públicos-alvo de histórico sempre incluem visitantes de retorno.
* Os públicos-alvo em tempo real são provenientes de CX Enterprise Audiences e avaliados em tempo real.

## Como os aplicativos usam os públicos-alvo

A tabela a seguir descreve como os públicos-alvo são usados nos aplicativos CX Enterprise:

| Solução | Descrição |
| --- | --- |
| Públicos-alvo corporativos CX | Crie, gerencie e compartilhe públicos-alvo originalmente usando a Biblioteca de público-alvo. É possível:<ul><li>Use públicos-alvo em tempo real usando atributos brutos de análise.</li><li>Combine públicos para criar compostos, unindo dados históricos e em tempo real.</li><li>Consulte as exibições gráficas do tamanho estimado dos públicos-alvo.</li></ul><br>Para obter sugestões sobre que tipo de público-alvo você deve criar, consulte [Opções de criação de públicos-alvo](https://experienceleague.adobe.com/docs/experience-cloud-kcs/kbarticles/KA-16471.html?lang=pt-BR). |
| Analytics | Na segmentação, você pode criar um segmento, combiná-lo a um conjunto de relatórios e, em seguida, publicar o segmento no CX Enterprise. A publicação do segmento o exibe na página [!DNL Audience Library] do CX Enterprise. (Consulte [Publicar segmentos no CX Enterprise](https://experienceleague.adobe.com/docs/analytics/components/segmentation/segmentation-workflow/seg-publish.html?lang=pt-BR) na ajuda do [!DNL Analytics] para obter detalhes.) O público-alvo também está disponível como um público-alvo direcionado para uma experiência de campanha oferecida por [!DNL Adobe Target] e em [!DNL Audience Manager]. Depois de compartilhar um público-alvo de [!DNL Adobe Analytics] e selecioná-lo para uso em uma campanha ativa, os perfis de visitante que atendem ao critério de definição de segmento dos últimos 90 dias são enviados para [!UICONTROL Audience Services]. O limite de públicos-alvo compartilhados foi aumentado para 75. Públicos-alvo compartilhados com CX Enterprise a partir de [!DNL Analytics] não podem exceder 20 milhões de membros únicos. Além disso, devido a questões relacionadas ao cache, conjuntos de relatórios excluídos no Analytics permanecem exibidos no CX Enterprise por 12 horas após a exclusão. |
| Mobile Services | Analise o tráfego de publicação de conteúdo para dispositivos móveis usando a exibição de explosão solar no relatório [!UICONTROL Device Types]. |
| [!DNL Target] | O [serviço de ID](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=pt-BR) unifica as IDs e os dados de visitantes em um perfil único e acionável para uso em diversos aplicativos. A caixa de seleção [!UICONTROL Publish to CX Enterprise] durante o processo de criação de segmento no Adobe Analytics permite que o segmento fique disponível na biblioteca de público-alvo personalizado no Adobe Target. Um segmento criado no [!DNL Analytics] ou no [!DNL Audience Manager] pode ser usado em atividades do [!DNL Target]. Por exemplo, é possível criar atividades de campanha baseadas nas métricas de conversão do [!DNL Analytics] e nos segmentos de público-alvo criados no [!DNL Analytics]. |
| [!DNL Audience Manager] | Os públicos-alvo compartilhados ficam disponíveis na segmentação do [!DNL Audience Manager]. Todos os públicos-alvo do CX Enterprise estão disponíveis nativamente no [!DNL Audience Manager], que oferece:<ul><li>Automação integrada em relação ao modo como eles são compartilhados e consumidos em fluxos de trabalho de aplicativos</li><li>Destinos externos</li><li>Modelo de semelhanças</li></ul> |
| Campaign | <ul><li>Importar públicos-alvo compartilhados de diferentes aplicativos Adobe CX Enterprise para o Adobe Campaign.</li><li>Exportar listas de destinatários em formato de públicos-alvo compartilhados. Esses públicos-alvo compartilhados podem ser usados nos diferentes aplicativos Adobe CX Enterprise que você usa.</li></ul> |
| Advertising Cloud | Use o público-alvo como destino. |

{style="table-layout:auto"}

>[!IMPORTANT]
>
>Depois que um visitante é qualificado para o público-alvo compartilhado do Analytics, existe um atraso de 4 a 8 horas antes de as informações serem ativadas no [!DNL Target], no Media Optimizer e no Campaign Standard.

## Elementos de interface da biblioteca de público-alvo

O [!DNL CX Enterprise] fornece uma biblioteca para criar e gerenciar públicos-alvo, com identificação de público-alvo nativa e em tempo real.

**[!UICONTROL CX Enterprise]** > **[!UICONTROL Experience Platform]** > **[!UICONTROL People]** > **[!UICONTROL Audience Library]**

![Adicionar público-alvo na Biblioteca de público-alvo](assets/audience_library.png)


| Elemento | Descrição |
| --- | --- |
| Novo | [Criar um público-alvo](https://experienceleague.adobe.com/pt-br/docs/core-services/interface/services/audiences/create). |
| Título e descrição | Um cabeçalho de coluna que identifica e descreve o público-alvo. |
| Autor | A pessoa que criou o segmento de público-alvo. |
| Fonte | Identifica onde o público-alvo foi criado.<ul><li>**Analytics:** um segmento criado no Adobe Analytics e, em seguida, publicado no CX Enterprise.</li><li>**CX Enterprise:** um novo público-alvo [criado no CX Enterprise Audiences](https://experienceleague.adobe.com/pt-br/docs/core-services/interface/services/audiences/create).</li><li>**Audience Manager:** públicos-alvo criados no Audience Manager são exibidos automaticamente no CX Enterprise Audiences.</li></ul> |
| Tamanho atual | O tamanho atual do público-alvo. |
| Ativo | O status ativo do segmento. |

{style="table-layout:auto"}

## Publicar públicos-alvo da Adobe Analytics

Consulte [Publicar segmentos no CX Enterprise](https://experienceleague.adobe.com/pt-br/docs/analytics/components/segmentation/segmentation-workflow/seg-publish) na documentação do Adobe Analytics para obter mais informações.
