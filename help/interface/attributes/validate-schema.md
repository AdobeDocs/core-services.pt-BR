---
description: Saiba como validar o schema de atributo do cliente no Adobe Experience Cloud.
keywords: Customer Attributes;Experience Cloud services
solution: Experience Cloud
title: Como validar o schema de atributo do cliente | Adobe Experience Cloud
uuid: 163a4dbe-d60b-4089-8ff8-65f7461fbdf7
translation-type: tm+mt
source-git-commit: 4bea0c29afa580dc63b21535ce5c275cd649c9a5
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 95%

---


# Validar o esquema

O processo de validação permite mapear os nomes de exibição e as descrições aos atributos carregados (sequências, números inteiros, números e assim por diante). Um esquema é criado com base nessas configurações. O esquema é usado para validar todos os dados futuros carregados nessa fonte de dados. Esse processo de mapeamento não altera os dados originais.

>[!NOTE]
>
>A atualização do esquema após a validação exclui os atributos do cliente. Consulte [Atualizar o esquema (também exclui os atributos)](../attributes/t-crs-usecase.md#task_6568898BB7C44A42ABFB86532B89063C).

**[!UICONTROL Fonte de atributos do cliente]** > **[!UICONTROL Criar nova fonte de atributos do cliente]** > **[!UICONTROL Exibir/editar esquema]**

![](assets/view_edit_schema.png)

Na página [!UICONTROL Validar esquema], cada linha do esquema representa uma coluna do arquivo CSV carregado.

![](assets/06_crs_usecase.png)

* **[!UICONTROL Adicionar dados:]** Faça upload dos novos dados do atributo para essa fonte de dados.

* **[!UICONTROL Exibir/editar esquema:]** Mapeie os nomes de exibição para os dados do atributo, conforme descrito na próxima etapa.

* **[!UICONTROL Configuração de FTP:]** [Faça upload dos dados via FTP](../attributes/t-upload-attributes-ftp.md#task_591C3B6733424718A62453D2F8ADF73B).

* **[!UICONTROL Pesquisa de ID:]** Insira uma ID do cliente (CID) em seu `.csv` para pesquisar informações da Experience Cloud para a ID. Esse recurso é útil para solucionar por que os dados do atributo não são exibidos para um visitante:

   * **[!UICONTROL ECID (Experience Cloud ID):]** exibe se você está usando o serviço de ID mais recente da Experience Cloud. Se você estiver no serviço da MCID, mas não houver IDs listadas, a Experience Cloud não recebeu um alias para essa CID. Isso indica que o visitante não está conectado ou que sua implementação não está transmitindo essa ID.

   * **[!UICONTROL CID (ID do cliente):]** os atributos associados a essa CID. Se você estiver usando uma prop ou eVar para fazer upload das CIDs (AVID) e visualizar os atributos exibidos, mas nenhuma AVID, isso indica que o visitante não está conectado ao seu site.

   * **[!UICONTROL AVID (ID de visitante do Analytics):]** exibe se você usa uma prop ou eVar para fazer upload das CIDs. Se essas IDs forem transmitidas para a Experience Cloud, todas as IDs de visitante associadas à CID inseridas serão exibidas aqui.

Também é possível fazer upload dos dados via FTP após criar uma fonte de atributo do cliente e uma conta FTP na Experience Cloud. É possível criar uma conta FTP por fonte de atributo. Os arquivos carregados são armazenados na pasta raiz dessa conta. Os dados devem estar em formato .csv, com um segundo arquivo .fin para indicar que o upload foi concluído.

Os nomes aplicados às sequências, números inteiros e números são usados para criar as métricas do [!DNL Analytics]. Consulte [Relatórios de atributos do cliente](https://docs.adobe.com/content/help/pt-BR/core-services/interface/customer-attributes/attributes.html) na ajuda do [!DNL Analytics] para obter mais informações.

* **[!UICONTROL Atributo:]** Os dados do atributo lidos no arquivo `.csv` carregado.

* **[!UICONTROL Tipo:]** Os tipos de dados, como:

   * **Cadeia de caracteres:** uma sequência de caracteres.

   * **Inteiros:** números inteiros.

   * **Números:** pode ter até duas casas decimais.

* **[!UICONTROL Nome de exibição:]** Um nome amigável para o atributo. Por exemplo, você pode alterar a idade de um atributo *idade do cliente* para *Cliente desde*.

* **[!UICONTROL Descrição:]** Uma descrição amigável do atributo.
