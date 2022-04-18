---
title: Accelerate content velocity with AEM style systems
description: Learn how to use AEM Style Systems to empower designers, content authors, and developers in your organization to create and deliver experiences at the speed and scale that your customers expect.
source-git-commit: 8b4f682739e785aa344e5813edd1c41bc639b233
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# Acelere a velocidade do conteúdo com sistemas de estilo AEM

In this article, you learn how to use AEM Style Systems to empower designers, content authors, and developers in your organization to create and deliver experiences at the speed and scale that your customers expect.

## Visão geral

AEM Style Systems tem quatro benefícios principais:

* Template authors can define style classes in the content policy of a component or page
* Content authors are able to select styles to apply to an entire page or when editing a component on a page
* Os componentes e modelos são mais flexíveis ao permitir que os autores renderizem variações visuais alternativas
* A necessidade de desenvolver um componente personalizado e/ou caixas de diálogo complexas para apresentar variações de componentes é reduzida ou totalmente eliminada

## Configuração inicial e uso

A configuração de 5 etapas é muito semelhante a um fluxo de trabalho de desenvolvimento de componente padrão.

| **Liderança** | **Designer** | **Developer / Architect** | **Autor do modelo** | **Autor do conteúdo** |
| --- | --- | --- | --- | --- |
| Determina o conteúdo e os objetivos desse componente | Determina a apresentação visual e experimental do conteúdo | Develops CSS and JS to support experience; defines and provides class names to be used | Configura políticas de modelo para componentes estilizados adicionando nomes de classe CSS definidos por desenvolvedores. Nomes amigáveis devem ser usados para cada estilo. | While authoring pages, applies styles as needed to achieve desired look and feel |

Embora essa seja a configuração inicial, muitos de nossos clientes tiveram agilidade adicional ao simplificar esse processo, por exemplo, ao fazer upload de seu CSS no DAM, o que permite atualizações em estilos sem a necessidade de implantação. Outros clientes têm um conjunto completo de classes de utilitários, o que permite desenvolver componentes e estilos que podem ser aproveitados sem implantação ou desenvolvimento.

Os sistemas de estilos apresentam alguns tipos diferentes:

1. Estilos de layout

   * Alterações multifacetadas no design e layout

   * Used for well-defined and identifiable rendition

1. Exibir estilos
   * Pequenas variações que não alteram a natureza fundamental do estilo

   * Por exemplo, alteração do esquema de cores, fonte, orientação da imagem etc.

1. Estilos informativos

   * Show / hide fields

>[!NOTE]
>
>Para uma demonstração desses recursos, recomendamos assistir ao webinário de sucesso do cliente com Will Brisbane e Joseph Van Buskirk: [https://adobecustomersuccess.adobeconnect.com/pob610c9mffjmp4/](https://adobecustomersuccess.adobeconnect.com/pob610c9mffjmp4/)

## Práticas recomendadas

* Solidificar primeiro o estilo padrão
   * Layout and display of component when dropped on page prior to application of style systems
   * Essa deve ser a representação mais usada
* Try to only show style options that have an effect when possible
   * Se as combinações ineficazes estiverem expostas, certifique-se de que não causam efeitos negativos
   * E.g. A layout style that dictates image position and is accompanied by ineffective display style that control image position
* Optar por estilos de layout em vez de estilos de exibição combinados
   * Reduces number of permutations that must be quality checked
   * Garante o cumprimento dos padrões da marca
   * Simplifies authoring for content authors
   * Ajuda a criar uma identidade de marca de site consistente
* Seja conservador com estilos combinados
   * Em todas as categorias e dentro delas
* Aloque o tempo adequado para testar estilos combinados completamente
   * Ajuda a evitar efeitos indesejáveis
* Minimize o número de opções e permutas de estilo
   * Muitas opções podem levar à falta de consistência da marca para aparência e comportamento
   * Can cause confusion for content authors on which combinations are needed to achieve desired effect
   * Aumenta as permutas que devem ser verificadas por qualidade
* Usar rótulos e categorias de estilo comerciais amigáveis ao usuário
   * &quot;Blue&quot; and &quot;Red&quot; instead of &quot;Primary&quot; and &quot;Secondary
   * &quot;Card&quot; and &quot;Hero&quot; instead of &quot;Variation A&quot; and &quot;Variation B&quot;
   * Tal pode ser mais generalista para alguns clientes; a equipe de design, a equipe de negócios e a equipe de conteúdo estão familiarizadas com as cores primárias e secundárias ou com que variações estão testando. Mas, para a flexibilidade e para qualquer potencial de mudanças futuras, a utilização de termos específicos pode ser mais eficiente.

## Capturas de chave

Os sistemas de estilos reduzem a necessidade de caixas de diálogo complexas, mas não são uma substituição de caixa de diálogo. They help simplify things but there may be some cases where you want to use component properties or dialog rather than creating a style system for it.

Eles podem simplificar processos de uma perspectiva de desenvolvimento. Você pode obter várias aparências do mesmo conteúdo com um sistema de estilos. Da mesma forma, de uma perspectiva de criação, em vez de treinar autores e autores que precisam lembrar qual componente usar em qual palácio, você pode acelerar a velocidade de criação.

Things are simply cleaner. A HTML dentro dos componentes principais é altamente detalhada. Fazer tudo isso no nível de CSS torna as criações do componente mais rápidas e o código também é mais limpo.

Por fim, o uso de Sistemas de Estilo é mais arte do que ciência. As we discussed, there are a number of best practices, but you will have flexibility in how customize your organization&#39;s setup.

Para obter mais informações, consulte nossa [Webinar de sucesso do cliente](https://adobecustomersuccess.adobeconnect.com/pob610c9mffjmp4/) com Will Brisbane e Joseph Van Buskirk