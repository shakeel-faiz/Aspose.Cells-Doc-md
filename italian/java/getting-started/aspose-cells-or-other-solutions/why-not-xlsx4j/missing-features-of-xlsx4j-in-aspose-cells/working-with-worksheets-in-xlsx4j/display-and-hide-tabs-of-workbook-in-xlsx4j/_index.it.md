﻿---
title: Mostra e nascondi le schede della cartella di lavoro in xlsx4j
type: docs
weight: 40
url: /it/java/display-and-hide-tabs-of-workbook-in-xlsx4j/
---
## **Aspose.Cells - Mostra e nascondi le schede della cartella di lavoro**
Aspose.Cells fornisce una classe, Workbook, che rappresenta un file Excel Microsoft. La classe Workbook fornisce un'ampia gamma di proprietà e metodi per la gestione di un file Excel. Per controllare la visibilità delle schede in un file Excel, gli sviluppatori possono utilizzare il metodo setShowTabs della classe Workbook.

**Java**

{{< highlight "java" >}}

 //Instantiating a Workbook object by excel file path

Workbook workbook = new Workbook(dataDir + "book1.xls");

//Hiding the tabs of the Excel file

workbook.getSettings().setShowTabs(false);

//Saving the modified Excel file in default (that is Excel 2003) format

workbook.save(dataDir + "AsposeHideTabs.xls");

// ===============================================================

//Displaying the tabs of the Excel file

workbook.getSettings().setShowTabs(true);

//Saving the modified Excel file in default (that is Excel 2003) format

workbook.save(dataDir + "AsposeDisplayTabs.xls");

{{< /highlight >}}
## **Scarica il codice in esecuzione**
- [Git Hub](https://github.com/aspose-cells/Aspose.Cells-for-Java/releases/tag/Aspose.Cells_Java_for_Xlsx4j-v1.0.0)
## **Scarica il codice di esempio**
- [Git Hub](https://github.com/aspose-cells/Aspose.Cells-for-Java/blob/master/Plugins/Aspose_Cells_Java_for_Xlsx4j/src/main/java/com/aspose/cells/examples/asposefeatures/worksheets/displayandhidetabs/AsposeDisplayAndHideTabs.java)
