﻿---
title: Aspose.Cells for .NET 22.7 ملاحظات الإصدار
type: docs
weight: 6
url: /ar/net/aspose-cells-for-net-22-7-release-notes/
---
{{% alert color="primary" %}}

 تحتوي هذه الصفحة على ملاحظات الإصدار لـ[Aspose.Cells for .NET 22.7](https://www.nuget.org/packages/Aspose.Cells/22.7.0).

{{% /alert %}}

|**مفتاح**|**ملخص**|**فئة**|
|:- |:- |:- |
|CELLSNET-51296| يستمر Gridweb في القفز إلى الأعلى عند محاولة النسخ واللصق|
|CELLSNET-51355|و Range.Top، Left، Width، Height بوحدة النقاط|
|CELLSNET-51367|تحويل كل الأوراق إلى صفحة واحدة عند الحفظ بتنسيق html.|
|CELLSNET-51486|تم تحويل النص إلى مربعات صغيرة|
|CELLSNET-51492|لا يتم تطبيق الخط الافتراضي عند تحويل XLSX إلى HTML|
|CELLSNET-51306|لم يتم نسخ أنماط الجدول المحوري بشكل صحيح باستخدام أحدث إصدار من Aspose.Cells for .NET|
|CELLSNET-51268|مشكلة في معالجة صيغة COUNTIFS للصفر بشكل غير صحيح|
|CELLSNET-51297|Cell.GetPrecedents () لا يوفر كل السابقات عندما تشير الصيغة إلى اسم معرف|
|CELLSNET-51399|تعرض Print_Titles النطاق المسمى والدالة MATCH خطأ # NAME|
|CELLSNET-51456|تقفز الخلايا عند استخدام ctrl + c ctrl + v عند ضبط ارتفاع GridWeb على 100٪|
|CELLSNET-51457|لا تظهر قائمة السياق عند ضبط الارتفاع على 100٪ بعد بعض الصفوف|
|CELLSNET-51471|لا تظهر قائمة التحقق في خلية فارغة|
|CELLSNET-51469|النص في الصورة مفقود بعد التحويل إلى pdf|
|CELLSNET-51476|يصبح عنصر السهم مشوهًا في الصورة|
|CELLSNET-51001|لا يتم وضع كائن الشكل على الرسم البياني بشكل جيد|
|CELLSNET-51156| الرسم البياني لتحويل الصورة - عرض مختلف للرسم البياني في صورة الإخراج|
|CELLSNET-51213|لم يتم عرض المخطط الدائري ثلاثي الأبعاد بشكل صحيح - تحويل المخطط إلى صورة|
|CELLSNET-51472|تسميات المخططات مفقودة من SVG عند ضبطها على النهاية الخارجية|
|CELLSNET-51491|تم استخدام قيم خاطئة في سلسلة الرسم البياني عند التقديم للصورة أو HTML|
|CELLSNET-51525|يختلف مخطط الشلال عند تصديره إلى HTML/PNG أو PDF|
|CELLSNET-51353|يؤدي تحويل ملف XLSB باستخدام ارتباط DDE إلى ملف XLSM إلى تغيير موضع تطبيق DDE في الارتباط|
|CELLSNET-51376|يتم تغيير حجم الصفحة تلقائيًا من A4؟ رسالة للورقة|
|CELLSNET-51379| تتم قراءة الارتباط الخارجي من النوع OLE في ملف XLS اعتبارًا من النوع DDE|
|CELLSNET-51402|يتم نقل المحتوى إلى خارج الخلية عند حفظ ملف html|
|CELLSNET-51417|تتم إزالة الروابط من شكل إلى ورقة في الملف بعد الترقية من 22.5 إلى 22.6.1|
|CELLSNET-51418|تم تغيير ارتباط خارجي من النوع xlPathMissing إلى نوع ExternalLinkPath عادي في تحويل XLSB إلى XLSM|
|CELLSNET-51420|الاختلافات في خصائص المستند في ملف app.xml|
|CELLSNET-51427|رابط خارجي يحتوي على رمز خاص "#" والذي لم يتم تجاوزه بواسطة Aspose.Cells|
|CELLSNET-51482|يؤدي دمج الأوراق من مصنفات مختلفة إلى ملف تالف يمكن أن يؤدي إلى تعطل MS Excel|
|CELLSNET-51507|يتم قراءة قيم الأرقام من ملف XLSX كـ 0|
|CELLSNET-51280|استثناء أثناء حفظ ملف ODS (RB-60121)|
|CELLSNET-51483|فشل تحميل الملف مع استثناء "لم يكن صفيف المصدر طويلاً بما يكفي ..."|

## **API العام والتغييرات غير المتوافقة مع الإصدارات السابقة**

فيما يلي قائمة بأي تغييرات تم إجراؤها على API العام مثل الأعضاء المضافين أو المعاد تسميتهم أو المحذوفون أو المهملون بالإضافة إلى أي تغيير غير متوافق مع الإصدارات السابقة تم إجراؤه على Aspose.Cells for .NET. إذا كانت لديك مخاوف بشأن أي تغيير مدرج ، فيرجى رفعه في منتدى الدعم Aspose.Cells.

### **يضيف Cells.GetDependentsInCalculation (int ، int ، bool) طريقة**

الحصول على جميع الخلايا التي تعتمد نتيجتها المحسوبة على الخلية المحددة بواسطة الصف والعمود وفقًا لسلسلة الحساب الحالية. بالنسبة للخلية الفارغة والتي لم يتم إنشاء مثيل لها في نموذج الخلايا الحالي ، يمكن للمستخدم استخدام هذه الطريقة بدلاً من Cell.GetDependentsInCalculation (منطقي) لأن الخلية اللاحقة تحتاج إلى إنشاء مثيل كائن الخلية في نموذج الخلايا الحالية في البداية.

### **يغير الحد الأيسر / الأيمن للخلية لـ Cell.GetStyle () عندما يكون العمود المجاور مخفيًا**

في الإصدارات القديمة ، إذا كان العمود المجاور مخفيًا لخلية واحدة ، فلن يتم التحقق من الحد الأيسر / الأيمن لهذه الخلية بالخلية المجاورة ، لذلك قد يختلف الحد الذي تم إرجاعه عما يظهر في مربع حوار ms excel عند تعيين حدود هذه الخلية. بدءًا من 22.7 ، نجعل الحد الذي يتم إرجاعه دائمًا هو القيمة الفعلية (التي يجب أن تكون متسقة مع حدود الخلية المجاورة) للخلية لـ Cell.GetStyle (). إذا احتاج المستخدم إلى ما يظهر للخلية في ms excel (عندما يكون العمود المجاور مخفيًا ، فقد تكون الحدود المعروضة هي العمود المرئي التالي) ، يمكن للمستخدم تجربة Cell.GetDisplayStyle ().

### **أضف خصائص Range.op و Range.Left و Range.Height و Range.Width.**

الحصول على موضع النطاق وحجمه بوحدة النقاط.

### **احذف الفئة PowerQueryFormulaCollction وأضف فئة PowerQueryFormulaCollection للفئة.**

هناك خطأ مطبعي في الطبقة القديمة.

### **قم بإضافة خصائص HtmlSaveOptions.ExportPageFooters و HtmlSaveOptions.ExportPageHeaders.**

يشير إلى ما إذا كان يتم تصدير الرؤوس والتذييلات عند الحفظ كملف html واحد.

### **إضافة الخاصية HtmlSaveOptions.ShowAllSheets.**

يشير إلى ما إذا كان سيتم عرض كل الأوراق عند الحفظ كملف html واحد.

### **Obsoletes HtmlSaveOptions.ExportHeadings الخاصية وإضافة HtmlSaveOptions.ExportRowColumnHeadings.**

الرجاء استخدام HtmlSaveOptions.ExportRowColumnHeadings بدلاً من ذلك.

### **Obsoletes Chart.ToImage (سلسلة نصية ، ImageFormat) وإضافة Chart.ToImage (سلسلة نصية ، ImageType)**

الرجاء استخدام Chart.ToImage (سلسلة ، ImageType) بدلاً من ذلك.

### **عفا عليها الزمن Chart.ToImage (دفق ، ImageFormat) وإضافة Chart.ToImage (دفق ، نوع الصورة)**

الرجاء استخدام Chart.ToImage (Stream ، ImageType) بدلاً من ذلك.

### **عفا عليها الزمن Shape.ToImage (Stream ، ImageFormat) وإضافة Shape.ToImage (Stream ، ImageType)**

الرجاء استخدام Shape.ToImage (Stream ، ImageType) بدلاً من ذلك.
