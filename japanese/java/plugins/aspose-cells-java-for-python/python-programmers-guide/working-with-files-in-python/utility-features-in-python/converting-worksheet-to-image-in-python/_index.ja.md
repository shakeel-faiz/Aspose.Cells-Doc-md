﻿---
title: Python でワークシートを画像に変換する
type: docs
weight: 40
url: /ja/java/converting-worksheet-to-image-in-python/
---
## **Aspose.Cells - ワークシートを画像に変換する**
Ruby で Aspose.Cells for Java を使用して Worksheet を Image に変換するには、単に Converter モジュールを呼び出します。

**Python コード**

{{< highlight "python" >}}

 imageFormat = self.ImageFormat

# Instantiate a workbook with path to an Excel file

book = self.Workbook(self.dataDir + "Book1.xls")

# Create an object for ImageOptions

imgOptions = self.ImageOrPrintOptions()

# Set the image type

imgOptions.setImageFormat(imageFormat.getPng())

# Get the first worksheet.

sheet = book.getWorksheets().get(0)

# Create a SheetRender object for the target sheet

sr =self.SheetRender(sheet, imgOptions)

for i in range(sr.getPageCount()):

# Generate an image for the worksheet

sr.toImage(i, self.dataDir + "mysheetimg" + ".png")


\# Print message

print "Images generated successfully."

{{< /highlight >}}
## **実行中のコードをダウンロード**
ダウンロード**ワークシートから画像へ (Aspose.Cells)**以下のソーシャルコーディングサイトのいずれかから：

- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-Java/releases/tag/Aspose.Cells_Java_for_Python-v1.0)
