﻿---
title: Çalışma Sayfalarını Çalışma Kitabı İçinde Taşıma
type: docs
weight: 30
url: /tr/net/move-worksheets-within-workbook/
---
Aspose.Cells, bir çalışma sayfasını elektronik tabloda başka bir konuma taşımak için kullanılan Aspose.Cells.Worksheet.MoveTo() yöntemini sağlar. Yöntem, hedef çalışma sayfası dizinini parametre olarak alır.

Aşağıdaki örnek, bir çalışma sayfasının çalışma kitabı içinde başka bir konuma nasıl taşınacağını gösterir.

{{< highlight "csharp" >}}

 string FilePath = @"..\..\..\Sample Files\";

string FileName = FilePath + "Move Worksheet.xlsx";

//Open an existing excel file.

Workbook wb = new Workbook(FileName);

//Create a Worksheets object with reference to

//the sheets of the Workbook.

WorksheetCollection sheets = wb.Worksheets;

//Get the first worksheet.

Worksheet worksheet = sheets[0];

string test = worksheet.Name;

//Move the first sheet to the third position in the workbook.

worksheet.MoveTo(2);

//Save the excel file.

wb.Save(FileName);

{{< /highlight >}}
## **Örnek Kodu İndir**
- [Github](https://github.com/aspose-cells/Aspose.Cells-for-.NET/releases/tag/MissingFeaturesOpenXMLExcelv1.1)
- [Bitbucket](https://bitbucket.org/asposemarketplace/aspose-for-openxml/downloads/Move%20Worksheet%20%28Aspose.Cells%29.zip)
