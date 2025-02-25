﻿---
title: Ruby での Excel ファイルの暗号化
type: docs
weight: 80
url: /ja/java/encrypting-excel-files-in-ruby/
---
## **Aspose.Cells - Excel ファイルの暗号化**
Ruby で Aspose.Cells for Java を使用して Excel ファイルに暗号化を適用するには、単に Encrypt モジュールを呼び出します。

**ルビーコード**

{{< highlight "ruby" >}}

 data_dir = File.dirname(File.dirname(File.dirname(__FILE__))) + '/data/'

\# Instantiating a Workbook object by excel file path

workbook = Rjb::import('com.aspose.cells.Workbook').new(data_dir + 'Book1.xls')

\# Password protect the file.

workbook.getSettings().setPassword("1234")

encryption_type = Rjb::import('com.aspose.cells.EncryptionType')        

\# Specify XOR encrption type.

workbook.setEncryptionOptions(encryption_type.XOR, 40)

\# Specify Strong Encryption type (RC4,Microsoft Strong Cryptographic Provider).

workbook.setEncryptionOptions(encryption_type.STRONG_CRYPTOGRAPHIC_PROVIDER, 128)

\# Saving the modified Excel file in default (that is Excel 2003) format

workbook.save(data_dir + "encrypt.xls")

puts "Apply encryption, please check the output file."

{{< /highlight >}}
## **実行中のコードをダウンロード**
ダウンロード**Excel ファイルの暗号化 (Aspose.Cells)**以下のソーシャルコーディングサイトのいずれかから：

- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-Java/blob/master/Plugins/Aspose_Cells_Java_for_Ruby/lib/asposecellsjava/encrypt.rb)
