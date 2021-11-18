---
solution: Experience Cloud
type: Documentation
title: 'Públicos da Adobe Experience Cloud '
uuid: 92faf3a8-1375-4e32-905b-74cad48144d3
description: Saiba como gerenciar a conversão dos dados do visitante em segmentação de público-alvo no serviço de público da Experience Cloud.
feature: Audience Library
topic: Administration
role: Admin
level: Experienced
exl-id: 1c6e54ac-4886-46ed-9df7-201d2df31847
source-git-commit: ae14748aa7b0f0d803d48fe980a6743f53d996ab
workflow-type: tm+mt
source-wordcount: '833'
ht-degree: 87%

---

# Públicos-alvo da Experience Cloud {#topic_679810123CAA4E0CA4FA3417FB0100C7}

Os públicos-alvo são coleções de visitantes (uma lista de IDs de visitante). A biblioteca de público-alvo da Adobe permite gerenciar a conversão dos dados do visitante em segmentação do público-alvo. Dessa forma, a criação e o gerenciamento de públicos é semelhante à criação e ao uso de segmentos. Você também pode compartilhar o segmento de público-alvo com produtos e serviços na [!DNL Experience Cloud].

![Públicos-alvo da Experience Cloud](assets/audiences.png)

Os públicos-alvo podem ser criados ou derivados de várias fontes, como:

* Novos, criados na [!DNL Experience Cloud]
* Segmentos do [!DNL Analytics] publicados na [!DNL Experience Cloud]
* [!DNL Audience Manager]

**Públicos-alvo em tempo real vs. históricos**

Todos os públicos-alvo, independentemente de sua fonte, podem ser acessados para casos de uso de direcionamento em tempo real. No entanto, os públicos-alvo compartilhados do Analytics para o Audience Manager não estão acessíveis para o direcionamento em tempo real. O sistema avalia os públicos-alvo de duas maneiras:

* Os públicos-alvo históricos do Analytics são avaliados a cada quatro horas. O tempo total para processar e compartilhar pode levar até oito horas. Os públicos-alvo de histórico sempre incluem visitantes de retorno.
* Os públicos-alvo em tempo real são provenientes da Experience Cloud Audiences e avaliados em tempo real.

## Como os aplicativos usam os públicos-alvo {#concept_01EB9345C5344597BC94A864EDD38EE1}

A tabela a seguir descreve como os públicos-alvo são usados em aplicativos do Experience Cloud:

