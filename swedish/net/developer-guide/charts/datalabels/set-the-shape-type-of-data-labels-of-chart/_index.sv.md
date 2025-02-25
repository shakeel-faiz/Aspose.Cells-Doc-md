﻿---
title: Ställ in formtypen för dataetiketter för diagram
type: docs
weight: 110
url: /sv/net/set-the-shape-type-of-data-labels-of-chart/
---
## **Möjliga användningsscenarier**
Du kan ändra formtypen för dataetiketter i diagrammet med egenskapen DataLabels.ShapeType. Den tar värdet av DataLabelShapeType-uppräkning och ändrar formtypen för dataetiketter i enlighet med detta. Några av dess värden är

{{< highlight "java" >}}

 DataLabelShapeType.BentLineCallout

DataLabelShapeType.DownArrowCallout

DataLabelShapeType.Ellipse

DataLabelShapeType.LineCallout

DataLabelShapeType.Rect

etc.

{{< /highlight >}}
## **Ställ in formtypen för dataetiketter för diagram**
 Följande exempelkod ändrar formtypen för dataetiketter i diagrammet till DataLabelShapeType.WedgeEllipseCallout. Vänligen se[exempel på Excel-fil](60489778.xlsx) används i den här koden och[utdata Excel-fil](60489779.xlsx) genereras av det. Skärmdumpen visar effekten av koden på exempel på Excel-fil.

![todo:image_alt_text](set-the-shape-type-of-data-labels-of-chart_1.png)
## **Exempelkod**
{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Charts-SetShapeTypeOfDataLabelsOfChart.cs" >}}
