﻿---
title: Перемещение рабочих листов в рабочей книге
type: docs
weight: 30
url: /ru/net/move-worksheets-within-workbook/
---
Aspose.Cells предоставляет метод Aspose.Cells.Worksheet.MoveTo(), используемый для перемещения рабочего листа в другое место электронной таблицы. Метод принимает индекс целевого рабочего листа в качестве параметра.

В следующем примере показано, как переместить лист в другое место в книге.

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
## **Скачать пример кода**
- [Гитхаб](https://github.com/aspose-cells/Aspose.Cells-for-.NET/releases/tag/MissingFeaturesOpenXMLExcelv1.1)
- [Битбакет](https://bitbucket.org/asposemarketplace/aspose-for-openxml/downloads/Move%20Worksheet%20%28Aspose.Cells%29.zip)
