﻿---
title: スマート マーカーの書式設定
type: docs
weight: 20
url: /ja/net/formatting-smart-markers/
---
## **スタイル属性をコピー**
スマート マーカーを使用しているときに、スマート マーカー タグを含むセルのスタイルをコピーしたい場合があります。この目的のために、スマート マーカーのタグの CopyStyle 属性を使用できます。
### **スマート マーカーを使用して Cells からスタイルをコピーする**
この例では、A2 セルと B2 セルに 2 つのマーカーがある単純なテンプレート Microsoft Excel ファイルを使用します。セル B2 に貼り付けられたマーカーは CopyStyle 属性を使用しますが、セル A2 のマーカーは使用しません。単純な書式を適用します (たとえば、フォントの色を**赤**セルの塗りつぶしの色を**黄**).

コードを実行すると、Aspose.Cells は書式を列 B のすべてのレコードにコピーしますが、列 A の書式は保持しません。



{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-SmartMarkers-UsingCopyStyleAttribute-1.cs" >}}
## **カスタム ラベルの追加**
### **序章**
スマート マーカーのグループ化データ機能を使用しているときに、集計行に独自のカスタム ラベルを追加する必要がある場合があります。また、「注文の小計」など、列の名前とそのラベルを連結したいとします。 Aspose.Cells は、Label および LabelPosition 属性を提供するため、カスタム ラベルをスマート マーカーに配置しながら、データのグループ化で小計行と連結できます。
### **カスタム ラベルを追加してスマート マーカーの小計行と連結する**
この例では、[データファイル](96927971.xlsx)そして[テンプレートファイル](96927972.xlsx)細胞内にいくつかのマーカーがあります。コードを実行すると、Aspose.Cells によって、グループ化されたデータの集計行にいくつかのカスタム ラベルが追加されます。

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-SmartMarkers-AddCustomLabels-1.cs" >}}
