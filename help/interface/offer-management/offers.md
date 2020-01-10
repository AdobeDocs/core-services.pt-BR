---
description: Crie e gerencie ofertas para serem usadas no Adobe Campaign.
seo-description: Crie e gerencie ofertas para serem usadas no Adobe Campaign.
seo-title: Gerenciamento de ofertas
title: Gerenciamento de ofertas
uuid: 83e1d4cd-c5fa-4df0-9603-2914eb4648f8
index: y
translation-type: tm+mt
source-git-commit: a0e0b51d731343d5cd4226ab29d917aca63317c2

---


# Ofertas

Crie e gerencie ofertas para serem usadas no Adobe Campaign.

Há dois tipos de ofertas no Gerenciamento [!UICONTROL de]ofertas:

| Tipo | Descrição |
|---|---|
| Oferta geral | Permite preencher o modelo de dados de oferta completo (regras de qualificação, datas de início e término e conteúdo). |
| Oferta de fallback | A última oferta de recurso se um cliente não estiver qualificado para nenhuma das outras ofertas selecionadas. Não é possível associar regras de qualificação ou datas de início e término a ofertas de fallback. |

>[!NOTE]
>
>Em uma atividade de oferta, você sempre será solicitado a selecionar uma oferta de fallback. Portanto, você deve ter pelo menos uma oferta de fallback no inventário da oferta antes de criar uma atividade da oferta.

## Criar uma oferta

Crie uma oferta para adicionar ao inventário da oferta.

1. Na guia [!UICONTROL Inventário] em Gerenciamento [!UICONTROL de]ofertas, clique em **[!UICONTROL Criar nova oferta]**e selecione**[!UICONTROL  Criar oferta]**.

   ![](assets/create-offerx.png)

1. Preencha os campos a seguir:

   | Campo | Descrição |
   |--- |--- |
   | Nome da oferta | O nome associado à oferta. Não é possível ter duas ofertas no inventário com nomes duplicados. |
   | Data de início | A data em que a oferta pode ser exibida. Se uma data inicial de 1/15/17 for selecionada, a oferta poderá ser exibida a partir das 12:00 da manhã, em 15/17.  O Gerenciamento de ofertas opera no padrão de tempo UTC. Isso significa que: <ul><li> As ofertas se tornam válidas às 00:00 UTC no dia em que a oferta está definida para iniciar.</li><li> As ofertas expiram às 00:00 UTC no dia seguinte à data de término. Por exemplo, se uma oferta estiver definida para ter uma data de término de 14/05, ela expirará às 00:00 UTC em 15/05. A oferta é então arquivada.</li><li>Quando os e-mails são preparados no Adobe Campaign, somente as ofertas válidas nesse momento serão exibidas.</li></ul> |
   | Data de término | A data em que a oferta termina. Se uma data de término de 20/01/17 for selecionada, a oferta não será mais exibida depois das 20/11:59PM. Quando uma oferta passa sua data de término, é arquivada automaticamente. O Gerenciamento de ofertas opera no padrão de tempo UTC. Consulte a linha acima para obter mais informações. |
   | Regras de elegibilidade | Você pode criar regras de qualificação de oferta com base nos dados disponíveis no banco de dados da Campanha. As regras de qualificação determinam para quem e quando uma oferta pode ser mostrada.  Por exemplo, você pode especificar que deseja que somente uma &#39;Oferta de roupas femininas de inverno&#39; seja exibida quando (Gênero = &#39;Feminino&#39;) e (Região = &#39;Nordeste&#39;). Os atributos usados para criar essas regras vêm do perfil do Campaign Standard.  Observação:  Quando você acessa o Gerenciamento de ofertas pela primeira vez, não há atributos disponíveis no construtor de regras. Você deve compartilhar atributos da interface do usuário da campanha. Depois de compartilhados, esses atributos ficam disponíveis. |
   | Limite máximo | Os períodos máximos em que uma oferta pode ser proposta.  Observação:  O número de vezes que uma oferta é proposta é calculado no momento da preparação do email. Por exemplo, se você preparar um e-mail com várias ofertas, esses números serão contados para a sua limitação máxima independentemente de o e-mail ser enviado ou não. |
   | Limite máximo por usuário | O número máximo de vezes que uma oferta pode ser proposta a um determinado usuário.  Observação:  O número de vezes que uma oferta é proposta a um determinado usuário é calculado no momento da preparação do email. Por exemplo, se você preparar um email com várias ofertas, esses números serão contados para o limite máximo por usuário, independentemente de o email ser enviado ou não. |
   | Rótulos | Adicione rótulos a uma oferta para agrupá-los. Você pode digitar e pressionar Enter para criar um novo rótulo ou começar a digitar e selecionar uma oferta existente no menu suspenso. |

1. Preencha os detalhes das representações.

   | Campo | Descrição |
   |---|---|
   | Canal | O canal no qual essa representação de conteúdo pode ser entregue. Os emails do Campaign Standard são o único canal disponível no momento. |
   | Disposição | Selecione a disposição na qual essa representação de conteúdo pode ser entregue. As disposições são preenchidas previamente na guia Disposições. É necessário associar cada representação de conteúdo a uma disposição do menu suspenso. Não é possível criar várias representações de conteúdo com a mesma disposição na mesma oferta. |
   | Tipo de conteúdo | Selecione um tipo de conteúdo de uma imagem, URL da imagem, texto ou HTML. |
   | Redirecionar link | Esse campo será exibido se você selecionar um tipo de conteúdo de imagem ou URL de imagem. Este é o link para o qual o usuário será redirecionado se clicar na oferta em um email. |

1. Clique em **[!UICONTROL Salvar e visualizar]**para revisar os detalhes da sua oferta antes do envio.
1. Clique em **[!UICONTROL Aprovar]**para aprovar a oferta. Quando a oferta estiver no estado aprovado, ela poderá ser usada em uma atividade de oferta.

   Se você não tiver as permissões necessárias para aprovar uma oferta, clique em **[!UICONTROL Enviar]**. A oferta será exibida na biblioteca de ofertas com um status pendente. Depois que um usuário com direitos de aprovação o aprovar, ele estará disponível para uso em uma atividade de oferta.
