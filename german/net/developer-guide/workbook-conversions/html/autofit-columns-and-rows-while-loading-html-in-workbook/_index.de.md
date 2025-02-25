﻿---
title: Spalten und Zeilen automatisch anpassen, während HTML in die Arbeitsmappe geladen wird
type: docs
weight: 120
url: /de/net/autofit-columns-and-rows-while-loading-html-in-workbook/
---
## **Mögliche Nutzungsszenarien**

Sie können Spalten und Zeilen automatisch anpassen, während Sie Ihre HTML-Datei in das Workbook-Objekt laden. Bitte setzen Sie die**[HtmlLoadOptions.AutoFitColsAndRows](https://reference.aspose.com/cells/net/aspose.cells/htmlloadoptions/properties/autofitcolsandrows)** Eigentum zu**wahr**für diesen Zweck.

## **Spalten und Zeilen automatisch anpassen, während HTML in die Arbeitsmappe geladen wird**

 Der folgende Beispielcode lädt zunächst das Beispiel HTML ohne Ladeoptionen in die Arbeitsmappe und speichert es im Format XLSX. Es lädt dann erneut das Beispiel HTML in die Arbeitsmappe, aber dieses Mal lädt es das HTML nach dem Festlegen von**[HtmlLoadOptions.AutoFitColsAndRows](https://reference.aspose.com/cells/net/aspose.cells/htmlloadoptions/properties/autofitcolsandrows)** Eigentum zu**wahr**und speichert es im Format XLSX. Bitte laden Sie beide ausgegebenen Excel-Dateien herunter, dh[Excel-Datei ohne AutoFitColsAndRows ausgeben](outputWithout_AutoFitColsAndRows.xlsx) und[Excel-Datei mit AutoFitColsAndRows ausgeben](outputWith_AutoFitColsAndRows.xlsx) . Der folgende Screenshot zeigt die Wirkung von**[HtmlLoadOptions.AutoFitColsAndRows](https://reference.aspose.com/cells/net/aspose.cells/htmlloadoptions/properties/autofitcolsandrows)**-Eigenschaft in beiden Excel-Ausgabedateien.

![todo: Bild_alt_Text](autofit-columns-and-rows-while-loading-html-in-workbook_1.png)

## **Beispielcode**

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-LoadingSavingConvertingAndManaging-AutoFitColumnsandRowsWhileLoadingHTMLInWorkbook-1.cs" >}}

