﻿---
title: فتح ملفات إصدارات Excel Microsoft المختلفة
type: docs
weight: 20
url: /ar/python-java/opening-different-microsoft-excel-versions-files/
---
{{% alert color="primary" %}}

يمكن لـ Aspose.Cells فتح نطاق من ملفات إصدارات Excel Microsoft المختلفة ، مثل Microsoft Excel 95/97-2003 ، SpreadsheetML ، فتح Microsoft Excel 2007/2010/2013/2016/2019 و Office 365 XLSX أو ملفات Excel المشفرة.

{{% /alert %}}

## **فتح ملفات مختلفة من إصدارات إكسل Microsoft**

 غالبًا ما يجب أن يكون التطبيق قادرًا على فتح ملفات Excel Microsoft التي تم إنشاؤها في إصدارات مختلفة ، على سبيل المثال ، Microsoft Excel 95،97 أو Microsoft Excel 2007/2010/2013/2016/2019 و Office 365. قد تحتاج إلى تحميل ملف بأي من التنسيقات المتعددة ، بما في ذلك XLS ، XLSX ، XLSM ، XLSB ، SpreadsheetML ، TabDelimited أو TSV ، CSV ، ODS وما إلى ذلك. استخدم المنشئ أو حدد**[مصنف] (https://reference.aspose.com/cells/python-java/asposecells.api/Workbook)** صف دراسي'**[setFileFormat] (https://reference.aspose.com/cells/python-java/asposecells.api/workbook#FileFormat)**طريقة لتحديد التنسيق باستخدام**[FileFormatType] (https://reference.aspose.com/cells/python-java/asposecells.api/FileFormatType)**تعداد.
	
 ال**[FileFormatType] (https://reference.aspose.com/cells/python-java/asposecells.api/FileFormatType)**يحتوي التعداد على العديد من تنسيقات الملفات المحددة مسبقًا والتي يرد بعضها أدناه.

|**أنواع تنسيق الملف**|**وصف**|
|:- |:- |
|CSV|يمثل ملف CSV|
|اكسل_97_TO_2003|يمثل ملف Excel 97 - 2003|
|XLSX|يمثل ملف Excel 2007/2010/2013/2016/2019 و Office 365 XLSX|
|XLSM|يمثل ملف Excel 2007/2010/2013/2016/2019 و Office 365 XLSM|
|XLTX|يمثل ملف Excel 2007/2010/2013/2016/2019 ونموذج Office 365 XLTX|
|XLTM|يمثل ملف XLTM ممكّن للماكرو في Excel 2007/2010/2013/2016/2019 و Office 365|
|XLSB|يمثل ملف Excel 2007/2010/2013/2016/2019 و Office 365 ثنائي XLSB|
|SPREADSHEET_ML|يمثل ملف SpreadsheetML|
|TSV|يمثل ملف قيم مفصولة بعلامات جدولة|
|علامة التبويب محدد|يمثل ملفًا نصيًا محددًا بعلامات جدولة|
|ODS|يمثل ملف ODS|
|HTML|يمثل ملف HTML|
|M_HTML|يمثل ملف MHTML|

### **فتح Microsoft ملفات Excel 95 / 5.0**

لفتح ملف Microsoft Excel 95 / 5.0 ، استخدم**[LoadOptions] (https://reference.aspose.com/cells/python-java/asposecells.api/LoadOptions)**وقم بتعيين السمة ذات الصلة لـ**LoadOptions**فئة ملف القالب المراد تحميله. يمكن تنزيل نموذج ملف لاختبار هذه الميزة من الرابط التالي:

[ملف Excel95](Excel95.xls)

{{< gist "aspose-cells-gists" "32e50c6aabc547111966569f3fd39694" "OpenExcel95Files.py" >}}

### **فتح Microsoft ملفات Excel 97-2003**

 لفتح ملف Microsoft Excel 97-2003 ، استخدم**[LoadOptions] (https://reference.aspose.com/cells/python-java/asposecells.api/LoadOptions)** وقم بتعيين السمة ذات الصلة لـ**LoadOptions**فئة ملف القالب المراد تحميله.

{{< gist "aspose-cells-gists" "32e50c6aabc547111966569f3fd39694" "OpenExcel97-2003Files.py" >}}

### **فتح Microsoft Excel 2007/2010/2013/2016/2019 وملفات Office 365 XLSX**

لفتح تنسيق Microsoft Excel 2007/2010/2013/2016/2019 وتنسيق Office 365 ، أي XLSX أو XLSB ، حدد مسار الملف. تستطيع ايضا استخذام**[LoadOptions] (https://reference.aspose.com/cells/python-java/asposecells.api/LoadOptions)** وقم بتعيين السمة / الخيارات ذات الصلة لـ**LoadOptions**فئة ملف القالب المراد تحميله.

{{< gist "aspose-cells-gists" "32e50c6aabc547111966569f3fd39694" "OpenExcel2007Files.py" >}}

### **فتح ملفات اكسل المشفرة**

 من الممكن إنشاء ملفات Excel مشفرة باستخدام Microsoft Excel. لفتح ملف مشفر ، استخدم ملحق**[LoadOptions] (https://reference.aspose.com/cells/net/aspose.cells/loadoptions)**وقم بتعيين سماته وخياراته (على سبيل المثال ، أعط كلمة مرور) لملف القالب المراد تحميله.
يمكن تنزيل نموذج ملف لاختبار هذه الميزة من الرابط التالي:

[اكسل مشفر](EncryptedExcel.xlsx)

{{< gist "aspose-cells-gists" "32e50c6aabc547111966569f3fd39694" "OpenEncryptedExcelFiles.py" >}}

يدعم Aspose.Cells أيضًا فتح ملفات Microsoft المحمية بكلمة مرور في Excel 2007 و 2010 و 2013 و 2016 و 2019 و Office 365.


