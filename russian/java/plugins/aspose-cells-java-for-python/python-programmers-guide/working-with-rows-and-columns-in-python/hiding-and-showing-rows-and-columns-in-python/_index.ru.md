﻿---
title: Скрытие и отображение строк и столбцов в Python
type: docs
weight: 50
url: /ru/java/hiding-and-showing-rows-and-columns-in-python/
---
## **Aspose.Cells — Управление видимостью строк и столбцов**
### **Скрытие строк и столбцов**
Разработчики могут скрыть строку или столбец, вызвав методы HideRow и HideColumn коллекции Cells соответственно. Оба метода принимают индекс строки/столбца в качестве параметра, чтобы скрыть конкретную строку или столбец.

**Рубиновый код**

{{< highlight "ruby" >}}

 def hide_rows_columns(self):

\# Instantiating a Workbook object by excel file path

workbook = self.Workbook(self.dataDir + 'Book1.xls')

\# Accessing the first worksheet in the Excel file

worksheet = workbook.getWorksheets().get(0)

cells = worksheet.getCells()

\# Hiding the 3rd row of the worksheet

cells.hideRow(2)

\# Hiding the 2nd column of the worksheet

cells.hideColumn(1)

\# Saving the modified Excel file in default (that is Excel 2003) format

workbook.save(self.dataDir + "Hide Rows And Columns.xls")

print "Hide Rows And Columns Successfully." 

{{< /highlight >}}
### **Отображение строк и столбцов**
Разработчики могут отобразить любую скрытую строку или столбец, вызвав методы UnhideRow и UnhideColumn коллекции Cells соответственно. Оба метода принимают два параметра:

- **Индекс столбца строки**- индекс строки или столбца, который используется для отображения конкретной строки или столбца.
- **Высота строки или ширина столбца**- высота строки или ширина столбца, назначенная строке или столбцу после его отображения.

**Рубиновый код**

{{< highlight "ruby" >}}

 def unhide_rows_columns(self):

\# Instantiating a Workbook object by excel file path

workbook = self.Workbook(self.dataDir + 'Book1.xls')

\# Accessing the first worksheet in the Excel file

worksheet = workbook.getWorksheets().get(0)

cells = worksheet.getCells()

\# Unhiding the 3rd row and setting its height to 13.5

cells.unhideRow(2,13.5)

\# Unhiding the 2nd column and setting its width to 8.5

cells.unhideColumn(1,8.5)

\# Saving the modified Excel file in default (that is Excel 2003) format

workbook.save(self.dataDir + "Unhide Rows And Columns.xls")

print "Unhide Rows And Columns Successfully." 

{{< /highlight >}}
## **Скачать рабочий код**
 Скачать**Управление видимостью строк и столбцов (Aspose.Cells)**с любого из нижеперечисленных сайтов социального кодирования:

- [Гитхаб](https://github.com/aspose-cells/Aspose.Cells-for-Java/releases/tag/Aspose.Cells_Java_for_Python-v1.0)
