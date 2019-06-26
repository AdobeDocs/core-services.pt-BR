---
description: Gerencie a tradução dos dados do visitante na segmentação do público-alvo.
seo-description: Gerencie a tradução dos dados do visitante na segmentação do público-alvo.
seo-title: Públicos-alvo
solution: Experience Cloud
title: Públicos-alvo
uuid: 92faf3a8-1375-4e32-905b-74cad48144d3
translation-type: ht
source-git-commit: 979b2202a70e2a5362aa86a65a17d7c4279b3a1a

---


# Públicos-alvo{#topic_679810123CAA4E0CA4FA3417FB0100C7}

Os públicos-alvo são coleções de visitantes (uma lista de IDs de visitante). Os serviços de público-alvo da Adobe gerenciam a conversão dos dados do visitante em segmentação do público-alvo. Assim, criar e gerenciar públicos-alvo é como criar e usar segmentos, com a capacidade adicional de compartilhar o segmento do público-alvo com a [!DNL Experience Cloud].

![](assets/audiences.png)

Os públicos-alvo podem ser criados ou derivados de várias fontes, como:

* Novos, criados na [!DNL Experience Cloud]
* Nos segmentos do [!DNL Analytics] publicados para a [!DNL Experience Cloud]
* De [!DNL Audience Manager]

**Públicos-alvo em tempo real vs. históricos**

Todos os públicos-alvo, independentemente de sua fonte, podem ser acessados para casos de uso de direcionamento em tempo real. No entanto, os públicos-alvo compartilhados do Analytics para o Audience Manager não estão acessíveis para o direcionamento em tempo real. O sistema avalia os públicos-alvo de duas maneiras:

* Os públicos-alvo de histórico provenientes de análises são avaliados a cada 12 horas. Os públicos-alvo de histórico sempre incluem os visitantes de retorno.
* Os públicos-alvo em tempo real são provenientes da Experience Cloud Audiences e avaliados em tempo real.


## Como as soluções usam os públicos-alvo {#concept_01EB9345C5344597BC94A864EDD38EE1}

A tabela a seguir descreve como os públicos-alvo são usados nas soluções da Experience Cloud:

