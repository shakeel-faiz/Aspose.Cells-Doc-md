﻿---
title: عام API تغييرات في Aspose.Cells 8.1.2
type: docs
weight: 60
url: /ar/net/public-api-changes-in-aspose-cells-8-1-2/
---
{{% alert color="primary" %}} 

يصف هذا المستند التغييرات التي تم إجراؤها على Aspose.Cells API من الإصدار 8.1.1 إلى 8.1.2 ، والتي قد تهم مطوري الوحدة / التطبيق. لا يشمل فقط الأساليب العامة الجديدة والمحدثة ، بل يشمل أيضًا وصفًا لأي تغييرات في السلوك خلف الكواليس في Aspose.Cells.

{{% /alert %}} 
## **تمت إضافة دعم للتحذير في حالة حدوث استبدال للخط**
مع Aspose.Cells for .NET 8.1.2 ، تمت إضافة خصائص WarningInfo و WarningType وواجهة IWarningCallback و SaveOptions.WarningCallback و ImageOrPrintOptions.WarningCallback لتسهيل تلقي المستخدم تحذيرًا إذا حدث استبدال الخط أثناء تحويل جداول البيانات إلى صور أو PDF.

{{% alert color="primary" %}} 

 يرجى مراجعة المقال المفصل على[الحصول على تحذيرات لاستبدال الخط أثناء عرض جداول البيانات](http://aspose.com/docs/display/cellsnet/Get+Warnings+for+Font+Substitution+while+Rendering+Excel+File)

{{% /alert %}}
## **تم حذف خاصية PdfSaveOptions.ChartImageType القديمة**
قام Aspose.Cells for .NET 8.1.2 بإزالة خاصية PdfSaveOptions.ChartImageType القديمة من API العامة.
