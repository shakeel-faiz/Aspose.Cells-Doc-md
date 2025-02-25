﻿---
title: Aspose.Cells for Java 18.1 Примечания к выпуску
type: docs
weight: 120
url: /ru/java/aspose-cells-for-java-18-1-release-notes/
---
{{% alert color="primary" %}} 

Эта страница содержит примечания к выпуску для Aspose.Cells for Java 18.1.

{{% /alert %}} 

|**Ключ**|**Резюме**|**Категория**|
|:- |:- |:- |
|CELLSJAVA-42493|Предоставьте возможность решить, следует ли экспортировать свойства книги (идентификатор родительской проблемы: CELLSJAVA-42471).|Новая особенность|
|CELLSJAVA-42491|Предоставьте возможность решить, следует ли экспортировать свойства документа (идентификатор родительской проблемы: CELLSJAVA-42471)|Новая особенность|
|CELLSJAVA-42498|Создайте PdfBookmarkEntry для листа диаграммы|Новая особенность|
|CELLSJAVA-42464|Требуется исправление для всех элементов управления ActiveX (идентификатор родительской проблемы: CELLSJAVA-42442)|Улучшение|
|CELLSJAVA-42490|Исключить неиспользуемые стили при экспорте файла Excel в HTML (идентификатор родительской проблемы: CELLSJAVA-42471)|Улучшение|
|CELLSJAVA-42473|Части изображений обрезаны или отсутствуют, и они не соответствуют оригинальным исходным изображениям.|Ошибка|
|CELLSJAVA-42469|Изображение выступает из фигуры на выходе PDF|Ошибка|
|CELLSJAVA-42461|Неправильная форма элемента в выводе HTML|Ошибка|
|CELLSJAVA-42495|Excel в Html — перенос текста игнорируется|Ошибка|
|CELLSJAVA-42489|XLSB файл повреждается после открытия и сохранения|Ошибка|
|CELLSJAVA-42487|HTML несоответствие вывода - проблема с пробелами|Ошибка|
|CELLSJAVA-42471|Неактуальные данные включены при сохранении в HTML|Ошибка|
|CELLSJAVA-42467|XLSB поврежден после повторного сохранения|Ошибка|
|CELLSJAVA-42488|15-значные числа не соответствуют тому, что есть в MS Excel|Ошибка|
|CELLSJAVA-42499|Различия в полях и макетах при сравнении вывода PDF (по Aspose.Cells) с сгенерированным MS Excel PDF|Ошибка|
|CELLSJAVA-42486|Функция не работает в Java - ResultSet|Ошибка|
|CELLSJAVA-42500|NullPointerException возникает при загрузке файла MS Excel|Исключение|
## **Public API и обратно несовместимые изменения**
Ниже приведен список любых изменений, внесенных в общедоступный номер API, таких как добавленные, переименованные, удаленные или устаревшие члены, а также любые несовместимые с предыдущими изменениями, внесенные в номер Aspose.Cells for Java. Если у вас есть сомнения по поводу каких-либо перечисленных изменений, сообщите об этом на форум поддержки Aspose.Cells.
### **Добавляет свойство LoadOptions.ParsingPivotCachedRecords.**
Указывает, выполняется ли синтаксический анализ кэшированных записей сводной таблицы при загрузке файла. Значение по умолчанию — false. Применяется только к форматам файлов Excel Xlsx, Xltx, Xltm, Xlsm и Xlsb.
### **Добавляет свойство HtmlSaveOptions.ExcludeUnusedStyles.**
Указывает, исключаются ли неиспользуемые стили. Значение по умолчанию — false. Если вы хотите импортировать файл HTML или Mht в Excel, оставьте значение по умолчанию.
### **Добавляет свойство HtmlSaveOptions.ExportDocumentProperties.**
Указывает, экспортируются ли свойства документа. Значение по умолчанию — true. Если вы хотите импортировать файл HTML или Mht в Excel, оставьте значение по умолчанию.
### **Добавляет свойство HtmlSaveOptions.ExportWorksheetProperties.**
Указывает, экспортируются ли свойства рабочего листа. Значение по умолчанию — true. Если вы хотите импортировать файл HTML или Mht в Excel, оставьте значение по умолчанию.
### **Добавляет свойство HtmlSaveOptions.ExportWorkbookProperties.**
Указывает, экспортируются ли свойства книги. Значение по умолчанию — true. Если вы хотите импортировать файл HTML или Mht в Excel, оставьте значение по умолчанию.
### **Добавляет метод PivotTable.GetChildren()**
Получает дочерние сводные таблицы, которые используют данные этой сводной таблицы в качестве источника данных.
