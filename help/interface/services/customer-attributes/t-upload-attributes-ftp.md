---
description: Saiba como fazer upload dos dados de atributos do cliente via FTP para o CX Enterprise.
solution: Experience Cloud
title: Fazer upload do arquivo de dados do atributo do cliente via FTP
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: ed9e4a8f-493a-4a0f-a87e-674c7da95b99
TQID: 'https://experienceleague.adobe.com/VkV54Ix1ryiVxbDsPejsS1-0EVLrZC9ZPqGiG3aQ-94'
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2:
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2: id:id:
role_v2: id:
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: f01d85af42b8f2c27dbada8f73546bc6fe4bf710
workflow-type: tm+mt
source-wordcount: 379
ht-degree: 53%

---

# Fazer upload do arquivo de dados via FTP (opcional)

Se você não fizer upload usando a função arrastar e soltar, será possível fazer upload do atributo do cliente via FTP para a CX Enterprise.

Você pode fazer upload dos dados depois de criar uma fonte de atributo do cliente e uma conta FTP no CX Enterprise. É possível criar uma conta FTP por fonte de atributo. Os arquivos carregados são armazenados na pasta raiz dessa conta. Os dados devem estar em formato `.csv`, com um segundo arquivo `.fin` para indicar que o upload foi concluído.

>[!IMPORTANT]
>
>Revise [fontes e arquivos de dados do atributo do cliente](crs-data-file.md) antes de carregar o arquivo.

Os uploads de arquivo para o site FTP de atributos do cliente podem ser feitos via FTP ou SFTP:

* Você precisa de um cliente compatível com conexões SFTP.
* Você pode se conectar ao SFTP usando o nome de usuário/senha ou sem usar senha, conforme descrito [aqui](https://experienceleague.adobe.com/docs/analytics/export/ftp-and-sftp/secure-file-transfer-protocol/ftp-sftp-cert-auth.html?lang=pt-BR).

**Para fazer upload do arquivo de dados via FTP**

1. [Crie uma fonte de atributo do cliente e faça upload do arquivo de dados...](t-crs-usecase.md).

   Verifique se você está conectado no site FTP em `ftp.adobe.com/<sftpname>`.

1. Clique em **[!UICONTROL Actions]** > **[!UICONTROL File Upload]**.

1. Faça upload de um arquivo `.fin`, para que o arquivo possa ser recuperado.

   O tipo de arquivo `.fin` é criado pelo usuário e indica que o upload foi concluído. Ele pode ser um arquivo do bloco de notas em branco. Por exemplo, se você fizer upload do `crs123.csv`, também será possível fazer upload do `crs123.fin`.

   Se o upload for bem-sucedido, ambos os arquivos serão movidos para uma pasta chamada **processados**.

   Consulte [Arquivos de dados e fontes de atributos do cliente](crs-data-file.md) para obter informações importantes sobre os nomes dos arquivos e a estrutura.

## Configurar uma conta FTP

Configure uma conta FTP por fonte de atributo.

Na página [!UICONTROL File Upload and Schema Validation], clique em **[!UICONTROL FTP Setup]**.

![Editar um esquema](assets/ftp-account.png)

Os arquivos carregados são armazenados na pasta raiz dessa conta. Os dados devem estar em formato `.csv`, com um segundo arquivo `.fin` para indicar que o upload foi concluído.

Os nomes aplicados às strings, números inteiros e números são usados para criar as métricas do [!DNL Analytics].

* **[!UICONTROL attribute:]** dados de atributo lidos do arquivo `.csv` carregado.

* **[!UICONTROL Type:]** Os tipos de dados, como:

   * **String:** uma sequência de caracteres.

   * **Inteiros:** números inteiros.

   * **Números:** pode ter até duas casas decimais.

* **[!UICONTROL Display Name:]** Um nome amigável para o atributo. Por exemplo, você pode alterar um atributo de *idade do cliente* para *cliente desde*.

* **[!UICONTROL Description:]** Uma descrição amigável do atributo.

