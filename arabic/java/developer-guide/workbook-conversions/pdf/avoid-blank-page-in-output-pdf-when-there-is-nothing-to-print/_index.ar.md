﻿---
title: تجنب الصفحة الفارغة في الإخراج PDF عندما لا يوجد شيء للطباعة
type: docs
weight: 30
url: /ar/java/avoid-blank-page-in-output-pdf-when-there-is-nothing-to-print/
---
## **سيناريوهات الاستخدام الممكنة**

عندما يكون ملف Excel فارغًا ويقوم المستخدم بحفظه في PDF باستخدام Aspose.Cells ، فإنه يعرض صفحة فارغة في الإخراج PDF. أحيانًا يكون هذا السلوك الافتراضي غير مرغوب فيه. يوفر Aspose.Cells ملف[**PdfSaveOptions.OutputBlankPageWhenNothingToPrint**](https://reference.aspose.com/cells/java/com.aspose.cells/pdfsaveoptions#OutputBlankPageWhenNothingToPrint) خاصية للتعامل مع هذه القضية. إذا قمت بتعيينه على أنه**خاطئة**، ومن بعد[**CellsException**](https://reference.aspose.com/cells/java/com.aspose.cells/CellsException)سيحدث عندما لا يوجد شيء يمكن طباعته في الإخراج PDF.

## **تجنب الصفحة الفارغة في الإخراج PDF عندما لا يوجد شيء للطباعة**

يقوم نموذج التعليمات البرمجية التالي بإنشاء مصنف فارغ ثم يحفظه كإخراج PDF بعد تعيين ملف[**PdfSaveOptions.OutputBlankPageWhenNothingToPrint**](https://reference.aspose.com/cells/java/com.aspose.cells/pdfsaveoptions#OutputBlankPageWhenNothingToPrint) الملكية مثل**خاطئة**. نظرًا لعدم وجود شيء يمكن طباعته في الإخراج PDF ، فإن ملف[**CellsException**](https://reference.aspose.com/cells/java/com.aspose.cells/CellsException)يحدث كما هو موضح أدناه.

## **عينة من الرموز**

{{< gist "aspose-cells-gists" "5876dc77e47649b66bdb5deefb4b5639" "Rendering-AvoidBlankPageInOutputPdfWhenThereIsNothingToPrint.java" >}}

## **استثناء**

{{< highlight "java" >}}

 Exception in thread "main" com.aspose.cells.CellsException: There is nothing to output/print.

	at com.aspose.cells.zcab.a(Unknown Source)

	at com.aspose.cells.zcab.a(Unknown Source)

	at com.aspose.cells.zcab.a(Unknown Source)

	at com.aspose.cells.Workbook.a(Unknown Source)

	at com.aspose.cells.Workbook.save(Unknown Source)

{{< /highlight >}}
