﻿---
title: Konvertieren des Arbeitsblatts in SVG in Python
type: docs
weight: 50
url: /de/java/converting-worksheet-to-svg-in-python/
---
## **Aspose.Cells - Konvertieren des Arbeitsblatts in SVG**
Um Worksheet in SVG mit Aspose.Cells for Java in Python zu konvertieren, rufen Sie einfach worksheet auf_zu_svg()-Methode des Converter-Moduls.

**Python Code**

{{< highlight "java" >}}

 saveFormat = self.SaveFormat

workbook = self.Workbook(self.dataDir + "Book1.xls")

# Convert each worksheet into svg format in a single page.

imgOptions = ImageOrPrintOptions()

imgOptions.setSaveFormat(saveFormat.SVG)

imgOptions.setOnePagePerSheet(True)

# Convert each worksheet into svg format

sheetCount = workbook.getWorksheets().getCount()

# for(i=0; i<sheetCount; i++)

for i in range(sheetCount):

sheet = workbook.getWorksheets().get(i)

sr = SheetRender(sheet, imgOptions)

pageCount = sr.getPageCount()

# for (k = 0 k < pageCount k++)

for k in range(pageCount):

# Output the worksheet into Svg image format

sr.toImage(k, self.dataDir + sheet.getName() + ".out.svg")



\# Print message

print "Excel to SVG conversion completed successfully."

{{< /highlight >}}
## **Laufcode herunterladen**
 Download**Konvertieren des Arbeitsblatts in SVG (Aspose.Cells)** von einer der unten genannten Social-Coding-Sites:

- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-Java/releases/tag/Aspose.Cells_Java_for_Python-v1.0)
