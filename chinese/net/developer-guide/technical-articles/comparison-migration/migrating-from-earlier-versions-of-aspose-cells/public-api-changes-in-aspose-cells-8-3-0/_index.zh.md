﻿---
title: 公共 API Aspose.Cells 8.3.0 的变化
type: docs
weight: 100
url: /zh/net/public-api-changes-in-aspose-cells-8-3-0/
---
{{% alert color="primary" %}} 

本文档描述了 Aspose.Cells API 从版本 8.2.2 到 8.3.0 的变化，模块/应用程序开发人员可能会感兴趣。

{{% /alert %}} 
## **添加的 API**
### **属性 WorkbookSettings.AutoRecover 添加**
新属性 AutoRecover 已添加到 WorkbookSettings 类，以允许开发人员为其应用程序中的电子表格设置自动恢复选项。

{{% alert color="primary" %}} 

请检查文章[设置电子表格自动恢复](http://aspose.com/docs/display/cellsnet/How+to+set+AutoRecover+property+of+Workbook)想要查询更多的信息。

{{% /alert %}} 

**C#**

{{< highlight "csharp" >}}

 var book = new Workbook("sample.xlsx");

var settings = book.Settings;

settings.AutoRecover = true;

{{< /highlight >}}


### **已添加属性 WorkbookSettings.CrashSave**
布尔类型属性 CrashSave 已添加到 WorkbookSettings 类，指示应用程序是否在崩溃后最后保存了工作簿文件。

**C#**

{{< highlight "csharp" >}}

 var book = new Workbook("sample.xlsx");

var settings = book.Settings;

Console.WriteLine(settings.CrashSave);

{{< /highlight >}}


### **已添加属性 WorkbookSettings.DataExtractLoad**
属性 DataExtractLoad 已添加到 WorkbookSettings 类，以便开发人员能够获取有关上次恢复的信息。如果属性DataExtractLoad 返回true，则表明已经对电子表格进行了数据恢复。

**C#**

{{< highlight "csharp" >}}

 var book = new Workbook("sample.xlsx");

var settings = book.Settings;

Console.WriteLine(settings.DataExtractLoad);

{{< /highlight >}}


### **已添加属性 WorkbookSettings.RepairLoad**
属性 RepairLoad 指示电子表格是否已在上次使用 Excel 应用程序加载时修复。

**C#**

{{< highlight "csharp" >}}

 var book = new Workbook("sample.xlsx");

var settings = book.Settings;

Console.WriteLine(settings.RepairLoad);

{{< /highlight >}}


### **已添加属性 TxtLoadOptions.KeepExactFormat**
属性 KeepExactFormat 已添加到 TxtLoadOptions 类，指示在将字符串/文本转换为数字或 DateTime 时是否应为单元格值保留精确格式。添加此属性以匹配 MS Excel 应用程序从 CSV 文件加载日期时间或数值的行为。为了模拟 MS Excel 的行为，将 KeepExactFormat 属性设置为 false，而默认值为 true，因此单元格值将被格式化为 CSV 文件中的字符串。

**C#**

{{< highlight "csharp" >}}

 var options = new TxtLoadOptions();

options.KeepExactFormat = false;

var book = new Workbook("sample.csv", options);

{{< /highlight >}}


### **已添加属性 Shape.Id**
属性 Id 已添加到 Shape 类以唯一标识给定电子表格中的每个形状对象。这个新属性还有助于识别电子表格中的 Chart 对象，如下所示。

**C#**

{{< highlight "csharp" >}}

 var book = new Workbook("sample.xlsx");

foreach(Chart chart in book.Worksheets[0].Charts)

{

    var shape = (Shape)chart.ChartObject;

    Console.WriteLine(shape.Id);

}

{{< /highlight >}}


### **添加了方法 PlotArea.SetPositionAuto**
方法 SetPositionAuto 已添加到 PlotArea 类，有助于将图表的绘图区域设置为自动模式。

**C#**

{{< highlight "csharp" >}}

 var book = new Workbook("sample.xlsx");

var chart = book.Worksheets[0].Charts[0];

chart.PlotArea.SetPositionAuto();

{{< /highlight >}}
