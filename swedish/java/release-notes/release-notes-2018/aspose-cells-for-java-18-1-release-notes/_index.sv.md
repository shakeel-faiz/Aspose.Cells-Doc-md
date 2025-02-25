﻿---
title: Aspose.Cells for Java 18.1 Release Notes
type: docs
weight: 120
url: /sv/java/aspose-cells-for-java-18-1-release-notes/
---
{{% alert color="primary" %}} 

Den här sidan innehåller utgåvor för Aspose.Cells for Java 18.1.

{{% /alert %}} 

|**Nyckel**|**Sammanfattning**|**Kategori**|
|:- |:- |:- |
|CELLSJAVA-42493|Ange ett alternativ för att bestämma om arbetsboksegenskaper ska exporteras (överordnat problem-id: CELLSJAVA-42471)|Ny funktion|
|CELLSJAVA-42491|Ge ett alternativ för att bestämma om dokumentegenskaper ska exporteras (överordnat ärende-id: CELLSJAVA-42471)|Ny funktion|
|CELLSJAVA-42498|Skapa ett PdfBookmarkEntry för ett diagramblad|Ny funktion|
|CELLSJAVA-42464|Fix krävs för alla ActiveX-kontroller (överordnat problem-id: CELLSJAVA-42442)|Förbättring|
|CELLSJAVA-42490|Uteslut oanvända stilar när du exporterar Excel-fil till HTML (förälder ärende-id: CELLSJAVA-42471)|Förbättring|
|CELLSJAVA-42473|Delar av bilderna är trunkerade eller saknas och de matchar inte originalbilderna|Insekt|
|CELLSJAVA-42469|Bilden sticker ut från formen i utgången PDF|Insekt|
|CELLSJAVA-42461|Elementformen är felaktig i utgången HTML|Insekt|
|CELLSJAVA-42495|Excel till HTML - Radbrytning av text ignoreras|Insekt|
|CELLSJAVA-42489|XLSB-filen blir korrupt efter att ha öppnats och sparats|Insekt|
|CELLSJAVA-42487|HTML utgångsavvikelse - Problem med mellanslag|Insekt|
|CELLSJAVA-42471|Irrelevant data inkluderas när du sparar till HTML|Insekt|
|CELLSJAVA-42467|XLSB skadad efter att ha sparats på nytt|Insekt|
|CELLSJAVA-42488|15-siffriga nummer stämmer inte överens med vad som finns i MS Excel|Insekt|
|CELLSJAVA-42499|Marginaler och layoutskillnader vid jämförelse av utdata PDF (av Aspose.Cells) med MS Excel genererad PDF|Insekt|
|CELLSJAVA-42486|Funktionen fungerar inte i Java - ResultSet|Insekt|
|CELLSJAVA-42500|NullPointerException inträffar när MS Excel-filen laddas|Undantag|
## **Offentlig API och bakåtinkompatibla ändringar**
Följande är en lista över alla ändringar som gjorts för allmänheten API, såsom tillagda, bytt namn, borttagna eller utfasade medlemmar samt alla icke-bakåtkompatibla ändringar som gjorts till Aspose.Cells for Java. Om du har frågor om någon ändring som anges, vänligen ta upp den på supportforumet Aspose.Cells.
### **Lägger till egenskapen LoadOptions.ParsingPivotCachedRecords**
Indikerar om tolkning av pivotcachade poster när filen laddas. Standardvärdet är falskt. Gäller endast filformaten Excel Xlsx, Xltx, Xltm, Xlsm och Xlsb.
### **Lägger till egenskapen HtmlSaveOptions.ExcludeUnusedStyles**
Anger om oanvända stilar exkluderas. Standardvärdet är falskt. Om du vill importera filen HTML eller Mht till Excel, behåll standardvärdet.
### **Lägger till egenskapen HtmlSaveOptions.ExportDocumentProperties**
Anger om dokumentegenskaper exporteras. Standardvärdet är sant. Om du vill importera filen HTML eller Mht till Excel, behåll standardvärdet.
### **Lägger till egenskapen HtmlSaveOptions.ExportWorksheetProperties**
Anger om kalkylbladsegenskaper exporteras. Standardvärdet är sant. Om du vill importera filen HTML eller Mht till Excel, behåll standardvärdet.
### **Lägger till egenskapen HtmlSaveOptions.ExportWorkbookProperties**
Anger om arbetsboksegenskaper exporteras. Standardvärdet är sant. Om du vill importera filen HTML eller Mht till Excel, behåll standardvärdet.
### **Lägger till metoden PivotTable.GetChildren().**
Får barnens pivottabeller som använder denna pivottabelldata som datakälla.
