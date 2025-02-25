﻿---
title: Регулировка высоты столбца строки в xlsx4j
type: docs
weight: 50
url: /ru/java/row-column-height-adjustment-in-xlsx4j/
---
## **Aspose.Cells - Регулировка высоты столбца строки**
Можно установить высоту одной строки, вызвав метод setRowHeight коллекции Cells. Метод setRowHeight принимает следующие параметры:

- **Индекс строки**, индекс строки, высоту которой вы меняете.
- **Высота строки**, высота строки, применяемая к строке.

Установите ширину столбца, вызвав метод setColumnWidth коллекции Cells. Метод setColumnWidth принимает следующие параметры:

- **Индекс столбца**, индекс столбца, ширину которого вы меняете.
- **Ширина колонки**, желаемая ширина столбца.

**Java**

{{< highlight "java" >}}

 //Instantiating a Workbook object

Workbook workbook = new Workbook();

//Accessing the first worksheet in the Excel file

Worksheet worksheet = workbook.getWorksheets().get(0);

Cells cells = worksheet.getCells();

//Setting the height of all rows in the worksheet to 8

worksheet.getCells().setStandardHeight(8f);

//Setting the height of the second row to 40

cells.setRowHeight(1, 40);



//Setting the width of the second column to 17.5

cells.setColumnWidth(1, 17.5);

{{< /highlight >}}
## **xlsx4j — регулировка высоты столбца строки**
Row.setHt используется для установки нестандартной высоты строк с помощью xlsx4j. setCustomHeight должно быть установлено в TRUE.

**Java**

{{< highlight "java" >}}

 SpreadsheetMLPackage pkg = SpreadsheetMLPackage.createPackage();

WorksheetPart sheet = pkg.createWorksheetPart(new PartName("/sheet1.xml"), "Sheet1", 1);

CTSheetFormatPr format = Context.getsmlObjectFactory().createCTSheetFormatPr();

format.setDefaultRowHeight(5);

format.setCustomHeight(Boolean.TRUE);

sheet.getJaxbElement().setSheetFormatPr(format);

SheetData sheetData = sheet.getJaxbElement().getSheetData();

Row row = Context.getsmlObjectFactory().createRow();

row.setHt(66.0);

row.setCustomHeight(Boolean.TRUE);

row.setR(1L);

Cell cell1 = Context.getsmlObjectFactory().createCell();

cell1.setV("1234");

row.getC().add(cell1);

Cell cell2 = Context.getsmlObjectFactory().createCell();

cell2.setV("56");

row.getC().add(cell2);

sheetData.getRow().add(row);

{{< /highlight >}}
## **Скачать рабочий код**
- [Гитхаб](https://github.com/aspose-cells/Aspose.Cells-for-Java/releases/tag/Aspose.Cells_Java_for_Xlsx4j-v1.0.0)
## **Скачать пример кода**
- [Гитхаб](https://github.com/aspose-cells/Aspose.Cells-for-Java/tree/master/Plugins/Aspose_Cells_Java_for_Xlsx4j/src/main/java/com/aspose/cells/examples/featurescomparison/worksheet/adjustheight)

{{% alert color="primary" %}} 

 Для получения более подробной информации посетите[Настройка высоты строки и ширины столбца](/java/adjusting-row-height-and-volumn-width).

{{% /alert %}}
