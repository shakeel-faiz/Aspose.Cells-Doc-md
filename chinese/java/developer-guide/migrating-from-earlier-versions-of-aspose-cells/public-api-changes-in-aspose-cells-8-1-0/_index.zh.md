﻿---
title: 公共 API Aspose.Cells 8.1.0 的变化
type: docs
weight: 50
url: /zh/java/public-api-changes-in-aspose-cells-8-1-0/
---
{{% alert color="primary" %}} 

本文档描述了 Aspose.Cells API 从版本 8.0.2 到 8.1.0 的更改，模块/应用程序开发人员可能会感兴趣。它不仅包括新的和更新的公共方法，还包括对 Aspose.Cells 中幕后行为的任何更改的描述。

{{% /alert %}} 
## **添加了 HtmlSaveOptions.ExportHiddenWorksheet 属性**
HtmlSaveOptions 类公开了 ExportHiddenWorksheet 属性，可用于指定隐藏工作表是否导出为 HTML 格式。默认值是true。而如果设置为 false，Aspose.Cells 将不会导出隐藏的工作表内容。

{{% alert color="primary" %}} 

请查看详细文章[防止导出隐藏的工作表](/cells/zh/java/prevent-exporting-hidden-worksheet-contents-on-saving-to/)

{{% /alert %}}
## **添加了 Cell.StringValueWithoutFormat 属性**
StringValueWithoutFormat 属性已添加到 Cell 类，以方便开发人员在不应用任何格式的情况下检索单元格值。

下面提供的代码片段演示了 Cell.getStringValueWithoutFormat 方法与 cell.getDisplayStringValue 方法的用法，方法是从头开始创建电子表格并将数字格式应用于其中一个单元格。

**Java**

{{< highlight "csharp" >}}

 //Create an instance of Workbook

Workbook book = new Workbook();

//Access first worksheet

Worksheet sheet = book.getWorksheets().get(0);

//Access A1 cell

Cell cell = sheet.getCells().get("A1");

//Put a value cell and convert it to number

cell.putValue("123456", true);

//Create a new Style object and add it to Workbook's Style Collection

int index = book.getStyles().add();

Style style = book.getStyles().get(index);

//Set Number format for Style object

style.setNumber(3);

//Create an instance of StyleFlag class

//and set NumberFormat to true

StyleFlag flag = new StyleFlag();

flag.setNumberFormat(true);

//Set the style of A1 cell

cell.setStyle(style, flag);

//Get formatted string value 

String formatted = cell.getDisplayStringValue();

System.out.println("Formatted String Value: " +formatted);

//Get un-formatted string value

String unformatted = cell.getStringValueWithoutFormat();

System.out.println("Un-formatted String Value: " + unformatted);

{{< /highlight >}}

{{% alert color="primary" %}} 

以上代码输出如下

格式化字符串值：123,456
未格式化的字符串值：123456

{{% /alert %}}
## **废弃的字节、字符、CharactersWithSpaces、行、段落属性**
从 Aspose.Cells for .NET 8.1.0 开始，BuiltInDocumentPropertyCollection 类的许多属性已被标记为过时。这些属性包括字节、字符、带空格的字符、行和段落。原因是，上述属性对 Excel 电子表格的保护没有用，因为 Excel 忽略了它们。这些属性最初是为 Word 文档和 PowerPoint 演示文稿编写的。
