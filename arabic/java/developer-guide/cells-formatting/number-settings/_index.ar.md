﻿---
title: إعدادات الرقم
type: docs
weight: 10
url: /ar/java/cells-number-settings/
---
## **ضبط تنسيقات العرض Numbers والتواريخ**

من الميزات القوية جدًا لبرنامج Microsoft Excel أنه يتيح للمستخدمين تعيين تنسيقات عرض القيم الرقمية والتواريخ. نحن نعلم أنه يمكن استخدام البيانات الرقمية لتمثيل قيم مختلفة بما في ذلك القيم العشرية والعملة والنسبة المئوية والكسر أو القيم المحاسبية ، إلخ. يتم عرض جميع هذه القيم الرقمية في تنسيقات مختلفة اعتمادًا على نوع المعلومات التي تمثلها. وبالمثل ، هناك العديد من التنسيقات التي يمكن عرض التاريخ أو الوقت بها.
Aspose.Cells يدعم هذه الوظيفة ويسمح للمطورين بتعيين أي تنسيق عرض لرقم أو تاريخ.

## **ضبط تنسيقات العرض في Microsoft Excel**

لتعيين تنسيقات العرض في Microsoft Excel:

1. انقر بزر الماوس الأيمن فوق أي خلية.
1.  يختار**شكل Cells**. سيظهر مربع حوار يستخدم لتعيين تنسيقات العرض لأي نوع من القيمة.

 في الجانب الأيسر من مربع الحوار ، هناك العديد من فئات القيم مثل**عام**, **عدد**, **عملة**, **محاسبة**, **تاريخ**, **وقت**, **النسبة المئوية،**الخ Aspose.Cells يدعم كل تنسيقات العرض هذه.

## **استخدام تنسيقات الأرقام المضمنة**

 يقدم Aspose.Cells بعض تنسيقات الأرقام المضمنة لتكوين تنسيقات عرض الأرقام والتواريخ. يتم إعطاء جميع تنسيقات الأرقام المضمنة قيمًا رقمية فريدة. يمكن للمطورين تعيين أي قيمة رقمية مطلوبة لملف[**عدد**](https://reference.aspose.com/cells/java/com.aspose.cells/style#Number) طريقة[**أسلوب**](https://reference.aspose.com/cells/java/com.aspose.cells/style) كائن لتطبيق تنسيق العرض. هذا النهج سريع. يتم سرد تنسيقات الأرقام المضمنة التي يدعمها Aspose.Cells أدناه.

|**قيمة**|**يكتب**|**تنسيق السلسلة**|
|:- |:- |:- |
|0|عام|عام|
|1|عدد عشري|0|
|2|عدد عشري|0.00|
|3|عدد عشري|# ,##0
|
|4|عدد عشري|# ,##0.00
|
|5|عملة|$#,##0;$-#,##0|
|6|عملة|$ # ، ## 0 ؛ [أحمر] $ - # ، ## 0|
|7|عملة|$#,##0.00;$-#,##0.00|
|8|عملة|$ # ، ## 0.00 ؛ [أحمر] $ - # ، ## 0.00|
|9|النسبة المئوية|0%|
|10|النسبة المئوية|0.00%|
|11|علمي|0.00E + 00|
|12|جزء|# ?/?
|
|13|جزء|# */*
|
|14|تاريخ|م / ي / س س س|
|15|تاريخ|د-ش ش-س ص|
|16|تاريخ|د ممممم|
|17|تاريخ|ش ش-س ص|
|18|وقت|ح: مم ص / م|
|19|وقت|h: mm: ss am / pm|
|20|وقت|همم|
|21|وقت|h: mm: ss|
|22|وقت|م / ي / س س س: مم|
|37|عملة|# ,##0;-#,##0
|
|38|عملة|# ، ## 0 ؛ [أحمر] - # ، ## 0
|
|39|عملة|# ,##0.00;-#,##0.00
|
|40|عملة|# ، ## 0.00 ؛ [أحمر] - # ، ## 0.00
|
|41|محاسبة|_ * #,##0_ ;_ * "_ ;_ @_|
|42|محاسبة|_ $* #,##0_ ;_ $* "_ ;_ @_|
|43|محاسبة|_ * #,##0.00_ ;_ * "??_ ;_ @_|
|44|محاسبة|_ $* #,##0.00_ ;_ $* "??_ ;_ @_|
|45|وقت|مم: ss|
|46|وقت|h: mm: ss|
|47|وقت|مم: ss.0|
|48|علمي|## 0.0E + 00
|
|49|نص|@|

{{< gist "aspose-cells-gists" "5876dc77e47649b66bdb5deefb4b5639" "UsingBuiltInNumberFormats-1.java" >}}

## **استخدام تنسيقات الأرقام المخصصة**

لتحديد سلسلة التنسيق المخصصة الخاصة بك لتعيين تنسيق العرض ، استخدم ملحق[**العادة**](https://reference.aspose.com/cells/java/com.aspose.cells/style#Custom). هذا النهج ليس بنفس سرعة استخدام التنسيقات المحددة مسبقًا ولكنه أكثر مرونة.


{{< gist "aspose-cells-gists" "5876dc77e47649b66bdb5deefb4b5639" "UsingCustomNumber-1.java" >}}

{{% alert color="primary" %}}

 إذا كنت تستخدم ملف[**العادة**](https://reference.aspose.com/cells/java/com.aspose.cells/style#Custom) لتعيين تنسيق الأرقام ، يتم تعيين أي تنسيق سابق باستخدام[**عدد**](https://reference.aspose.com/cells/java/com.aspose.cells/style#Number） is overridden and vice versa.

{{% /alert %}}

## **Advance topics**
- [Check Custom Number Format when Setting Style.Custom Property](/cells/java/check-custom-number-format-when-setting-style-custom-property/)
- [حدد رقم عشري مخصص وفواصل المجموعات للمصنف](/cells/ar/java/specify-custom-number-decimal-and-group-separators-for-workbook/)
- [تحديد تنسيق نمط مخصص DBNum](/cells/ar/java/specifying-dbnum-custom-pattern-formatting/)
