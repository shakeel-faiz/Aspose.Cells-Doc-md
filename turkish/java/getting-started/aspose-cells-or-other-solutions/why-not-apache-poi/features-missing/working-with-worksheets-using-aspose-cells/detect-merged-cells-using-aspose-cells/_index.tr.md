﻿---
title: Aspose.Cells kullanarak Birleştirilmiş Cells'i algıla
type: docs
weight: 30
url: /tr/java/detect-merged-cells-using-aspose-cells/
---
## **Aspose.Cells - Birleştirilmiş Algıla Cells**
Microsoft Excel'de birkaç hücre birleştirilebilir. Bu genellikle karmaşık tablolar oluşturmak veya birkaç sütuna yayılan bir başlığı içeren bir hücre oluşturmak için kullanılır.
Aspose.Cells, bir çalışma sayfasındaki birleştirilmiş hücre alanlarını belirlemenizi sağlar. Onları da ayırabilirsin.

**Java**

{{< highlight "java" >}}

 //Get the merged cells list to put it into the arraylist object

ArrayList<CellArea> al = worksheet.getCells().getMergedCells();

//Define cellarea

CellArea ca;

//Define some variables

int frow, fcol, erow, ecol;

// Print Message

System.out.println("Merged Areas: \n"+ al.toString());

//Loop through the arraylist and get each cellarea to unmerge it

for(int i = al.size()-1 ; i > -1; i--)

{

	ca = new CellArea();

	ca = (CellArea)al.get(i);

	frow = ca.StartRow;

	fcol = ca.StartColumn;

	erow = ca.EndRow;

	ecol = ca.EndColumn;

	System.out.println((i+1) + ". [" + fcol +"," + frow +"] " + "[" + ecol +"," + erow +"]");

	worksheet.getCells().unMerge(frow, fcol, erow, ecol);

}

{{< /highlight >}}
## **Çalışan Kodu İndir**

- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-Java/releases/tag/Aspose.Cells_Java_for_Apache_POI_SS-v1.0.0)
## **Örnek Kodu İndir**
- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-Java/blob/master/Plugins/Aspose_Cells_for_Apache_POI/Aspose-Cells-for-Apache-POI-(Maven)/src/main/java/com/aspose/cells/examples/asposefeatures/worksheets/AsposeDetectMergeCells.java)

{{% alert color="primary" %}} 

 Daha fazla ayrıntı için, ziyaret edin[Çalışma Sayfasında Birleştirilmiş Cells'i Algıla](/cells/tr/java/detect-merged-cells-in-a-worksheet).

{{% /alert %}}
