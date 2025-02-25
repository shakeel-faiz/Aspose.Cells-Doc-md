﻿---
title: قم بتثبيت Aspose.Cells على Windows
type: docs
weight: 20
url: /ar/net/installing-aspose-cells-on-windows/
---
{{% alert color="primary" %}} 

 في بعض الأحيان قد تواجه بعض المشاكل في التثبيت**Aspose.Cells** باستخدام حزمة المثبت الخاصة به (Aspose.Cells.msi ... Windows Installer Package) في**Windows فيستا** . يشرح هذا المستند كيف يمكننا التعامل معه وتنفيذ التثبيت الناجح للمكون. في الواقع**Aspose.Cells**يحتاج برنامج التثبيت إلى إنشاء مجلد افتراضي على IIS لنشر العروض التوضيحية على الويب (Asp.NET Demos) على جهازك ، لذلك يجب أن يكون لديك امتيازات الإدارة قبل التثبيت**Aspose.Cells** باستخدام المثبت الخاص به. يتطلب المثبت الوصول إلى النظام على مستوى المسؤول بشكل صريح للقيام بذلك.

{{% /alert %}} 
## **العوامل الممكنة**
 عادة ، في**Windows فيستا** ، دائمًا ما يتم تنفيذ المنتجات / المكونات التي تقوم بتثبيتها / استخدامها بموجب أذونات "المستخدم العادي" ، حتى لو كنت أحد مستخدمي**مدير** . يُسمح للبرامج فقط بالوصول المحدود إلى نظام الملفات ، حتى إذا قمت بتسجيل الدخول كملف**مدير** . هذا له بعض الآثار الجانبية المؤسفة التي لن تواجهها عادة في Windows XP عند تسجيل الدخول باعتبارك**مدير**.
## **UAC (التحكم في حساب المستخدم)**
**UAC** هو جزء من**Windows فيستا** يطلب منك الإذن. ال**UAC** الوضع (المعروف أيضًا باسم**وضع موافقة المسؤول** ) هو وضع تشغيل يؤثر (بشكل أساسي) على طريقة عمل حسابات المسؤول. متي**UAC**قيد التشغيل (وهو افتراضيًا) ، يجب أن تمنح إذنًا صريحًا لأي برنامج يريد استخدام صلاحيات "المسؤول". سيتم رفض الوصول إلى أي برنامج يحاول استخدام صلاحيات المسؤول دون إذنك.**UAC** مطلوب أيضًا لميزات الأمان الأخرى لـ**Windows فيستا** ، بما فيها**وضع حماية** في Internet Explorer. يعمل الوضع المحمي في Internet Explorer على حماية جهاز الكمبيوتر الخاص بك من صفحات الويب المارقة ونقاط الضعف الأخرى المتعلقة بالويب ، بما في ذلك تلك غير المعروفة.

 متي**UAC** تم تمكين الوضع ، سيتم منح كل برنامج تقوم بتشغيله وصول "مستخدم قياسي" فقط إلى النظام ، حتى عندما تقوم بتسجيل الدخول كمسؤول.**Windows فيستا** لديه القدرة المدمجة على الحد تلقائيًا من إمكانات المؤخرات الأمنية في النظام. يقوم بذلك عن طريق تمكين هذه الميزة المسماة تلقائيًا**التحكم في حساب المستخدم** (أو**UAC** لفترة قصيرة). ال**UAC**يفرض على المستخدمين الذين يشكلون جزءًا من مجموعة المسؤولين المحليين العمل كما لو كانوا مستخدمين عاديين بدون امتيازات إدارية. رغم**UAC** يحسن الأمن بشكل واضح**Windows فيستا** ، في ظل بعض السيناريوهات ، قد ترغب في تعطيله ، على سبيل المثال عند تقديم عروض توضيحية أمام الجمهور (العروض التوضيحية التي لا تتعلق بالأمان ، على سبيل المثال). قد يميل بعض المستخدمين المنزليين إلى التعطيل**UAC** بسبب استخدام موارد إضافية لنظامهم.
## **الخطوات المتضمنة للتثبيت الناجح للمكون**
-  يرجى التأكد من تثبيت IIS على نظام التشغيل Vista قبل التثبيت**Aspose.Cells** . إنه إلزامي لأن**Aspose.Cells** يحتاج برنامج التثبيت إلى إنشاء مجلد ظاهري على IIS لنشر العروض التوضيحية على الويب (Asp.NET Demos).
-  تحتاج إلى تعطيل**UAC** (التحكم في حساب المستخدم). عليك التأكد من أن لديك ملف**امتيازات المسؤول** مع التحكم الكامل في النظام قبل التثبيت**Aspose.Cells** . وإلا فقد تحصل على خطأ # 2869 أثناء التثبيت**Aspose.Cells**باستخدام المثبت الخاص به.

فيما يلي بعض الطرق لتحقيق ذلك.
### **باستخدام سطر الأوامر**
1.  ابحث عن cmd.exe في دليل windows ، ثم انقر بزر الماوس الأيمن فوقه وحدد تشغيل باسم ...**مدير**
 2. الآن ، قم بتشغيل الأمر التالي في موجه الأوامر: msiexec / i<your path>/Aspose.Cells.msi وإدخال.
### **باستخدام لوحة التحكم**
- انقر فوق ابدأ
- انقر فوق لوحة التحكم
- انقر فوق حسابات المستخدمين وأمان العائلة
- انقر فوق حسابات المستخدمين
- انقر فوق تشغيل التحكم في حساب المستخدم أو إيقاف تشغيله
- قم بإلغاء تحديد خانة الاختيار
- انقر فوق موافق

{{% alert color="primary" %}} 

ستحتاج إلى إعادة تشغيل جهاز الكمبيوتر حتى يسري التغيير. يؤثر هذا التغيير على جميع الحسابات على الكمبيوتر ، وليس حسابك فقط.

{{% /alert %}}
