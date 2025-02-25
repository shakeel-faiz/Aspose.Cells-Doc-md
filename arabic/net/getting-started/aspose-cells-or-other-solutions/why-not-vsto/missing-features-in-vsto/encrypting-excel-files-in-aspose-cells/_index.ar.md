﻿---
title: تشفير ملفات Excel في Aspose.Cells
type: docs
weight: 90
url: /ar/net/encrypting-excel-files-in-aspose-cells/
---
{{% alert color="primary" %}} 

يمكّنك Microsoft Excel (97-2007) من تشفير جداول البيانات وحمايتها بكلمة مرور. يستخدم الخوارزميات التي يوفرها مزود خدمة التشفير ، أو CSP ، وهي مجموعة من خوارزميات التشفير ذات الخصائص المختلفة. CSP الافتراضي هو "متوافق مع Office 97/2000" أو "تشفير ضعيف (XOR)". من المهم اختيار طول مفتاح التشفير المناسب. لا يدعم بعض CSPs أكثر من 40 أو 56 بت. يعتبر هذا تشفيرًا ضعيفًا. للتشفير القوي ، يجب ألا يقل طول المفتاح عن 128 بت. يحتوي Microsoft Windows على CSPs الذين يقدمون أنواع تشفير قوية أيضًا ، على سبيل المثال "موفر التشفير القوي Microsoft". لإعطائك فكرة ، تشفير 128 بت هو ما تستخدمه البنوك لتشفير الاتصال بأنظمتها المصرفية عبر الإنترنت.

يسمح لك Aspose.Cells بتشفير وحماية كلمة مرور Microsoft ملفات Excel بنوع التشفير المطلوب.

{{% /alert %}} 
## **باستخدام Microsoft إكسل**
لتعيين إعدادات تشفير الملفات في Microsoft Excel (هنا Microsoft Excel 2003):

1.  من**أدوات** القائمة ، حدد**خيارات**.
 يظهر مربع حوار.
1.  حدد ملف**حماية** التبويب.
1.  أدخل كلمة مرور وانقر**متقدم** 
   **مربع حوار الخيارات** 

![ما يجب القيام به: image_بديل_نص](encrypting-excel-files-in-aspose-cells_1.png)




1.  اختر نوع التشفير وقم بتأكيد كلمة المرور.

   **مربع حوار نوع التشفير** 

![ما يجب القيام به: image_بديل_نص](encrypting-excel-files-in-aspose-cells_2.png)



## **التشفير مع Aspose.Cells**
يوضح المثال التالي كيفية تشفير وحماية كلمة المرور لملف excel باستخدام Aspose.Cells API.

**C#**

{{< highlight "csharp" >}}

 //Instantiate a Workbook object.

//Open an excel file.

Workbook workbook = new Workbook("Book1.xls");

//Specify XOR encryption type.

workbook.SetEncryptionOptions(EncryptionType.XOR,40);

//Specify Strong Encryption type (RC4,Microsoft Strong Cryptographic Provider).

workbook.SetEncryptionOptions(EncryptionType.StrongCryptographicProvider, 128);

//Password protect the file.

workbook.Settings.Password = "1234";

//Save the excel file.

workbook.Save("encryptedBook1.xls");



{{< /highlight >}}
## **قم بتنزيل كود التشغيل**
- [جيثب](https://github.com/aspose-cells/Aspose.Cells-for-.NET/tree/master/Plugins/Aspose.Cells%20Vs%20VSTO%20Spreadsheets/Aspose.Cells%20Features%20missing%20in%20VSTO/Encrypting%20Excel%20Files)
## **تنزيل نموذج التعليمات البرمجية**
- [جيثب](https://github.com/aspose-cells/Aspose.Cells-for-.NET/releases/tag/MissingFeaturesAsposeCellsForVSTO1.1))
