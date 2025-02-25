﻿---
title: Aspose.Cells for .NET 22.11 发行说明
type: docs
weight: 2
url: /zh/net/aspose-cells-for-net-22-11-release-notes/
---
{{% alert color="primary" %}}

此页面包含发行说明[Aspose.Cells for .NET 22.11](https://www.nuget.org/packages/Aspose.Cells/22.11.0).

{{% /alert %}}

|**钥匙**|**概括**|**类别**|
|:- |:- |:- |
|CELLSNET-52026|支持复制时间轴|
|CELLSNET-52022|区分或区分 CSE 遗留数组公式和普通数组公式|
|CELLSNET-52156|将 XLSX 保存到 HTML 时禁用合并表格单元格|
|CELLSNET-52159|支持在将 html 转换为 excel 时解析折叠属性|
|CELLSNET-51939|XLSX 到 PDF：内容错位|
|CELLSNET-51940|XLS 到 PDF：单元格中的内容未对齐|
|CELLSNET-52068|XLSX 至 PDF：形状丢失/布局折叠|
|CELLSNET-52092|Excel图形中的字符打印和间距被截断|
|CELLSNET-52186|将 XLSX 文档转换为 PDF 时形状/框为空|
|CELLSNET-52225|XLSX 到 PDF 文本框中的字符反转|
|CELLSNET-52086|生成的文件中的外部连接已损坏|
|CELLSNET-52133|Excel公式在重新保存的xlsb文件中用花括号括起来|
|CELLSNET-52158|不正确的循环引用检测|
|CELLSNET-52174|Cell.IsArrayFormula 在从 xlsb 模板文件中读取后对于数组公式是错误的|
|CELLSNET-52217|某些大数的查找函数计算不正确|
|CELLSNET-52221|XLOOKUP 的动态数组公式未正确溢出|
|CELLSNET-52232|从外部链接的工作表名称中删除单引号|
|CELLSNET-52198|将图表转换为图像文件时出现重叠问题|
|CELLSNET-52043|使用 HorizontalPageBreaks 计算“PageSetup.Zoom”时出现问题|
|CELLSNET-52157|转换为 pdf 时页面边框与文本重叠|
|CELLSNET-52118|在 OpenOffice 和 LibreCalc 中将 html 设置为单元格时，不同格式的结果不一致|
|CELLSNET-52125|索引超出范围。用图片复制|
|CELLSNET-52143|将 XLS 文件转换为 XLSM 时链接的关系类型发生变化|
|CELLSNET-52144|XLS 到 XLSM 转换更改链接关系类型|
|CELLSNET-52151|保存 xlsb 用最后一条评论替换所有评论|
|CELLSNET-52152|通过Aspose.Cells应用AutoFit行操作时行高值不正确|
|CELLSNET-52155|范围复制后条件格式丢失|
|CELLSNET-52181|XLSX 至 HTML：Cells 范围未正确导出|
|CELLSNET-52214|最后一行内容在输出 Excel 文件中被截断|
|CELLSNET-52236|智能标记（组：合并）不适用于合并的单元格|
|CELLSNET-52241|文档中的框（形状）未出现在输出中 PDF|
|CELLSNET-52243|保存工作簿时修改 VBA 项目会抛出错误|

## **公共 API 和向后不兼容的更改**

以下是对公众 API 所做的任何更改的列表，例如添加、重命名、删除或弃用成员，以及对 Aspose.Cells for .NET 所做的任何非向后兼容更改。如果您对列出的任何更改有疑虑，请在Aspose.Cells 支持论坛。

### **添加 Cell.IsDynamicArrayFormula 属性**

指示单元格的公式是动态数组公式 (true) 还是遗留数组公式 (false)。

### **废弃 SparklineGroup.SparklineCollection 属性并添加 SparklineGroup.Sparklines 属性**

请改用 SparklineGroup.Sparklines 属性。

### **废弃 Worksheet.SparklineGroupCollection 属性并添加 Worksheet.SparklineGroups 属性**

请改用 Worksheet.SparklineGroups 属性。
