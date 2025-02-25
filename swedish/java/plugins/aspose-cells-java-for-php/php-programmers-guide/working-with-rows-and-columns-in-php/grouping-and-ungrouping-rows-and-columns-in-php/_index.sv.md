﻿---
title: Gruppera och dela upp rader och kolumner i PHP
type: docs
weight: 40
url: /sv/java/grouping-and-ungrouping-rows-and-columns-in-php/
---
## **Aspose.Cells - Koncernledning av rader och kolumner**
### **Gruppera rader och kolumner**
Det är möjligt att gruppera rader eller kolumner genom att anropa metoderna groupRows och groupColumns i samlingen Cells. Båda metoderna tar följande parametrar:

- Första rad-/kolumnindex, den första raden eller kolumnen i gruppen.
- Sista raden/kolumnindex, den sista raden eller kolumnen i gruppen.
- Är dold, en boolesk parameter som anger om rader/kolumner ska döljas efter gruppering eller inte.

**PHP-kod**

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
### **Dela upp rader och kolumner**
Dela upp grupperade rader eller kolumner genom att anropa Cells-samlingens metoder för UgroupRows och UngroupColumns. Båda metoderna tar samma parametrar:

- Första raden eller kolumnindex, den första raden/kolumnen som ska delas upp.
- Sista raden eller kolumnindex, den sista raden/kolumnen som ska delas upp.

**PHP-kod**

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
## **Ladda ner Running Code**
 Ladda ner**Gruppera och dela upp rader och kolumner (Aspose.Cells)**från någon av nedan nämnda webbplatser för social kodning:

- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-Java/blob/master/Plugins/Aspose_Cells_Java_for_PHP/src/aspose/cells/WorkingWithRowsAndColumns/RowsAndColumns.php)
