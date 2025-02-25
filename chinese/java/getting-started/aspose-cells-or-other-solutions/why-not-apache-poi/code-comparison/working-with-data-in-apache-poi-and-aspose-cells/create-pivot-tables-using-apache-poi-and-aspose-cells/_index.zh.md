﻿---
title: 使用 Apache POI 和 Aspose.Cells 创建数据透视表
type: docs
weight: 40
url: /zh/java/create-pivot-tables-using-apache-poi-and-aspose-cells/
---
## **Aspose.Cells - 创建数据透视表**
使用 Aspose.Cells 创建数据透视表：

1. 使用 Cell 对象的 setValue 方法将一些数据添加到工作表单元格。您还可以使用已填充数据的模板文件。数据将用作数据透视表的数据源。
1. 通过调用 PivotTableCollection 添加方法（封装在 {{Worksheet }} 对象中）向工作表添加数据透视表。
1. 通过传递其索引从 PivotTableCollection 集合访问新的 PivotTable 对象。

**Java**

{{< highlight "java" >}}

 // Instantiating a Workbook object

Workbook workbook = new Workbook();

// Obtaining the reference of the newly added worksheet

Worksheet sheet = workbook.getWorksheets().get(0);

sheet.setName("PivotTable");

Cells cells = sheet.getCells();

// Setting the value to the cells

Cell cell = cells.get("A1");

cell.setValue("Sport");

cell = cells.get("B1");

cell.setValue("Quarter");

cell = cells.get("C1");

cell.setValue("Sales");

cell = cells.get("A2");

cell.setValue("Golf");

cell = cells.get("A3");

cell.setValue("Golf");

cell = cells.get("A4");

cell.setValue("Tennis");

cell = cells.get("A5");

cell.setValue("Tennis");

cell = cells.get("A6");

cell.setValue("Tennis");

cell = cells.get("A7");

cell.setValue("Tennis");

cell = cells.get("A8");

cell.setValue("Golf");

cell = cells.get("B2");

cell.setValue("Qtr3");

cell = cells.get("B3");

cell.setValue("Qtr4");

cell = cells.get("B4");

cell.setValue("Qtr3");

cell = cells.get("B5");

cell.setValue("Qtr4");

cell = cells.get("B6");

cell.setValue("Qtr3");

cell = cells.get("B7");

cell.setValue("Qtr4");

cell = cells.get("B8");

cell.setValue("Qtr3");

cell = cells.get("C2");

cell.setValue(1500);

cell = cells.get("C3");

cell.setValue(2000);

cell = cells.get("C4");

cell.setValue(600);

cell = cells.get("C5");

cell.setValue(1500);

cell = cells.get("C6");

cell.setValue(4070);

cell = cells.get("C7");

cell.setValue(5000);

cell = cells.get("C8");

cell.setValue(6430);

PivotTableCollection pivotTables = sheet.getPivotTables();

// Adding a PivotTable to the worksheet

int index = pivotTables.add("=A1:C8", "E3", "PivotTable1");

// Accessing the instance of the newly added PivotTable

PivotTable pivotTable = pivotTables.get(index);

// Unshowing grand totals for rows.

pivotTable.setRowGrand(false);

// Dragging the first field to the row area.

pivotTable.addFieldToArea(PivotFieldType.ROW, 0);

// Dragging the second field to the column area.

pivotTable.addFieldToArea(PivotFieldType.COLUMN, 1);

// Dragging the third field to the data area.

pivotTable.addFieldToArea(PivotFieldType.DATA, 2);

{{< /highlight >}}
## **Apache POI SS (HSSF + XSSF) - 创建数据透视表**
**Java**

{{< highlight "java" >}}

 XSSFWorkbook wb = new XSSFWorkbook();

XSSFSheet sheet = wb.createSheet();

//Create some data to build the pivot table on

setCellData(sheet);

XSSFPivotTable pivotTable = sheet.createPivotTable(new AreaReference("A1:D4"), new CellReference("H5"));

//Configure the pivot table

//Use first column as row label

pivotTable.addRowLabel(0);

//Sum up the second column

pivotTable.addColumnLabel(DataConsolidateFunction.SUM, 1);

//Set the third column as filter

pivotTable.addColumnLabel(DataConsolidateFunction.AVERAGE, 2);

//Add filter on forth column

pivotTable.addReportFilter(3);

{{< /highlight >}}
## **下载运行代码**
下载运行示例**使用 Apache POI 和 Aspose.Cells 创建数据透视表**来自以下任何社交编码网站：

- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-Java/releases/tag/Aspose.Cells-Java-vs-POI-SS-v1.5)
## **下载源代码**
下载源代码**使用 Apache POI 和 Aspose.Cells 创建数据透视表**来自以下任何社交编码网站：

- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-Java)

{{% alert color="primary" %}} 

欲了解更多详情，请访问[创建数据透视表和数据透视图](/cells/zh/java/create-pivot-tables-and-pivot-charts/).

{{% /alert %}}
