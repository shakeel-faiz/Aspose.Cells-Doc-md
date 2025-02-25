﻿---
title: Aspose.Cells for Java 20.5 ملاحظات الإصدار
type: docs
weight: 20
url: /ar/java/aspose-cells-for-java-20-5-release-notes/
---
{{% alert color="primary" %}}

 تحتوي هذه الصفحة على ملاحظات الإصدار لـ[Aspose.Cells for Java 20.5](https://downloads.aspose.com/cells/java/new-releases/aspose.cells-for-java-20.5/).

{{% /alert %}}

|**مفتاح**|**ملخص**|**فئة**|
|:- |:- |:- |
|CELLSJAVA-43173|عندما يحتوي حقل المجموعة على قيمة فارغة ، فإن نتيجة الإجمالي الفرعي تفقد الإجمالي الفرعي للمجموعة الخالية|التعزيز|
|CELLSJAVA-43162|برنامج Excel إلى تقديم HTML - تستغرق عملية التحويل وقتًا طويلاً|خلل برمجي|
|CELLSJAVA-43164|HTML لتحويل Excel لا يحتفظ بتنسيقات rich text في المخرجات|خلل برمجي|
|CELLSJAVA-43166|لا يتم عرض النص الذي تم تدويره بشكل جيد في التحويل من XLSX إلى HTML|خلل برمجي|
|CELLSJAVA-43178|يتم فقد تنسيقات RichText عند تصدير الملف إلى HTML|خلل برمجي|
|CELLSJAVA-43165|تم استبدال السلسلة "20TT1" بالرقم 43850 أثناء التحويل CSV إلى XLSB|خلل برمجي|
|CELLSJAVA-43026|بعد تقديم المخطط إلى صورة ، قم بتغيير نمط تسميات البيانات ، والقيم ليست هي نفسها|خلل برمجي|
|CELLSJAVA-43154|تتداخل بعض نقاط الرسم البياني حسب التسمية|خلل برمجي|
|CELLSJAVA-43089|تم قلب المخطط النسيجي وقيم المحور غير متطابقة مع المخطط الأصلي في التحويل XLS إلى PDF|خلل برمجي|
|CELLSJAVA-43171|المستند تالف بعد نسخ الأوراق|خلل برمجي|
|CELLSJAVA-43172|مشكلة في العلامات الذكية في الخلايا المدمجة|خلل برمجي|
|CELLSJAVA-43183|استثناء "ClassCastException: ...." عند حساب PivotTable|استثناء|
|CELLSJAVA-43177|ينتج عن المصنف الجديد الذي يحتوي على ملف CSV "java.lang.IndexOutOfBoundsException: مللي ثانية"|استثناء|
|CELLSJAVA-43168|استثناء "IllegalStateException: هذا ليس ملف تخزين منظم" عند دمج ملفات Excel|استثناء|
|CELLSJAVA-43179|NumberFormatException الاستثناء: لسلسلة الإدخال: "keep"|استثناء|
|CELLSJAVA-43182|استثناء 'lang.IllegalStateException: ترميز غير صالح: فارغ' أثناء تحميل ملف XLS|استثناء|
## **API العام والتغييرات غير المتوافقة مع الإصدارات السابقة**
فيما يلي قائمة بأي تغييرات تم إجراؤها على API العام مثل الأعضاء المضافين أو المعاد تسميتهم أو المحذوفون أو المهملون بالإضافة إلى أي تغيير غير متوافق مع الإصدارات السابقة تم إجراؤه على Aspose.Cells for Java. إذا كانت لديك مخاوف بشأن أي تغيير مدرج ، فيرجى رفعه في منتدى الدعم Aspose.Cells.
### **يضيف طريقة WorkbookSettings.GetThemeFont ().**
يحصل على خط الموضوع.
### **يضيف خاصية DataLabels.LinkedSource.**
يحصل على المصدر المرتبط ويعينه.
### **إضافة تعداد DefaultEditLanguage.**
يمثل لغة التحرير الافتراضية.
### **إضافة خاصية ImageOrPrintOptions.DefaultEditLanguage.**
الحصول على أو تعيين لغة التحرير الافتراضية.
قد يعرض / يعرض تخطيطات مختلفة للفقرات النصية عند تعيين لغات تحرير مختلفة.
### **يضيف خاصية PdfSaveOptions.DefaultEditLanguage.**
الحصول على أو تعيين لغة التحرير الافتراضية.
قد يعرض / يعرض تخطيطات مختلفة للفقرات النصية عند تعيين لغات تحرير مختلفة.
