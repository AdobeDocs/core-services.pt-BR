---
description: Saiba como fazer upload dos dados de Atributos do cliente via FTP para o Experience Cloud.
solution: Experience Cloud
title: Fazer upload do arquivo de dados do atributo do cliente via FTP
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: ed9e4a8f-493a-4a0f-a87e-674c7da95b99
source-git-commit: f229ec33ff721527e6a4c920ea63eabb4102935a
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 77%

---

# Opcional - Fazer upload do arquivo de dados via FTP

Se você não fizer upload usando a função arrastar e soltar, será possível fazer upload do atributo do cliente via FTP para o Experience Cloud.

Você pode fazer upload dos dados depois de criar uma fonte de atributo do cliente e uma conta FTP no Experience Cloud. É possível criar uma conta FTP por fonte de atributo. Os arquivos carregados são armazenados na pasta raiz dessa conta. Os dados devem estar em formato `.csv`, com um segundo arquivo `.fin` para indicar que o upload foi concluído.

>[!IMPORTANT]
>
>Analise [os requisitos do arquivo de dados para fazer upload dos atributos do cliente](crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19) antes de fazer upload do arquivo.

Os uploads de arquivo para o site FTP de atributos do cliente podem ser feitos via FTP ou SFTP:

* Você precisa de um cliente compatível com conexões SFTP.
* Você pode se conectar ao SFTP usando o nome de usuário/senha ou sem usar senha, conforme descrito [aqui](https://experienceleague.adobe.com/docs/analytics/export/ftp-and-sftp/secure-file-transfer-protocol/ftp-sftp-cert-auth.html?lang=pt-BR).

**Para fazer upload do arquivo de dados via FTP**

1. [Crie uma fonte de atributo do cliente e faça upload do arquivo de dados...](t-crs-usecase.md#task_BCC327B2A0EF4A1BBB2934013AB92B78).

   Verifique se você está conectado no site FTP em `ftp.adobe.com/<sftpname>`.

1. Selecione **[!UICONTROL Ações]** > **[!UICONTROL Fazer upload de arquivo]**.

1. Faça upload de um arquivo `.fin`, para que o arquivo possa ser recuperado.

   O tipo de arquivo `.fin` é criado pelo usuário e indica que o upload foi concluído. Ele pode ser um arquivo do bloco de notas em branco. Por exemplo, se você fizer upload do [!DNL crs123.csv], também será possível fazer upload do [!DNL crs123.fin].

   Se o upload for bem-sucedido, ambos os arquivos serão movidos para uma pasta chamada **processados**.

   Consulte [Requisitos do arquivo de dados para fazer upload dos atributos do cliente](crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19) para obter informações importantes sobre os nomes dos arquivos e a estrutura.
