﻿---
title: تعديل نمط موجود
type: docs
weight: 90
url: /ar/net/modify-an-existing-style/
---
{{% alert color="primary" %}}

لتطبيق نفس خيارات التنسيق على الخلايا ، قم بإنشاء كائن نمط تنسيق جديد. كائن نمط التنسيق عبارة عن مجموعة من خصائص التنسيق ، مثل الخط وحجم الخط والمسافة البادئة والرقم والحدود والأنماط وما إلى ذلك ، والتي يتم تسميتها وتخزينها كمجموعة. عند تطبيقه ، يتم تطبيق كل التنسيقات بهذا النمط.

يمكنك أيضًا استخدام نمط موجود وحفظه في المصنف واستخدامه لتنسيق المعلومات بنفس السمات.

 عندما لا يتم تنسيق الخلايا بشكل صريح ، فإن ملف**طبيعي** يتم تطبيق النمط (النمط الافتراضي للمصنف). يعرف Microsoft Excel مسبقًا عدة أنماط بالإضافة إلى النمط العادي بما في ذلك الفاصلة والعملة والنسبة المئوية.

يسمح Aspose.Cells بتعديل أي من هذه الأنماط أو أي نمط آخر تقوم بتعريفه بالسمات التي تريدها.

{{% /alert %}}

## **باستخدام Microsoft إكسل**

لتحديث نمط في Microsoft Excel 97-2003:

1.  على ال**شكل** القائمة ، انقر فوق**أسلوب**.
1.  حدد النمط الذي تريد تعديله من ملف**اسم النمط** قائمة.
1.  انقر**يُعدِّل**.
1. حدد خيارات النمط التي تريدها باستخدام علامات التبويب في مربع الحوار تنسيق Cells.
1.  انقر**نعم**.
1.  تحت**يشمل النمط**، حدد ميزات النمط التي تريدها.
1.  انقر**نعم** لحفظ النمط وتطبيقه على النطاق المحدد.

## **باستخدام Aspose.Cells**

 توضح الأمثلة التالية كيفية الاستخدام[**النمط**](https://reference.aspose.com/cells/net/aspose.cells/style/methods/update)طريقة.

### **إنشاء وتعديل النمط**

 هذا المثال ينشئ ملف[**أسلوب**](https://reference.aspose.com/cells/net/aspose.cells/style) كائن ، يطبقه على نطاق من الخلايا ويعدل[**أسلوب**](https://reference.aspose.com/cells/net/aspose.cells/style)موضوع. يتم تطبيق التعديلات تلقائيًا على الخلية والنطاق الذي تم تطبيق النمط عليه.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Articles-ModifyExistingStyle-ModifyThroughStyleObject-1.cs" >}}

### **تعديل نمط موجود**

يستخدم هذا المثال ملف Excel نموذجيًا بسيطًا تم تطبيق نمط يسمى النسبة المئوية بالفعل على نطاق. المثال:

1. يحصل على الاسلوب
1. يخلق كائن نمط و
1. يعدل تنسيق النمط.

يتم تطبيق التعديلات تلقائيًا على النطاق الذي تم تطبيق النمط عليه.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Articles-ModifyExistingStyle-ModifyThroughSampleExcelFile-1.cs" >}}
