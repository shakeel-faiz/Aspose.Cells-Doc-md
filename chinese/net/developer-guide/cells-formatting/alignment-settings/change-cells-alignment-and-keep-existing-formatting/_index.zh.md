﻿---
title: 更改 Cells 对齐并保持现有格式
type: docs
weight: 340
url: /zh/net/change-cells-alignment-and-keep-existing-formatting/
---
## **可能的使用场景**

有时，您想要更改多个单元格的对齐方式，但又想保留现有格式。 Aspose.Cells 允许您使用[**StyleFlag.Alignments**](https://reference.aspose.com/cells/net/aspose.cells/styleflag/properties/alignments)财产。如果你会设置它**真的** 否则不会发生对齐方式的变化。请注意，[**风格旗帜**](https://reference.aspose.com/cells/net/aspose.cells/styleflag)对象作为参数传递给[**范围.ApplyStyle()**](https://reference.aspose.com/cells/net/aspose.cells/range/methods/applystyle)实际上将格式应用于一系列单元格的方法。

## **更改 Cells 对齐并保持现有格式**

下面的示例代码加载[示例 Excel 文件](67338585.xlsx) , 创建范围并居中水平和垂直对齐并保持现有格式不变。以下屏幕截图比较了示例 Excel 文件和[输出Excel文件](67338586.xlsx)并显示单元格的所有现有格式都是相同的，除了单元格现在水平和垂直居中对齐。

![待办事项：图片_替代_文本](change-cells-alignment-and-keep-existing-formatting_1.png)

## **示例代码**

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Data-ChangeCellsAlignmentAndKeepExistingFormatting.cs" >}}
