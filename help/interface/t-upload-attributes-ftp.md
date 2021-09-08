---
description: Saiba como fazer upload dos dados de atributos do cliente via FTP para a Experience Cloud.
keywords: Atributos do cliente;serviços principais
solution: Experience Cloud
title: 'Fazer upload do arquivo de dados do atributo do cliente via FTP '
uuid: 5df565dd-b6f8-420e-981f-4b6fc6f7d0e4
feature: Atributos do cliente
topic: Administração
role: Admin
level: Experienced
exl-id: ed9e4a8f-493a-4a0f-a87e-674c7da95b99
source-git-commit: 1fb1abc7311573f976f7e6b6ae67f60ada10a3e7
workflow-type: ht
source-wordcount: '271'
ht-degree: 100%

---

# Opcional - Fazer upload do arquivo de dados via FTP

Se você não fizer upload usando a função arrastar e soltar, será possível fazer upload do atributo do cliente via FTP para a Experience Cloud.

Você pode fazer upload dos dados depois de criar uma fonte de atributo do cliente e uma conta FTP na Experience Cloud. É possível criar uma conta FTP por fonte de atributo. Os arquivos carregados são armazenados na pasta raiz dessa conta. Os dados devem estar em formato `.csv`, com um segundo arquivo `.fin` para indicar que o upload foi concluído.

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
