﻿---
title: 在 PHP 中对行和列进行分组和取消分组
type: docs
weight: 40
url: /zh/java/grouping-and-ungrouping-rows-and-columns-in-php/
---
## **Aspose.Cells - 行列分组管理**
### **分组行和列**
可以通过调用 Cells 集合的 groupRows 和 groupColumns 方法对行或列进行分组。这两种方法都采用以下参数：

- 第一行/列索引，组中的第一行或第一列。
- 最后一行/列索引，组中的最后一行或最后一列。
- is hidden，布尔型参数，指定分组后是否隐藏行/列。

**PHP代码**

{{< highlight "php" >}}

 public static function group_rows_columns($dataDir)

{

    # Instantiating a Workbook object by excel file path

    $workbook = new Workbook($dataDir . 'Book1.xls');

    # Accessing the first worksheet in the Excel file

    $worksheet = $workbook->getWorksheets()->get(0);

    $cells = $worksheet->getCells();;

    # Grouping first six rows (from 0 to 5) and making them hidden by passing true

    $cells->groupRows(0,5,true);

    # Grouping first three columns (from 0 to 2) and making them hidden by passing true

    $cells->groupColumns(0,2,true);

    # Saving the modified Excel file in default (that is Excel 2003) format

    $workbook->save($dataDir . "Group Rows And Columns.xls");

    print "Group Rows And Columns Successfully." . PHP_EOL;

}

{{< /highlight >}}
### **取消分组行和列**
通过调用 Cells 集合的 UngroupRows 和 UngroupColumns 方法取消分组行或列。两种方法都采用相同的参数：

- 第一行或第一列索引，要取消分组的第一行/列。
- 最后一行或最后一列索引，要取消分组的最后一行/列。

**PHP代码**

{{< highlight "php" >}}

 public static function ungroup_rows_columns($dataDir)

{

    # Instantiating a Workbook object by excel file path

    $workbook = new Workbook($dataDir . 'Group Rows And Columns.xls');

    # Accessing the first worksheet in the Excel file

    $worksheet = $workbook->getWorksheets()->get(0);

    $cells = $worksheet->getCells();;

    # Ungrouping first six rows (from 0 to 5)

    $cells->ungroupRows(0,5);

    # Ungrouping first three columns (from 0 to 2)

    $cells->ungroupColumns(0,2);

    # Saving the modified Excel file in default (that is Excel 2003) format

    $workbook->save($dataDir . "Ungroup Rows And Columns.xls");

    print "Ungroup Rows And Columns Successfully." . PHP_EOL;

}

{{< /highlight >}}
## **下载运行代码**
下载**分组和取消分组行和列 (Aspose.Cells)**来自以下任何社交编码网站：

- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-Java/blob/master/Plugins/Aspose_Cells_Java_for_PHP/src/aspose/cells/WorkingWithRowsAndColumns/RowsAndColumns.php)
