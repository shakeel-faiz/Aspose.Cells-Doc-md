﻿---
title: 設定パラメータ
type: docs
weight: 10
url: /ja/jasperreports/configuration-parameters/
---
{{% alert color="primary" %}} 

次の表に、構成パラメータを示します。

{{% /alert %}} 

|**パラメータ名** |**説明** |
|:- |:- |
|FORMAT_TYPE| 「EXCEL97TO2003」または「EXCEL2007」に設定して、Microsoft Excel 79 0 2003 または Excel 2007 形式のファイルを生成できます。|
|は_一_ページ_あたり_シート|各レポート ページを異なる XLS ワークシートに書き込むかどうかを指定するブール値。|
|は_削除する_空_スペース_BETWEEN_ROWS|行間に表示される空白を削除するかどうかを指定するブール値。|
|は_削除する_空_スペース_ BETWEEN_COLUMNS|列間に表示される空白を削除するかどうかを指定するブール値。|
|は_白い_PAGE_BACKGROUND|ページの背景を白にするか、デフォルトの背景色 XLS にするかを指定するブール値。 XLS の背景色は、XLS ビューアのプロパティまたはオペレーティング システムの配色によって異なる場合があります。|
|は_探知_CELL_TYPE|エクスポータが元のテキスト フィールド式のタイプを考慮し、それに応じてセルのタイプと値を設定する必要があるかどうかを示すために使用されるフラグ。|
|シート名|カスタム シート名を表す文字列の配列。これは、IS で使用する場合に便利です。_一_ページ_あたり_シート パラメータ。|
|は_フォント_サイズ_修理_有効|テキストが指定されたセルの高さに収まるようにフォント サイズを小さくするためのフラグ。|
|最大_行_PER_SHEET|シートに表示できる最大行数を指定する整数値。設定すると、残りの行を表示するための新しいシートが作成されます。負の値またはゼロは、制限が設定されていないことを意味します。|
|は_無視_グラフィックス|グラフィック要素を無視し、テキスト要素のみをエクスポートするためのフラグ。|
|は_崩壊_ROW_SPAN|行スパンを折りたたむためのフラグを立て、行をまたいでセルをマージしないようにします。|
|は_無視_ CELL_BORDER|セル境界を無視するためのフラグ。|
|は_使用する_EXCEL_CHART| Microsoft 静的な画像ではなく、Excel 形式の編集可能なグラフを使用するためのフラグ。デフォルト値は true です。|

