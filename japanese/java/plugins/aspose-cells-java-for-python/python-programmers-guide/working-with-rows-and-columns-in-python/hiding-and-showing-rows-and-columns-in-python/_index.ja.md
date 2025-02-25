﻿---
title: Python での行と列の非表示と表示
type: docs
weight: 50
url: /ja/java/hiding-and-showing-rows-and-columns-in-python/
---
## **Aspose.Cells - 行と列の可視性の制御**
### **行と列を非表示にする**
開発者は、Cells コレクションの HideRow メソッドと HideColumn メソッドをそれぞれ呼び出すことで、行または列を非表示にできます。どちらのメソッドも、特定の行または列を非表示にするために、行/列のインデックスをパラメーターとして受け取ります。

**ルビーコード**

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
### **行と列の表示**
開発者は、Cells コレクションの UnhideRow メソッドと UnhideColumn メソッドをそれぞれ呼び出すことで、非表示の行または列を再表示できます。どちらのメソッドも次の 2 つのパラメーターを取ります。

- **行または列のインデックス**特定の行または列を表示するために使用される行または列のインデックス。
- **行の高さまたは列の幅**- 行または列が表示された後に割り当てられる行の高さまたは列の幅。

**ルビーコード**

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
## **実行中のコードをダウンロード**
ダウンロード**行と列の可視性の制御 (Aspose.Cells)**以下のソーシャルコーディングサイトのいずれかから：

- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-Java/releases/tag/Aspose.Cells_Java_for_Python-v1.0)
