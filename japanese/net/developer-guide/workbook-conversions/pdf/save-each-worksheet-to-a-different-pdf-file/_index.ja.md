﻿---
title: 各ワークシートを別の PDF ファイルに保存する
type: docs
weight: 130
url: /ja/net/save-each-worksheet-to-a-different-pdf-file/
---
{{% alert color="primary" %}} 

Aspose.Cells は、XLS ファイル (画像、チャートなどを含む) を PDF ドキュメントに変換することをサポートします。 Aspose.Cells for .NET は独立してスプレッドシートを PDF に変換できます。変換に Aspose.PDF for .NET を使用する必要はありません。プロセス全体をメモリ内で実行できるため、変換ではソフトウェアが一時ファイルを作成または使用する必要はありません。

{{% /alert %}} 
## **各ワークシートを別の PDF ファイルに保存する**
異なる PDF ファイルを生成するためにテンプレート Excel ファイルに各ワークシートを保存する必要がある場合、これは簡単に実現できます。ファイル内のシートを非表示にし、一度に 1 つのシートを表示して PDF にレンダリングすることを試みることができます。

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Articles-SaveEachWorksheetToDifferentPDF-1.cs" >}}

{{% alert color="primary" %}} 

スプレッドシートに数式が含まれている場合は、[Workbook.CalculateFormula()](https://reference.aspose.com/cells/net/aspose.cells/workbook/methods/calculateformula)スプレッドシートを PDF 形式にレンダリングする直前。そうすることで、式に依存する値が再計算され、正しい値が PDF に表示されるようになります。

{{% /alert %}}
