---
description: Gerencie a tradução dos dados do visitante na segmentação do público-alvo.
seo-description: Gerencie a tradução dos dados do visitante na segmentação do público-alvo.
seo-title: Públicos-alvo
solution: Experience Cloud
title: Audiences
uuid: 92faf3a8-1375-4e32-905b-74cad48144d3
translation-type: tm+mt
source-git-commit: 14d6e0ae15b023ad4dd3f8aca0606f26b39a21e9

---


# Públicos-alvo {#topic_679810123CAA4E0CA4FA3417FB0100C7}

Os públicos-alvo são coleções de visitantes (uma lista de IDs de visitante). Os serviços de público-alvo da Adobe gerenciam a conversão dos dados do visitante em segmentação do público-alvo. Assim, criar e gerenciar públicos-alvo é como criar e usar segmentos, com a capacidade adicional de compartilhar o segmento do público-alvo com a [!DNL Experience Cloud].

![](assets/audiences.png)

Os públicos-alvo podem ser criados ou derivados de várias fontes, como:

* Novos, criados na [!DNL Experience Cloud]
* Nos segmentos do [!DNL Analytics] publicados para a [!DNL Experience Cloud]
* De [!DNL Audience Manager]

**Públicos-alvo em tempo real vs. históricos**

Todos os públicos-alvo, independentemente de sua fonte, podem ser acessados para casos de uso de direcionamento em tempo real. No entanto, os públicos-alvo compartilhados do Analytics para o Audience Manager não estão acessíveis para o direcionamento em tempo real. O sistema avalia as audiências de duas maneiras:

* audiências antigas do Analytics são avaliadas a cada quatro horas. O tempo total para processar e compartilhar pode levar até 8 horas.  audiências históricas sempre incluem visitantes de retorno.
* Os públicos-alvo em tempo real são provenientes da Experience Cloud Audiences e avaliados em tempo real.

## Como as soluções usam os públicos-alvo {#concept_01EB9345C5344597BC94A864EDD38EE1}

A tabela a seguir descreve como as audiências são usadas nas soluções da Experience Cloud:

