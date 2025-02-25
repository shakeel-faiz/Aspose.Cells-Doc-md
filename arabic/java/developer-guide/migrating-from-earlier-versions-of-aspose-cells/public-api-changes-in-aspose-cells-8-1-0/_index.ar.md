﻿---
title: API العام التغييرات في Aspose.Cells 8.1.0
type: docs
weight: 50
url: /ar/java/public-api-changes-in-aspose-cells-8-1-0/
---
{{% alert color="primary" %}} 

يصف هذا المستند التغييرات التي تم إجراؤها على Aspose.Cells API من الإصدار 8.0.2 إلى 8.1.0 ، والتي قد تهم مطوري الوحدة / التطبيق. لا يشمل فقط الأساليب العامة الجديدة والمحدثة ، بل يشمل أيضًا وصفًا لأي تغييرات في السلوك خلف الكواليس في Aspose.Cells.

{{% /alert %}} 
## **تمت إضافة خاصية HtmlSaveOptions.ExportHiddenWorksheet**
كشفت فئة HtmlSaveOptions عن خاصية ExportHiddenWorksheet التي يمكن استخدامها لتحديد ما إذا كان سيتم تصدير أوراق العمل المخفية بتنسيق HTML. القيمة الافتراضية هي الحقيقية. بينما إذا تم الضبط على "خطأ" ، فلن يقوم Aspose.Cells بتصدير محتويات ورقة العمل المخفية.

{{% alert color="primary" %}} 

 يرجى مراجعة المقال المفصل على[منع تصدير ورقة العمل المخفية](/cells/ar/java/prevent-exporting-hidden-worksheet-contents-on-saving-to/)

{{% /alert %}}
## **تمت إضافة Cell.StringValueWithoutFormat خاصية**
 تمت إضافة خاصية StringValueWithoutFormat إلى الفئة Cell ، من أجل تسهيل استرجاع المطورين لقيمة الخلية دون تطبيق أي تنسيق.

يوضح مقتطف الكود أدناه استخدام طريقة Cell.getStringValueWithoutFormat مقارنةً بالخلية cell.getDisplayStringValue عن طريق إنشاء جدول بيانات من البداية وتطبيق تنسيق الأرقام على إحدى الخلايا.

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

إخراج الكود أعلاه على النحو التالي

قيمة السلسلة المنسقة: 123،456
قيمة السلسلة غير المنسقة: 123456

{{% /alert %}}
## **البايت المتقادمة ، الأحرف ، الأحرف مع المسافات ، الخطوط ، خصائص الفقرات**
 تم تمييز العديد من العقارات من فئة BuiltInDocumentPropertyCollection بأنها قديمة بدءًا من Aspose.Cells for .NET 8.1.0. تتضمن هذه الخصائص Bytes و Characters و CharactersWithSpaces و Lines & Paragraphs. السبب هو أن الخصائص المذكورة أعلاه لا تفيد في الحفاظ على جداول بيانات Excel لأن Excel يغفلها. حيث تمت كتابة هذه الخصائص في الأصل لمستندات Word والعروض التقديمية PowerPoint.
