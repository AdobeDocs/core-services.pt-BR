---
description: Se você não fizer upload usando a função arrastar e soltar, será possível fazer upload do atributo do cliente via FTP na Experience Cloud.
keywords: atributos do cliente, serviços principais
seo-description: Se você não fizer upload usando a função arrastar e soltar, será possível fazer upload do atributo do cliente via FTP na Experience Cloud.
seo-title: Opcional - Fazer upload do arquivo de dados via FTP
solution: Experience Cloud
title: Opcional - Fazer upload do arquivo de dados via FTP
uuid: 5df565dd-b6f8-420e-981f-4b6fc6f7d0e4
translation-type: tm+mt
source-git-commit: f8b48077d936e289d66c1a93a96fe9ebaa4f0136

---


# Opcional - Fazer upload do arquivo de dados via FTP

Se você não fizer upload usando a função arrastar e soltar, será possível fazer upload do atributo do cliente via FTP na Experience Cloud.

Você pode fazer upload dos dados depois de criar uma fonte de atributo do cliente e uma conta FTP na Experience Cloud. É possível criar uma conta FTP por fonte de atributo. Os arquivos carregados são armazenados na pasta raiz dessa conta. Os dados devem estar em formato `.csv`, com um segundo arquivo `.fin` para indicar que o upload foi concluído.

>[!IMPORTANT]
>
>Analise [os requisitos do arquivo de dados para fazer upload dos atributos do cliente](../attributes/crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19) antes de fazer upload do arquivo.


Os uploads do arquivo para o site FTP dos atributos do cliente podem ser realizados via FTP ou SFTP.

* O cliente precisa ter suporte para conexões SFTP.
* Você pode conectar-se com o SFTP usando o nome de usuário/senha ou sem usar senha, conforme descrito [aqui](https://marketing.adobe.com/resources/help/en_US/whitepapers/ftp/?f=ftp_sftp_cert_auth).



<!-- <p>Error states - get with Matt and Dave </p> 
<p>What are the most common reasons for doing this? Retail? Do a use case example, then show an AN example. </p> 
<p>You create one FTP per attribute source. Files go to the root folder in that account. The file type .fin is user-created. (For example, upload a .csv then a .fin of the same name, which signals you have completed the upload. https://wiki.corp.adobe.com/display/marketingcloud/Customer+Record+Services#CustomerRecordServices-FileFormats (leverage for doc). Possibly link from FTP File Reqs page to a help file about naming conventions. Need a new file type page for this. Similar content here: https://marketing.adobe.com/resources/help/en_US/reference/c_general_file_structure.html and here: https://marketing.adobe.com/resources/help/en_US/whitepapers/ftp/ftp_datasources.html </p> 
<p>Drag-n-drop and zip functionality for uploads - 1/21/2015. S/b less than 100 megs for drag and drop zip file. Fin file not required for drag/drop. </p> 
<p>Preview Data - shows the last upload (?) </p> 
<p>Need a link to the "instructions" on that information icon with the image. </p> 
<p>Workflow: Drag and drop, validate schema, configure subscription, save/activate. </p> -->
**Para fazer upload do arquivo de dados via FTP**

1. [Crie uma fonte de atributo do cliente e faça upload do arquivo de dados...](../attributes/t-crs-usecase.md#task_BCC327B2A0EF4A1BBB2934013AB92B78).

   Verifique se você está conectado no site FTP em [!DNL ftp.adobe.com/<sftpname>].

1. Clique em **[!UICONTROL Ações]** &gt; **[!UICONTROL Upload do arquivo]**.

1. Faça upload de um arquivo `.fin`, para que o arquivo possa ser recuperado.

   O tipo de arquivo `.fin` é criado pelo usuário e indica que o upload foi concluído. Ele pode ser um arquivo do bloco de notas em branco. Por exemplo, se você fizer upload do [!DNL crs123.csv], também será possível fazer upload do [!DNL crs123.fin].

   Se o upload for bem-sucedido, ambos os arquivos serão movidos para uma pasta chamada **processados**.


   Consulte [os requisitos do arquivo de dados para fazer upload dos atributos do cliente](../attributes/crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19) para obter informações importantes sobre os nomes dos arquivos e a estrutura.
