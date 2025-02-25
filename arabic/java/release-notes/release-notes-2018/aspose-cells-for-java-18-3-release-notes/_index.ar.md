﻿---
title: Aspose.Cells for Java 18.3 ملاحظات الإصدار
type: docs
weight: 100
url: /ar/java/aspose-cells-for-java-18-3-release-notes/
---
{{% alert color="primary" %}} 

تحتوي هذه الصفحة على ملاحظات إصدار Aspose.Cells for Java 18.3.

{{% /alert %}} 

|**مفتاح**|**ملخص**|**فئة**|
|:- |:- |:- |
|CELLSJAVA-42519|أضف PdfSaveOptions.DrawObjectEventHandler على غرار ImageOrPrintOptions.DrawObjectEventHandler|ميزة جديدة|
|CELLSJAVA-42543|استخراج اسم التسمية الذي يمكن تعيينه لكائنات الحزمة المضمنة في ملف MS Excel|ميزة جديدة|
|CELLSJAVA-42535|استخدام دفق لاستيراد ملف Excel عبر GridWebBean.importExcelFile () غير صالح أو غير موجود|التعزيز|
|CELLSJAVA-42529|كيفية تحديد أشكال ورقة العمل عبر DrawObjectEventHandler|التعزيز|
|CELLSJAVA-42558|تعذر الوصول إلى عناصر تسمية محور الفئة الأفقية|التعزيز|
|CELLSJAVA-42552|الإخراج HTML لا يتطابق مع MS Excel|خلل برمجي|
|CELLSJAVA-42536|تلف ملفات Excel بعد الفتح / الحفظ بواسطة Aspose.Cells APIs|خلل برمجي|
|CELLSJAVA-42513|تأتي الأعمدة الإضافية في نهاية كل صف في الإخراج HTML لنطاق|خلل برمجي|
|CELLSJAVA-42542|ملف Excel تالف وتغيرت بعض الخلايا بعد الحفظ|خلل برمجي|
|CELLSJAVA-42524|توجد أخطاء حسابية في الورقة المخفية وهي "KD020"|خلل برمجي|
|CELLSJAVA-42514|لا يعمل ImportTableOptions.setInsertRows () أثناء استيراد ResultSet إلى ورقة العمل|خلل برمجي|
|CELLSJAVA-42505|لا تظهر التعليقات المرفقة بالخلايا (في ملف القالب) عند استيراد ملف Excel إلى GridWeb|خلل برمجي|
|CELLSJAVA-42520|إحداثيات خلية غير متسقة تم الإبلاغ عنها بواسطة ImageOrPrintOptions.DrawObjectEventHandler|خلل برمجي|
|CELLSJAVA-42518|تتم محاذاة حدود الصفوف بشكل غير صحيح في الإخراج PDF|خلل برمجي|
|CELLSJAVA-42561|مقياس المحور X غير صحيح في PNG إخراج مخطط Excel|خلل برمجي|
|CELLSJAVA-42556|عرض المخطط غير صحيح في الإخراج PDF|خلل برمجي|
|CELLSJAVA-42547|يتم استبدال الرسم البياني بـ X باللون الأحمر عند تحويل XLSX إلى ODS|خلل برمجي|
|CELLSJAVA-42546|فقدت الصور عند التحويل ODS إلى XLSX|خلل برمجي|
|CELLSJAVA-42538|لم يتم استخراج الخصائص من ملفات XLS و XLSX|خلل برمجي|
|CELLSJAVA-42534|يؤدي حفظ XLS إلى XLSB إلى إزالة allowEditRanges|خلل برمجي|
|CELLSJAVA-42532|التحكم في الموارد الخارجية باستخدام WorkbookSetting.StreamProvider - يعمل for .NET ولكنه لا يعمل for Java|خلل برمجي|
|CELLSJAVA-42525|حدد حقول الصيغة أثناء استيراد البيانات إلى ورقة العمل - تعمل for .NET ولكنها لا تعمل for Java|خلل برمجي|
|CELLSJAVA-42521|لا يتم عرض الأحرف الصينية في اسم الملف المضمن (العنوان) بشكل جيد في المفكرة|خلل برمجي|
|CELLSJAVA-42533|حدث الاستثناء "NullPointerException" عند استخراج نص شكل SmartArt|استثناء|
|CELLSJAVA-42545|استثناء "يمكن استدعاء ReadElementString فقط عندما يكون المحتوى بسيطًا أو فارغًا" عند تحميل ملف ODS|استثناء|
|CELLSJAVA-42526|خطأ في الخلية B4 - صيغة غير صالحة - يحدث استثناء عند إعداد الصيغة|استثناء|
|CELLSJAVA-42522|ArrayIndexOutOfBoundsException عند فتح الملف عبر Aspose.Cells|استثناء|
|CELLSJAVA-42517|استثناء "com.aspose.cells.CellsException: صيغة غير صالحة:" عند تحميل ملف ODS|استثناء|
# **API العام والتغييرات غير المتوافقة مع الإصدارات السابقة**
فيما يلي قائمة بأي تغييرات تم إجراؤها على API العام مثل الأعضاء المضافين أو المعاد تسميتهم أو المحذوفون أو المهملون بالإضافة إلى أي تغيير غير متوافق مع الإصدارات السابقة تم إجراؤه على Aspose.Cells for Java. إذا كانت لديك مخاوف بشأن أي تغيير مدرج ، فيرجى رفعه في منتدى الدعم Aspose.Cells.
#### **إضافة الخاصية HtmlSaveOptions.ExportSimilarBorderStyle**
يشير إلى ما إذا كان تصدير نمط الحدود المماثل عندما لا تدعم المستعرضات نمط الحدود. إذا كنت تريد استيراد ملف HTML أو MHT إلى Excel ، فالرجاء الاحتفاظ بالقيمة الافتراضية. القيمة الافتراضية هي كاذبة.
#### **يضيف خاصية Axis.AxisLabels**
يحصل على تسميات المحور بعد استدعاء طريقة Chart.Calculate ().
#### **يضيف نوع تعداد جديد: GridValidationType.CustomServerFunction**
يمثل التحقق من صحة الوظيفة المخصصة من جانب الخادم.
#### **يضيف ChartType.Map enum**
يمثل مخطط الخريطة.
#### **إضافة خاصية OleObject.Label**
الحصول على تسمية العرض الخاصة بكائن Ole المرتبط وتعيينها.
#### **إضافة خاصية BuiltInDocumentPropertyCollection.DocumentVersion**
يمثل إصدار الملف.
#### **يضيف StyleFlag.QuotePrefix enum**
يشير إلى ما إذا كان يتم تطبيق خاصية QuotePrefix الخاصة بالنمط.
#### **يضيف فئة DialogBox**
يمثل ورقة مربع الحوار.
#### **يضيف خاصية PdfSaveOptions.DrawObjectEventHandler**
الحصول على DrawObjectEventHandler وتعيينه للحصول على DrawObject و Bound أثناء العرض.
#### **إضافة خاصية DrawObject.Shape**
يحصل على الشكل المرتبط أثناء التقديم.
