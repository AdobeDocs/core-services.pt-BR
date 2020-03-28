---
description: Uma visão geral de novos recursos e atualizações na Experience Cloud.
keywords: core services
seo-description: Uma visão geral de novos recursos e atualizações na Experience Cloud.
seo-title: Novidades da Experience Cloud
solution: Experience Cloud
title: Novidades da Experience Cloud
uuid: bc1b1542-1a37-4da1-bcfd-fc86af881642
translation-type: tm+mt
source-git-commit: 43de353155c640b3ddc519147c94d7e9ffcafe4e

---


# Novidades da Experience Cloud

Uma visão geral de novos recursos e atualizações na Experience Cloud.

## Agosto de 2018 {#section_7388CDAB723B49809AABEFEE85CF6378}

Correções e aprimoramentos para agosto de 2018.

* Aprimoramentos feitos na sincronização de comentários de ativos na Creative Cloud e na Experience Cloud. (CORE-15971)
* Adição de um sinalizador de recurso para controlar sincronização de ativos entre a Experience Cloud e a Creative Cloud. (CORE-15938)
* Melhorias na criação de segmentos de Audiência, incluindo uma melhor experiência em pesquisa e listagem. (CORE-5833, CORE-14278)
* Correção de um problema de alta prioridade que bloqueava o compartilhamento de pastas do MAC para a Creative Cloud. (CORE-16677)

## 19 de julho de 2018 {#section_EBB549EBABB7480884A180237ADCCD02}

Correções e aprimoramentos para julho de 2018.

* Implantação de um recurso de back-end para controlar o compartilhamento de ativos entre a Experience Cloud e o AEM e entre a Experience Cloud e a Creative Cloud. (CORE-14386)
* Correção de um problema que bloqueava o provisionamento de novos locatários em alguns ambientes. (CORE-15509)
* Correção de um problema que redirecionava usuários para [!DNL experiencecloud.adobe.com] ao acessarem [!DNL experiencecloud.adobe.com] por meio de [!DNL http] em vez de [!DNL https] (seguro). (CORE-15587)
* Correção de um problema que bloqueava notificações para alguns novos inquilinos. (CORE-15240)

## 14 de junho de 2018 {#section_7ABC327992CB46B0B8E4A631B8B68899}

Correções e melhorias para junho de 2018.

* Habilitação de um link de acesso de GDPR para Administradores. (CORE-11731)
* Atualização do recurso Beta Feedback para restringir tipos de arquivos que podem ser anexados ao feedback. (CORE-10474)
* Correção de um problema com a exclusão de audiências da Biblioteca de Audiências. (CORE-12792)
* Correção de um problema que resultava em uma tela em branco ao acessar links do Workspace usando Federated IDs. (CORE-11620)

## 10 de maio de 2018 {#section_498AF78DA17C4720AA0F32B51493E550}

Novos recursos e correções na interface da [!DNL Adobe Experience Cloud].

| Recurso | Descrição |
|--- |--- |
| Nova landing page de administração | Ao fazer logon na Experience Cloud e navegar até a página Administração, uma nova interface intuitiva está disponível para ajudá-lo a acessar rapidamente as soluções da Experience Cloud e os principais serviços. |

**Correções**

* Correção de um problema em que o carregamento da imagem falhava devido a uma atualização do Scene7. (CORE-12746)
* Foram feitas atualizações para descartar o suporte ao protocolo TLS 1.0, conforme exigido pela PCI para eliminar a vulnerabilidade de segurança. (CORE-7695)

## 26 de outubro de 2017 {#section_11195859B4094177A939C0561428B525}

**Problema conhecido**

Muitas das notificações de manutenção sobre manutenção programada / atualizações de produto estão ausentes do resumo de email de notificações. Estamos trabalhando para garantir que todas as notificações de manutenção sejam incluídas no resumo do email.

## August 8, 2017 {#section_2313A875454044F490B418506DD24593}

| Recurso | Descrição |
|--- |--- |
| Notificações - Configurações granulares | É possível habilitar notificações sobre atividades e eventos de soluções e produtos e de atividades de upload de [Atributos de clientes](../attributes/attributes.md). |
| Notificações - Notificações de manutenção | Nas configurações de Notificação, você pode ativar notificações de manutenção para produtos e soluções. |
| Admin Console para Soluções da Experience Cloud | Os novos clientes da Experience Cloud podem começar a usar o Admin Console, um local central para gerenciar seus direitos da Adobe em toda a organização.<br>A migração para o Admin Console no gerenciamento de usuários acontecerá em etapas. A Adobe entrará em contato com você (administradores do sistema) quando chegar o momento de migrar.<br>Administradores do Analytics, consulte Migração [](https://docs.adobe.com/content/help/en/analytics/admin/user-product-management/user-management/migrate-users/c-migration-tool.html)do Analytics. |

## 22 de maio de 2017 {#section_242FE649FA1B4BFA88EC6E353D175ACC}

| Recurso | Descrição |
|--- |--- |
| Mapeamento em massa do conjunto de relatórios | Em Administração > Mapeamento do conjunto de relatórios, agora você pode selecionar vários conjuntos de relatórios e mapeá-los a uma organização. (Anteriormente, você tinha que mapeá-los individualmente.)  <br>[Mapear conjuntos de relatórios](../core-services/core-services.md) para uma única organização ajuda a habilitar recursos e serviços entre soluções na Experience Cloud. |
| Atualizações aos públicos-alvo da Experience Cloud | **Aplicação dos conjuntos de relatórios **<br>Agora é possível aplicar um conjunto de relatórios a todas as suas[regras de público-alvo](../audience-library/t-audience-create.md). (Anteriormente, você tinha que especificar um conjunto de relatórios em cada definição de regra.)<br>**Props e variáveis**<br>Agora é possível incluir props do Analytics e variáveis padrão (além das eVars e eventos) em públicos-alvo em tempo real. |

## 8 de novembro de 2016 - 16.11.1 {#section_7065A9BCCDF544C2BB37E9A7D661EA6A}

| Recurso | Descrição |
|--- |--- |
| Atualizar para Perfil e senhas | Não é mais possível editar informações de perfil IMS na seção Detalhes pessoais em Editar perfil > Perfil e senhas. Em vez disso, os usuários são direcionados para `accounts.adobe.com`. Isso aplica-se a todos os tipos de identidade (Adobe ID, Enterprise e Federated). |

**Correções**

* Correção de um problema com senhas técnicas que causava um erro no compartilhamento de pastas entre a Creative Cloud e a Experience Cloud. (MAC-31067, MAC-32014)
* Corrigido um problema com o upload de certos tipos de arquivo, incluindo PDF, que foi encontrado depois da versão de outubro no Assets Core Service. (MAC-32517)
