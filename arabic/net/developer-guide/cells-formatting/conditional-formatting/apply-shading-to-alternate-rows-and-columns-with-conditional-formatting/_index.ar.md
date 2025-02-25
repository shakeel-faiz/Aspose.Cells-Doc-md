﻿---
title: تطبيق التظليل على الصفوف والأعمدة البديلة بالتنسيق الشرطي
type: docs
weight: 30
url: /ar/net/apply-shading-to-alternate-rows-and-columns-with-conditional-formatting/
---
{{% alert color="primary" %}}

 توفر واجهات برمجة التطبيقات Aspose.Cells وسائل لإضافة قواعد التنسيق الشرطي ومعالجتها لـ[**ورقة عمل**](https://reference.aspose.com/cells/net/aspose.cells/worksheet)موضوع. يمكن تخصيص هذه القواعد بعدة طرق للحصول على التنسيق المطلوب بناءً على الشروط أو القواعد. ستوضح هذه المقالة استخدام واجهات برمجة تطبيقات Aspose.Cells for .NET لتطبيق التظليل على صفوف وأعمدة بديلة بمساعدة قواعد التنسيق الشرطي والوظائف المضمنة في Excel.

{{% /alert %}}

تستخدم هذه المقالة الوظائف المضمنة في Excel مثل ROW و COLUMN & MOD. فيما يلي بعض التفاصيل حول هذه الوظائف من أجل فهم أفضل لمقتطف الشفرة المقدم مسبقًا.

- **صف()** تقوم الدالة بإرجاع رقم الصف لمرجع الخلية. إذا تم حذف المعلمة المرجعية ، فإنها تفترض أن المرجع هو عنوان الخلية التي تم إدخال الدالة ROW فيها.
- **عمود()** تقوم الدالة بإرجاع رقم العمود لمرجع الخلية. إذا تم حذف المعلمة المرجعية ، فإنها تفترض أن المرجع هو عنوان الخلية التي تم إدخال الدالة COLUMN فيها.
- **عصري()** تُرجع الدالة الباقي بعد قسمة الرقم على القاسم ، حيث تكون المعلمة الأولى للدالة هي القيمة الرقمية التي ترغب في العثور على الباقي والمعلمة الثانية هي الرقم المستخدم للقسمة على معامل الرقم. إذا كان المقسوم عليه 0 ، فسيتم إرجاع # DIV / 0! خطأ.

لنبدأ في كتابة بعض التعليمات البرمجية لتحقيق هذا الهدف بمساعدة Aspose.Cells for .NET API.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Articles-ManageConditionalFormatting-ApplyShadingToAlternateRowsColumns-1.cs" >}}

تُظهر اللقطة التالية جدول البيانات الناتج الذي تم تحميله في تطبيق Excel.

|![ما يجب القيام به: image_بديل_نص](apply-shading-to-alternate-rows-and-columns-with-conditional-formatting_1.png)|
|:- |

 لتطبيق التظليل على أعمدة بديلة ، كل ما عليك فعله هو تغيير الصيغة**= MOD (ROW ()، 2) = 0** مثل**= MOD (عمود () ، 2) = 0** ، هذا هو؛ بدلاً من الحصول على فهرس الصف ، قم بتعديل الصيغة لاسترداد فهرس العمود.
سيبدو جدول البيانات الناتج ، في هذه الحالة ، على النحو التالي.

|![ما يجب القيام به: image_بديل_نص](apply-shading-to-alternate-rows-and-columns-with-conditional-formatting_2.png)|
|:- |
