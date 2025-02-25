﻿---
title: Aspose.Cells for Java 8.0.0 ملاحظات الإصدار
type: docs
weight: 70
url: /ar/java/aspose-cells-for-java-8-0-0-release-notes/
---
{{% alert color="primary" %}}

 تحتوي هذه الصفحة على ملاحظات الإصدار لـ[Aspose.Cells for Java 8.0.0](https://downloads.aspose.com/cells/java/new-releases/aspose.cells-for-java-8.0.0/)

{{% /alert %}}

تم تحديث Aspose.Cells for Java إلى الإصدار 8.0.0 ويسعدنا أن نعلن أن هذا الإصدار يجلب إضافة أكثر من 30 تحسينًا مفيدًا جديدًا.
باستخدام Aspose.Cells for Java يمكنك العمل مع XLS ، SpreadsheetML ، OOXML ، XLSB ، CSV ، HTML ، ODS ، PDF ، XPS وتنسيقات أخرى في تطبيقاتك. يمكنك أيضًا إنشاء المصنفات وتعديلها وتحويلها وعرضها وطباعتها دون استخدام Microsoft Excel.
قم بزيارة الوثائق لمعرفة كيفية البدء مع Aspose.Cells for Java.
لاحظ أن هذا التنزيل يحتوي على إصدار كامل من المنتج ، ولكن بدون تعيين ترخيص ، سيتم تشغيله في وضع التقييم مع بعض القيود. لاختبار Aspose.Cells بدون قيود التقييم هذه ، يمكنك طلب ترخيص مؤقت مجاني لمدة 30 يومًا.
فيما يلي قائمة بالتغييرات في هذا الإصدار Aspose.Cells for Java.

الميزات الرئيسية

يمكن استخدام خيار استخدام الذاكرة للنظر في الأداء.
عند إنشاء مصنف مع مجموعة بيانات خلايا كبيرة ، قد يعمل الخيار MemorySetting.MEMORY_PREFERENCE على تحسين استخدام الذاكرة لبيانات الخلايا لتقليل تكلفة الذاكرة.

تحسينات وتغييرات أخرى

ميزات جديدة

(CELLSJAVA-40749) - احصل على فهارس البداية للصف / العمود وإنهاء الصف / العمود لصفحة من ورقة العمل
(CELLSJAVA-40744) - دعم ميزة إظهار الصيغ MS Excel
(CELLSJAVA-40423) - تبعيات Aspose.Cells و Maven
(CELLSJAVA-40770) - اضبط وقت الإنشاء في PDF الذي تم إنشاؤه

التحسينات

(CELLSJAVA-40751) - خطأ مطبعي في اسم الأسلوب - SeriesCollection.setSecondCategoryData
(CELLSJAVA-40753) - فاصل بيانات السلسلة المخصص
(CELLSJAVA-40764) - Cell. لم يتم حساب DisplayStringValue بدقة للمسافات المحددة بواسطة عرض العمود و "*" في نمط مخصص

البق

(CELLSJAVA-40738) - setExportActiveWorksheet فقط تغيير محاذاة الجدول في HTML
(CELLSJAVA-40747) - لا يتم نسخ صورة الخلفية إلى المصنف الوجهة عند استدعاء Workbook.copy
(CELLSJAVA-40276) - يبدو أن النص الموجود داخل الصورة معكوس أثناء حفظ مصنف Excel كـ PDF
(CELLSJAVA-40573) - يتم فصل بعض الكلمات عند الحفظ في PDF
(CELLSJAVA-40743) - لا يعمل عامل التصفية التلقائي للجدول بتنسيق xls ولكنه يعمل بشكل جيد في تنسيق xlsx
(CELLSJAVA-40750) - عند التصدير إلى HTML ، تفقد الخلايا المغطاة بالصورة لون الخلفية
(CELLSJAVA-40748) - مسار صورة الخلفية غير صحيح
(CELLSJAVA-40731) - مشكلة نص عمودي
(CELLSJAVA-40737) - مشكلة تنسيق الأشكال / عناصر التحكم في Excel لتحويل PDF
(CELLSJAVA-40742) - التفاف غير صحيح لملصقات المحور عند تحويل XLSX إلى PDF
(CELLSJAVA-40757) - تمت قراءة أعمدة التاريخ والوقت بشكل غير صحيح من CSV بالإعدادات المحلية الأوروبية
(CELLSJAVA-40282) - انعكاس إخراج الصورة أثناء تحويل ورقة عمل Excel إلى PDF
(CELLSJAVA-40585) - Aspose.Cells: مخطط مخطط سيجما المضمن لم يتم تقديمه بشكل صحيح إلى PDF / الصور
(CELLSJAVA-40742) - التفاف غير صحيح لملصقات المحور عند تحويل XLSX إلى PDF
(CELLSJAVA-40758) - البيانات غير صحيحة في ملف pdf الناتج
(CELLSJAVA-40762) - Cell.getDependents (صحيح) مشكلة - Cells من الأوراق الأخرى التي لا ينبغي أن تكون في القائمة
(CELLSJAVA-40756) - استثناء الخلايا: فارغ في Workbook.calculateFormula (خطأ)
(CELLSJAVA-40748) - مسار صورة الخلفية غير صحيح
(CELLSJAVA-40754) - تصدير الأشكال إلى html مع لون خلفية خطأ
(CELLSJAVA-40766) - XLSX إلى HTML: مشكلة مع hideColumn تنتج قيم خالية في HTML
(CELLSJAVA-40769) - صيغة خلية إعادة الحساب

(CELLSJAVA-40771) - مشكلة مخفية في الصف وارتفاع الصف


استثناءات

(CELLSJAVA-40736) - com.aspose.cells.CellsException: اسم خلية غير صالح
(CELLSJAVA-40767) - NullpointerException عند حفظ كتاب
(CELLSJAVA-40755) - CellsException: تجاوز في String لتحويل int. قيمة السلسلة: # N / A.
(CELLSJAVA-40761) - CellsException: خطأ من شكل إلى صورة!

API العام والتغييرات غير المتوافقة مع الإصدارات السابقة

فيما يلي قائمة بأي تغييرات تم إجراؤها على API العام مثل الأعضاء المضافين أو المعاد تسميتهم أو المحذوفون أو المهملون بالإضافة إلى أي تغيير غير متوافق مع الإصدارات السابقة تم إجراؤه على Aspose.Cells for Java. إذا كانت لديك مخاوف بشأن أي تغيير مدرج ، فيرجى رفعه في منتدى الدعم Aspose.Cells.

تقادم خاصية AutoFilter.FilterColumnCollection
يستخدم AutoFilter.FilterColumns بدلاً من ذلك.

يضيف خاصية Worksheet.ShowFormulas
يشير إلى ما إذا كان يتم إظهار الصيغ أو قيمة الصيغ.

يضيف خاصية PdfSaveOptions.CreatedTime
الحصول على وتعيين وقت إنشاء مستند pdf.

يضيف FileFormatType.Ooxml enum
يمثل ملف xml المفتوح (مثل XLSX ، DOCX ، PPTX ، إلخ).

إضافة خاصية LoadOptions.MemorySetting و WorkbookSettings.MemorySetting الخاصية
من هذا الإصدار نقدم خيار استخدام الذاكرة للمستخدم للنظر في الأداء. يتم تطبيق الخيار الافتراضي MemorySetting.NORMAL على كافة الإصدارات. بالنسبة لبعض المواقف مثل إنشاء مصنف مع مجموعة بيانات كبيرة للخلايا ، قد يعمل خيار MemorySetting.MEMORY_PREFERENCE على تحسين استخدام الذاكرة وتقليل تكلفة الذاكرة لتطبيق المستخدم. ومع ذلك ، قد يؤدي هذا الخيار إلى تدهور الأداء في بعض الحالات الخاصة مثل الوصول إلى الخلايا بشكل عشوائي ومتكرر.

Obsoletes SeriesCollection.SecondCatergoryData وإضافة خاصية SeriesCollection.SecondCategoryData
يستخدم SeriesCollection.SecondCategoryData لاستبدال SeriesCollection.SecondCatergoryData.

تم تغيير تطبيقات Row / Cell / RowCollection
في الإصدارات القديمة ، يتم الاحتفاظ بكائنات Row و Cell في الذاكرة لتمثيل الصف والخلية المقابلة في ورقة العمل. سيتم إرجاع نفس الحالة كلما قام المستخدم باستدعاء طرق مثل RowCollection [فهرس int] ، Cells [int ، int] وهكذا. للنظر في أداء الذاكرة ، بدءًا من هذا الإصدار سيتم الاحتفاظ بخصائص وبيانات Row و Cell فقط في الذاكرة. يصبح الكائن Row / Cell غلافًا لتلك الخصائص والبيانات لراحة المستخدم في معالجة نموذج الخلايا وسيتم إنشاء مثيل له حديثًا عند استدعاء المستخدم تلك الأساليب. لذلك ، سيحصل المستخدم الآن على كائنات مختلفة عند استدعاء نفس الطريقة للحصول على Row / Cell عدة مرات على الرغم من أن هذه الكائنات المختلفة تشير جميعها إلى نفس الصف / الخلية في ورقة العمل ، وقد يؤثر هذا التغيير على تطبيق المستخدم في المواقف التالية: 1. إذا استخدم المستخدم رمز likeif (row1 == row2) ... إذا (cell1 == cell2) ... للتحقق من نفس الصف / Cell ، فقد تفشل هذه الاختبارات في الإصدارات الجديدة. الرجاء استخدام row1.equals (row2) و cell1.equals (cell2) بدلاً من ذلك. نظرًا لأنه تم إنشاء كائنات الصف / Cell حديثًا وفقًا لاستدعاء المستخدم ، فلن يتم الاحتفاظ بها وإدارتها في الذاكرة بواسطة مكون الخلايا. بعد بعض عمليات الإدراج / الحذف ، قد لا يتم تحديث موضعها (فهرس الصف / العمود) أو حتى أسوأ ، هذه الأشياء تصبح غير صالحة. على سبيل المثال ، للتعليمات البرمجية التالية: Cell cell = cells.get ("A2")؛ System.out.println (cell.getName () + ":" + cell.getValue ())؛ cells.insertRange (CellArea.createCellArea ( "A1" ، "A1") ، ShiftType.DOWN) ؛ System.out.println (cell.getName () + ":" + cell.getValue ()) ؛ في الإصدارات القديمة ، ستشير الخلية إلى A3 بعد الإدراج العملية وقيمتها هي نفسها مع القيمة السابقة للإدراج. ومع ذلك ، مع الإصدار الجديد ، سيصبح كائن الخلية غير صالح أو سيظل يشير إلى A2 بقيمة أخرى. لمثل هذا النوع من المواقف ، يحتاج المستخدم إلى الحصول على كائن صف / Cell مرة أخرى من مجموعة الخلايا للحصول على النتيجة الصحيحة: Cell cell = cells.get ("A2")؛ System.out.println (cell.getName () + ": "+ cell.getValue ()) ؛ cells.insertRange (CellArea.createCellArea (" A1 "،" A1 ")، ShiftType.DOWN)؛ cell = cells.get (" A3 ")؛ System.out.println (خلية. getName () + ":" + cell.getValue ()) ؛ 3. لا يرث RowCollection الآن CollectionBase لأنه لم يعد هناك كائن صف في قائمته الداخلية.

Cell تم تغيير StringValue لنمط التنسيق الخاص بـ "*" و "_"
في الإصدارات القديمة ، نمط خاص* سيتم تجاهله عند تنسيق قيمة الخلية لـ Cell.StringValue و '** ينتج دائمًا حرفًا واحدًا في النتيجة المنسقة. من هذا الإصدار نغير منطق العمل بـ "* و "**" لجعل النتيجة المنسقة مماثلة لما يمكنك الحصول عليه من ms excel عند نسخ خلية كنص (مثل نسخ خلية إلى محرر نص أو تصدير الخلية إلى csv). على سبيل المثال ، استخدم "* ($ * #، ## 0.00 *)" المخصص لتنسيق قيمة الخلية 123 ، بالإصدارات القديمة Cell. ستعطي StringValue النتيجة كـ "123.00 دولارًا". الآن مع الإصدارات الجديدة Cell.StringValue ستعطي النتيجة "$ 123.00" وهو نفس ما يمكنك الحصول عليه من ms excel عن طريق نسخ هذه الخلية إلى نص.

ملحوظة
نظرًا لأن قاعدة الكود Aspose.Cells for Java تطابق رمز إصدار .NET ذي الصلة ، فإن معظم التغييرات والتحسينات والإصلاحات المضمنة في Aspose.Cells for .NET v8.0.0 مدرجة أيضًا في Aspose.Cells for Java v8.0.0.