| Solução | Descrição |
|--- |--- |
| Públicos-alvo da Experience Cloud | Crie, gerencie e compartilhe públicos-alvo originalmente usando a interface da [Biblioteca de público-alvo](../audience-library/audience-library.md). É possível:<ul><li>Usar públicos-alvo em tempo real usando atributos de análise brutos</li><li>Combinar públicos-alvo para criar alguns compostos, reunindo dados históricos e em tempo real</li><li>Consultar as visualizações gráficas do tamanho dos públicos-alvo previstos</li></ul><br>Para obter sugestões sobre o tipo de público-alvo que deseja criar, consulte: [Experience Cloud Audiences](https://helpx.adobe.com/br/marketing-cloud-core/kb/People/Audience-Creation-Options.html). |
| Analytics | Na segmentação, é possível criar um segmento, combiná-lo com um conjunto de relatórios e [publicar o segmento na Experience Cloud](../audience-library/audience-library.md). O segmento publicado é exibido na página [Públicos-alvo](../audience-library/audience-library.md). O público-alvo também fica disponível como um público-alvo direcionado para uma experiência de campanha oferecida pelo Adobe Target e no Audience Manager.   Quando o público-alvo é compartilhado no Analytics e selecionado para uso em uma campanha ativa, todos os perfis do visitante que satisfazem o critério de definição de segmento nos últimos 90 dias são enviados para a plataforma de Serviços de público-alvo da Experience Cloud.   Importante: é preciso limitar para 20 o número de públicos-alvo compartilhados por meio do Analytics para evitar atrasos adicionais de processamento. Públicos-alvo compartilhados com a Experience Cloud a partir do Analytics não podem exceder 20 milhões de membros únicos. Além disso, devido a questões relacionadas ao cache, conjuntos de relatórios excluídos no Analytics permanecem exibidos na Experience Cloud por 12 horas após a exclusão. |
| Mobile Services | Analise o tráfego de publicação de conteúdo para dispositivos móveis usando a visualização de sunburst nos [Tipos de dispositivo](https://marketing.adobe.com/resources/help/pt_BR/mobile/?f=reports_devices). |
| Target | O [serviço de ID](https://marketing.adobe.com/resources/help/pt_BR/mcvid/) unifica as IDs de visitante e os dados em um único perfil acionável para uso nas soluções. A caixa de seleção [Publicar na Experience Cloud](../audience-library/audience-library.md) durante o processo de criação de segmento no Adobe Analytics permite que o segmento fique disponível na biblioteca de público-alvo-alvo personalizado no Adobe Target. Um segmento criado no Analytics ou no Audience Manager pode ser usado em atividades no Target.  Por exemplo, é possível criar atividades de campanha baseadas nas métricas de conversão do Analytics e nos segmentos de público-alvo criados no Analytics. |
| Audience Manager | Os públicos-alvo compartilhados ficam disponíveis na segmentação do Audience Manager. Todos os públicos-alvo da Experience Cloud estão disponíveis originalmente no Audience Manager, que oferece:<ul><li>Automação integrada com relação à maneira como eles são compartilhados e consumidos nos fluxos de trabalho da solução</li><li>Destinos externos</li><li>Modelagem semelhante</li></ul> |
| Campanha | <ul><li>Importar públicos-alvo compartilhados de diferentes soluções da Adobe Experience Cloud para o Adobe Campaign.</li><li>Exportar listas de destinatários em formato de públicos-alvo compartilhados. Esses públicos-alvo compartilhados podem ser utilizados nas diferentes soluções da Adobe Experience Cloud que você usa.</li></ul> |
| Media Optimizer | Use o público-alvo como metas. |


>[!IMPORTANT]
>
>Depois que um visitante é qualificado para o público-alvo compartilhado do Analytics, existe um atraso de 24 a 48 horas antes de as informações serem ativadas no Target, no Media Optimizer e no Campaign.

## Mais ajuda: perguntas, instruções e casos de uso {#section_C7F151644D8A45F7B6FC54F58845635D}


| Ajuda com | Recurso |
|--- |--- |
| Não consegue encontrar os Públicos-alvo? | Verifique se você foi provisionado. Consulte [Introdução - ativar as soluções dos serviços principais](../core-services/core-services.md).<br>Clique [aqui](https://www.adobe.com/go/audiences) para solicitar acesso a Perfis e públicos-alvo (formulário de provisionamento de integrações). |
| Casos de uso | Para obter mais instruções sobre qual solução usar, acesse [Opções da criação de público-alvo](https://helpx.adobe.com/br/marketing-cloud-core/kb/People/Audience-Creation-Options.html) na knowledge base. |
| Fórum | O [fórum de públicos-alvo](https://forums.adobe.com/community/experience-cloud/platform/core-services/people-service/audiences) é um recurso adicional para obter ajuda com os públicos-alvo. |


## Elementos de interface da biblioteca de público-alvo {#section_D04ACEF61CEF4B189AE6BA9F40D0DBF4}

A [!DNL Experience Cloud] oferece uma biblioteca para criar e gerenciar públicos-alvo, com identificação de público-alvo nativa e em tempo real.

**[!UICONTROL Experience Cloud]** &gt; **[!UICONTROL Biblioteca de público-alvo]**

![](assets/audience_library.png)

| Elemento | Descrição |
|--- |--- |
| Novo | [Criar um público-alvo](../audience-library/audience-library.md). |
| Título e descrição | Um cabeçalho de coluna que identifica e descreve o público-alvo. |
| Autor | A pessoa que criou o segmento de público-alvo. |
| Fonte | Identifica onde o público-alvo foi criado.<ul><li>**Analytics:** Um segmento criado em relatórios e análises ou análises ad hoc, em seguida [publicado na Experience Cloud](../audience-library/audience-library.md).</li><li>**Experience Cloud:** um novo público-alvo [criado a partir dos públicos-alvo da Experience Cloud](../audience-library/audience-library.md).</li><li>**Audience Manager:** públicos-alvo criados no Audience Manager são exibidos automaticamente nos Públicos-alvo da Experience Cloud.</li></ul> |
| Tamanho atual | O tamanho atual do público-alvo. |
| Ativo | O status ativo do segmento. |
