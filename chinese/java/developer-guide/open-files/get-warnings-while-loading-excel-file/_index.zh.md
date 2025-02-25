﻿---
title: 加载 Excel 文件时收到警告
type: docs
weight: 60
url: /zh/java/get-warnings-while-loading-excel-file/
---
## **可能的使用场景**

有时，用户尝试加载有些损坏但可加载的工作簿。在这种情况下，Aspose.Cells 在加载工作簿时会引发警告。您可以通过实施**[IWarningCallback](https://reference.aspose.com/cells/java/com.aspose.cells/IWarningCallback)**界面与设置**[LoadOptions.WarningCallback](https://reference.aspose.com/cells/java/com.aspose.cells/loadoptions#WarningCallback)**财产。

## **加载 Excel 文件时收到警告**

以下示例代码解释了如何在加载 excel 文件时获取警告。代码加载[示例 excel 文件](sampleDuplicateDefinedName.xlsx)哪个抛出**[DuplicateDefinedName](https://reference.aspose.com/cells/java/com.aspose.cells/warningtype#DUPLICATE_DEFINED_NAME)**加载警告。这个警告然后被捕获**[IWarningCallback.Warning()](https://reference.aspose.com/cells/java/com.aspose.cells/iwarningcallback#warning(com.aspose.cells.WarningInfo))**在控制台上打印警告消息的方法。然后代码将工作簿另存为[输出excel文件](outputDuplicateDefinedName.xlsx).如果您在 Microsoft Excel 中打开示例 excel 文件，它也会向您显示此屏幕截图所示的警告。另请检查下面给出的代码的控制台输出以获得更多理解。

![待办事项：图片_替代_文本](get-warnings-while-loading-excel-file_1.png)

## **示例代码**

{{< gist "aspose-cells-gists" "5876dc77e47649b66bdb5deefb4b5639" "Examples-src-main-java-com-aspose-cells-examples-loading_saving-WarningCallback-WarningCallback.java" >}}

{{< gist "aspose-cells-gists" "5876dc77e47649b66bdb5deefb4b5639" "Examples-src-main-java-com-aspose-cells-examples-loading_saving-GetWarningLoadingAnExcel-GetWarningLoadingAnExcel.java" >}}

## **控制台输出**

这是使用提供的执行时上述代码的控制台输出[示例 excel 文件](sampleDuplicateDefinedName.xlsx).

{{< highlight "java" >}}

Duplicate Defined Name Warning: Name:PRINT_AREA;ReferTo:Introduction!$D$16:$D$17

Duplicate Defined Name Warning: Name:PRINT_AREA;ReferTo:Panel!$B$228

Duplicate Defined Name Warning: Name:PRINT_AREA;ReferTo:'Queries '!$D$14:$D$16

{{< /highlight >}}
