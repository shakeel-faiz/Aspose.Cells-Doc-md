﻿---
title: Aspose.Cells for .NET 8.7.1 ملاحظات الإصدار
type: docs
weight: 130
url: /ar/net/aspose-cells-for-net-8-7-1-release-notes/
---
### **تحسينات وتغييرات أخرى**

|**مفتاح** |**ملخص** |**فئة** |
|:- |:- |:- |
|CELLSNET-44154 |دعم جدول الاستعلام القراءة / الكتابة.|ميزة جديدة|
|CELLSNET-43616 | دعم صيغة صفيف تتضمن وظيفة "TABLE".|ميزة جديدة|
|CELLSNET-44195 | يتم فتح الملف في طريقة العرض المحمية بعد التحويل إلى تنسيق ملف XLS| التعزيز|
|CELLSNET-44182 | Cells البحث باستخدام التنسيق المخصص يعمل في الإصدار الأقدم ولكن ليس في الإصدار الأحدث| التعزيز|
|CELLSNET-44187 | تم استبدال قيم Cell بشكل غير صحيح بـ # عند التحويل إلى HTML| خلل برمجي|
|CELLSNET-44161 | يؤدي Aspose.Cells الذي تم إنشاؤه XLSX إلى قيام Excel 2007 بإصلاح جدول البيانات| خلل برمجي|
|CELLSNET-44063 | يفقد الجدول المحوري ترتيب الرأس بعد العمل مع ملف الإدخال| خلل برمجي|
|CELLSNET-44215 | حفظ في pdf لإظهار البيانات الدخيلة على يمين الجدول| خلل برمجي|
|CELLSNET-44201 | مشكلة تتعلق بمؤشرات الأحرف غير المدعومة في صيغة CHAR| خلل برمجي|
|CELLSNET-44193 | لا يتم عرض تظليل الخلية المائل بشكل صحيح إلى PDF| خلل برمجي|
|CELLSNET-44213 | ينتج عن حفظ الصورة من ورقة العمل صورة مختلفة قليلاً| خلل برمجي|
|CELLSNET-44192 | تتم محاذاة تسميات الفئات الموجودة أعلى المخطط إلى اليمين بدلاً من محاذاة جهة اليسار| خلل برمجي|
|CELLSNET-44240 | مشكلة في إعادة تسمية نطاق مسمى| خلل برمجي|
|CELLSNET-44239 | Cell.ContainsExternalLink إرجاع صحيح إذا كانت الصيغة = WEEKNUM| خلل برمجي|
|CELLSNET-44231 |إعادة حفظ جدول البيانات يفسد النتيجة| خلل برمجي|
|CELLSNET-44222 | تلف المصنف الذي يحتوي على وحدات الماكرو مع الإصدار 8.7.0| خلل برمجي|
|CELLSNET-44220 | يؤدي تعيين إعدادات WorkbookSettings.Password إلى إتلاف جدول البيانات الناتج| خلل برمجي|
|CELLSNET-44218 | إعادة حفظ XLSX يعيد تسمية ملف xl \ embeddings \ oleObject1.bin| خلل برمجي|
|CELLSNET-44214 | لا يحتفظ نطاق النسخ بإعدادات ListObject| خلل برمجي|
|CELLSNET-44203 | يختلف مراجع الصيغ في 8.6.2 و 8.7.0 لعملية ورقة العمل| خلل برمجي|
|CELLSNET-44241 | System.IndexOutOfRangeException في Cells.ImportData| استثناء|
|CELLSNET-44226 | System.ArgumentException في Workbook.Save أثناء الحفظ بتنسيق ODS| استثناء|
|CELLSNET-44225 | استثناء: "نص غير صالح للاسم المحدد." حدث أثناء نسخ ورقة العمل| استثناء|
|CELLSNET-44223 | NullReferenceException عند تحميل ملف XLSX محدد| استثناء|
|CELLSNET-44212 | استثناء NullReference عند فتح ملف Excel المصدر| استثناء|
|CELLSNET-44204 | CellsException: حجم الخط خارج النطاق ، في مُنشئ المصنف| استثناء|
|CELLSNET-44196 | توفير القدرة على اكتشاف العمود الذي تمت تصفيته والقيمة التي سيتم تصفيتها على واجهة GridWeb|ميزة جديدة|
|CELLSNET-44232 |مشكلة GridDesktop مع RemoveRow (index) حيث يكون الفهرس "0"| خلل برمجي|
### **API العام والتغييرات غير المتوافقة مع الإصدارات السابقة**
فيما يلي قائمة بأي تغييرات تم إجراؤها على API العام مثل الأعضاء المضافين أو المعاد تسميتهم أو المحذوفون أو المهملون بالإضافة إلى أي تغيير غير متوافق مع الإصدارات السابقة تم إجراؤه على Aspose.Cells for .NET. إذا كانت لديك مخاوف بشأن أي تغيير مدرج ، فيرجى رفعه في منتدى الدعم Aspose.Cells.
#### **يضيف خاصية LookInType.OriginalValues.**
ابحث فقط عن كائن من القيم الأصلية بدون تنسيق.
