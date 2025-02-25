﻿---
title: 访问 GridWeb 的超链接对象 Cell
type: docs
weight: 60
url: /zh/java/access-hyperlink-object-of-the-gridweb-cell/
---
## **可能的使用场景**
您可以使用以下两种方法检查单元格是否包含超链接。如果单元格不包含超链接，这些方法将返回 null；如果单元格包含超链接，则将返回 GridHyperlink 对象。

- GridHyperlinkCollection.getHyperlink(GridCell 单元格)
- GridHyperlinkCollection.getHyperlink(int row,int column)
## **在新窗口或现有窗口中打开超链接**
如果您的 excel 文件包含链接到某些 URL 的超链接，例如<http://wwww.aspose.com/>然后将其加载到 GridWeb 中，然后超链接将在 target 属性设置为_空白的。这意味着，当您单击 GridWeb 单元格中的超链接时，它将在新窗口而不是现有窗口中打开。此外，如果您想在现有窗口中打开超链接，请将 GridHyperlink.Target 设置为_自己。
## **访问 GridWeb 的超链接对象 Cell**
下面的示例代码访问单元格 A1 的超链接。如果单元格 A1 包含超链接，则返回 GridHyperlink 对象，否则返回 null。
## **示例代码**
{{< gist "aspose-cells-gists" "5876dc77e47649b66bdb5deefb4b5639" "examples-cells-AccessHyperlinkobjectofGridWebCell-AccessHyperlinkobjectofGridWebCell.jsp" >}}
