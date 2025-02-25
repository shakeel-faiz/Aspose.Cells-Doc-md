﻿---
title: Aspose.Cells を使用してチャートを画像に変換する
type: docs
weight: 30
url: /ja/java/convert-chart-to-images-using-aspose-cells/
---
## **Aspose.Cells - チャートを画像に変換**
グラフは視覚的に魅力的であり、ユーザーはデータの比較、パターン、および傾向を簡単に確認できます。
Chart クラスの toImage メソッドは、チャートをディスクまたはストリームに保存できる画像ファイルに変換します。

**Java**

{{< highlight "java" >}}

 //Get the Chart image

ImageOrPrintOptions imgOpts = new ImageOrPrintOptions();

imgOpts.setImageFormat(ImageFormat.getPng());

//Save the chart image file.

chart.toImage(new FileOutputStream(dataDir + "AsposeChartImage.png"), imgOpts);

{{< /highlight >}}
## **実行中のコードをダウンロード**

- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-Java/releases/tag/Aspose.Cells_Java_for_Apache_POI_SS-v1.0.0)
## **サンプルコードをダウンロード**
- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-Java/blob/master/Plugins/Aspose_Cells_for_Apache_POI/Aspose-Cells-for-Apache-POI-(Maven)/src/main/java/com/aspose/cells/examples/asposefeatures/charts/AsposeChartToImage.java)

{{% alert color="primary" %}} 

詳細については、次を参照してください。[チャートを画像に変換する](/java/converting-chart-to-image).

{{% /alert %}}
