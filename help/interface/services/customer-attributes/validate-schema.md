---
description: Saiba como validar o esquema  [!DNL Customer Attributes]  no Adobe CX Enterprise.
solution: Experience Cloud
title: 'Como validar o esquema  [!DNL Customer Attributes] '
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 776d1fd3-c733-4970-a76b-4c3c0119ee77
TQID: https://experienceleague.adobe.com/J-AaDn4HtD1bS-VCPn2XiPLVBbTnYyl5o1NpJ9HFj1g
product_v2: id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2: id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2: id: b75843fa-0a67-4a44-a6b1-cc627b0481dcid: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 1a77ef8d31211fb11c790152e78037a8c3b238a2
workflow-type: tm+mt
source-wordcount: 308
ht-degree: 43%

---

# Validar o esquema

O processo de validação permite mapear os nomes de exibição e as descrições aos atributos carregados (strings, números inteiros, números e assim por diante).

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

   ![Editar página de esquema na CX Enterprise](assets/schema-edit.png)

**Ações**

* **[!UICONTROL Add Data:]** Carregue novos dados de atributo para esta fonte de dados.

* **[!UICONTROL View/Edit Schema:]** Mapeie os nomes de exibição para os dados do atributo, conforme descrito na próxima etapa.

* **[!UICONTROL FTP Setup:]** Crie sua conta FTP para [carregar seus dados via FTP](t-upload-attributes-ftp.md) (opcional).

* **[!UICONTROL ID Lookup:]** Insira uma ID do cliente (CID) em seu `.csv` para pesquisar informações da CX Enterprise para a ID. Esse recurso é útil para solucionar por que os dados do atributo não são exibidos para um visitante:

   * **[!UICONTROL ECID (CX Enterprise ID):]** Exibe se você está usando o Serviço da CX Enterprise ID mais recente. Se você estiver no serviço da MCID, mas não houver IDs listadas, a CX Enterprise não recebeu um alias para essa CID. Isso indica que o visitante não está conectado ou que sua implementação não está transmitindo essa ID.

   * **[!UICONTROL CID (customer ID):]** Os atributos associados a esta CID. Se você estiver usando uma prop ou eVar para fazer upload das CIDs (AVID) e visualizar os atributos exibidos, mas nenhuma AVID, isso indica que o visitante não está conectado ao seu site.

   * **[!UICONTROL AVID (Analytics visitor ID):]** Exibe se você usa uma prop ou eVar para carregar CIDs. Se essas IDs forem transmitidas para o CX Enterprise, todas as IDs de visitante associadas à CID inseridas serão exibidas aqui.
