﻿---
title: LightCells の使用 API
type: docs
weight: 160
url: /ja/net/using-lightcells-api/
---
{{% alert color="primary" %}} 

場合によっては、ワークシート内のデータやコンテンツの膨大なリストを含む大きな Microsoft Excel ファイルを読み書きする必要があります。 LightCells API は、巨大な Excel スプレッドシートを作成するのに役立ちます。これを使用すると、必要なメモリが少なくなり、パフォーマンスと効率が向上します。

{{% /alert %}} 
# イベント駆動型アーキテクチャ
Aspose.Cells は LightCells API を提供します。これは主に、(Cell コレクションなどを使用して) 完全なデータ モデル ブロックをメモリに構築することなく、セル データを 1 つずつ操作するように設計されています。イベント駆動モードで動作します。

ワークブックを保存するには、保存時にセルの内容をセルごとに提供し、コンポーネントはそれを出力ファイルに直接保存します。

テンプレート ファイルを読み取るとき、コンポーネントはすべてのセルを解析し、その値を 1 つずつ提供します。

どちらの手順でも、1 つの Cell オブジェクトが処理されてから破棄され、Workbook オブジェクトはコレクションを保持しません。したがって、このモードでは、Microsoft 大量のメモリを使用する大規模なデータ セットを含む Excel ファイルをインポートおよびエクスポートするときに、メモリが節約されます。

LightCells API は XLSX および XLS ファイルに対して同じ方法でセルを処理します (実際にはすべてのセルをメモリにロードするのではなく、1 つのセルを処理してから破棄します)。 2 つの形式の異なるデータ モデルと構造。

でも、**XLS ファイルの場合**、より多くのメモリを節約するために、開発者は、保存プロセス中に生成された一時データを保存するための一時的な場所を指定できます。一般的に、**LightCells API を使用して XLSX ファイルを保存すると、50% 以上のメモリを節約できる場合があります**一般的な方法を使用するよりも、**XLS を保存すると、約 20 ～ 40% のメモリを節約できます**.
## 大きな Excel ファイルの書き込み
Aspose.Cells は、プログラムに実装する必要があるインターフェイス LightCellsDataProvider を提供します。インターフェイスは、軽量モードで大きなスプレッドシート ファイルを保存するためのデータ プロバイダーを表します。

このモードでワークブックを保存する場合、ワークブック内のすべてのワークシートを保存するときに StartSheet(int) がチェックされます。 1 つのシートの場合、StartSheet(int) が true の場合、保存されるこのシートの行とセルのすべてのデータとプロパティは、この実装によって提供されます。まず、保存する次の行インデックスを取得するために NextRow() が呼び出されます。有効な行インデックスが返された場合 (行を保存するには行インデックスが昇順である必要があります)、この行を表す Row オブジェクトが実装用に提供され、StartRow(Row) によってそのプロパティを設定します。

1 つの行については、NextCell() が最初にチェックされます。有効な列インデックスが返された場合 (1 行のすべてのセルを保存するには、列インデックスが昇順である必要があります)、そのセルを表す Cell オブジェクトが実装用に提供され、StartCell(Cell) によってデータとプロパティを設定します。セルのデータが設定されると、セルは生成されたスプレッドシート ファイルに直接保存され、次のセルがチェックされて処理されます。
### 大きな Excel ファイルの書き込み:例
次のサンプル コードを参照して、LightCells API の動作を確認してください。必要に応じて、コード セグメントを追加、削除、または更新してください。

プログラムは巨大なファイルを作成します**10,000 (10000x30 マトリックス) レコード**をワークシートに挿入し、それらにダミー データを入力します。 Main() メソッドの rowsCount 変数と colsCount 変数を変更することで、独自のマトリックスを指定できます。



{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Articles-UsingLightCellsAPI-WritingLargeExcelFile.cs" >}}
## 大きな Excel ファイルの読み取り
Aspose.Cells は、プログラムに実装する必要があるインターフェイス LightCellsDataHandler を提供します。インターフェイスは、軽量モードで大きなスプレッドシート ファイルを読み取るためのデータ プロバイダーを表します。

このモードでブックを読み取る場合、ブック内のすべてのワークシートを読み取るときに StartSheet がチェックされます。シートの場合、StartSheet が true を返す場合、シートの行と列のセルのすべてのデータとプロパティがチェックされ、このインターフェイスの実装によって処理されます。行ごとに StartRow が呼び出され、処理が必要かどうかが確認されます。行を処理する必要がある場合、そのプロパティが最初に読み取られ、開発者は ProcessRow を使用してそのプロパティにアクセスできます。行のセルも処理する必要がある場合、ProcessRow は true を返す必要があり、行内の既存のすべてのセルに対して StartCell が呼び出され、1 つのセルを処理する必要があるかどうかがチェックされます。 1 つのセルを処理する必要がある場合は、ProcessCell を呼び出して、このインターフェイスの実装によってセルを処理します。
### 大きな Excel ファイルの読み取り:例
次のサンプル コードを参照して、LightCells API の動作を確認してください。必要に応じて、コード セグメントを追加、削除、または更新してください。

プログラムは、ワークシートに何百万ものレコードを含む巨大なファイルを読み取ります。ワークブックの各シートを読み取るには、少し時間がかかります。サンプル コードはファイルを読み取り、各ワークシートの合計セル数、文字列数、および数式数を取得します。



{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Articles-UsingLightCellsAPI-ReadingLargeExcelFile.cs" >}}
