﻿---
title: Python'de Kılavuz Çizgilerini Görüntüleyin veya Gizle
type: docs
weight: 10
url: /tr/java/display-or-hide-gridlines-in-python/
---
## **Aspose.Cells - Kılavuz Çizgilerini Gizle'yi Görüntüle**
### **Kılavuz Çizgilerini Gizleme**
 kullanarak çalışma sayfasını gizlemek için**Yakut için Aspose.Cells Java** , Arama**displayhidegridlines** modül.

**Python Kod**

{{< highlight "java" >}}

 workbook = self.Workbook(self.dataDir + "Book1.xls")

# Accessing the first worksheet in the Excel file

worksheets = workbook.getWorksheets()

worksheet = worksheets.get(0)

# Hiding the grid lines of the first worksheet of the Excel file

worksheet.setGridlinesVisible(False)

# Saving the modified Excel file in default (that is Excel 2000) format

workbook.save(self.dataDir + "output.xls")

\# Print message

print "Grid lines are now hidden on sheet 1, please check the output document."

{{< /highlight >}}
### **Kılavuz Çizgilerini Görünür Hale Getirme**
Kılavuz çizgilerini görünür yapmak için Worksheet sınıfının setGridlinesVisible(true) yöntemini kullanın.

**Python Kod**

{{< highlight "python" >}}

 # Displaying the gridlines of the worksheet

worksheet.setGridlinesVisible(True)

{{< /highlight >}}
## **Çalışan Kodu İndir**
 İndirmek**DisplayHideGridlines (Aspose.Cells)** aşağıda belirtilen sosyal kodlama sitelerinin herhangi birinden:

- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-Java/releases/tag/Aspose.Cells_Java_for_Python-v1.0)
