﻿---
title: Escludi stili inutilizzati durante la conversione da Excel a HTML
type: docs
weight: 30
url: /it/java/exclude-unused-styles-during-excel-to-html-conversion/
---
## **Possibili scenari di utilizzo**

Microsoft Il file Excel può contenere molti stili inutilizzati. Quando si esporta il file Excel nel formato HTML, vengono esportati anche questi stili inutilizzati. Ciò può aumentare la dimensione di HTML. È possibile escludere gli stili inutilizzati durante la conversione del file Excel in HTML utilizzando il[**HtmlSaveOptions.ExcludeUnusedStyles**](https://reference.aspose.com/cells/java/com.aspose.cells/htmlsaveoptions#ExcludeUnusedStyles)proprietà. Quando lo imposti**VERO**, tutti gli stili inutilizzati sono esclusi dall'output HTML. Lo screenshot seguente mostra uno stile inutilizzato di esempio all'interno dell'output HTML.

![cose da fare:immagine_alt_testo](exclude-unused-styles-during-excel-to-html-conversion_1.png)

## **Escludi stili inutilizzati durante la conversione da Excel a HTML**

Il codice di esempio seguente crea una cartella di lavoro e crea anche uno stile denominato inutilizzato. Dal momento che il[**HtmlSaveOptions.ExcludeUnusedStyles**](https://reference.aspose.com/cells/java/com.aspose.cells/htmlsaveoptions#ExcludeUnusedStyles)è impostato per**VERO**, quindi questo stile con nome inutilizzato non verrà esportato in[uscita HTML](61767781.zip). Ma se lo imposti**falso**, allora questo stile inutilizzato sarà presente all'interno dell'output HTML che puoi quindi vedere nel markup HTML come mostrato nello screenshot sopra.

## **Codice d'esempio**

{{< gist "aspose-cells-gists" "5876dc77e47649b66bdb5deefb4b5639" "HTML-ExcludeUnusedStylesInExcelToHTML.java" >}}
