---
description: Saiba como validar o esquema  [!DNL Customer Attributes]  no Adobe Experience Cloud.
solution: Experience Cloud
title: 'Como validar o esquema  [!DNL Customer Attributes] '
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 776d1fd3-c733-4970-a76b-4c3c0119ee77
source-git-commit: e63dd988abba199049da2b3620eed9ebf51043d1
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 37%

---

# Validar o esquema

O processo de validação permite mapear nomes de exibição e descrições para atributos carregados (sequências, números inteiros, números e assim por diante).

Um esquema é criado com base nessas configurações. O esquema é usado para validar todos os dados futuros carregados nessa fonte de dados. Esse processo de mapeamento não altera os dados originais.

>[!NOTE]
>
>A atualização do esquema após a validação exclui os atributos do cliente. Consulte [Atualizar o esquema (também exclui os atributos)](t-crs-usecase.md).

**Para validar o esquema**

1. Em [!DNL Customer Attributes], clique na fonte de atributo para editar.

1. No **[!UICONTROL Edit Customer Attribute Source]**, clique em **[!UICONTROL File Upload]**.

1. Na página [!UICONTROL File Upload and Schema Validation], clique em **[!UICONTROL Actions]** > **[!UICONTROL View/Edit Schema]**

   ![Editar um esquema](assets/actions.png)

   Na página [!UICONTROL Edit Schema], cada linha do esquema representa uma coluna do arquivo CSV carregado.

   ![Editar página de esquema na Experience Cloud](assets/schema-edit.png)

**Ações**

* **[!UICONTROL Add Data:]** Carregue novos dados de atributo para esta fonte de dados.

* **[!UICONTROL View/Edit Schema:]** Mapeie os nomes de exibição para os dados do atributo, conforme descrito na próxima etapa.

* **[!UICONTROL FTP Setup:]** Crie sua conta FTP para [carregar seus dados via FTP](t-upload-attributes-ftp.md) (opcional).

* **[!UICONTROL ID Lookup:]** Insira uma ID do cliente (CID) em seu `.csv` para pesquisar informações da Experience Cloud para a ID. Esse recurso é útil para solucionar por que os dados do atributo não são exibidos para um visitante:

   * **[!UICONTROL ECID (Experience Cloud ID):]** Exibe se você está usando o Serviço da Experience Cloud ID mais recente. Se você estiver no serviço da MCID, mas não houver IDs listadas, a Experience Cloud não recebeu um alias para essa CID. Isso indica que o visitante não está conectado ou que sua implementação não está transmitindo essa ID.

   * **[!UICONTROL CID (customer ID):]** Os atributos associados a esta CID. Se você estiver usando uma prop ou eVar para fazer upload das CIDs (AVID) e visualizar os atributos exibidos, mas nenhuma AVID, isso indica que o visitante não está conectado ao seu site.

   * **[!UICONTROL AVID (Analytics visitor ID):]** Exibe se você usa uma prop ou eVar para carregar CIDs. Se essas IDs forem transmitidas para o Experience Cloud, todas as IDs de visitante associadas à CID inseridas serão exibidas aqui.
