---
title: Monitoramento do uso de IA de agente
description: Saiba mais sobre os painéis para o monitoramento do uso de IA no CX Enterprise. Acompanhe a adoção, analise conversas e comentários e gerencie créditos de IA para uso, qualidade e visibilidade de custos.
solution: Experience Cloud, Experience Platform
topic: Artificial Intelligence
feature: Agentic AI, AI Tools
role: Admin, User
level: Intermediate
autotag-review: '2026-05-27T16:30:16.764Z'
TQID: 'https://experienceleague.adobe.com/J74yr0gGkFu1bzTmMvhrQ8TNaRX6nRjWY9WAwd3uydk'
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
  - id: e1971122-7081-4556-9222-8a31bd71800c
feature_v2:
  - id: f84b2906-3ce9-4ef0-86f6-cda249273937
subfeature_v2:
  - id: cda95149-19e1-4cfa-a57e-751283a32378
topic_v2:
  - id: bbbea26f-9621-49eb-9ab8-e06fb3bbce8c
source-git-commit: 9c847f904b899fbe1273b91bd776083d0b4a71a1
workflow-type: tm+mt
source-wordcount: 881
ht-degree: 2%

---

# Painéis de monitoramento de IA corporativa

O painel de monitoramento da IA corporativa oferece aos membros do Centro de Excelência (COE) e a outras partes interessadas da governança visibilidade sobre o uso e a adoção da IA corporativa. Você pode visualizar tendências ao longo de períodos de 7 ou 30 dias para ver quem usa o [!DNL AI Assistant] ou outras superfícies de conversação (como o [Adobe Marketing Agent for Microsoft 365 Copilot](https://experienceleague.adobe.com/pt-br/docs/experience-cloud-ai/experience-cloud-ai/agents/ama-ms)) para interagir com o [!DNL Experience Platform Agents], o que eles fazem nessas interações e o valor que eles recebem. Juntas, essas visualizações ajudam a orientar a adoção de agentes com dados em vez de suposições.

O painel de monitoramento do Agentic AI inclui as seguintes exibições:

| Painel | Finalidade |
| --- | --- |
| **Visão geral** | Métricas agregadas entre usuários, conversas, feedback e consumo de crédito |
| **Usuários** | Frequência de uso, distribuição e envolvimento por usuário |
| **Feedback** | Sinais sobre a qualidade da resposta e a satisfação do usuário |
| **Créditos de IA** | Tendências de consumo de crédito e saldo restante |

Os agentes no escopo para monitoramento de uso estão listados em [Agentes de IA em aplicativos CX Enterprise existentes](agentic-ai.md#existing-apps-table) na [IA de agente na documentação do Adobe CX Enterprise](agentic-ai.md).

[Exibir vídeo de introdução](https://video.tv.adobe.com/v/3491864?learn=on)

## Habilitar permissões de painel {#permissions}

Conceda acesso ao painel em [!DNL Adobe Experience Platform] atualizando o perfil do produto ou a função para cada usuário autorizado. O recurso [!UICONTROL Monitoramento] é exibido para os usuários na home page do CX Enterprise após a habilitação das permissões.

1. Vá para [!DNL Experience Platform] **Administração** > **Permissões**.

1. Abra o perfil de produto ou a função que deseja atualizar.

   ![Habilitar Permissões do Painel](../features/assets/dashboards-permissions.png)

1. Em **[!UICONTROL Permissões do Assistente de IA]**, clique em **[!UICONTROL Adicionar recurso]** e habilite o **[!UICONTROL Exibir painel de uso do Assistente de IA]**.

   Essa permissão concede acesso aos painéis de monitoramento de uso da IA de agente.

1. Em **[!UICONTROL Painéis]** permissões, configure o acesso ao painel com base nas responsabilidades de cada usuário.

   ![Habilitar Permissões do Painel](../features/assets/dashboards-add-resource.png)

   Permissões recomendadas para usuários autorizados do controle:

   * **[!UICONTROL Exibir Painel de Uso de Licenças]**
   * **[!UICONTROL Exibir Painéis Padrão]**
   * **[!UICONTROL Exportar Dados do Painel]** (opcional, somente para usuários de governança aprovados)

   Permissões adicionais que você pode conceder quando necessário:

   * **[!UICONTROL Gerenciar Painéis Personalizados]**
   * **[!UICONTROL Exibir Painéis Personalizados]**
   * **[!UICONTROL Gerenciar Painéis Padrão]**

1. Para exibir painéis, retorne à página inicial do CX Enterprise e clique em **[!UICONTROL Monitoramento]**.

   ![Painel de monitoramento do Agentic AI](../features/assets/monitoring.png)

## Painel de visão geral

O painel Visão geral é o local central para métricas de adoção e envolvimento em toda a organização. Ele conecta tendências de alto nível a análises mais profundas. De qualquer métrica, você pode detalhar conversas individuais para ver o que direciona os números.

### Métricas no painel Visão geral

* **Avisos ao longo do tempo:** Crescimento do uso geral e tendências de adoção.
* **Usuários e conversas ativos:** Contagem de usuários interagindo com [!DNL Experience Platform Agents].
* **Média de prompts por conversa:** Profundidade da participação por conversa.
* **Feedback:** Distribuição de miniaturas para cima e miniaturas para baixo do feedback dos usuários (somente para [!DNL AI Assistant] interações).

[Exibir vídeo](https://video.tv.adobe.com/v/3491865?learn=on)

### Repetição da conversa

A repetição da conversa mostra interações individuais, não apenas agregações. Você pode analisar padrões em várias conversas e mudar de tendências de alto nível para uma conversa específica.

* **Histórico de prompts e respostas:** o prompt do usuário e as respostas entregues.
* **Sinais de feedback:** Interações de usuários marcadas com polegares para cima ou para baixo, para identificar necessidades de atrito, bloqueadores ou de habilitação. Essas informações ajudam a sua organização a melhorar a relevância imediata e ajudam a Adobe a melhorar a qualidade da resposta ao longo do tempo.

[Exibir vídeo](https://video.tv.adobe.com/v/3491866?learn=on)

## Painel de usuários

O painel Usuários mostra como a adoção e o engajamento do agente variam entre os usuários ao longo do tempo. Você pode ver quem usa ativamente o [!DNL Experience Platform Agents], qual superfície ele usa e com que frequência ele interage. Os administradores e membros do COE podem detalhar atividades e conversas de usuários individuais para entender os padrões de engajamento e o comportamento de uso.

### Métricas no painel Usuários

* **Tendências de adoção e envolvimento ao longo do tempo:** Rastreie como os segmentos de usuários mudam durante o período selecionado. Os usuários são classificados como:
   * **Novo:** primeira atividade no período selecionado, sem atividade nos 12 meses anteriores.
   * **Repetir:** atividade tanto no período selecionado quanto no período anterior.
   * **Retorno:** Atividade no período selecionado, mas não no período anterior.
   * **Inativo:** nenhuma atividade no período selecionado, mas a atividade no período anterior.
* **Padrões de engajamento do usuário:** a frequência com que os usuários interagem com agentes e como o engajamento muda ao longo do tempo.
* **Atividade de conversa:** Número de conversas e prompts por usuário.
* **Principais usuários ativos:** usuários e equipes altamente engajados que impulsionam a adoção de agentes.

[Exibir vídeo](https://video.tv.adobe.com/v/3491868?learn=on)

## Painel de comentários

O painel Feedback mostra o feedback do usuário enviado para interações do agente. Você pode ver quais conversas os usuários marcaram de forma positiva ou negativa e investigar as interações por trás do feedback. A partir de resumos de feedback, aprofunde-se em conversas individuais para revisar prompts, respostas, detalhes de raciocínio e notas de feedback.

### Métricas no painel de Feedback

* **Tendências dos comentários ao longo do tempo:** como os comentários dos usuários mudam ao longo do tempo.
* **Feedback para cima e para baixo:** sinais de interação positivos e negativos.
* **Categorias de comentários:** lógica por trás de cada miniatura para cima e miniatura para baixo.
* **Histórico de prompts e respostas:** prompts do usuário e as respostas associadas ao feedback enviado.
* **Detalhes e observações do feedback:** Contexto e comentários adicionais dos usuários durante o envio do feedback.

[Exibir vídeo](https://video.tv.adobe.com/v/3491878?learn=on)

## Painel Créditos de IA

O painel Créditos de IA mostra como o uso de [!DNL Experience Platform Agents] pela sua organização se traduz no consumo de Créditos de IA.

### Métricas no painel Créditos de IA

* **Total de créditos de IA consumidos:** Uso geral do agente em créditos de IA.
* **Tendências diárias e mensais:** picos, declínios e alterações nos padrões de consumo.
* **Créditos de IA restantes:** saldo restante para que você possa planejar de forma proativa e evitar excedentes.

[Exibir vídeo](https://video.tv.adobe.com/v/3491867?learn=on)

## Mais ajuda sobre este tópico

* [Painel de uso de licença](https://experienceleague.adobe.com/pt-br/docs/experience-platform/dashboards/guides/license-usage) em [!DNL Experience Platform]
* [IA de agente na Adobe CX Enterprise](agentic-ai.md)
* [Trabalhos de agentes e consumo de crédito de IA](ai-credit-consumption.md)
* [Painel de uso de licenças](https://experienceleague.adobe.com/pt-br/docs/experience-platform/dashboards/guides/license-usage) (Experience Platform)
