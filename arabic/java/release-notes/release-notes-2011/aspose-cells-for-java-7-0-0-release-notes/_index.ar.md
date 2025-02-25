﻿---
title: Aspose.Cells for Java 7.0.0 ملاحظات الإصدار
type: docs
weight: 40
url: /ar/java/aspose-cells-for-java-7-0-0-release-notes/
---
{{% alert color="primary" %}} 

 تحتوي هذه الصفحة على ملاحظات الإصدار لـ[Aspose.Cells for Java 7.0.0](https://downloads.aspose.com/cells/java/new-releases/aspose.cells-for-java-7.0.0/)

{{% /alert %}} 

 مقدمة

يسعدنا أن نعلن Aspose.Cells for Java v7.0.0 للمستخدمين. هذا هو الإصدار الأول الذي نقلناه تلقائيًا من كود .NET الخاص بنا ، وبالتالي ، قد يحتوي على العديد من الميزات التي كانت مفقودة في الإصدارات السابقة Aspose.Cells for Java. هذا الإصدار هو معلم رئيسي لأنه من الآن فصاعدًا يمكننا العمل بكفاءة أكبر وهذا يعني ببساطة أفضل Aspose.Cells for Java بالنسبة لك. والسبب في ذلك هو أنه يمكننا الآن الاحتفاظ بمنتجين Aspose.Cells for Java و Aspose.Cells for .NET من قاعدة شفرة مصدر واحدة. من الآن فصاعدًا ، يشتمل المنتجان على نفس مجموعة الميزات والإصلاحات تقريبًا ويتم إصدارهما في نفس اليوم أيضًا.

 نظرة عامة على التغييرات

 ليس من الشائع بالنسبة لنا إجراء تغييرات كسر على API ونحاول دائمًا تجنب ذلك كلما أمكن ذلك ، ولكن في بعض الأحيان يكون ذلك ضروريًا. في هذه الحالة تحدث التغييرات في الإصدار الجديد للأسباب التالية:

- خطوة نحو استخدام Aspose Unified Framework الذي يملي API محسّنًا للتحميل والحفظ. هذا يجعل API أكثر تنظيماً واتساقاً ليتم استخدامه في جميع منتجات Aspose.
- سيتم الآن تحويل رمز المصدر من النظام الأساسي .NET تلقائيًا إلى النظام الأساسي Java. سيؤدي هذا إلى تمكين Aspose.Cells for Java لمطابقة Aspose.Cells for .NET ميزة تلو الأخرى.

 الميزات / التحسينات الجديدة



 هناك بعض الميزات التي تم تضمينها / تحسينها الآن.

-  إصدارات مجمعة منفصلة من المنتج لمختلف JDKs ، على سبيل المثال 1.4 ، 1.5 ، 1.6
 قم بتعيين الصيغ مع المراجع الخارجية
 دعم ListObjects / الجداول
 دعم كائنات الأشكال التلقائية
 تم إجراء تحسينات لميزة Shape-to-Image
 تم إجراء تحسينات لميزة الرسم البياني للصورة
 تم إجراء تحسينات لميزة "الورقة إلى الصورة"
 تم إجراء تحسينات لميزة Excel-to-PDF
 تم إجراء تحسينات على ميزة "احتواء تلقائي للصفوف / الأعمدة"

المشكلات / القيود المعروفة



 هناك عدد من القيود المعروفة في هذا الإصدار. هناك بعض الميزات التي قد لا تكون مدعومة في الإصدار 7.0.0 والتي كانت مدعومة بالفعل في الإصدارات الأقدم:

- استخدام واجهات برمجة تطبيقات LightCells
 قراءة HTML ملفات
 قراءة / حفظ المخططات / الأشكال لملفات ODS
 الاحتفاظ بوحدات الماكرو عند قراءة ملف ODS وحفظ وحدات الماكرو مرة أخرى إلى ملف ODS



 تغييرات ملحوظة للمستخدمين الحاليين



في هذا الإصدار (Aspose.Cells for Java v7.0.0) ، قمنا بإعادة تسمية بعض واجهات برمجة التطبيقات التي تم تعيينها لتنظيف بنية API لتتناسب مع Aspose.Cells for .NET. لدينا بعض فئات التجميع ولكن أسمائهم لا تبررهم وفقًا لمعايير .NET. لذلك ، قررنا تغيير أسماء بعض الفئات والأعضاء الآخرين وفقًا لذلك. بسبب هذه التغييرات ، قد تحتاج إلى إصلاح أجزاء معينة من مقاطع الكود الموجودة لديك عند الترقية من إصدارك السابق رقم Aspose.Cells for Java. إذا لم تستخدم أيًا من الأعضاء المذكورين أدناه ، فعلى الأرجح أنك لن تحتاج إلى إجراء أي تغييرات حيث سيتم بالفعل ترجمة التعليمات البرمجية الخاصة بك بنجاح مع الإصدار الجديد. تظل جميع الوظائف نفسها كما هي ، وتم نقل الوصول إلى بعض الأعضاء فقط أو إعادة تسميته أو دمجه في طرق أخرى.

ملاحظة: لقد بذلنا قصارى جهدنا لنفقد أي وظيفة من الإصدارات / الإصلاحات السابقة من خلال إعادة تحليل API ، لكنني أخشى أنك قد تجد بعض المشكلات وقد لا يجتاز هذا الإصدار جميع حالات الاختبار. نحن نعمل باستمرار على تحسينه للتأكد من أن الإصدار الجديد يعمل بشكل جيد بنسبة 100٪ مع جميع المشكلات السابقة (التي تم إصلاحها في الإصدارات / إصلاحات المنتج السابقة). نحن بحاجة إلى مزيد من الوقت لتقييمها جميعًا وجعل المنتج أكثر قوة. كما نشجعكم جميعًا على تقييم المشكلات السابقة مع هذا الإصدار الجديد في بيئاتكم المتنوعة. لا تتردد في إعلامنا بأي مشكلة باستخدام منتدى Aspose.Cells. إن تعاونك في هذا الصدد محل تقدير كبير.
