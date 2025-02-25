﻿---
title: الترخيص
type: docs
weight: 21
url: /ar/python-net/licensing/
---
{{% alert color="primary" %}}

 يمكنك بسهولة تنزيل نسخة تقييمية لـ Aspose.Cells Python عبر .Net من موقعه[صفحة التحميل](https://pypi.org/project/aspose-cells-python/) Pypi repos. يوفر الإصدار التقييمي نفس الإمكانات تمامًا مثل الإصدار المرخص من المكون. علاوة على ذلك ، يصبح الإصدار التقييمي مرخصًا ببساطة عند شراء ترخيص وإضافة سطرين من التعليمات البرمجية لتطبيق الترخيص.

{{% /alert %}}

## **قيود إصدار التقييم**

توفر نسخة التقييم من Aspose.Cells Python عبر منتج نت (بدون ترخيص محدد) وظائف المنتج الكاملة ، ولكنها تقتصر على فتح 100 ملف في برنامج واحد وورقة عمل إضافية مع علامة مائية للتقييم.

القيود موضحة أدناه:

- **عدد الملفات المفتوحة** (Aspose.Cells Python عبر .Net)
 عند تشغيل برنامجك ، يمكنك فقط فتح 100 ملف Excel باستخدام Aspose.Cells Python عبر .Net library. إذا تجاوز التطبيق الخاص بك هذا الرقم ، فسيتم طرح استثناء.


علاوة على ذلك ، ستظهر ورقة العمل التي تحتوي على علامة مائية للتقييم دائمًا على أنها ورقة العمل النشطة في ملف Excel الذي تم إنشاؤه باستخدام Aspose.Cells Python عبر المكتبة. فقط في الإصدار المرخص ، يمكنك تعيين ورقة العمل النشطة على أوراق عمل أخرى. في الإخراج PDF أو ملف الصورة بواسطة Aspose.Cells Python عبر ، سيتم لصق علامة مائية للتقييم في أعلى المستند / الصورة.

{{% alert color="primary" %}}

 إذا كنت ترغب في اختبار Aspose.Cells Python عبر بدون قيود إصدار التقييم ، يمكنك أيضًا طلب[ترخيص مؤقت لمدة 30 يومًا](https://purchase.aspose.com/temporary-license).

{{% /alert %}}

## **تطبيق رخصة في Aspose.Cells Python عبر المكون**

الترخيص عبارة عن ملف XML نص عادي يحتوي على تفاصيل مثل اسم المنتج وعدد المطورين المرخص لهم وتاريخ انتهاء الاشتراك وما إلى ذلك. الملف موقّع رقميًا ، لذا لا تعدّل الملف. حتى الإضافة غير المقصودة لكسر سطر إضافي في الملف سوف يبطل ذلك. تحتاج إلى تعيين ترخيص قبل استخدام Aspose.Cells Python عبر إذا كنت تريد تجنب قيود التقييم الخاصة به. مطلوب فقط تعيين ترخيص مرة واحدة لكل تطبيق (أو عملية). يمكن تحميل الترخيص من ملف.

Aspose.Cells Python عن طريق محاولة العثور على الترخيص في مواقع المسار الصريح.

هناك طريقتان شائعتان لتطبيق ترخيص من ملف.

### **تطبيق ترخيص من القرص**

أسهل طريقة لتعيين ترخيص ، هي وضع ملف الترخيص في المسار الصريح.

{{< highlight "csharp" >}}

 //Instantiate an instance of license and set the license file through its path

license = License();
 //For Windows
license.set_license("D:\Aspose.Cells.lic");
 //For Linux or MacOS
license.set_license("/home/yourusername/Aspose.Cells.lic"); 
{{< /highlight >}}

{{% alert color="primary" %}}

عند استدعاء المجموعة_طريقة الترخيص ، يجب أن يكون اسم الترخيص هو نفسه اسم ملف الترخيص الخاص بك. على سبيل المثال ، يمكنك تغيير اسم ملف الترخيص إلى ** Aspose.Cells.lic.xml **. ثم في التعليمات البرمجية الخاصة بك ، يجب عليك استخدام اسم الترخيص المعدل (** Aspose.Cells.lic.xml **) للمجموعة_طريقة الترخيص.

{{% /alert %}}


