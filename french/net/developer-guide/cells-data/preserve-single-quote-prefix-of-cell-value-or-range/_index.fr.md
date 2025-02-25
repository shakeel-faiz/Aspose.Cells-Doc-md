﻿---
title: Conserver le préfixe de guillemets simples de la valeur ou de la plage Cell
type: docs
weight: 310
url: /fr/net/preserve-single-quote-prefix-of-cell-value-or-range/
---
## **Scénarios d'utilisation possibles**

Lorsque vous mettez une valeur dans la cellule qui comporte une apostrophe ou un guillemet simple, Microsoft Excel la masque, mais lorsque vous sélectionnez la cellule, elle affiche l'apostrophe ou le guillemet simple dans une barre de formule, comme indiqué dans la capture d'écran suivante.

![tâche : image_autre_texte](preserve-single-quote-prefix-of-cell-value-or-range_1.png)

Aspose.Cells masque également l'apostrophe principale ou le guillemet simple comme Microsoft Excel mais il définit le[**Style.QuotePrefix**](https://reference.aspose.com/cells/net/aspose.cells/style/properties/quoteprefix) comme**vrai** pour cette cellule. Si vous définissez un style de cellule vide, alors[**Style.QuotePrefix**](https://reference.aspose.com/cells/net/aspose.cells/style/properties/quoteprefix) devient**faux** de nouveau. Afin de faire face à ce problème, le Aspose.Cells fournit[**StyleFlag.QuotePrefix**](https://reference.aspose.com/cells/net/aspose.cells/styleflag/properties/quoteprefix) propriété, lorsqu'elle est définie**faux** , ensuite[**Style.QuotePrefix**](https://reference.aspose.com/cells/net/aspose.cells/style/properties/quoteprefix)n'est pas du tout mis à jour et son ancienne valeur est conservée. Cela signifie que si l'ancienne valeur de[**Style.QuotePrefix**](https://reference.aspose.com/cells/net/aspose.cells/style/properties/quoteprefix)la propriété était**vrai** , il restera**vrai** et si l'ancienne valeur était**faux** , il restera**faux**.

## **Conserver le préfixe de guillemets simples de la valeur ou de la plage Cell**

 L'exemple de code suivant explique l'utilisation de[**StyleFlag.QuotePrefix**](https://reference.aspose.com/cells/net/aspose.cells/styleflag/properties/quoteprefix)propriété telle que décrite précédemment. Veuillez lire les commentaires à l'intérieur du code et voir la sortie de la console du code ci-dessous pour plus d'aide.

## **Exemple de code**

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Data-PreserveSingleQuotePrefixOfCellValueOrRange.cs" >}}

## **Sortie console**

{{< highlight "java" >}}

Quote Prefix of Cell A1: False

Quote Prefix of Cell A1: True

When StyleFlag.QuotePrefix is False, it means, do not update the value of Cell.Style.QuotePrefix.

Similarly, when StyleFlag.QuotePrefix is True, it means, update the value of Cell.Style.QuotePrefix.

Quote Prefix of Cell A1: True

Quote Prefix of Cell A1: False

{{< /highlight >}}
