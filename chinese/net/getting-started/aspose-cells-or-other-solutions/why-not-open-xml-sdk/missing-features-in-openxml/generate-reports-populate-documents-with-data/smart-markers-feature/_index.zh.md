﻿---
title: Aspose.Cells 中的智能标记功能
type: docs
weight: 30
url: /zh/net/smart-markers-feature-in-aspose-cells/
---
**智能标记**用于让 Aspose.Cells 知道在 Microsoft Excel 设计器电子表格中放置哪些信息。智能标记允许您创建仅包含特定信息和格式的模板。
## **设计师电子表格和智能标记**
Designer 电子表格是标准的 Excel 文件，其中包含视觉格式、公式和智能标记。它们可以包含引用一个或多个数据源的智能标记，例如来自项目的信息和相关联系人的信息。智能标记被写入您需要信息的单元格中。

所有智能标记都以 &= 开头。 &=Party.FullName 是数据标记的示例。如果数据标记产生多个项目，例如，一个完整的行，则随后的行将自动向下移动以为所有新信息腾出空间。因此，小计和总计可以放在数据标记之后的行上，以根据插入的数据进行计算。要对插入的行进行计算，请使用动态公式。

智能标记包括**数据源**和**字段名称**大多数信息的部分。特殊信息也可以与变量和变量数组一起传递。变量始终只填充一个单元格，而变量数组可能填充多个单元格。每个细胞只使用一个数据标记。未使用的智能标记将被删除。

智能标记也可能包含参数。参数允许您修改信息的布局方式。它们作为逗号分隔列表附加到括号中智能标记的末尾。
### **智能标记选项**
- &=数据源.字段名
- &=数据源.字段名
- &=$变量名
- &=$变量数组
- &==动态公式
- &=&=重复动态公式
### **参数**
允许使用以下参数：

- noadd - 不要添加额外的行来适应数据。
- skip:n - 为每行数据跳过 n 行。
- ascending:n 或 descending:n - 在智能标记中对数据进行排序。如果 n 为 1，则该列是排序器的第一个键。对数据源进行处理后对数据进行排序。例如 &=Table1.Field3（升序：1）。
- horizontal - 从左到右而不是从上到下写入数据。
- 数字 - 如果可能，将文本转换为数字。仅在 .NET 版本中受支持。
- shift - 向下或向右移动，创建额外的行或列以适应数据。 shift 参数的工作方式与 Microsoft Excel 中的相同。例如在 MS Excel 中，当您选择一系列单元格时，右键单击并选择插入并指定向下移动单元格、向右移动单元格和其他选项。简而言之，shift 参数为垂直/正常（从上到下）或水平（从左到右）智能标记填充相同的功能。
- copystyle - 将基本单元格的样式复制到该列中的所有单元格。

参数**没有添加**和 skip 可以组合以在交替行上插入数据。因为模板是从下往上处理的，所以你应该在第一行添加noadd以避免在备用行之前插入额外的行。

本节包括以下主题

- [分组数据在 Aspose.Cells](/cells/zh/net/grouping-data-in-aspose-cells/)
- [Aspose.Cells 中的图像标记](/cells/zh/net/image-markers-in-aspose-cells/)
- [在 Aspose.Cells 中使用匿名类型或自定义对象](/cells/zh/net/using-anonymous-types-or-custom-objects-in-aspose-cells/)
- [在 Aspose.Cells 中使用嵌套对象](/cells/zh/net/using-nested-objects-in-aspose-cells/)
