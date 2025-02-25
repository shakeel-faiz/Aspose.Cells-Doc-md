﻿---
title: Отображение или скрытие заголовков столбцов строк в Ruby
type: docs
weight: 20
url: /ru/java/display-or-hide-row-column-headers-in-ruby/
---
## **Aspose.Cells — Показать или скрыть заголовки столбцов строк**
### **Скрытие заголовков строк/столбцов**
 Чтобы скрыть заголовки строк/столбцов с помощью**Aspose.Cells Java для рубина** , вызов**DisplayHideRowColumnHeaders** модуль.

**Рубиновый код**

{{< highlight "ruby" >}}

 data_dir = File.dirname(File.dirname(File.dirname(__FILE__))) + '/data/'

\# Instantiating a Workbook object by excel file path

workbook = Rjb::import('com.aspose.cells.Workbook').new(data_dir + 'Book1.xls')

\# Accessing the first worksheet in the Excel file

worksheets = workbook.getWorksheets()

sheet_index = worksheets.add()

worksheet = worksheets.get(sheet_index)

\# Hiding the headers of rows and columns

worksheet.setRowColumnHeadersVisible(false)

\# Saving the modified Excel file in default (that is Excel 2003) format

workbook.save(data_dir + "output.xls")

puts "Headers of rows and columns are now hidden, please check the output file."

{{< /highlight >}}
### **Отображение заголовков строк/столбцов**
Сделайте заголовки строк и столбцов видимыми с помощью метода setRowColumnHeadersVisible(true) класса Worksheet.

**Рубиновый код**

{{< highlight "ruby" >}}

 # Displaying the headers of rows and columns

worksheet.setRowColumnHeadersVisible(true)

{{< /highlight >}}
## **Скачать рабочий код**
Скачать**Отображение или скрытие заголовков столбцов строк (Aspose.Cells)**с любого из нижеперечисленных сайтов социального кодирования:

- [Гитхаб](https://github.com/aspose-cells/Aspose.Cells-for-Java/blob/master/Plugins/Aspose_Cells_Java_for_Ruby/lib/asposecellsjava/displayhiderowcolumnheaders.rb)
