﻿---
title: Ricampionamento delle immagini aggiunte - Conversione da Excel a PDF
type: docs
weight: 150
url: /it/net/resampling-added-images-excel-to-pdf-conversion/
---
{{% alert color="primary" %}}

Mentre si lavora con grandi file Excel Microsoft con molte immagini, potrebbe essere necessario comprimere le immagini che sono state aggiunte per ridurre le dimensioni del file di output PDF e migliorare le prestazioni complessive della conversione. Aspose.Cells supporta il ricampionamento delle immagini aggiunte per ridurre le PDF dimensioni del file di output e migliorare in qualche modo le prestazioni.

{{% /alert %}}

Vedere il seguente codice di esempio che descrive come eseguire l'attività utilizzando Aspose.Cells API. L'esempio converte un file Excel Microsoft in un file PDF durante la compressione delle immagini nel file.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Articles-ResamplingAddedImages-1.cs" >}}

{{% alert color="primary" %}}

 Usando il[**SetImageResample**](https://reference.aspose.com/cells/net/aspose.cells/pdfsaveoptions/methods/setimageresample)L'opzione riduce al minimo la dimensione dell'output PDF ma potrebbe influire leggermente sulla qualità dell'immagine.

{{% /alert %}} {{% alert color="primary" %}}

Se il tuo foglio di calcolo contiene formule, è meglio chiamare[**Workbook.CalculateFormula()**](https://reference.aspose.com/cells/net/aspose.cells/workbook/methods/calculateformula)appena prima di eseguire il rendering del foglio di calcolo nel formato PDF. In questo modo si assicurerà che i valori dipendenti dalla formula vengano ricalcolati e che i valori corretti vengano visualizzati in PDF.

{{% /alert %}}
