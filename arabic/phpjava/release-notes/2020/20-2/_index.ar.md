﻿---
title: Aspose.Cells for PHP via Java 20.2 ملاحظات الإصدار
type: docs
weight: 10
url: /ar/php-java/aspose-cells-for-php-via-java-20-2-release-notes/
---
{{% alert color="primary" %}} 

تحتوي هذه الصفحة على ملاحظات إصدار Aspose.Cells for PHP via Java 20.2.

{{% /alert %}} 

|**مفتاح**|**ملخص**|**فئة**|
|:- |:- |:- |
|CELLSJAVA-43076|عيّن نوع الصورة EMF في الملف HTML الذي تم تقديمه|التعزيز|
|CELLSJAVA-43113|التحويل إلى PDF - java.lang.NumberFormatException: لسلسلة الإدخال|التعزيز|
|CELLSJAVA-43114|التحويل إلى PDF - صيغة غير صحيحة: "'APRIL" 12'.A1:' APRIL "12'.I23 "|التعزيز|
|CELLSJAVA-43117|التحويل إلى PDF - الست عشري ليس رقم ست عشري صالح|التعزيز|
|CELLSJAVA-43118|التحويل إلى PDF - java.lang.NumberFormatException: لسلسلة الإدخال: "341،403،811.74"|التعزيز|
|CELLSJAVA-43077|تم رفع استثناء "نوع صورة غير متوقع" أثناء تقديم ورقة العمل إلى HTML|خلل برمجي|
|CELLSJAVA-43096|توقف البرنامج أثناء تحويل ملف Excel إلى HTML|خلل برمجي|
|CELLSJAVA-43107|التحويل إلى PDF - com.aspose.cells.CellsException: خطأ من الشكل إلى الصورة!|خلل برمجي|
|CELLSJAVA-43108|التحويل إلى PDF - com.aspose.cells.CellsException|خلل برمجي|
|CELLSJAVA-43088|لم يتم تقديم المخطط النسيجي في ملف الإخراج في تحويل XLSX إلى PDF|خلل برمجي|
|CELLSJAVA-43091|تتداخل تسميات البيانات على مخطط الكعك في ملف PDF|خلل برمجي|
|CELLSJAVA-43099|لا يتم عرض صورة ورقة العمل بشكل صحيح|خلل برمجي|
|CELLSJAVA-43093|لم يتم الكشف عن عنصر تحكم ActiveX بتنسيق ملف XLS|خلل برمجي|
|CELLSJAVA-43104|مشاكل متعلقة بـ getShowTabs و setShowTabs|خلل برمجي|
|CELLSJAVA-43121|OOM تحاول الحصول على عدد الصفحات في XLS|خلل برمجي|
|CELLSJAVA-43125|يتم تكرار كائنات النموذج و ActiveX|خلل برمجي|
|CELLSJAVA-43094|استثناء عند تحميل تنسيق ملف XLSX|استثناء|
|CELLSJAVA-43100|استثناء "java.lang.ArrayIndexOutOfBoundsException" عند استدعاء Workbook.calculateFormula () في ملف Excel|استثناء|
|CELLSJAVA-43123|ArrayIndexOutOfBoundsException أثناء استخدام MEMORY_PREFERENCE|استثناء|
|CELLSJAVA-43105|التحويل إلى PDF - java.lang.ArrayIndexOutOfBoundsException: 60|استثناء|
|CELLSJAVA-43106|التحويل إلى PDF - java.lang.IllegalArgumentException|استثناء|
|CELLSJAVA-43109|التحويل إلى PDF - java.lang.NullPointerException|استثناء|
|CELLSJAVA-43111|التحويل إلى PDF - com.aspose.cells.CellsException: بيانات غير صالحة!|استثناء|
|CELLSJAVA-43112|التحويل إلى PDF - java.lang.NullPointerException|استثناء|
|CELLSJAVA-43115|التحويل إلى PDF - java.lang.NegativeArraySizeException|استثناء|
|CELLSJAVA-43116|التحويل إلى PDF - java.lang.IllegalStateException: يبدو أن التخزين المهيكل تالف.|استثناء|
|CELLSJAVA-43120|java.lang.NumberFormatException أثناء تحويل المصنف إلى PDF|استثناء|
### **API العام والتغييرات غير المتوافقة مع الإصدارات السابقة**
فيما يلي قائمة بأي تغييرات تم إجراؤها على API العام مثل الأعضاء المضافين أو المعاد تسميتهم أو المحذوفون أو المهملون بالإضافة إلى أي تغيير غير متوافق مع الإصدارات السابقة تم إجراؤه على via Java for PHP Aspose.Cells Aspose.Cells. في منتدى الدعم Aspose.Cells.
#### **يضيف خاصية FormulaParseOptions.Parse.**
يشير إلى ما إذا كان سيتم تحليل الصيغة أثناء تعيين تعبير صيغة إلى خلية. القيمة الافتراضية هي الحقيقية. إذا كانت خاطئة ، فسيتم الاحتفاظ بتعبير صيغة الإدخال كما هو الحال بالنسبة للخلية حتى يستدعي المستخدم طرقًا أخرى لتحليلها أو أن بيانات الصيغة المحللة مطلوبة من خلال عمليات أخرى مثل حساب الصيغ.
#### **يضيف طريقة Workbook.ParseFormulas (bool ignoreError).**
يوزع كل الصيغ التي لم يتم تحليلها عند تحميلها أو تعيينها إلى خلية.
#### **إضافة خاصية PivotTable.ExternalConnectionDataSource.**
يحصل على مصدر بيانات الاتصال الخارجي.
#### **يضيف FileFormatType.Numbers35 enum.**
يمثل الملفات رقم 3.5 منذ Office 2014. فقط لإلقاء تنسيق الملف عند القراءة.
#### **يضيف خاصية LoadOptions.CheckDataValid.**
يستدعي ما إذا كان يجب التحقق من البيانات غير الصالحة عند تحميل الملفات.

