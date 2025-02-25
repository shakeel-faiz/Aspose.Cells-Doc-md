﻿---
title: データの並べ替え時の並べ替え警告の指定
type: docs
weight: 140
url: /ja/net/specifying-sort-warning-while-sorting-data/
---
## **考えられる使用シナリオ**

このテキスト データ、つまり {11, 111, 22} を考慮してください。このテキスト データは、テキストに関しては 111 が 22 の前に来るため、並べ替えられます。ただし、このデータをテキストとしてではなく数値として並べ替えたい場合は、数値的には 111 が 22 の後に来るため、{11, 22, 111} になります。 Aspose.Cells提供[**DataSorter.SortAsNumber**](https://reference.aspose.com/cells/net/aspose.cells/datasorter/properties/sortasnumber)この問題に対処するプロパティ。このプロパティを設定してください**真実**テキストデータは数値データとしてソートされます。次のスクリーンショットは、数値データのように見えるテキスト データが並べ替えられたときに、Microsoft Excel によって表示される並べ替えの警告を示しています。

![todo:画像_代替_文章](specifying-sort-warning-while-sorting-data_1.png)

## **サンプルコード**

次のサンプル コードは、[**DataSorter.SortAsNumber**](https://reference.aspose.com/cells/net/aspose.cells/datasorter/properties/sortasnumber)プロパティは、前述のとおりです。チェックしてください[サンプル Excel ファイル](43352075.xlsx)と[出力エクセルファイル](43352076.xlsx)さらにヘルプが必要です。

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-SpecifyingSortWarningWhileSortingData.cs" >}}
