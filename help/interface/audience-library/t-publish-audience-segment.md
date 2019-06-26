---
description: Publique um segmento de público-alvo do Analytics na Experience Cloud e no Adobe Target para as atividades de marketing do público-alvo.
keywords: principais serviços
seo-description: Publique um segmento de público-alvo do Analytics na Experience Cloud e no Adobe Target para as atividades de marketing do público-alvo.
seo-title: Publicar um segmento de público-alvo do Analytics
solution: Experience Cloud
title: Publicar um segmento de público-alvo do Analytics
uuid: 4201dc22-4b79-457c-a614-949bba087617
translation-type: ht
source-git-commit: 85879d92104d8b6d739fb4d17dc8cfb7483a9343

---


# Publicar um segmento de público-alvo do Analytics

Publique um segmento de público-alvo do Analytics na Experience Cloud e no Adobe Target para as atividades de marketing do público-alvo.

1. No Analytics, [crie um segmento](https://marketing.adobe.com/resources/help/pt_BR/analytics/segment/?f=seg_build).
1. No Construtor de segmentos, habilite a opção **[!UICONTROL Faça deste um público-alvo da Experience Cloud]**.

   ![](assets/ec_audience_example.png)

   | Elemento | Descrição |
   |--- |---|
   | Faça deste um público-alvo da Experience Cloud (para &lt;nome do conjunto de relatórios&gt;) | Publica esse segmento na Experience Cloud. Você pode usar o público-alvo para as atividades de marketing no Adobe Target e a segmentação no Audience Manager.<br>Os campos Título e Descrição são obrigatórios para o segmento ser publicado.<br>Quando essa opção é ativada, o título e a definição do segmento do público-alvo são compartilhados, mas os dados reais não são. Quando o público-alvo é associado a uma campanha ativa no Target, o Analytics começa a enviar IDs para os visitantes que se qualificaram para esse público-alvo da Experience Cloud e do Target. Nesse momento, o nome do público-alvo e os dados correspondentes começam a ser exibidos na página Públicos-alvo da Experience Cloud.<br>Públicos-alvo compartilhados com a Experience Cloud a partir do Analytics não podem exceder 20 milhões de membros do público-alvo.<br>Devido a questões relacionadas ao cache, conjuntos de relatórios excluídos no Analytics permanecem exibidos na Experience Cloud por 12 horas após a exclusão.<br>No Analytics, você pode editar ou excluir um segmento publicado. Se o segmento estiver em uso, uma mensagem de aviso será emitida quando um segmento for editado. Não é possível excluir um segmento publicado que esteja sendo usado pelo Adobe Target.<br>Depois que um visitante é qualificado para o público-alvo compartilhado do Analytics, existe um atraso de 24 a 48 horas antes de as informações serem ativadas no Target, no Media Optimizer e no Campaign.<br>**Privacidade dos dados**<br>Os públicos-alvo não são filtrados com base no estado de autenticação de um visitante. Se um visitante consegue navegar em seu site em estados de autenticação e de não autenticação, as ações que ocorrem quando um visitante não está autenticado podem fazer com que um visitante seja incluído em um público-alvo. Analise a [Visão geral da privacidade do Analytics](https://marketing.adobe.com/resources/help/pt_BR/reference/?f=c_Privacy_Overview) para compreender as implicações completas de privacidade do compartilhamento de público-alvo. |
   | Selecione a janela para a criação de público-alvo | Observe que esta é uma janela de tempo **flutuante**, e não de tempo fixo. |

1. Clique em **[!UICONTROL Salvar]**.
1. Acesse [!DNL Adobe Target], clique [!UICONTROL em Públicos-alvo].
1. Na página [!UICONTROL Públicos-alvo], localize o público-alvo proveniente da Experience Cloud.

   Esses públicos-alvo estão disponíveis para uso em atividades.
