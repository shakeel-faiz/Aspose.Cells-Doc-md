﻿---
title: Ausblenden von Zeilen und Spalten im Arbeitsblatt
type: docs
weight: 60
url: /de/net/hiding-rows-and-columns-in-worksheet/
---
## **Aspose.Cells – Ausblenden von Zeilen und Spalten im Arbeitsblatt**
**C#**

{{< highlight "cs" >}}

 Workbook workbook = new Workbook();

//Accessing the first worksheet in the Excel file

Worksheet worksheet = workbook.Worksheets[0];

worksheet.Cells["A1"].PutValue("1");

worksheet.Cells["A2"].PutValue("2");

worksheet.Cells["B1"].PutValue(11);

//Hiding the 1st row of the worksheet

worksheet.Cells.HideRow(0);

//Hiding the 1st column of the worksheet

worksheet.Cells.HideColumn(0);

//Saving the modified Excel file

workbook.Save("Output-HideRowsandColumns.xls");

{{< /highlight >}}
## **NPOI - HSSF XSSF - Ausblenden von Zeilen und Spalten im Arbeitsblatt**
**C#**

{{< highlight "cs" >}}

 HSSFWorkbook hssfworkbook = new HSSFWorkbook();

ISheet s = hssfworkbook.CreateSheet("Sheet1");

IRow r1 = s.CreateRow(0);

IRow r2 = s.CreateRow(1);

//hide Row 0

r1.ZeroHeight = true;

//hide column C

s.SetColumnHidden(0, true);

FileStream file = new FileStream(@"HidingRowsandColumn(NPOI).xls", FileMode.Create);

hssfworkbook.Write(file);

file.Close();


{{< /highlight >}}
## **Laufcode herunterladen**
 Download**Ausblenden von Zeilen und Spalten im Arbeitsblatt** Bilden Sie eine der unten genannten Social-Coding-Sites:

- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-.NET/releases/download/Aspose.Cells_Vs_NPOI_HWPF_and_XWPF_v1.3/Hiding.Rows.and.Columns.zip)

{{% alert color="primary" %}} 

 Weitere Informationen finden Sie unter[Arbeiten mit Arbeitsblättern](/cells/de/net/working-with-worksheets-in-npoi-and-aspose-cells/).

{{% /alert %}}
