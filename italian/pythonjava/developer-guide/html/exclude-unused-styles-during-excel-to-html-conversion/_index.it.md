﻿---
title: Escludi stili inutilizzati durante la conversione da Excel a HTML
type: docs
weight: 30
url: /it/python-java/exclude-unused-styles-during-excel-to-html-conversion/
---
## **Escludi stili inutilizzati durante la conversione da Excel a HTML**
Microsoft I file Excel possono contenere molti stili inutilizzati. Quando questi file vengono esportati nel formato HTML, vengono esportati anche gli stili inutilizzati. Ciò comporta l'aumento delle dimensioni dell'output HTML. Aspose.Cells for Python via Java supporta l'esclusione di questi stili durante la conversione del file Excel in HTML. Per questo, API fornisce il[HtmlSaveOptions.ExcludeUnusedStyles](https://reference.aspose.com/cells/python/asposecells.api/htmlsaveoptions#ExcludeUnusedStyles)proprietà. Impostazione del valore di[HtmlSaveOptions.ExcludeUnusedStyles](https://reference.aspose.com/cells/python/asposecells.api/htmlsaveoptions#ExcludeUnusedStyles) proprietà a**Vero** escluderà tutti gli stili inutilizzati dall'output HTML.

Lo screenshot seguente mostra gli stili inutilizzati nel file HTML che verranno rimossi impostando il valore di[HtmlSaveOptions.ExcludeUnusedStyles](https://reference.aspose.com/cells/python/asposecells.api/htmlsaveoptions#ExcludeUnusedStyles) proprietà a**Vero**.

![cose da fare:immagine_alt_testo](HtmlSaveOptions-Exclude-Unused-Styles.png)

Il codice di esempio seguente illustra la rimozione degli stili inutilizzati durante la conversione da Excel a HTML.

{{< gist "aspose-cells-gists" "32e50c6aabc547111966569f3fd39694" "HTML-ExcludeUnusedStylesInExcelToHTML.py" >}}
