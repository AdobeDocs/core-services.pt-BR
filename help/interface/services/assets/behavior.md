---
description: Saiba mais sobre as regras de como as pastas compartilhadas se comportam quando movidas, excluídas e restauradas na Experience Cloud.
keywords: compartilhamento de ativos, Creative Cloud,
solution: Experience Cloud
title: Comportamento das pastas compartilhadas
uuid: 86348401-f4b1-4efe-acd1-7e73a7030edf
feature: Assets
topic: Administration
role: Admin
level: Experienced
exl-id: 5ddcb2f0-b491-466d-b357-aeacbfcf0b8e
source-git-commit: e63dd988abba199049da2b3620eed9ebf51043d1
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 96%

---

# Comportamento das pastas compartilhadas

Regras sobre como as pastas compartilhadas se comportam quando são movidas, excluídas ou restauradas.

>[!NOTE]
>
>As pastas e os ativos compartilhados do Experience Cloud são espelhados na área de trabalho do Creative Cloud em uma relação 1:1. Se um usuário da Experience Cloud mudar uma pasta (excluir, adicionar ou remover o compartilhamento), a ação será espelhada no desktop da Creative Cloud e na Web. Assim, se o compartilhamento de uma pasta for cancelado, a pasta e os ativos serão excluídos da máquina local. Depois que o compartilhamento for removido, a pasta e seu conteúdo serão movidos para a lixeira do computador local, onde você poderá restaurá-los manualmente para o computador.

## Pasta não compartilhada na pasta compartilhada

Movimenta uma pasta não compartilhada para uma pasta compartilhada:

![Pasta não compartilhada para a pasta compartilhada](../../assets/01_assets_move.png)

**Resultado**: ambas as pastas se tornam compartilhadas.

## Pasta compartilhada na pasta não compartilhada

Movimenta uma pasta compartilhada para uma pasta não compartilhada.

![Pasta compartilhada para a pasta não compartilhada](../../assets/02_assets_move.png)

**Resultado**: a pasta não compartilhada permanece não compartilhada. A pasta compartilhada permanece compartilhada.

## Conteúdo da pasta não compartilhada na pasta compartilhada

Movimenta o conteúdo de uma pasta não compartilhada para uma pasta compartilhada.

![Conteúdo da pasta não compartilhada para a pasta compartilhada](../../assets/03_assets_move.png)

**Resultado:** o conteúdo agora é compartilhado e todos os colaboradores podem visualizá-lo. O armazenamento aumenta de acordo com o tamanho do conteúdo.

## Conteúdo compartilhado arquivado e excluído

Arquiva ou exclui o conteúdo presente em uma pasta compartilhada.

![Conteúdo compartilhado arquivado e excluído](../../assets/04_assets_move.png)

**Resultado:** o conteúdo é arquivado para o proprietário da pasta. Os colaboradores que não possuem o conteúdo não podem mais acessá-lo.

## Conteúdo compartilhado próprio em uma pasta não compartilhada

Movimenta o conteúdo de uma pasta compartilhada de sua propriedade para uma pasta não compartilhada.

![Conteúdo compartilhado próprio para uma pasta não compartilhada](../../assets/05_assets_move.png)

**Resultado:** o conteúdo agora não é compartilhado. Os colaboradores da pasta compartilhada não têm mais acesso ao conteúdo.

## Conteúdo não próprio em uma pasta não compartilhada

Movimenta o conteúdo de uma pasta compartilhada de propriedade de outra pessoa para uma pasta não compartilhada.

![Conteúdo não proprietário para uma pasta não compartilhada](../../assets/06_assets_move.png)

**Resultado:** o conteúdo aparece na pasta não compartilhada e é removido da pasta compartilhada. Os colaboradores da pasta compartilhada não têm mais acesso ao conteúdo. O conteúdo é arquivado para o proprietário da pasta compartilhada.

Os proprietários e editores podem mover o conteúdo que não é de sua propriedade, mas os visualizadores não. Se os proprietários e editores moverem o conteúdo, ele não estará disponível em uma pasta compartilhada para nenhum usuário.

## Pasta própria arquivada ou excluída

Arquiva (pela Web) ou exclui (pelo desktop) uma pasta compartilhada de sua propriedade.

![Pasta própria arquivada ou excluída](../../assets/07_assets_move.png)

**Resultado:** a pasta não é compartilhada e é arquivada. Os colaboradores não têm mais acesso à pasta.

## Pasta compartilhada em outra pasta compartilhada

Movimenta uma pasta compartilhada de sua propriedade para outra pasta compartilhada, de sua propriedade ou não.

![Pasta compartilhada para outra pasta compartilhada](../../assets/09_assets_move.png)

**Resultado:** À medida que a pasta é movida para a Pasta 2, ela se torna compartilhada com os novos colaboradores.

## Conteúdo compartilhado em outra pasta compartilhada

Movimenta o conteúdo de uma pasta compartilhada para outra pasta compartilhada.

![Conteúdo compartilhado para outra pasta compartilhada](../../assets/11_assets_move.png)

**Resultado:** o conteúdo é exibido na Pasta 2 e agora é compartilhado com os novos colaboradores. O conteúdo é removido da Pasta 1, e o proprietário o vê como arquivado, enquanto os outros colaboradores não têm mais acesso a ele.

## Conteúdo restaurado no arquivo

Você restaura o conteúdo de um arquivo que pertence a uma pasta compartilhada. Você era o proprietário do conteúdo no momento em que ele foi arquivado.

![Conteúdo restaurado a partir do arquivo](../../assets/12_assets_move.png)

**Resultado:** o conteúdo é restaurado para a pasta compartilhada e todos os colaboradores podem acessá-lo novamente. Se a pasta compartilhada não existir mais, o conteúdo será colocado em uma cópia não compartilhada de sua(s) pasta(s) pai original(is).
