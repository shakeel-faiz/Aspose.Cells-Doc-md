﻿---
title: Aspose.Cells for Node.js via Java 22.11 リリースノート
type: docs
weight: 2
url: /ja/nodejs-java/aspose-cells-for-node-js-via-java-22-11-release-notes/
---
{{% alert color="primary" %}}

このページには、[Aspose.Cells for Node.js via Java 22.11](https://releases.aspose.com/cells/nodejs/new-releases/aspose.cells-for-node.js-via-java-22.11/).

{{% /alert %}}

|**鍵**|**概要**|**カテゴリー**|
|:- |:- |:- |
|CELLSJAVA-44888|変換後に「+」と「-」が消えた - Excel を HTML にレンダリング|
|CELLSJAVA-44775|グラフから画像へのレンダリングでグラフ ラベルが重なる|
|CELLSJAVA-44882|チャートから画像へのレンダリング - ラベルの 1 つがドーナツ チャート内にあります|
|CELLSJAVA-44943|XLSX から PDF: グラフ ラベルが正しく表示されない|
|CELLSJAVA-44928|XLS ～ PDF: 画像のデータが不足しています|
|CELLSJAVA-44910|Excel を HTML に変換すると、何千もの同様の小さな画像が生成されます|
|CELLSJAVA-44944|表のサイズを変更すると、セルの書式が変更されます|
|CELLSJAVA-44948|HTML を Excel に変換すると、シートに画像が表示されない|
|CELLSJAVA-44908|大きな XLSB ファイルをロードするときの例外「java.lang.OutOfMemoryError: Java ヒープ領域」|
|CELLSJAVA-44929|リグレッション: Workbook.calculateFormula() での「java.lang.NullPointerException」|
|CELLSJAVA-44927|Excel ファイルを HTML に変換すると、例外「java.lang.IndexOutOfBoundsException: インデックス: 5、サイズ: 5」が発生する|
|CELLSJAVA-44939|エラー "java.lang.StringIndexOutOfBoundsException: String index out of range: 0" が Excel ファイルの読み取り中に発生する|

## **Public API および下位互換性のない変更**

以下は、Aspose.Cells for Java に対して行われた下位互換性のない変更と同様に、追加、名前変更、削除、または廃止されたメンバーなど、パブリック API に対して行われた変更のリストです。リストされている変更について懸念がある場合は、 Aspose.Cells サポート フォーラム。

### **Cell.IsDynamicArrayFormula プロパティを追加**

セルの数式が動的配列数式 (true) か従来の配列数式 (false) かを示します。

### **SparklineGroup.SparklineCollection プロパティを廃止し、SparklineGroup.Sparklines プロパティを追加します**

代わりに SparklineGroup.Sparklines プロパティを使用してください。

### **Worksheet.SparklineGroupCollection プロパティを廃止し、Worksheet.SparklineGroups プロパティを追加**

代わりに Worksheet.SparklineGroups プロパティを使用してください。