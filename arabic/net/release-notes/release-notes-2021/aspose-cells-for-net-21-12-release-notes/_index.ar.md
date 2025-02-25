﻿---
title: Aspose.Cells for .NET 21.12 ملاحظات الإصدار
type: docs
weight: 1
url: /ar/net/aspose-cells-for-net-21-12-release-notes/
---
{{% alert color="primary" %}}

 تحتوي هذه الصفحة على ملاحظات الإصدار لـ[Aspose.Cells for .NET 21.12](https://www.nuget.org/packages/Aspose.Cells/21.12.0).

{{% /alert %}}

|**مفتاح**|**ملخص**|**فئة**|
|:- |:- |:- |
|CELLSNET-49680|دعم تحويل Excel إلى نصوص SQL.|ميزة جديدة|
|CELLSNET-49717|دعم تحويل بيانات Excel إلى xml|ميزة جديدة|
|CELLSNET-49853| دعم استيراد بيانات xml|ميزة جديدة|
|CELLSNET-48190|قم بتحديث الأولويات عند إضافة شرط تنسيق جديد|التعزيز|
|CELLSNET-49758| يؤثر الفرز باستخدام DataSorter على تنسيق الجدول|التعزيز|
|CELLSNET-49828|يعطي FormatConditionCollection.AddCondition () سلوكًا مختلفًا للصيغة|التعزيز|
|CELLSNET-49981|إضافة خيار تصفية لسجلات المراجعة أثناء إنشاء مصنف من ملف القالب|التعزيز|
|CELLSNET-49739|تجاهل المراجع ثلاثية الأبعاد للتنسيق الشرطي عند النسخ إلى مصنف آخر|التعزيز|
|CELLSNET-49984|اقرأ بعض البيانات من ملف xls التالف.|التعزيز|
|CELLSNET-49990|دعم إعداد صيغة صف المجاميع المخصصة للجدول.|التعزيز|
|CELLSNET-49825|مشكلة في الأداء مع سمة ExportImagesAsBase64 في Excel لتحويل HTML|أداء|
|CELLSNET-49827|تم تخطي النطاق المحدد بشكل غير صحيح|خلل برمجي|
|CELLSNET-49759|لا يزال يتم تصدير الخلايا الفارغة كعناصر XML فارغة|خلل برمجي|
|CELLSNET-49817|لم يتم محاذاة النص إلى الوسط مع خط "Credit Suisse Type Light" أثناء تقديمه إلى Emf|خلل برمجي|
|CELLSNET-49864|تظهر الكلمات بترتيب عكسي للنص من اليمين إلى اليسار في عرض XLSX إلى PDF|خلل برمجي|
|CELLSNET-49873|من Xlsx إلى pdf: يختلف فاصل الصفحة عن ملف pdf الذي تم إنشاؤه بواسطة Excel|خلل برمجي|
|CELLSNET-49922|لا تلائم الأحرف صفحة واحدة ويتم تغيير موضع الطباعة في Excel إلى عرض PDF|خلل برمجي|
|CELLSNET-49998|لا يمكن عرض ملف XLS محدد بعلامة HTML|خلل برمجي|
|CELLSNET-49742|الاختلافات في chart1.xml بعد الحفظ|خلل برمجي|
|CELLSNET-49875|XLSX إلى EMF علامات التجزئة المتداخلة|خلل برمجي|
|CELLSNET-49904|لم يتم تحويل المخطط إلى PNG التواريخ بشكل صحيح|خلل برمجي|
|CELLSNET-49905|الانحدار: مشكلة عند تحويل المخطط إلى PNG|خلل برمجي|
|CELLSNET-49969|حدث خطأ في تجاوز السعة عند حفظ مستند XLS في XLSX / XSLM|خلل برمجي|
|CELLSNET-49760|تظهر المنطقة المدمجة بشكل خاطئ عند التحويل إلى html.|خلل برمجي|
|CELLSNET-49789|لا ينبغي تغيير شبكة Excel الأصلية عند حفظ ملف html|خلل برمجي|
|CELLSNET-49850|الصورة: معلمة FitToCell لا تعمل في العلامات الذكية للصور|خلل برمجي|
|CELLSNET-49870|يصبح العنوان أوسع عند دمج أوراق متعددة في جداول بيانات Excel|خلل برمجي|
|CELLSNET-49898|إظهار حدود الخلايا أثناء ملائمة الصور للخلايا باستخدام العلامات الذكية|خلل برمجي|
|CELLSNET-49924|Aspose تم فتح ملفات XLSX التي تم إنشاؤها مع وجود خطأ|خلل برمجي|
|CELLSNETCORE-301|تفشل إضافة ورقة العمل عندما يكون للارتباط التشعبي عنوان فارغ|خلل برمجي|
|CELLSNET-49812|استثناء عند فتح ملف ODS|استثناء|
|CELLSNET-49876|استثناء عند إعادة حفظ ملف XLSX|استثناء|
|CELLSNET-49943|System.NullReferenceException عند نسخ المصنف|استثناء|
|


## **API العام والتغييرات غير المتوافقة مع الإصدارات السابقة**

فيما يلي قائمة بأي تغييرات تم إجراؤها على API العام مثل الأعضاء المضافين أو المعاد تسميتهم أو المحذوفون أو المهملون بالإضافة إلى أي تغيير غير متوافق مع الإصدارات السابقة تم إجراؤه على Aspose.Cells for .NET. إذا كانت لديك مخاوف بشأن أي تغيير مدرج ، فيرجى رفعه في منتدى الدعم Aspose.Cells.

### **المزيد من القيود لإضافة مناطق للتحقق من الصحة.**

لقد قمنا بتغيير نموذج المنطقة للتحقق من الصحة والتنسيق الشرطي للنظر في الأداء. يتطلب النموذج الجديد مزيدًا من القيود لتسلسل المناطق المضافة. من أجل Validation.AddArea (CellArea cellArea ، bool checkIntersection ، bool checkEdge) and Validation.AddAreas (CellArea [] area ، bool checkIntersection ، bool checkEdge) ، إذا كانت معلمتا "check" خاطئة ، يحتاج المستخدم للتأكد من أن المناطق المضافة مرتبة ترتيبًا تصاعديًا حسب الزوايا العلوية اليسرى. وإلا فقد يتم الحصول على نتيجة غير متوقعة لعمليات أخرى. في الإصدار الجديد ، نظرًا لأن أداء إضافة كمية كبيرة من المناطق قد تم تحسينه بشكل كبير ، لا نعتقد أن ميزة Validation. لذلك نعتقد أن المستخدمين يمكنهم فقط الاتصال بـ AddArea (CellArea cellArea) مباشرة ، دون الحاجة إلى استخدام هاتين الطريقتين الخاصتين.

### **تم تغيير سلوك إضافة شرط التنسيق إلى FormatConditionCollection.**

بالنسبة إلى طرق FormatConditionCollection.AddCondition (...) ، فإن الإصدارات القديمة تجعل أولوية الأسلوب المُضاف حديثًا هي الأقل. إنه يختلف عن سلوك ms excel. من هذا الإصدار ، تمامًا مثل ما ستحصل عليه للعملية في ms excel ، نجعل أولوية شرط التنسيق المضافة حديثًا هي الأعلى.

### **إضافة خاصية AbstractInterruptMonitor.TerminateWithoutException.**

تشير هذه الخاصية إلى وقت الحاجة إلى مقاطعة لإحدى العمليات ، وما إذا كان يجب إنهاء العملية بواسطة استثناء أو الخروج بهدوء. بشكل افتراضي ، تكون هذه الخاصية خاطئة ، أي أنه سيتم إنهاء العملية بواسطة استثناء عند مقاطعتها.

### **يضيف خاصية WorkbookSettings.ResourceProvider.**

تمت إعادة تسمية خاصية WorkbookSettings.StreamProvider لجعلها أكثر ملاءمة لوظيفتها وتسهيل فهمها على المستخدمين.

### **يضيف خيار LoadDataFilterOptions.Revision.**

قد تحتوي بعض ملفات القوالب على كمية كبيرة من سجلات المراجعة مما يتسبب في ضعف أداء تحميل المصنف. يمكن للمستخدم استخدام هذا الخيار للتحكم في ما إذا كان يجب تحميل سجلات المراجعة أم لا.

### **خاصية Obsoletes WorkbookSettings.StreamProvider.**

الرجاء استخدام الخاصية WorkbookSettings.ResourceProvider بدلاً من ذلك.

### **يحذف الخاصية القديمة PdfSaveOptions.StreamProvider.**

الرجاء استخدام الخاصية WorkbookSettings.ResourceProvider بدلاً من ذلك.

### **يضيف خاصية JsonLoadOptions.MultipleWorksheets.**

الإشارة إلى ما إذا كان استيراد كل سمة من سمات كائن JsonObject كورقة عمل واحدة عندما تكون جميع العقد الفرعية عبارة عن عقد صفيف.

### **يضيف FileFormatType.SqlScript و SaveFormat.SqlScript و SqlScriptSaveOptions**

يمثل خيارات حفظ سكربت SQL.

### **يضيف SaveFormat.Xml و LoadFormat.Xml و XmlSaveOptions و XmlLoadOptions**

يمثل خيارات ملفات R / W xml.

### **إضافة خاصية HtmlSaveOptions.SaveAsSingleFile.**

 يشير إلى ما إذا كان حفظ Excel كملف واحد.

### **يضيف خاصية JsonLoadOptions.MultipleWorksheets.**

 يشير إلى ما إذا كان يتم تحميل بيانات ملف Json إلى أوراق عمل متعددة

### **يضيف PdfSaveOptions.Producer خاصية.**

 الحصول على وتعيين منتج مستند pdf الذي تم إنشاؤه.

### **إضافة أساليب ListColumn.GetCustomTotalsRowFormula () و ListColumn.SetCustomTotalsRowFormula ()**

 الحصول على الصيغة المخصصة لصف الإجماليات في الجدول وتعيينها.

