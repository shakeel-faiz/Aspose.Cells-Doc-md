﻿---
title: Установить область печати
type: docs
weight: 40
url: /ru/java/set-print-area/
---
## **Aspose.Cells - Установить область печати**
По умолчанию только область печати включает все области рабочего листа, содержащие данные. Разработчики могут установить определенную область печати рабочего листа.

Чтобы выбрать конкретную область печати, используйте кнопку[Настройка страницы](/java/pagesetup)метод setPrintArea класса. Назначьте этому свойству диапазон ячеек, определяющий область печати.

**Java**

{{< highlight "java" >}}

 // Instantiating a Workbook object

Workbook workbook = new Workbook();

// Accessing the first worksheet in the Workbook file

WorksheetCollection worksheets = workbook.getWorksheets();

Worksheet sheet = worksheets.get(0);

// Obtaining the reference of the PageSetup of the worksheet

PageSetup pageSetup = sheet.getPageSetup();

// Specifying the cells range (from A1 cell to F20 cell) of the print area

pageSetup.setPrintArea("A1:F20");

{{< /highlight >}}
## **Apache POI SS — HSSF XSSF — установка области печати**
Метод Workbook.setPrintArea доступен для установки свойств страницы области печати.

**Java**

{{< highlight "java" >}}

 Workbook wb = new HSSFWorkbook();

Sheet sheet = wb.createSheet("Sheet1");

//sets the print area for the first sheet

wb.setPrintArea(0, "$A$1:$C$2");

//Alternatively:

wb.setPrintArea(

        0, //sheet index

        0, //start column

        1, //end column

        0, //start row

        0  //end row

);

{{< /highlight >}}
## **Скачать рабочий код**
- [Гитхаб](https://github.com/aspose-cells/Aspose.Cells-for-Java/releases/tag/Aspose.Cells_Java_for_Apache_POI_SS-v1.0.0)
## **Скачать пример кода**
- [Гитхаб](https://github.com/aspose-cells/Aspose.Cells-for-Java/tree/master/Plugins/Aspose_Cells_for_Apache_POI/Aspose-Cells-for-Apache-POI-(Maven)/src/main/java/com/aspose/cells/examples/featurescomparison/workbook/setprintarea)

{{% alert color="primary" %}} 

 Для получения более подробной информации посетите[Настройка параметров печати](/cells/ru/java/page-setup-features/#setting-print-options).

{{% /alert %}}
