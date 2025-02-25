﻿---
title: Aspose.Cells for Node.js via Java 22.11 Release Notes
type: docs
weight: 2
url: /sv/nodejs-java/aspose-cells-for-node-js-via-java-22-11-release-notes/
---
{{% alert color="primary" %}}

 Den här sidan innehåller release notes för[Aspose.Cells for Node.js via Java 22.11](https://releases.aspose.com/cells/nodejs/new-releases/aspose.cells-for-node.js-via-java-22.11/).

{{% /alert %}}

|**Nyckel**|**Sammanfattning**|**Kategori**|
|:- |:- |:- |
|CELLSJAVA-44888|"+" och "-" försvann efter konvertering - Excel till HTML rendering|
|CELLSJAVA-44775|Diagrametiketter överlappade i diagram till bildrendering|
|CELLSJAVA-44882|Tabell-till-bild-rendering - En av etiketterna finns inuti munkdiagrammet|
|CELLSJAVA-44943|XLSX till PDF: Diagrametiketter renderade inte korrekt|
|CELLSJAVA-44928|XLS till PDF: Otillräckliga data för en bild|
|CELLSJAVA-44910|Konvertera Excel till HTML resulterar i tusentals liknande små bilder|
|CELLSJAVA-44944|Ändra storlek på tabeller ändra formateringen av celler|
|CELLSJAVA-44948| Bilder kan inte visas i arket när HTML konverteras till Excel|
|CELLSJAVA-44908|Undantag "java.lang.OutOfMemoryError: Java heap space" när stora XLSB filer laddas|
|CELLSJAVA-44929|Regression: "java.lang.NullPointerException" på Workbook.calculateFormula()|
|CELLSJAVA-44927|Undantag "java.lang.IndexOutOfBoundsException: Index: 5, Storlek: 5" vid konvertering av Excel-fil till HTML|
|CELLSJAVA-44939|Fel "java.lang.StringIndexOutOfBoundsException: Strängindex utanför intervallet: 0" vid försök att läsa en Excel-fil|

## **Offentlig API och bakåtinkompatibla ändringar**

Följande är en lista över alla ändringar som gjorts för allmänheten API, såsom tillagda, bytt namn, borttagna eller utfasade medlemmar samt alla icke-bakåtkompatibla ändringar som gjorts till Aspose.Cells for Java. Om du har frågor om någon ändring som anges, vänligen ta upp den på supportforumet Aspose.Cells.

### **Lägger till egenskapen Cell.IsDynamicArrayFormula**

Anger om cellens formel är dynamisk matrisformel (sant) eller äldre matrisformel (falsk).

### **Föråldrade egendomen SparklineGroup.SparklineCollection och lägger till egendomen SparklineGroup.Sparklines**

Använd egenskapen SparklineGroup.Sparklines istället.

### **Föråldrade egendomen Worksheet.SparklineGroupCollection och lägger till egenskapen Worksheet.SparklineGroups**

Använd egenskapen Worksheet.SparklineGroups istället.