| Solução | Descrição |
|--- |--- |
| Públicos-alvo da Experience Cloud | Crie, gerencie e compartilhe públicos-alvo originalmente usando a interface da [Biblioteca de público-alvo](../audience-library/audience-library.md). É possível:<ul><li>Usar audiências em tempo real usando atributos brutos de análise</li><li>Combinar audiências para criar compostos, unindo dados históricos e em tempo real</li><li>Veja visualizações gráficas do tamanho estimado das audiências</li></ul><br>Para obter sugestões sobre que tipo de audiência você deseja criar, consulte: Audiências [da Experience Cloud](https://helpx.adobe.com/marketing-cloud-core/kb/People/Audience-Creation-Options.html). |
| Analytics | Na segmentação, você pode criar um segmento, combiná-lo com um conjunto de relatórios e, em seguida, [publicar o segmento na Experience Cloud](../audience-library/audience-library.md). O segmento publicado é exibido na página [Públicos-alvo](../audience-library/audience-library.md). O público-alvo também fica disponível como um público-alvo direcionado para uma experiência de campanha oferecida pelo Adobe Target e no Audience Manager.   Quando o público-alvo é compartilhado no Analytics e selecionado para uso em uma campanha ativa, todos os perfis do visitante que satisfazem o critério de definição de segmento nos últimos 90 dias são enviados para a plataforma de Serviços de público-alvo da Experience Cloud.   O limite para audiências compartilhadas foi aumentado para 75.  As Audiências compartilhadas com a Experience Cloud a partir do Analytics não podem exceder 20 milhões de membros únicos. Além disso, devido ao cache, conjuntos de relatórios excluídos no Analytics permanecem exibidos na Experience Cloud por 12 horas antes da exclusão. |
| Mobile Services | Analise o tráfego móvel usando a visualização em forma de raio de sol no relatório Tipos [!UICONTROL de] dispositivo. |
| Target | The [ID service](https://docs.adobe.com/content/help/en/id-service/using/home.html) unifies visitor IDs and data into a single, actionable profile for use across solutions. A caixa de seleção [Publicar na Experience Cloud](../audience-library/audience-library.md) durante o processo de criação de segmento no Adobe Analytics permite que o segmento fique disponível na biblioteca de público-alvo-alvo personalizado no Adobe Target. Um segmento criado no Analytics ou no Audience Manager pode ser usado em atividades no Target.  Por exemplo, é possível criar atividades de campanha baseadas nas métricas de conversão do Analytics e nos segmentos de público-alvo criados no Analytics. |
| Audience Manager | Os públicos-alvo compartilhados ficam disponíveis na segmentação do Audience Manager. Todos os públicos-alvo da Experience Cloud estão disponíveis originalmente no Audience Manager, que oferece:<ul><li>Automação integrada em relação ao modo como são compartilhados e consumidos em workflows de solução</li><li>Destinos externos</li><li>Modelagem semelhante</li></ul> |
| Campanha | <ul><li>Importar públicos-alvo compartilhados de diferentes soluções da Adobe Experience Cloud para o Adobe Campaign.</li><li>Exportar listas de destinatários em formato de públicos-alvo compartilhados. Essas audiências compartilhadas podem ser usadas nas diferentes soluções da Adobe Experience Cloud que você usa.</li></ul> |
| Media Optimizer | Use a audiência como públicos alvos. |

>[!IMPORTANT]
>
>Quando um visitante se qualifica para a audiência compartilhada do Analytics, há um atraso de 4 a 8 horas antes que essas informações sejam acionáveis no Público alvo, na Ad Cloud e no Campaign Standard.

## Mais ajuda: perguntas, instruções e casos de uso {#section_C7F151644D8A45F7B6FC54F58845635D}

| Ajuda com | Recurso |
|--- |--- |
| Não consegue encontrar Audiências? | Verifique se você foi provisionado. See [Getting started - enable your solutions for core services](../core-services/core-services.md).<br>Clique [aqui](https://www.adobe.com/go/audiences) para solicitar acesso a Perfis e Audiência (formulário de provisionamento de integrações). |
| Casos de uso | Para obter mais orientações sobre qual solução usar, acesse Opções [de criação de](https://helpx.adobe.com/marketing-cloud-core/kb/People/Audience-Creation-Options.html) Audiências na Base de conhecimento. |
| Fórum | The [Audiences forum](https://forums.adobe.com/community/experience-cloud/platform/core-services/people-service/audiences) is an additional resource to get help with audiences. |

## Elementos de interface da biblioteca de público-alvo {#section_D04ACEF61CEF4B189AE6BA9F40D0DBF4}

A [!DNL Experience Cloud] oferece uma biblioteca para criar e gerenciar públicos-alvo, com identificação de público-alvo nativa e em tempo real.

**[!UICONTROL Experience Cloud]** > Plataforma **** da Experience Cloud > **[!UICONTROL Pessoas]** > Biblioteca **[!UICONTROL de Audiências]**

![](assets/audience_library.png)

| Elemento | Descrição |
|--- |--- |
| Novo | [Criar um público-alvo](../audience-library/audience-library.md). |
| Título e descrição | Um cabeçalho de coluna que identifica e descreve o público-alvo. |
| Autor | A pessoa que criou o segmento de audiência. |
| Fonte | Identifica onde a audiência foi criada.<ul><li>**Analytics:** Um segmento criado em relatórios e análises ou análises ad hoc, em seguida [publicado na Experience Cloud](../audience-library/audience-library.md).</li><li>**Experience Cloud:** um novo público-alvo [criado a partir dos públicos-alvo da Experience Cloud](../audience-library/audience-library.md).</li><li>**Audience Manager:** públicos-alvo criados no Audience Manager são exibidos automaticamente nos Públicos-alvo da Experience Cloud.</li></ul> |
| Tamanho atual | O tamanho atual da audiência. |
| Ativo | O status ativo do segmento. |