| Solução | Descrição |
|--- |--- |
| Públicos-alvo da Experience Cloud | Crie, gerencie e compartilhe públicos-alvo originalmente usando a interface da [Biblioteca de público-alvo](audience-library.md). É possível:<ul><li>Usar públicos-alvo em tempo real usando atributos brutos de análise</li><li>Combinar públicos-alvo para criar compostos, unindo dados históricos e em tempo real</li><li>Veja as exibições gráficas do tamanho estimado dos públicos-alvo</li></ul><br>Para obter sugestões sobre que tipo de público-alvo você deseja criar, consulte: [Públicos-alvo da Experience Cloud](https://experienceleague.adobe.com/docs/experience-cloud-kcs/kbarticles/KA-16471.html?lang=pt-BR). |
| Analytics | Na segmentação, você pode criar um segmento, combiná-lo a um conjunto de relatórios e, em seguida, publicar o segmento na Experience Cloud. A publicação do segmento o exibe na página [!UICONTROL Biblioteca de público-alvo] na Experience Cloud. (Consulte [Publicar segmentos na Experience Cloud](https://experienceleague.adobe.com/docs/analytics/components/segmentation/segmentation-workflow/seg-publish.html?lang=pt-BR) na ajuda do Analytics para obter detalhes.) O público-alvo também fica disponível como um público-alvo direcionado para uma experiência de campanha oferecida pelo Adobe Target e no Audience Manager. Depois de compartilhar um público-alvo do Adobe Analytics e selecioná-lo para uso em uma campanha ativa, os perfis de visitante que atendem ao critério de definição de segmento dos últimos 90 dias são enviados para [!UICONTROL Serviços de público-alvo]. O limite de públicos-alvo compartilhados foi aumentado para 75. Os públicos-alvo compartilhados com a Experience Cloud a partir do Analytics não podem exceder 20 milhões de membros exclusivos. Além disso, devido a questões relacionadas ao cache, os conjuntos de relatórios excluídos no Analytics permanecem exibidos na Experience Cloud por 12 horas após a exclusão. |
| Mobile Services | Analise o tráfego móvel usando a exibição de explosão solar no relatório [!UICONTROL Tipos de dispositivo]. |
| [!DNL Target] | O [Serviço de ID](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=pt-BR) unifica as IDs de visitante e os dados em um perfil único e acionável para uso em aplicativos. A caixa de seleção [Publicar na Experience Cloud](audience-library.md) durante o processo de criação de segmento no Adobe Analytics permite que o segmento fique disponível na biblioteca de público-alvo-alvo personalizado no Adobe Target. Um segmento criado no Analytics ou no Audience Manager pode ser usado em atividades no [!DNL Target]. Por exemplo, é possível criar atividades de campanha baseadas nas métricas de conversão do [!DNL Analytics] e nos segmentos de público-alvo criados no [!DNL Analytics]. |
| Audience Manager | Os públicos-alvo compartilhados ficam disponíveis na segmentação do Audience Manager. Todos os públicos-alvo da Experience Cloud estão disponíveis originalmente no Audience Manager, que oferece:<ul><li>Automação integrada em relação ao modo como são compartilhados e consumidos em fluxos de trabalho de aplicativos</li><li>Destinos externos</li><li>Modelo de semelhanças</li></ul> |
| Campaign | <ul><li>Importe públicos compartilhados de diferentes aplicativos Adobe Experience Cloud para o Adobe Campaign.</li><li>Exportar listas de destinatários em formato de públicos-alvo compartilhados. Esses públicos-alvo compartilhados podem ser usados nos diferentes aplicativos do Adobe Experience Cloud que você usa.</li></ul> |
| Advertising Cloud | Use o público-alvo como destino. |

{style=&quot;table-layout:auto&quot;}

>[!IMPORTANT]
>
>Depois que um visitante é qualificado para o público-alvo compartilhado do Analytics, existe um atraso de 4 a 8 horas antes de as informações serem ativadas no [!DNL Target], no Media Optimizer e no Campaign Standard.

## Mais ajuda: perguntas, instruções e casos de uso {#section_C7F151644D8A45F7B6FC54F58845635D}

| Ajuda com | Recurso |
|--- |--- |
| Não consegue encontrar Públicos-alvo? | Verifique se você foi provisionado. Consulte [Introdução - ativar os aplicativos dos serviços principais](core-services.md).<br>Solicite [aqui](https://adobe.allegiancetech.com/cgi-bin/qwebcorporate.dll?idx=X8SVES) acesso a Perfis e públicos (formulário de provisionamento de integrações). |
| Casos de uso | Para obter mais instruções sobre qual aplicativo usar, acesse [Opções de criação de público-alvo](https://experienceleague.adobe.com/docs/experience-cloud-kcs/kbarticles/KA-16471.html?lang=en) na Base de conhecimento. |
| Fórum | O [fórum de públicos-alvo](https://experienceleaguecommunities.adobe.com/t5/Adobe-Experience-Cloud-Audiences/ct-p/experience-cloud-audiences-community) é mais um recurso para obter ajuda com os públicos-alvo. |

{style=&quot;table-layout:auto&quot;}

## Elementos de interface da biblioteca de público-alvo {#section_D04ACEF61CEF4B189AE6BA9F40D0DBF4}

A [!DNL Experience Cloud] oferece uma biblioteca para criar e gerenciar públicos-alvo, com identificação de público-alvo nativa e em tempo real.

**[!UICONTROL Experience Cloud]** > **[!UICONTROL Experience Platform]** > **[!UICONTROL People]** > **[!UICONTROL Biblioteca de públicos-alvo]**

![Adicionar público-alvo na biblioteca de público-alvo](assets/audience_library.png)

| Elemento | Descrição |
|--- |--- |
| Novo | [Criar um público-alvo](audience-library.md). |
| Título e descrição | Um cabeçalho de coluna que identifica e descreve o público-alvo. |
| Autor | A pessoa que criou o segmento de público-alvo. |
| Fonte | Identifica onde o público-alvo foi criado.<ul><li>**Analytics:** um segmento criado no Adobe Analytics e, em seguida, [publicado na Experience Cloud](audience-library.md).</li><li>**Experience Cloud:** um novo público-alvo [criado a partir dos públicos-alvo da Experience Cloud](audience-library.md).</li><li>**Audience Manager:** públicos-alvo criados no Audience Manager são exibidos automaticamente nos Públicos-alvo da Experience Cloud.</li></ul> |
| Tamanho atual | O tamanho atual do público-alvo. |
| Ativo | O status ativo do segmento. |

{style=&quot;table-layout:auto&quot;}
