﻿---
title: Python'de Satırları ve Sütunları Otomatik Sığdır
type: docs
weight: 20
url: /tr/java/autofit-rows-and-columns-in-python/
---
## **Aspose.Cells - Satırları ve Sütunları Otomatik Sığdır**
### **Satırı Otomatik Sığdır**
Bir satırın genişliğini ve yüksekliğini otomatik olarak boyutlandırmak için en basit yaklaşım, Worksheet sınıfının autoFitRow yöntemini çağırmaktır. autoFitRow yöntemi, parametre olarak bir satır dizini (yeniden boyutlandırılacak satırın) alır.

**Python Kod**

{{< highlight "python" >}}

 def autofit_row(self):

\# Instantiating a Workbook object by excel file path

workbook = self.Workbook(self.dataDir + 'Book1.xls')

\# Accessing the first worksheet in the Excel file

worksheet = workbook.getWorksheets().get(0)

\# Auto-fitting the 3rd row of the worksheet

worksheet.autoFitRow(2)

\# Auto-fitting the 3rd row of the worksheet based on the contents in a range of

\# cells (from 1st to 9th column) within the row

# worksheet.autoFitRow(2,0,8) # Uncomment this line if you to do AutoFit Row in a Range of Cells. Also, comment line 288.

\# Saving the modified Excel file in default (that is Excel 2003) format

workbook.save(self.dataDir + "Autofit Row.xls")

print "Autofit Row Successfully." 

{{< /highlight >}}
### **Otomatik Sığdırma Sütunu**
Bir sütunun genişliğini ve yüksekliğini otomatik olarak boyutlandırmanın en kolay yolu, Worksheet sınıfının autoFitColumn yöntemini çağırmaktır. autoFitColumn yöntemi, sütun dizinini (yeniden boyutlandırılmak üzere olan sütunun) parametre olarak alır.

**Python Kod**

{{< highlight "python" >}}

 def autofit_column(self):

\# Instantiating a Workbook object by excel file path

workbook = self.Workbook(self.dataDir + 'Book1.xls')

\# Accessing the first worksheet in the Excel file

worksheet = workbook.getWorksheets().get(0)

\# Auto-fitting the 4th column of the worksheet

worksheet.autoFitColumn(3)

\# Auto-fitting the 4th column of the worksheet based on the contents in a range of

\# cells (from 1st to 9th row) within the column

# worksheet.autoFitColumn(3,0,8) #Uncomment this line if you to do AutoFit Column in a Range of Cells. Also, comment line 310.

\# Saving the modified Excel file in default (that is Excel 2003) format

workbook.save(self.dataDir + "Autofit Column.xls")

print "Autofit Column Successfully." 

{{< /highlight >}}
## **Çalışan Kodu İndir**
İndirmek**Satırları ve Sütunları Otomatik Sığdır (Aspose.Cells)**aşağıda belirtilen sosyal kodlama sitelerinin herhangi birinden:

- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-Java/releases/tag/Aspose.Cells_Java_for_Python-v1.0)
