﻿---
title: فتح ملفات بتنسيقات مختلفة
type: docs
weight: 30
url: /ar/python-java/opening-files-with-different-formats/
description: Aspose.Cells for .NET API يسمح لك بفتح / قراءة تنسيقات مختلفة مثل XLSX ، HTML ، CSV ، ODS ، TSV ، SXC ، FODS ، إلخ.
keywords: open xlsx files, open html files, read fods files, read ods files, read sxc files, open csv files, Tab Delimited, SpreadsheetML, tsv, mhtml
---
{{% alert color="primary" %}}

 باستخدام Aspose.Cells يمكنك فتح الملفات بتنسيقات مختلفة.**Aspose.Cells** يمكن فتح مجموعة من تنسيقات الملفات مثل Microsoft جداول بيانات Excel (XLS ، XLSX ، XLSM ، XLSB) ، SpreadsheetML ، قيم مفصولة بفواصل (CSV) ، ملفات مفصولة بعلامات جدولة أو ملفات مفصولة بعلامات جدولة (TSV) إلخ.

إذا كنت بحاجة إلى معرفة جميع تنسيقات الملفات المدعومة ، فيرجى الرجوع إلى الصفحات التالية:
[تنسيقات الملفات المدعومة](https://docs.aspose.com/cells/python-java/supported-file-formats/)

{{% /alert %}}

## **فتح ملفات بتنسيقات مختلفة**

Aspose.Cells يسمح للمطورين بفتح ملفات جداول البيانات بتنسيقات مختلفة مثل SpreadsheetML ، قيم مفصولة بفواصل (CSV) ، قيم مفصولة بعلامات جدولة أو قيم مفصولة بعلامات جدولة (TSV) ، ملفات ODS. لفتح مثل هذه الملفات ، يمكن للمطورين استخدام نفس المنهجية التي يستخدمونها لفتح ملفات مختلفة من إصدارات Microsoft Excel.

### **فتح SpreadsheetML الملفات**

ملفات SpreadsheetML عبارة عن تمثيلات XML لجداول البيانات بما في ذلك جميع المعلومات المتعلقة بها ، مثل التنسيق والصيغ وما إلى ذلك. منذ Microsoft Excel XP ، تمت إضافة خيار تصدير XML إلى Microsoft Excel الذي يقوم بتصدير جداول البيانات الخاصة بك إلى ملفات SpreadsheetML.

{{< gist "aspose-cells-gists" "32e50c6aabc547111966569f3fd39694" "OpenSpreadsheetMLFile.py" >}}

### **فتح HTML الملفات**

Aspose.Cells يسمح لك بفتح ملف HTML في كائن المصنف. يجب أن يكون الملف HTML موجهًا إلى Microsoft Excel ، أي يجب أن يكون MS-Excel قادرًا على فتحه.

{{< gist "aspose-cells-gists" "32e50c6aabc547111966569f3fd39694" "OpenHTMLFile.py" >}}

### **فتح CSV الملفات**

تحتوي ملفات القيم المفصولة بفواصل (CSV) على سجلات حيث يتم فصل القيم بفاصلات. يتم تخزين البيانات كجدول حيث يتم فصل كل عمود عن طريق الفاصلة ويتم اقتباسها بحرف اقتباس مزدوج. إذا احتوت قيمة الحقل على علامة اقتباس مزدوجة ، يتم تخطيها بزوج من علامات الاقتباس المزدوجة. يمكنك أيضًا استخدام Microsoft Excel لتصدير بيانات جدول البيانات إلى CSV.

{{< gist "aspose-cells-gists" "32e50c6aabc547111966569f3fd39694" "OpenCSVFile.py" >}}

#### **فتح CSV الملفات واستبدال الحروف غير الصالحة**

في Excel ، عند فتح ملف CSV بأحرف خاصة ، يتم استبدال الأحرف تلقائيًا. يتم القيام بنفس الشيء بواسطة Aspose.Cells API والذي هو موضح في مثال الكود الموضح أدناه.

{{< gist "aspose-cells-gists" "32e50c6aabc547111966569f3fd39694" "OpenCSVFileAndReplaceInvalidCharacters.py" >}}

يمكن تنزيل نموذج ملف المصدر من الروابط التالية لاختبار هذه الميزة.

[InvalidCharacters.csv](InvalidCharacters.csv)

### **فتح ملفات نصية باستخدام فاصل مخصص**

تُستخدم الملفات النصية للاحتفاظ ببيانات جدول البيانات بدون تنسيق. الملف عبارة عن ملف نصي عادي يمكن أن يحتوي على بعض المحددات المخصصة.

{{< gist "aspose-cells-gists" "32e50c6aabc547111966569f3fd39694" "OpenTextFilewithCustomSeparator.py" >}}

يمكن تنزيل نموذج ملف المصدر من الروابط التالية لاختبار هذه الميزة.

[CustomSeparator.txt](CustomSeparator.txt)

### **فتح ملفات محدده بعلامات تبويب**

يحتوي الملف المحدد بعلامات جدولة (نص) على بيانات جدول بيانات ولكن بدون أي تنسيق. يتم ترتيب البيانات في صفوف وأعمدة كما هو الحال في الجداول وجداول البيانات. بشكل أساسي ، الملف المحدد بعلامات جدولة هو نوع خاص من ملفات النص العادي مع علامة تبويب بين كل عمود.

{{< gist "aspose-cells-gists" "32e50c6aabc547111966569f3fd39694" "OpenTabDelimitedFile.py" >}}

يمكن تنزيل نموذج ملف المصدر من الروابط التالية لاختبار هذه الميزة.

[TabDelimited.txt](TabDelimited.txt)

### **فتح ملفات قيم مفصولة بعلامات جدولة (TSV)**

يحتوي ملف القيم المفصولة بعلامات جدولة (TSV) على بيانات جدول بيانات ولكن بدون أي تنسيق. هو نفسه مع ملف محدد بعلامات جدولة حيث يتم ترتيب البيانات في صفوف وأعمدة كما هو الحال في الجداول وجداول البيانات.

{{< gist "aspose-cells-gists" "32e50c6aabc547111966569f3fd39694" "OpenTSVFile.py" >}}

### **فتح SXC الملفات**

StarOffice Calc مشابه لـ Microsoft Excel ويدعم الصيغ والمخططات والوظائف ووحدات الماكرو. يتم حفظ جداول البيانات التي تم إنشاؤها باستخدام هذا البرنامج بالملحق SXC. يتم استخدام ملف SXC أيضًا لملفات جداول بيانات OpenOffice.org Calc. يمكن Aspose.Cells قراءة ملفات SXC كما هو موضح في نموذج التعليمات البرمجية التالي.

{{< gist "aspose-cells-gists" "32e50c6aabc547111966569f3fd39694" "OpenSXCFile.py" >}}

### **فتح FODS الملفات**

الملف FODS هو جدول بيانات محفوظ في OpenDocument XML بدون أي ضغط. يمكن لـ Aspose.Cells قراءة ملفات FODS كما هو موضح في نموذج التعليمات البرمجية التالي.

{{< gist "aspose-cells-gists" "32e50c6aabc547111966569f3fd39694" "OpenFODSFile.py" >}}
