﻿---
title: Aspose.Cells for .NET 7.1.2 ملاحظات الإصدار
type: docs
weight: 90
url: /ar/net/aspose-cells-for-net-7-1-2-release-notes/
---
{{% alert color="primary" %}} 

 تحتوي هذه الصفحة على ملاحظات الإصدار لـ[Aspose.Cells for .NET 7.1.2](https://downloads.aspose.com/cells/net/new-releases/aspose.cells-for-.net-7.1.2/)

{{% /alert %}} 

 يسعدنا أن نعلن Aspose.Cells for .NET v7.1.2! 1) Aspose.Cells

 ميزات جديدة

 ` `- دعم الجداول في ملفات XLS - تخصيص الشريط XML40452 - Support Workbook.ContentTypePropertiesEnhancements

` `- ترجع الصيغة IF () "0" بدلاً من "# N / A" - مشاكل مع خاصية FirstPageNumber - تم تغيير التخطيط عند تحويل المستند إلى PDF - الخاصية "DragData" مفقودة في "PivotField" - تغيير مصدر البيانات في Pivot Table . - المشكلات المتعلقة بالجداول المحورية - تحويل الرسم التخطيطي / الأشكال لسير العمل إلى أداء صورة (صور)

 ` `- Worksheet.RemoveFormulas - مشكلة الأداء - Pdf Generation => OutOfMemoryException - الاستخدام المفرط للذاكرة عند تحويل Excel إلى PDF - الحفظ إلى PDF يستخدم 3 غيغابايت لملف Excel بحجم 10 ميغابايت - يستغرق فتح المصنف وقتًا طويلاً لفتح استثناءات

 ` `- استثناء NullReference أثناء عملية Save إذا كان نسخ ورقة العمل من مصنف آخر - Crash on Workbook.CalculateFormula () - طرح سمة RowSpan استثناء - حدث ArgumentOutOfRangeException أثناء تهيئة fileBugs

` `- مشكلات وظائف VLOOKUP و OFFSET - لم يتم حساب IRR بشكل صحيح - مشكلات حسابات MS Excel - تنسخ صيغة الصفيف باستخدام الدالة غير المباشرة () قيمة واحدة فقط - استثناء الخلايا في حساب صيغة TREND () - نسخة ورقة العمل تستبدل الرأس والتذييل - مشكلة طباعة Excel ملف يحتوي على صور EMF مضمنة - مشكلة الجدول المحوري - خطأ عامل التصفية في التنسيق - حقل PivotField - قراءة العناصر من ذاكرة التخزين المؤقت - مشكلات متعددة أثناء الترقية إلى أحدث الإصدارات - لا يعمل إنشاء مصنف باستخدام InputStream - تعطل الملف XLS المُنشأ MS Excel - القائمة المنسدلة والمخطط هما تمت إزالته من المصنف بعد حفظ - Aspose.Cells لا يطبق تنسيق الخلية المخصص بشكل صحيح - ملفات XLSM تالفة في ظل ظروف معينة - تم تغيير تنسيق حجم الخط Cell برقم غير صحيح - أدخل الرمز في نهاية قيمة الخلية 2) GridDesktop

 البق

` `- يتم عرض قيم الرسم البياني بشكل خاطئ لملف XLSX - مشكلة SUM () في ورقة عمل GridDesktop - يطرح GridDesktop.emportExcelFile () استثناء - كان الفهرس خارج حدود المصفوفة - مشكلة GridDestop في خلية (خلايا) الصيغة - Griddesktop.ImportExcelFile () يلقي OutOfMemoryException
