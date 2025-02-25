﻿---
title: حساب الصيغ
type: docs
weight: 125
url: /ar/net/calculate-formulas/
---
## **إضافة الصيغ وحساب النتائج**

Aspose.Cells له محرك حساب معادلة مضمنة. لا يمكنه فقط إعادة حساب الصيغ المستوردة من قوالب المصمم ، ولكنه يدعم أيضًا حساب نتائج الصيغ المضافة في وقت التشغيل.

 يدعم Aspose.Cells معظم الصيغ أو الوظائف التي تعد جزءًا من Microsoft Excel (قراءة[قائمة بالوظائف التي يدعمها محرك الحساب](/cells/ar/net/supported-formula-functions/)). يمكن استخدام هذه الوظائف من خلال واجهات برمجة التطبيقات أو جداول بيانات المصمم. يدعم Aspose.Cells مجموعة ضخمة من الصيغ الرياضية ، والجمل ، والمنطقية ، والتاريخ / الوقت ، والإحصائية ، وقاعدة البيانات ، والبحث ، والصيغ المرجعية.

 استخدم ال[**معادلة**](https://reference.aspose.com/cells/net/aspose.cells/cell/properties/formula) الملكية أو[**SetFormula (...]**](https://reference.aspose.com/cells/net/aspose.cells.cell/setformula/methods/2) طرق[**Cell**](https://reference.aspose.com/cells/net/aspose.cells/cell)فئة لإضافة صيغة إلى خلية. عند تطبيق صيغة ، ابدأ السلسلة دائمًا بعلامة يساوي (=) كما تفعل عند إنشاء صيغة في Microsoft Excel واستخدم فاصلة (،) لتحديد معاملات الدالة.

 لحساب نتائج الصيغ ، يمكن للمستخدم استدعاء[**احسب الصيغة**](https://reference.aspose.com/cells/net/aspose.cells.workbook/calculateformula/methods/1) طريقة[**دفتر العمل**](https://reference.aspose.com/cells/net/aspose.cells/workbook)فئة تعالج جميع الصيغ المضمنة في ملف Excel. أو ، يمكن للمستخدم استدعاء[**احسب الصيغة**](https://reference.aspose.com/cells/net/aspose.cells/worksheet/methods/calculateformula) طريقة[**ورقة**](https://reference.aspose.com/cells/net/aspose.cells/worksheet) فئة تعالج جميع الصيغ المضمنة في ورقة. أو ، يمكن للمستخدم أيضًا الاتصال بـ[**احسب**](https://reference.aspose.com/cells/net/aspose.cells/cell/methods/calculate) طريقة[**Cell**](https://reference.aspose.com/cells/net/aspose.cells/cell)فئة تعالج صيغة واحدة Cell:

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Formulas-CalculatingFormulas-1.cs" >}}

### **من المهم أن تعرف**

{{% alert color="primary" %}}

 ال**معادلة** الملكية و**SetFormula (...]** طرق[**Cell**](https://reference.aspose.com/cells/net/aspose.cells/cell)فئة العمل بشكل مختلف عن**احسب** طرق[**دفتر العمل**](https://reference.aspose.com/cells/net/aspose.cells/workbook), [**ورقة عمل**](https://reference.aspose.com/cells/net/aspose.cells/worksheet) و[**Cell**](https://reference.aspose.com/cells/net/aspose.cells/cell) الطبقات. ال**معادلة** الملكية و**SetFormula (...]** الطرق ببساطة تضيف الصيغة إلى خلية ولكن لا تحسب النتيجة في وقت التشغيل. للحصول على نتيجة الصيغ ، يرجى الاتصال**احسب** أساليب.

{{% /alert %}}

## **الحساب المباشر للصيغة**

Aspose.Cells له محرك حساب معادلة مضمنة. بالإضافة إلى حساب الصيغ المستوردة من ملف مصمم ، يمكن أن يحسب Aspose.Cells نتائج الصيغة مباشرة.

في بعض الأحيان ، تحتاج إلى حساب نتائج الصيغة مباشرة دون إضافتها إلى ورقة عمل. قيم الخلايا المستخدمة في الصيغة موجودة بالفعل في ورقة عمل وكل ما تحتاجه هو العثور على نتيجة هذه القيم بناءً على بعض صيغة Excel Microsoft دون إضافة الصيغة في ورقة العمل.

 يمكنك استخدام Aspose.Cells 'واجهات برمجة تطبيقات محرك حساب الصيغة لـ[**ورقة عمل**](https://reference.aspose.com/cells/net/aspose.cells/worksheet) إلى[**احسب**](https://reference.aspose.com/cells/net/aspose.cells.worksheet/calculateformula/methods/3) نتائج هذه الصيغ دون إضافتها إلى ورقة العمل:

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Formulas-DirectCalculationFormula-1.cs" >}}

ينتج الكود أعلاه المخرجات التالية:
{{< highlight "net" >}}
Value of A1: 20
Value of A2: 30
Result of Sum(A1:A2): 50.0
{{< /highlight >}}

## **تكرار حساب الصيغ**

 عندما يكون هناك الكثير من الصيغ في المصنف ويحتاج المستخدم إلى حسابها بشكل متكرر مع تعديل جزء صغير منها فقط ، فقد يكون من المفيد للأداء تمكين سلسلة حساب الصيغة:[**FormulaSettings.EnableCalculationChain**](https://reference.aspose.com/cells/net/aspose.cells/formulasettings/properties/enablecalculationchain).

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Formulas-CalculatingFormulasOnce-1.cs" >}}

### **من المهم أن تعرف**

{{% alert color="primary" %}}

بشكل افتراضي ، يتم تعطيل سلسلة الحساب. لأن إنشاء السلسلة يحتاج أيضًا إلى وقت إضافي ، فإن أول مرة يتم فيها حساب الصيغ ([**المصنف .CalculateFormula (...]**](https://reference.aspose.com/cells/net/aspose.cells.workbook/calculateformula/methods/1)) قد يستهلك المزيد من وقت معالجة وحدة المعالجة المركزية والذاكرة عند المقارنة بحساب الصيغ بدون سلسلة. إذا لم يكن المستخدم بحاجة إلى حساب الصيغ بشكل متكرر ، فيجب أن يكون السلوك الافتراضي (حساب الصيغة مباشرة دون إنشاء سلسلة حسابية) هو الطريقة الأفضل.

{{% /alert %}}


## **موضوعات مسبقة**
- [أضف Cells إلى Microsoft نافذة مشاهدة Excel Formula](/cells/ar/net/add-cells-to-microsoft-excel-formula-watch-window/)
- [حساب دالة IFNA باستخدام Aspose.Cells](/cells/ar/net/calculating-ifna-function-using-aspose-cells/)
- [حساب صيغة صفيف لجداول البيانات](/cells/ar/net/calculation-of-array-formula-of-data-tables/)
- [حساب وظائف Excel 2016 MINIFS و MAXIFS](/cells/ar/net/calculation-of-excel-2016-minifs-and-maxifs-functions/)
- [إنقاص وقت الحساب إلى Cell.Calculate طريقة](/cells/ar/net/decrease-the-calculation-time-of-cell-calculate-method/)
- [كشف المرجع الدائري](/cells/ar/net/detecting-circular-reference/)
- [حساب مباشر لوظيفة مخصصة دون كتابتها في ورقة عمل](/cells/ar/net/direct-calculation-of-custom-function-without-writing-it-in-a-worksheet/)
- [قم بتطبيق محرك الحساب المخصص لتوسيع محرك الحساب الافتراضي لـ Aspose.Cells](/cells/ar/net/implement-custom-calculation-engine-to-extend-the-default-calculation-engine-of-aspose-cells/)
- [مقاطعة أو إلغاء حساب صيغة المصنف](/cells/ar/net/interrupt-or-cancel-the-formula-calculation-of-workbook/)
- [إرجاع نطاق من القيم باستخدام AbstractCalculationEngine](/cells/ar/net/returning-a-range-of-values-using-abstractcalculationengine/)
- [إرجاع نطاق من القيم باستخدام وظيفة ICustomFunction](/cells/ar/net/returning-a-range-of-values-using-icustomfunction/)
- [إعداد طريقة حساب الصيغة في المصنف](/cells/ar/net/setting-formula-calculation-mode-of-workbook/)
- [استخدام دالة FormulaText في Aspose.Cells](/cells/ar/net/using-formulatext-function-in-aspose-cells/)
- [استخدام ميزة ICustomFunction](/cells/ar/net/using-icustomfunction-feature/)
