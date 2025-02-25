﻿---
title: PHP'de Satırları ve Sütunları Gizleme ve Gösterme
type: docs
weight: 50
url: /tr/java/hiding-and-showing-rows-and-columns-in-php/
---
## **Aspose.Cells - Satırların ve Sütunların Görünürlüğünü Kontrol Etme**
### **Satırları ve Sütunları Gizleme**
Geliştiriciler, sırasıyla Cells koleksiyonunun HideRow ve HideColumn yöntemlerini çağırarak bir satırı veya sütunu gizleyebilirsiniz. Her iki yöntem de belirli satır veya sütunu gizlemek için satır/sütun dizinini parametre olarak alır.

**PHP Kodu**

{{< highlight "php" >}}

 public static function hide_rows_columns($dataDir)

{

    # Instantiating a Workbook object by excel file path

    $workbook = new Workbook($dataDir . 'Book1.xls');

    # Accessing the first worksheet in the Excel file

    $worksheet = $workbook->getWorksheets()->get(0);

    $cells = $worksheet->getCells();;

    # Hiding the 3rd row of the worksheet

    $cells->hideRow(2);

    # Hiding the 2nd column of the worksheet

    $cells->hideColumn(1);

    # Saving the modified Excel file in default (that is Excel 2003) format

    $workbook->save($dataDir . "Hide Rows And Columns.xls");

    print "Hide Rows And Columns Successfully." . PHP_EOL;

}

{{< /highlight >}}
### **Satırları ve Sütunları Gösterme**
Geliştiriciler, sırasıyla Cells koleksiyonunun UnhideRow ve UnhideColumn yöntemlerini çağırarak herhangi bir gizli satırı veya sütunu gösterebilir. Her iki yöntem de iki parametre alır:

- **Rowor sütun dizini**- belirli bir satır veya sütunu göstermek için kullanılan bir satır veya sütun dizini.
- **Satır yüksekliği veya sütun genişliği**- gösterildikten sonra satıra veya sütuna atanan satır yüksekliği veya sütun genişliği.

**PHP Kodu**

{{< highlight "php" >}}

 public static function unhide_rows_columns($dataDir)

{

    # Instantiating a Workbook object by excel file path

    $workbook = new Workbook($dataDir . 'Book1.xls');

    # Accessing the first worksheet in the Excel file

    $worksheet = $workbook->getWorksheets()->get(0);

    $cells = $worksheet->getCells();;

    # Unhiding the 3rd row and setting its height to 13.5

    $cells->unhideRow(2,13.5);

    # Unhiding the 2nd column and setting its width to 8.5

    $cells->unhideColumn(1,8.5);

    # Saving the modified Excel file in default (that is Excel 2003) format

    $workbook->save($dataDir . "Unhide Rows And Columns.xls");

    print "Unhide Rows And Columns Successfully." . PHP_EOL;

}

{{< /highlight >}}
## **Çalışan Kodu İndir**
 İndirmek**Satırların ve Sütunların Görünürlüğünü Kontrol Etme (Aspose.Cells)**aşağıda belirtilen sosyal kodlama sitelerinin herhangi birinden:

- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-Java/blob/master/Plugins/Aspose_Cells_Java_for_PHP/src/aspose/cells/WorkingWithRowsAndColumns/RowsAndColumns.php)
