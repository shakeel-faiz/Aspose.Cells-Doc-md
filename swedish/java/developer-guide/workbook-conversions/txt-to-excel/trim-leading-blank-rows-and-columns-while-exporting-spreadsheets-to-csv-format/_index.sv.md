﻿---
title: Trimma ledande tomma rader och kolumner samtidigt som du exporterar kalkylblad till formatet CSV
type: docs
weight: 50
url: /sv/java/trim-leading-blank-rows-and-columns-while-exporting-spreadsheets-to-csv-format/
---
## **Möjliga användningsscenarier**

Ibland har din Excel- eller CSV-fil ledande tomma kolumner eller rader. Tänk till exempel på den här linjen

{{< highlight "java" >}}

 ,,,data1,data2

{{< /highlight >}}

Här är de tre första cellerna eller kolumnerna tomma. När du öppnar en sådan CSV-fil i Microsoft Excel, kasserar Microsoft Excel dessa inledande tomma rader och kolumner.

 Som standard kasserar Aspose.Cells inte inledande tomma kolumner och rader när du sparar, men om du vill ta bort dem precis som Microsoft Excel gör, ger Aspose.Cells**[TxtSaveOptions.TrimLeadingBlankRowAndColumn](https://reference.aspose.com/cells/java/com.aspose.cells/txtsaveoptions#TrimLeadingBlankRowAndColumn)** fast egendom. Vänligen ställ in den på**Sann**och sedan kommer alla de tomma raderna och kolumnerna att slängas när du sparar.

{{% alert color="primary" %}}

 Före lanseringen av Aspose.Cells for .NET 20.4 var standardvärdet för**[TxtSaveOptions.TrimLeadingBlankRowAndColumn](https://reference.aspose.com/cells/java/com.aspose.cells/txtsaveoptions#TrimLeadingBlankRowAndColumn)** var**falsk** . Sedan versionen 20.4 har standardvärdet på**[TxtSaveOptions.TrimLeadingBlankRowAndColumn](https://reference.aspose.com/cells/java/com.aspose.cells/txtsaveoptions#TrimLeadingBlankRowAndColumn)** är**Sann.**

{{% /alert %}}

## **Trimma ledande tomma rader och kolumner samtidigt som du exporterar kalkylblad till formatet CSV**

 Följande exempelkod laddar källexcel-filen som har två ledande tomma kolumner. Den sparar först excel-filen i CSV-format utan några ändringar och sedan ställer den in**[TxtSaveOptions.TrimLeadingBlankRowAndColumn](https://reference.aspose.com/cells/java/com.aspose.cells/txtsaveoptions#TrimLeadingBlankRowAndColumn)** egendom till**Sann** och sparar den igen. Skärmdumpen visar[source excel-fil](sampleTrimBlankColumns.xlsx), [utgång CSV fil utan trimning](outputWithoutTrimBlankColumns.csv), och den[utgång CSV fil med trimning](outputTrimBlankColumns.csv).

![todo:image_alt_text](trim-leading-blank-rows-and-columns-while-exporting-spreadsheets-to-csv-format_1.png)

## **Exempelkod**

{{< gist "aspose-cells-gists" "5876dc77e47649b66bdb5deefb4b5639" "Examples-src-main-java-com-aspose-cells-examples-loading_saving-TrimBlankRowsAndColsWhileExportingSpreadsheetsToCSVFormat-TrimBlankRowsAndColsWhileExportingSpreadsheetsToCSVForm.Java" >}}
