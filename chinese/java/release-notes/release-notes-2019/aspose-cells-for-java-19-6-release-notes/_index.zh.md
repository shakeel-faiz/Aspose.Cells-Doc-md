﻿---
title: Aspose.Cells for Java 19.6 发行说明
type: docs
weight: 70
url: /zh/java/aspose-cells-for-java-19-6-release-notes/
---
{{% alert color="primary" %}} 

此页面包含 Aspose.Cells for Java 19.6 的发行说明。

{{% /alert %}} 

|**钥匙**|**概括**|**类别**|
|:- |:- |:- |
|CELLSJAVA-42914|大条件格式导致 OOM 异常|强化|
|CELLSJAVA-42916|Workbook.save() 后的数据格式问题|强化|
|CELLSJAVA-42930|Excel95加载失败|强化|
|CELLSJAVA-42927|删除列后保存的文件在 Excel 中打开速度很慢|强化|
|CELLSJAVA-42932|Style.getDisplayStyle 方法的条件格式错误|漏洞|
|CELLSJAVA-42928|XLSX 到 PDF 转换中有些行没有体现|漏洞|
|CELLSJAVA-42904|标题图像似乎损坏了文件|漏洞|
|CELLSJAVA-42907|保存工作簿后过滤器丢失|漏洞|
|CELLSJAVA-42915|将工作表添加到工作簿后更改过滤器|漏洞|
|CELLSJAVA-42918|转换后文件的图表扁平化（XLS 到 XLSX 转换）|漏洞|
|CELLSJAVA-42938|加载 XLSX 文件暂停应用程序|漏洞|
|CELLSJAVA-42859|从 ODS 文件加载名称的 CellsException|例外|
|CELLSJAVA-42908|调用 Name.getRefersTo() 时出现异常|例外|
|CELLSJAVA-42926|加载工作簿时出现 IllegalStateException|例外|

## **公共 API 和向后不兼容的更改**
以下是对公众 API 所做的任何更改的列表，例如添加、重命名、删除或弃用成员，以及对 Aspose.Cells for Java 所做的任何非向后兼容更改。如果您对列出的任何更改有疑虑，请在Aspose.Cells 支持论坛。
### **添加枚举 FileFormatType.FODS、FileFormatType.SXC、LoadFormat.FODS、LoadFormat.SXC、SaveFormat.FODS 和 SaveFormat.SXC**
表示 .FODS 和 .SXC 文件格式类型。
### **添加枚举 WarningType.UnsupportedFileFormat**
表示警告类型不支持的文件格式。
### **添加枚举 ODSGeneratorType**
表示ods的生成器类型。
### **OoxmlSaveOptions.EmbedOoxmlAsOleObject**
指示是否将 OOXML 文件嵌入为 OleObject。
### **添加 Row.CopySettings(Aspose.Cells.Row,System.Boolean)**
复制行的设置，例如样式、高度、可见性等。
