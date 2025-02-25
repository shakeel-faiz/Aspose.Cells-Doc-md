﻿---
title: كيفية الترحيل إلى Aspose.Cells 7.0.0 أو أعلى
type: docs
weight: 10
url: /ar/java/how-to-migrate-to-aspose-cells-7-0-0-or-higher/
---
{{% alert color="primary" %}}

في هذه المقالة ، شاركنا التغييرات الملحوظة في API التي تم إجراؤها في Aspose.Cells for Java 7.0.0 والإصدارات اللاحقة مقارنة بالإصدارات السابقة من Aspose.Cells for Java. ستساعد هذه المقالة المستخدمين على الهجرة بسرعة من API القديم إلى الجديد. API من خلال فهم التغييرات التي تم إجراؤها وتنفيذها في تطبيقاتهم.

{{% /alert %}}

## **تغييرات ملحوظة للمستخدمين الحاليين**

منذ إصدار Aspose.Cells for Java v7.0.0 ، أجرينا بعض التعديلات الرئيسية في API وأضفنا كل تلك الميزات الموجودة في Aspose.Cells for .NET حتى الآن. لذلك ، سيكون كل من Aspose.Cells for Java و .NET قابلين للمقارنة الآن من حيث الميزات وحتى من حيث أسماء الأساليب والخصائص.

على غرار الطريقة القديمة ، يمكنك فقط استيراد بيان استيراد واحد فقط في التطبيق الخاص بك لجلب جميع الفئات والواجهات وما إلى ذلك.

[**Java**]{{< highlight "java" >}}

 import com.aspose.cells.*;

{{< /highlight >}}

لقد أعدنا تسمية مجموعة API معينة لتنظيف بنية API لمطابقتها مع Aspose.Cells for .NET. لقد أضفنا بعض فئات المجموعة الآن واستبدلناها بفئات التجميع الحالية. تم استبدال فئة مثل أوراق العمل بـ**ورقة العمل** . وبالمثل ، تم استبدال فئة الأشكال بـ**ShapeCollection**. ومع ذلك ، لم تتأثر وظائف الفئات بل تم تحسينها.

إذا كنت ترغب في الانتقال إلى API الجديد ، فقد تحتاج إلى إجراء التغييرات التالية في التطبيق الخاص بك لجعل الأمور تعمل من أجلك. تحتوي القائمة التالية على التغييرات التي تم إجراؤها في الفصول الدراسية وطرقها أيضًا.

## **ملخص التغييرات في API**

1) المجموعات في الإصدار 2.5.4 أو ما قبله والتي تمت إعادة تسمية أسمائها المنتهية بـ 's'. في الإصدار 7.0.0 أو أعلى ، تمت تسمية المجموعات باسم:
على سبيل المثال ، الأشكال (القديمة) -> ShapeCollection (جديد) ، وأوراق العمل (القديمة) -> WorksheetCollection (جديد) ، ... ، إلخ.

2) تغيير الحصول على عنصر من المجموعة. على سبيل المثال ، في الإصدار 2.5.4 أو ما قبله ، اعتدنا القيام بذلك كـ getXXX (int) ، في الإصدار 7.0.0 أو أعلى ، الآن نقوم بذلك على أنه get (int):
على سبيل المثال ، Worksheets.getSheet (int) (Old) -> WorksheetCollection.get (int) (New) ، ... إلخ.

3) تغيير حجم (عدد العناصر) لمجموعة واحدة. في الإصدار 2.5.4 أو ما قبله ، اعتدنا القيام بذلك بالحجم () ، في الإصدار 7.0.0 أو أعلى ، والآن نقوم بذلك باستخدام getCount ():
Worksheets.size () (قديم) -> WorksheetCollection.getCount () (جديد) ، ... ، إلخ.

4) تم تغيير طرق الحصول على الخصائص المنطقية في الإصدار 2.5.4 أو ما قبله والتي تبدأ أسماؤها بـ "is". في الإصدار 7.0.0 ، بدأت هذه بـ "get":
على سبيل المثال ، PageSetup.isBlackAndWhite () (قديم) -> PageSetup.getBlackAndWhite () (جديد) ، ... ، إلخ.
