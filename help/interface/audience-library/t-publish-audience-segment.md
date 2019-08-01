---
description: Publique um segmento de público-alvo do Analytics na Experience Cloud e no Adobe Target para as atividades de marketing do público-alvo.
keywords: principais serviços
seo-description: Publique um segmento de público-alvo do Analytics na Experience Cloud e no Adobe Target para as atividades de marketing do público-alvo.
seo-title: Publicar um segmento de público-alvo do Analytics
solution: Experience Cloud
title: Publicar um segmento de público-alvo do Analytics
uuid: 4201dc22-4b79-457c-a614-949bba087617
translation-type: tm+mt
source-git-commit: b74e0a08b43dfa8e5b35c5a650d159a58485883c

---


# Publicar um segmento de público-alvo do Analytics

Publique um segmento de público-alvo do Analytics na Experience Cloud e no Adobe Target para as atividades de marketing do público-alvo.

1. No Analytics, [crie um segmento](https://marketing.adobe.com/resources/help/en_US/analytics/segment/seg_build.html).
1. On the Segment Builder, enable the **[!UICONTROL Publish this segment to the Experience Cloud]** option.

   ![](assets/ec_audience_example.png)

   | Elemento | Descrição |
   |--- |---|
   | Publicar esse segmento na Experience Cloud (para &lt; nome do conjunto de relatórios &gt;) | Publica esse segmento na Experience Cloud. Você pode usar o público-alvo para atividades de marketing e segmentação no Adobe Target, no Audience Manager, na Advertising Cloud, na campanha e no Audience Analytics.<br>Os campos Título e Descrição são obrigatórios para o segmento ser publicado.<br>Quando essa opção é ativada, o título e a definição do segmento do público-alvo são compartilhados, mas os dados reais não são. Quando o público-alvo é associado a uma campanha ativa no Target, o Analytics começa a enviar IDs para os visitantes que se qualificaram para esse público-alvo da Experience Cloud e do Target. Nesse momento, o nome do público-alvo e os dados correspondentes começam a ser exibidos na página Públicos-alvo da Experience Cloud.<br>Públicos-alvo compartilhados com a Experience Cloud a partir do Analytics não podem exceder 20 milhões de membros do público-alvo.<br>Devido a questões relacionadas ao cache, conjuntos de relatórios excluídos no Analytics permanecem exibidos na Experience Cloud por 12 horas após a exclusão.<br>Para excluir um segmento publicado na Experience Cloud, é necessário cancelá-lo primeiro. To unpublish a segment, just **unclick** the checkbox that you used to publish it. **Não é possível** cancelar a publicação de um segmento que está em uso por qualquer uma das seguintes soluções da Adobe: [!DNL Analytics] (in [!DNL Audience Analytics]), [!DNL Campaign]( [!DNL Advertising Cloud] para [!DNL Core Service] &amp; [!DNL Audience Manager] clientes) e todos os outros parceiros externos (para [!DNL Audience Manager] clientes). You **can** unpublish a segment that is in use by [!DNL Target].<br>Depois que um visitante é qualificado para o público-alvo compartilhado do Analytics, existe um atraso de 24 a 48 horas antes de as informações serem ativadas no Target, no Media Optimizer e no Campaign.<br>**Privacidade dos dados**<br>Os públicos-alvo não são filtrados com base no estado de autenticação de um visitante. Se um visitante consegue navegar em seu site em estados de autenticação e de não autenticação, as ações que ocorrem quando um visitante não está autenticado podem fazer com que um visitante seja incluído em um público-alvo. Analise [Visão geral da privacidade do Analytics](https://marketing.adobe.com/resources/help/en_US/reference/?f=c_Privacy_Overview) para conhecer todas as implicações de privacidade do compartilhamento de público-alvo. |
   | Selecione a janela para a criação de público-alvo | Observe que esta é uma janela de tempo **flutuante**, e não de tempo fixo. |

1. Clique em **[!UICONTROL Salvar]**.
1. Acesse [!DNL Adobe Target], clique [!UICONTROL em Públicos-alvo].
1. Na página [!UICONTROL Públicos-alvo], localize o público-alvo proveniente da Experience Cloud.

   Esses públicos-alvo estão disponíveis para uso em atividades.
