﻿---
title: Aspose.Cells for .NET 22.9 发行说明
type: docs
weight: 4
url: /zh/net/aspose-cells-for-net-22-9-release-notes/
---
{{% alert color="primary" %}}

此页面包含发行说明[Aspose.Cells for .NET 22.9](https://www.nuget.org/packages/Aspose.Cells/22.9.0).

{{% /alert %}}

|**钥匙**|**概括**|**类别**|
|:- |:- |:- |
|CELLSNET-51935|支持xls文件的离散组数据|
|CELLSNET-51925|支持渐变填充的预设渐变设置|
|CELLSNET-51740|支持为数据表设置表格公式|
|CELLSNET-51853|支持将 ozm 转换为 lbm 以实现 CONVERT 功能|
|CELLSNET-51931|提高用户对 Style.Custom 输入的识别为内置|
|CELLSNET-51709|支持 .Numbers 工作表中的多个表|
|CELLSNET-51810|支持将空单元格导出为 null 到 Json|
|CELLSNET-51811|增强检测首行是否为表头行的功能|
|CELLSNET-51910|支持将带有 ThemeColor 的轮廓边框应用于范围|
|CELLSNET-51928|支持xlsb的SHA-512算法读写保护范围|
|CELLSNET-51743|将 Excel 文件转换为 PDF 后，一些符号发生了变化|
|CELLSNET-51747|mm 变成“？？” PDF格式|
|CELLSNET-50960|重新保存的 XLSM 文件（包含数据透视表）已损坏|
|CELLSNET-51506|generated 文件中的外部连接已损坏|
|CELLSNET-51735|将 Excel 数据透视表转换为 PDF 时文本粗体样式错误|
|CELLSNET-51761|当带有数据透视表的 XLS 文件转换为 XLSM 时，数据连接详细信息被删除|
|CELLSNET-51899|XLS 到 XLSM 的转换 - MS Excel 无法打开输出 XLSM 文件|
|CELLSNET-51716|动态数组公式不会填充溢出的单元格|
|CELLSNET-51753|某些公式未计算以在更改选择时更新工作表中的数据|
|CELLSNET-51800|来自 XLSX 的值在输出 PDF 中不正确|
|CELLSNET-51801|使用计算链计算后，工作簿的重新计算速度很慢|
|CELLSNET-51897|HLOOKUP 值不正确|
|CELLSNET-51187|垂直虚线与图表中轴上的标签未对齐以呈现 SVG|
|CELLSNET-51734|System.Security.Cryptography.Pkcs 6.0.1 依赖需要 .NET Core 3.1|
|CELLSNET-51912|将 Excel 转换为 PDF 时，生成的 PDF 无法正确显示轴|
|CELLSNET-51744|Gridweb 一直往回跳|
|CELLSNET-51608|将 Excel 导出到 docker 上的 HTML 时，数字隐藏在红色/绿色圆圈后面（Azure 云 kubernetes）|
|CELLSNET-51864|使用 HorizontalPageBreaks 计算“PageSetup.Zoom”时出现问题|
|CELLSNET-51938|XLSX 到 PDF：字符间距错误|
|CELLSNET-51226|在 Excel 工作簿中为图表/组添加标识符属性|
|CELLSNET-51461|Excel中的数据添加了不必要的边框到DOCX转换|
|CELLSNET-51736|Cell 边界在结果 PDF 中丢失|
|CELLSNET-51738|单个单元格的无效记录导致生成的文件损坏|
|CELLSNET-51760|Worksheet.AutoFitColumns 无法正常工作|
|CELLSNET-51770|保存为 PowerPoint 文件时，合并的 Cells 无法正常工作|
|CELLSNET-51771|合并单元格后，生成的 PowerPoint 文件中的一些数据丢失|
|CELLSNET-51772|将 XLS 文件转换为 XLSM 时连接信息发生变化|
|CELLSNET-51778|将 XLS 文件转换为 XLSM 会删除命名范围中链接末尾的几个字符|
|CELLSNET-51785|DOCX >> Html 表格 >> Excel 工作表未正确转换|
|CELLSNET-51825|AutoFit 在 v22.1.0 和 v22.8.0 中的工作方式不同|
|CELLSNET-51829|XLS 到 XLSM 文件转换导致一些自定义属性丢失|
|CELLSNET-51830|在为特定文件创建工作簿后过早处理输入文档流|
|CELLSNET-51865|XLS 工作表没有数据，而您可以在 Excel 中看到填充的行|
|CELLSNET-51880|XLSB 到 XLSM 转换 - 输出 XLSM 文件已损坏|
|CELLSNET-51898|XLS 到 XLSM 转换 - 输出 XLSM 文件已损坏|
|CELLSNET-51921|如果不将其标志设置为显式或使用标志，则无法应用复制的样式|
|CELLSNET-51922|Cell 打开并重新保存 XLSX 文件后保护丢失|
|CELLSNET-51923|导入数据时，DataTable 列标题属性未在输出 Excel 中得到尊重和呈现|
|CELLSNET-51924|图表文本元素中的区域设置不正确|
|CELLSNET-51944|内置样式的名称不会根据地区自动更改|
|CELLSNET-51848|计算工作簿抛出 Stackoverflow 异常|
|CELLSNET-51965|将会计格式的 XLSX 文件导入 Aspose.Cells.GridDesktop 时出现异常|
|CELLSNET-51961|将 ODS 渲染到 PDF 时出现异常“索引超出范围”|
|CELLSNET-51863|CollectionBase.Exists 中的 System.StackOverflowException|

## **公共 API 和向后不兼容的更改**

以下是对公众 API 所做的任何更改的列表，例如添加、重命名、删除或弃用成员，以及对 Aspose.Cells for .NET 所做的任何非向后兼容更改。如果您对列出的任何更改有疑虑，请在Aspose.Cells 支持论坛。

### **添加 Cell.SetTableFormula(...) 方法**

支持为单元格区域设置公式，创建双变量数据表和单变量数据表。

### **添加 Cell.SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, object[][] values, bool calculateRange, bool calculateValue, CalculationOptions copts) 方法**

支持设置自定义计算选项的动态数组公式，特别是当公式中有需要用户自定义引擎计算的函数时。

### **添加 Workbook.RefreshDynamicArrayFormulas(bool calculate, CalculationOptions copts) 方法**

支持刷新带有自定义选项的动态数组公式进行计算，特别是当动态数组公式中有需要用户自定义计算引擎的函数时。

### **添加 ChartFrame.TextOptions 属性。**

表示图表文本的字体选项。

### **添加 ExportRangeToJsonOptions.ExportEmptyCells 属性。**

指示是否在单元格为空时导出 null。

### **添加 NumbersLoadOptions 构造函数。**

代表加载号码的选项。

### **添加枚举 LoadNumbersTableType。**

表示在 Mac.numbers 的工作表中加载多表的类型。

### **添加 ProtectedRange.IsProtectedWithPassword 属性。**

指示范围是否受密码保护。

### **添加 ImportTableOptions.ExportCaptionAsFieldName 属性**

导入数据表时是否将标题导出为字段名。

### **添加 TextOptions.LanguageCode 属性。**

获取和设置字体的语言代码。

### **添加枚举 PresetThemeGradientType。**

代表预设的主题渐变类型。

### **添加 GradientFill.SetPresetThemeGradient() 方法。**

设置预设主题渐变类型。

### **添加覆盖 Style.SetBorder() 方法。**

设置各种颜色的边框。

### **添加 Range.SetOutlineBorder() 和 Range.SetOutlineBorders() 方法**

用各种颜色设置范围的边界。
