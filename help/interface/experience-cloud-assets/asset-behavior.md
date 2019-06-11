---
description: Regras sobre como as pastas compartilhadas se comportam quando são movidas, excluídas ou restauradas.
keywords: compartilhamento de ativos; Creative Cloud; principais serviços
seo-description: Regras sobre como as pastas compartilhadas se comportam quando são movidas, excluídas ou restauradas.
seo-title: Comportamento das pastas compartilhadas
solution: Experience Cloud
title: Comportamento das pastas compartilhadas
uuid: 86348401-f 4 b 1-4 efe-acd 1-7 e 73 a 7030
translation-type: tm+mt
source-git-commit: af5339fe58ce884345804574c209907d6504a483

---


# Comportamento das pastas compartilhadas

Regras sobre como as pastas compartilhadas se comportam quando são movidas, excluídas ou restauradas.

>[!NOTE]
>
>As pastas e os ativos compartilhados da Experience Cloud são espelhados na área de trabalho da Creative Cloud em uma relação 1:1. Se um usuário da Experience Cloud mudar uma pasta (excluir, adicionar ou remover o compartilhamento), a ação será espelhada no desktop da Creative Cloud e na Web. Assim, se o compartilhamento de uma pasta for cancelado, a pasta e os ativos serão excluídos da máquina local. Quando o compartilhamento é removido, a pasta e seu conteúdo são movidos para a lixeira do computador local, onde é possível restaurá-los manualmente para a máquina.

## Pasta não compartilhada na pasta compartilhada {#section_A9BAC1A244A246A984AC62660E61E0C0}

Você move uma pasta não compartilhada em uma pasta compartilhada:

![](assets/01_assets_move.png)

**Resultado**: ambas as pastas se tornam compartilhadas.

## Pasta compartilhada na pasta não compartilhada {#section_8BA83001DCEC4CF084B980C4A660F59A}

Você move uma pasta compartilhada para uma pasta não compartilhada.

![](assets/02_assets_move.png)

**Resultado**: a pasta não compartilhada permanece não compartilhada. A pasta compartilhada permanece compartilhada.

## Conteúdo da pasta não compartilhada na pasta compartilhada {#section_2941ED0DC52E4573AC1AB4C22313DD8E}

Você move o conteúdo de uma pasta não compartilhada em uma pasta compartilhada.

![](assets/03_assets_move.png)

**Resultado:** o conteúdo agora é compartilhado e todos os colaboradores podem visualizá-lo. O armazenamento aumenta de acordo com o tamanho do conteúdo.

## Conteúdo compartilhado arquivado e excluído {#section_5210D5F4943A44D0BA675D8EB4EAE20F}

Você arquiva ou exclui o conteúdo de uma pasta compartilhada.

![](assets/04_assets_move.png)

**Resultado:** o conteúdo é arquivado para o proprietário da pasta. Os colaboradores que não possuem o conteúdo não podem mais acessá-lo.

## Conteúdo compartilhado próprio para uma pasta não compartilhada {#section_3810A364B67E4B8C9CA244BC52BF91BB}

Você move o conteúdo de uma pasta compartilhada que possui em uma pasta não compartilhada.

![](assets/05_assets_move.png)

**Resultado:** o conteúdo agora não é compartilhado. Os colaboradores da pasta compartilhada não têm mais acesso ao conteúdo.

## Conteúdo não próprio para uma pasta não compartilhada {#section_310766EBF0DC4C0BB4AB3E8A4DAEBE07}

Você move o conteúdo da pasta compartilhada de propriedade de outra pessoa para uma pasta não compartilhada.

![](assets/06_assets_move.png)

**Resultado:** o conteúdo aparece na pasta não compartilhada e é removido da pasta compartilhada. Os colaboradores da pasta compartilhada não têm mais acesso ao conteúdo. O conteúdo é arquivado para o proprietário da pasta compartilhada.

Os proprietários e editores podem mover o conteúdo que não é de sua propriedade, mas os visualizadores não. Se os proprietários e editores moverem o conteúdo, ele não estará disponível em uma pasta compartilhada para um usuário.

## Pasta proprietária arquivada ou excluída {#section_B314B13512A5409C87C49DFDB7602E14}

Você arquiva (pela Web) ou exclui (pelo desktop) uma pasta compartilhada de sua propriedade.

![](assets/07_assets_move.png)

**Resultado:** a pasta não é compartilhada e é arquivada. Os colaboradores não têm mais acesso à pasta.

## Pasta compartilhada em outra pasta compartilhada {#section_0A3F203D048D4D1586E9850DC92C51E9}

Você move uma pasta compartilhada de sua propriedade para outra pasta compartilhada de sua propriedade ou não.

![](assets/09_assets_move.png)

**Resultado:** quando a pasta é movida para a Pasta 2, ela passa a ser compartilhada com os novos colaboradores.

## Conteúdo compartilhado para outra pasta compartilhada {#section_69F6C312792A4CD2831BD14A340F850E}

Você move conteúdo de uma pasta compartilhada para outra pasta compartilhada.

![](assets/11_assets_move.png)

**Resultado:** o conteúdo é exibido na Pasta 2 e agora é compartilhado com os novos colaboradores. O conteúdo é removido da Pasta 1 e o proprietário o visualiza como arquivado, ao passo que outros colaboradores não têm mais acesso a ele.

## Conteúdo restaurado do arquivamento {#section_DEA990B3581741F89FBB81D18C2AB449}

Você restaura o conteúdo de um arquivo que pertence a uma pasta compartilhada. Você se torna proprietário do conteúdo no momento em que ele foi arquivado.

![](assets/12_assets_move.png)

**Resultado:** o conteúdo é restaurado para a pasta compartilhada e todos os colaboradores podem acessá-lo novamente. Se a pasta compartilhada não existir mais, o conteúdo será colocado em uma cópia não compartilhada da pasta pai original.
