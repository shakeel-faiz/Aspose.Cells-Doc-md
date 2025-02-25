﻿---
title: Limiter le nombre de pages générées - Conversion Excel à PDF
type: docs
weight: 180
url: /fr/net/limit-the-number-of-pages-generated-excel-to-pdf-conversion/
---
{{% alert color="primary" %}}

Parfois, vous souhaitez imprimer une plage de pages dans un fichier de sortie PDF. Aspose.Cells a la capacité de définir une limite sur le nombre de pages générées lors de la conversion d'une feuille de calcul Excel au format de fichier PDF.

{{% /alert %}}

## **Limiter le nombre de pages générées**

L'exemple suivant montre comment rendre une plage de pages (3 et 4) dans un fichier Excel Microsoft en PDF.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Articles-LimitNumberOfPagesGenerated-1.cs" >}}

{{% alert color="primary" %}}

 Si la feuille de calcul contient des formules, il est préférable d'appeler[**Workbook.CalculateFormula()**](https://reference.aspose.com/cells/net/aspose.cells/workbook/methods/calculateformula) juste avant de le rendre à PDF. Cela garantit que les valeurs dépendantes de la formule sont recalculées et que les valeurs correctes sont rendues dans le fichier de sortie.

{{% /alert %}}
