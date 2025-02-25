﻿---
title: Python での行と列のコピー
type: docs
weight: 30
url: /ja/java/copying-rows-and-columns-in-python/
---
## **Aspose.Cells - 行と列のコピー**
### **行のコピー**
Aspose.Cells は、Cells クラスの copyRow メソッドを提供します。このメソッドは、数式、値、コメント、セル形式、非表示のセル、画像、およびその他の描画オブジェクトを含むすべての種類のデータをソース行から宛先行にコピーします。

copyRow メソッドは、次のパラメーターを取ります。

- ソース Cells オブジェクト、
- ソース行インデックス、および
- 宛先行インデックス。

**Python コード**

{{< highlight "java" >}}

 def copy_rows(self):

\# Instantiating a Workbook object by excel file path

workbook = self.Workbook(self.dataDir + 'Book1.xls')

\# Accessing the first worksheet in the Excel file

worksheet = workbook.getWorksheets().get(0)

\# Copy the second row with data, formattings, images and drawing objects

\# to the 12th row in the worksheet.

worksheet.getCells().copyRow(worksheet.getCells(),1,11)

\# Saving the modified Excel file in default (that is Excel 2003) format

workbook.save(self.dataDir + "Copy Rows.xls")

print "Copy Rows Successfully." 

{{< /highlight >}}
### **列のコピー**
Aspose.Cells は Cells クラスの copyColumn メソッドを提供します。このメソッドは、式 (更新された参照を含む) を含むすべてのタイプのデータ、および値、コメント、セル形式、非表示のセル、画像、およびその他の描画オブジェクトをソース列から宛先列にコピーします。

copyColumn メソッドは、次のパラメーターを取ります。

- ソース Cells オブジェクト、
- ソース列インデックス、および
- 宛先列のインデックス。

**Python コード**

{{< highlight "ruby" >}}



def copy_columns(self):

\# Excel ファイル パスによる Workbook オブジェクトのインスタンス化

ワークブック = セルフ.ワークブック()

\# Excel ファイルの最初のワークシートにアクセス

ワークシート = workbook.getWorksheets().get(0)

\# データをヘッダ行に入れる (A1:A4)

私は= 0

私がいる間< 5:

worksheet.getCells().get(i, 0).setValue("Header Row #i")





\# Put some detail data (A5:A999)

i = 5

while i < 1000:

worksheet.getCells().get(i, 0).setValue("Detail Row #i")


\# Create another Workbook.

workbook1 = Workbook()

\# Get the first worksheet in the book.

worksheet1 = workbook1.getWorksheets().get(0)

\# Copy the first column from the first worksheet of the first workbook into

\# the first worksheet of the second workbook.

worksheet1.getCells().copyColumn(worksheet.getCells(),0,2)

\# Autofit the column.

worksheet1.autoFitColumn(2)

\# Saving the modified Excel file in default (that is Excel 2003) format

workbook.save(self.dataDir + "Copy Columns.xls")

print "Copy Columns Successfully." 

{{< /highlight >}}
## **実行中のコードをダウンロード**
ダウンロード**行と列のコピー (Aspose.Cells)**以下のソーシャルコーディングサイトのいずれかから：

- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-Java/releases/tag/Aspose.Cells_Java_for_Python-v1.0)
