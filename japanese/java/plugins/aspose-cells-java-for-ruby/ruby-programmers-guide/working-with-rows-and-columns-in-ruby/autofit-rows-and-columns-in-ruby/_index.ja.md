﻿---
title: Ruby で行と列を自動調整する
type: docs
weight: 20
url: /ja/java/autofit-rows-and-columns-in-ruby/
---
## **Aspose.Cells - 行と列の自動調整**
### **行の自動調整**
行の幅と高さを自動的にサイズ変更する最も簡単な方法は、Worksheet クラスの autoFitRow メソッドを呼び出すことです。 autoFitRow メソッドは、(サイズ変更する行の) 行インデックスをパラメーターとして受け取ります。

**ルビーコード**

{{< highlight "ruby" >}}

 def autofit_row()

        data_dir = File.dirname(File.dirname(File.dirname(__FILE__))) + '/data/'



        # Instantiating a Workbook object by excel file path

        workbook = Rjb::import('com.aspose.cells.Workbook').new(data_dir + 'Book1.xls')

        # Accessing the first worksheet in the Excel file

        worksheet = workbook.getWorksheets().get(0)

        # Auto-fitting the 3rd row of the worksheet

        worksheet.autoFitRow(2)

        # Auto-fitting the 3rd row of the worksheet based on the contents in a range of

        # cells (from 1st to 9th column) within the row

        #worksheet.autoFitRow(2,0,8) # Uncomment this line if you to do AutoFit Row in a Range of Cells. Also, comment line 288.

        # Saving the modified Excel file in default (that is Excel 2003) format

        workbook.save(data_dir + "Autofit Row.xls")

        puts "Autofit Row Successfully."

    end

{{< /highlight >}}
### **列の自動調整**
列の幅と高さを自動的にサイズ変更する最も簡単な方法は、Worksheet クラスの autoFitColumn メソッドを呼び出すことです。 autoFitColumn メソッドは、(サイズ変更しようとしている列の) 列インデックスをパラメーターとして受け取ります。

**ルビーコード**

{{< highlight "ruby" >}}

 def autofit_column()

    data_dir = File.dirname(File.dirname(File.dirname(__FILE__))) + '/data/'



    # Instantiating a Workbook object by excel file path

    workbook = Rjb::import('com.aspose.cells.Workbook').new(data_dir + 'Book1.xls')

    # Accessing the first worksheet in the Excel file

    worksheet = workbook.getWorksheets().get(0)

    # Auto-fitting the 4th column of the worksheet

    worksheet.autoFitColumn(3)

    # Auto-fitting the 4th column of the worksheet based on the contents in a range of

    # cells (from 1st to 9th row) within the column

    #worksheet.autoFitColumn(3,0,8) #Uncomment this line if you to do AutoFit Column in a Range of Cells. Also, comment line 310.

    # Saving the modified Excel file in default (that is Excel 2003) format

    workbook.save(data_dir + "Autofit Column.xls")

    puts "Autofit Column Successfully."

end

{{< /highlight >}}
## **実行中のコードをダウンロード**
ダウンロード**行と列の自動調整 (Aspose.Cells)**以下のソーシャルコーディングサイトのいずれかから：

- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-Java/blob/master/Plugins/Aspose_Cells_Java_for_Ruby/lib/asposecellsjava/rowsandcolumns.rb)
