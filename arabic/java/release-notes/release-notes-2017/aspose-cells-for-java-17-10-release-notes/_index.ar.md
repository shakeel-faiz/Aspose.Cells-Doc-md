﻿---
title: Aspose.Cells for Java 17.10 ملاحظات الإصدار
type: docs
weight: 30
url: /ar/java/aspose-cells-for-java-17-10-release-notes/
---
{{% alert color="primary" %}} 

 تحتوي هذه الصفحة على ملاحظات الإصدار لـ[Aspose.Cells for Java 17.10](https://downloads.aspose.com/cells/java/new-releases/aspose.cells-for-java-17.10/).

{{% /alert %}} 

|**مفتاح**|**ملخص**|**فئة**|
|:- |:- |:- |
|CELLSJAVA-42423|قم بإلغاء الحساب طويل المدى لأسلوب Workbook.calculateFormula|ميزة جديدة|
|CELLSJAVA-42414|احصل على حقل SheetId الخاص بورقة عمل MS Excel|ميزة جديدة|
|CELLSJAVA-42402|مطلوب HTML للمرفق HTML|التعزيز|
|CELLSJAVA-42372|لا يكون موضع الواصلات الطويلة مثل Microsoft Excel|التعزيز|
|CELLSJAVA-42399|نقاط الأسهم غير واضحة في ملف PDF الناتج|خلل برمجي|
|CELLSJAVA-42419|يتم قطع النص في الإخراج HTML|خلل برمجي|
|CELLSJAVA-42418|لا يتطابق لون الحد مثل MS Excel في الإخراج HTML|خلل برمجي|
|CELLSJAVA-42417|لا يتطابق لون الخلفية مثل MS Excel في الإخراج HTML|خلل برمجي|
|CELLSJAVA-42385|لم يتم استدعاء IFilePathProvider مطلقًا ومن ثم فإن الملف HTML يحتوي على "فارغ" في المسار|خلل برمجي|
|CELLSJAVA-42412|تسميات محور القيمة مفقودة عند تحويل Excel إلى PDF|خلل برمجي|
|CELLSJAVA-42408|مشكلة تداخل النص بعد عرض ورقة العمل على الصورة|خلل برمجي|
|CELLSJAVA-42420|مشكلة الإلغاء ونفاد الذاكرة بسبب نطاق البيانات الكبير للمخطط|خلل برمجي|
|CELLSJAVA-42415|مخطط الإخراج ليس مثل الرسم البياني الأصلي في الإخراج HTML|خلل برمجي|
|CELLSJAVA-42410|يتم عرض منطقة المخطط ، والتسميات ، ومفاتيح الرسم البياني ، وما إلى ذلك بشكل غير صحيح في الإخراج PDF و PNG|خلل برمجي|
|CELLSJAVA-42409|لم يتم تقديم منطقة المخطط بشكل صحيح في مخرجات PDF و PNG من مخطط MS Excel|خلل برمجي|
|CELLSJAVA-41046|تم تغيير تسلسل وسيلة إيضاح الرسم البياني أثناء تحويل جدول البيانات إلى تنسيق PDF|خلل برمجي|
|CELLSJAVA-40416|تم فقد ألوان وأسلوب الرسم البياني|خلل برمجي|
## **API العام والتغييرات غير المتوافقة مع الإصدارات السابقة**
فيما يلي قائمة بأي تغييرات تم إجراؤها على API العام مثل الأعضاء المضافين أو المعاد تسميتهم أو المحذوفون أو المهملون بالإضافة إلى أي تغيير غير متوافق مع الإصدارات السابقة تم إجراؤه على Aspose.Cells for Java. إذا كانت لديك مخاوف بشأن أي تغيير مدرج ، فيرجى رفعه في منتدى الدعم Aspose.Cells.
### **يضيف طريقة AbstractCalculationMonitor.Interrupt (سلسلة)**
يسمح للمستخدمين بمقاطعة تقدم حسابات الصيغة.
### **يضيف HtmlCrossType.MSExport التعداد**
تعرض السلسلة مثل تصدير MS Excel HTML.
### **يضيف خاصية Worksheet.TabId**
يحصل على المعرف الداخلي للورقة.
### **يضيف تعداد OLEDBCommandType**
نوع الأمر غير محدد.
### **يضيف تعداد ConnectionDataSourceType**
يمثل نوع مصدر البيانات للاتصال.
### **تقادم ExternalConnection.Credentials and ExternalConnection.ReConnectionMethod property**
استخدم خاصية ExternalConnection.CredentialsMethodType و ExternalConnection.ReconnectionMethodType بدلاً من ذلك.
### **حذف خاصية WebQueryConnection.EditPage القديمة**
استخدم خاصية WebQueryConnection.EditWebPage بدلاً من ذلك.
### **يضيف خاصية Series.ValuesFormatCode**
يمثل رمز تنسيق الرقم لقيم السلسلة.


### **أمثلة على الاستخدام**
يرجى التحقق من قائمة مواضيع المساعدة المضافة في Aspose.Cells مستندات Wiki:

- [قم بتعيين رمز تنسيق القيم لسلسلة التخطيطات](/cells/ar/java/set-the-values-format-code-of-chart-series/)
- [استخدم خاصية Sheet.SheetId الخاصة بـ OpenXml باستخدام Aspose.Cells](/cells/ar/java/utilize-sheet-sheetid-property-of-openxml-using-aspose-cells/)
- [قراءة وكتابة الاتصال الخارجي لملف XLSB](/cells/ar/java/read-and-write-external-connection-of-xlsb-or-xls-file/)
- [مقاطعة أو إلغاء حساب صيغة المصنف](/cells/ar/java/interrupt-or-cancel-the-formula-calculation-of-workbook/)
- [حدد كيفية عبور السلسلة في الإخراج HTML باستخدام HtmlCrossType](/cells/ar/java/specify-how-to-cross-string-in-output-html-using-htmlcrosstype/)
