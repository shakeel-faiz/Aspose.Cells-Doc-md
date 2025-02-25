﻿---
title: Aspose.Cells for .NET 22.10 发行说明
type: docs
weight: 3
url: /zh/net/aspose-cells-for-net-22-10-release-notes/
---
{{% alert color="primary" %}}

此页面包含发行说明[Aspose.Cells for .NET 22.10](https://www.nuget.org/packages/Aspose.Cells/22.10.0).

{{% /alert %}}

|**钥匙**|**概括**|**类别**|
|:- |:- |:- |
|CELLSNET-42037|数据透视表时间线筛选器在加载 excel 文档和更新后消失|
|CELLSNET-51963|支持 CRTX 文件|
|CELLSNET-51952|MAXIFS 公式需要很长时间才能计算|
|CELLSNET-52064|使用 Cells.InsertRows 方法时，不允许将非空单元格推离工作表错误的末尾|
|CELLSNET-52029|根据语言环境/区域设置翻译图例条目标签|
|CELLSNET-51419|将 XLS 文件转换为 XLSM 时，数据透视表的外部链接被删除|
|CELLSNET-51984|XLSX 数据透视表文件在重新保存后损坏|
|CELLSNET-51987|数据透视表和数据透视图中的一些智能标记（插入）出现问题|
|CELLSNET-52065|转换外部连接时错误的外部数据连接|
|CELLSNET-52088|创建经典数据透视表时添加额外的行|
|CELLSNET-52018|使用 NotBetween 运算符的 GetValidationValue 不正确|
|CELLSNET-52069|Cell.Formula 结果中的十进制值可能与 ms excel 显示的不同|
|CELLSNET-52078|Style.SetPatternColor(BackgroundType,Color,Color) 不生效|
|CELLSNET-52105|LightCellsDataHandler.StartSheet(Worksheet) 在为 xlsb 模板文件返回 false 时无法跳过工作表|
|CELLSNET-46764|转换为 pdf 时缺少图表标题|
|CELLSNET-52049|XLSX 到 PDF：文本格式不正确|
|CELLSNET-52073|关于 Excel 中 Arial Tur 字体的问题到 PDF 渲染|
|CELLSNET-52083|一些具有会计数字格式的单元格呈现为#####。|
|CELLSNET-52091|将工作表内容设置为黑白时，它仍然以彩色打印并且不必要地显示边框|
|CELLSNET-51972|复制工作表时无法正确识别包含按钮对象的工作表|
|CELLSNET-51973|HTML 表格到 Excel 工作表未正确转换|
|CELLSNET-52001|重新保存 XLSX 文件生成损坏的文件|
|CELLSNET-52015|无法从 Excel 文件加载幂查询公式|
|CELLSNET-52054|保存并重新打开 Aspose.Cells 生成的工作簿后样式损坏|
|CELLSNET-52056|超链接重复问题|
|CELLSNET-52071|Excel 到 XML 的转换 - 元素名称未转义|
|CELLSNET-52074|HTML 到 XLSX：缺少单元格内容|
|CELLSNET-52084|“Northwind Traders”文本的位置不正确（左缩进值未正确解释）。|
|CELLSNET-52063|PivotTable.CalculateData 导致 NullReferenceException|
|CELLSNET-51986|使用启用的计算链计算工作簿两次导致异常|
|CELLSNET-52081|打开样式已被删除的 XLSX 文件抛出异常|
|CELLSNET-52044|在 GridWeb 中导入客户文件时出现异常|
|CELLSNET-52002|尝试使用密码打开未受保护的文档时抛出异常|

## **公共 API 和向后不兼容的更改**

以下是对公众 API 所做的任何更改的列表，例如添加、重命名、删除或弃用成员，以及对 Aspose.Cells for .NET 所做的任何非向后兼容更改。如果您对列出的任何更改有疑虑，请在Aspose.Cells 支持论坛。

### **更改了将单元格移出工作表以插入行的限制**

在旧版本中，如果单元格有格式设置但没有值，将被移出工作表，则不允许插入操作。从 22.10 开始，允许对这种情况进行插入操作，这种行为现在与 ms excel 相同。

### **添加 DataModelConnection 类**

指定数据模型连接。

### **添加 Chart.ChangeTemplate(byte[]) 方法**

使用预设模板文件更改图表类型。

### **添加 ChartCollection.Add(byte[] data, string dataRange, bool isVertical, int topRow, int leftColumn,int rightRow, int bottomColumn) 方法。**

添加带有预设模板文件的图表。
