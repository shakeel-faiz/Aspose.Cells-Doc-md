﻿---
title: إدارة التعليقات والملاحظات
linktitle: التعليقات والملاحظات
type: docs
weight: 128
url: /ar/net/comments-and-notes/
description: قم بإدراج وإدارة التعليقات أو الملاحظات باستخدام Aspose.Cells لـ .Net.
keywords: insert comments, insert notes
---
## **مقدمة**

تستخدم التعليقات لإضافة معلومات إضافية إلى الخلايا. يوفر Aspose.Cells طريقتين لإضافة التعقيبات إلى الخانات. الأول هو إنشاء تعليقات في ملف المصمم يدويًا. ثم يتم استيراد هذه التعليقات باستخدام Aspose.Cells. والثاني هو إضافة تعليقات باستخدام Aspose.Cells API في وقت التشغيل. يناقش هذا الموضوع إضافة التعليقات إلى الخلايا باستخدام Aspose.Cells API. سيتم أيضًا شرح تنسيق التعليقات.

## **إضافة تعليق**

 أضف تعليقًا إلى خلية عن طريق استدعاء[**تعليقات**](https://reference.aspose.com/cells/net/aspose.cells/commentcollection) المجموعة[**يضيف**](https://reference.aspose.com/cells/net/aspose.cells/commentcollection/methods/add/index) طريقة (مغلفة في[**ورقة عمل**](https://reference.aspose.com/cells/net/aspose.cells/worksheet) موضوع). الجديد[**تعليق**](https://reference.aspose.com/cells/net/aspose.cells/comment) يمكن الوصول إلى الكائن من خلال[**تعليقات**](https://reference.aspose.com/cells/net/aspose.cells/commentcollection) المجموعة عن طريق تمرير فهرس التعليقات. بعد الوصول إلى ملف[**تعليق**](https://reference.aspose.com/cells/net/aspose.cells/comment) ، قم بتخصيص ملاحظة التعليق باستخدام[**تعليق**](https://reference.aspose.com/cells/net/aspose.cells/comment) أشياء[**ملحوظة**](https://reference.aspose.com/cells/net/aspose.cells/comment/properties/note)خاصية.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-DrawingObjects-Comments-AddingComment-1.cs" >}}

## **تنسيق التعليق**

من الممكن أيضًا تنسيق مظهر التعليقات من خلال تكوين إعدادات الطول والعرض والخط.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-DrawingObjects-Comments-CommentFormatting-1.cs" >}}

## **أضف صورة للتعليق**

باستخدام Microsoft Excel 2007 ، من الممكن أيضًا الحصول على صورة كخلفية لتعليق الخلية. يتم تحقيق ذلك في Excel 2007 عن طريق القيام بالخطوات التالية. (يفترضون أنك قمت بالفعل بإضافة تعليق خلية.)

1. انقر بزر الماوس الأيمن فوق الخلية التي تحتوي على التعليق.
1.  يختار**إظهار / إخفاء التعليقات**، وامسح أي نص من التعليق.
1. انقر فوق حد التعليق لتحديده.
1.  يختار**شكل** ، ومن بعد**تعليق**.
1.  على ال**الألوان والخطوط** علامة التبويب ، قم بتوسيع**اللون** قائمة.
1.  انقر**تأثيرات التعبئة**.
1.  على ال**صورة** علامة التبويب ، انقر فوق**حدد صورة**.
1. حدد موقع الصورة وحددها.
1.  انقر**نعم** حتى يتم إغلاق جميع الحوارات.

يوفر Aspose.Cells أيضًا هذه الميزة. يوجد أدناه نموذج رمز يقوم بإنشاء ملف XLSX من البداية ، مضيفًا تعليقًا إلى الخلية "A1" مع تعيين صورة كخلفية لها.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-DrawingObjects-Comments-AddImageToComment-1.cs" >}}

## **موضوعات مسبقة**
- [تغيير اتجاه النص للتعليق](/cells/ar/net/change-text-direction-of-the-comment/)
- [كيفية تغيير لون خط التعليق](/cells/ar/net/how-to-change-the-comment-font-color/)
- [كيفية تعيين خلفية التعليق](/cells/ar/net/how-to-set-comment-background/)
- [تعليقات مترابطة](/cells/ar/net/threaded-comments/)

