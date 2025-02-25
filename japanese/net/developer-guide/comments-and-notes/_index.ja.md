﻿---
title: コメントとメモの管理
linktitle: コメントとメモ
type: docs
weight: 128
url: /ja/net/comments-and-notes/
description: .Net の Aspose.Cells でコメントやメモを挿入して管理します。
keywords: insert comments, insert notes
---
## **序章**

コメントは、セルに追加情報を追加するために使用されます。 Aspose.Cells は、セルにコメントを追加するための 2 つの方法を提供します。 1 つ目は、デザイナー ファイルに手動でコメントを作成することです。これらのコメントは、Aspose.Cells を使用してインポートされます。2 つ目は、実行時に Aspose.Cells API を使用してコメントを追加することです。このトピックでは、Aspose.Cells API を使用してセルにコメントを追加する方法について説明します。コメントの書式設定についても説明します。

## **コメントを追加する**

を呼び出して、セルにコメントを追加します。[**コメント**](https://reference.aspose.com/cells/net/aspose.cells/commentcollection)コレクションの[**追加**](https://reference.aspose.com/cells/net/aspose.cells/commentcollection/methods/add/index)メソッド ([**ワークシート**](https://reference.aspose.com/cells/net/aspose.cells/worksheet)物体）。新しい[**コメント**](https://reference.aspose.com/cells/net/aspose.cells/comment)からアクセスできます。[**コメント**](https://reference.aspose.com/cells/net/aspose.cells/commentcollection)コメント インデックスを渡してコレクションを作成します。にアクセスした後、[**コメント**](https://reference.aspose.com/cells/net/aspose.cells/comment)オブジェクトを使用して、コメント ノートをカスタマイズします。[**コメント**](https://reference.aspose.com/cells/net/aspose.cells/comment)オブジェクトの[**ノート**](https://reference.aspose.com/cells/net/aspose.cells/comment/properties/note)財産。

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-DrawingObjects-Comments-AddingComment-1.cs" >}}

## **コメントのフォーマット**

コメントの高さ、幅、およびフォント設定を構成して、コメントの外観をフォーマットすることもできます。

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-DrawingObjects-Comments-CommentFormatting-1.cs" >}}

## **コメントに画像を追加する**

Microsoft Excel 2007 では、セル コメントの背景として画像を使用することもできます。 Excel 2007 では、これは次の手順を実行することによって実現されます。 (彼らは、セルのコメントが既に追加されていると想定しています。)

1. コメントを含むセルを右クリックします。
1. 選択する**コメントの表示/非表示**、コメントからテキストをクリアします。
1. コメントの枠線をクリックして選択します。
1. 選択する**フォーマット**、 それから**コメント**.
1. 上で**色と線**タブで、**色**リスト。
1. クリック**塗りつぶし効果**.
1. 上で**写真**タブ、クリック**画像を選択**.
1. 画像を見つけて選択します。
1. クリック**わかった**すべてのダイアログが閉じるまで。

Aspose.Cells もこの機能を提供します。以下は、ゼロから XLSX ファイルを作成し、セル "A1" にコメントを追加し、背景として画像を設定するコード サンプルです。

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-DrawingObjects-Comments-AddImageToComment-1.cs" >}}

## **先行トピック**
- [コメントのテキスト方向を変更する](/cells/ja/net/change-text-direction-of-the-comment/)
- [コメントのフォントの色を変更する方法](/cells/ja/net/how-to-change-the-comment-font-color/)
- [コメント背景の設定方法](/cells/ja/net/how-to-set-comment-background/)
- [スレッド化されたコメント](/cells/ja/net/threaded-comments/)

