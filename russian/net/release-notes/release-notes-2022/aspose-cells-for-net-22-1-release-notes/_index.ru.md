﻿---
title: Aspose.Cells for .NET 22.1 Примечания к выпуску
type: docs
weight: 12
url: /ru/net/aspose-cells-for-net-22-1-release-notes/
---
{{% alert color="primary" %}}

 Эта страница содержит примечания к выпуску для[Aspose.Cells for .NET 22.1](https://www.nuget.org/packages/Aspose.Cells/22.1.0).

{{% /alert %}}

|**Ключ**|**Резюме**|**Категория**|
|:- |:- |:- |
|CELLSNET-50082|Поддержка возврата исходных индексов отсортированных строк/столбцов для функции sort().|Новая особенность|
|CELLSNET-50088|Поддержка установки имени задания на печать с помощью PrinterSettings во время рендеринга на принтер.|Новая особенность|
|CELLSNET-50060|Определите, является ли текстовый файл CSV или TSV.|Новая особенность|
|CELLSNET-49939|Ингорировать скрытые строки и столбцы при получении Cells.MaxDisplayRange|Улучшение|
|CELLSNET-50054|Неверный результат для вычисления функции ЧАСТОТА в формуле массива|Улучшение|
|CELLSNET-50072|Неподдерживаемая функция: КУБМНОЖ|Улучшение|
|CELLSNET-50017|Как добавить пузырь рядом с заголовком диаграммы и текстом оси диаграммы|Улучшение|
|CELLSNET-50038| Различное поведение при сворачивании и развертывании многоуровневых групп|Улучшение|
|CELLSNET-50041| BMP файлы изображений не отображаются в верхнем/нижнем колонтитуле|Улучшение|
|CELLSNET-50108|XLS в PDF: Преобразование останавливается из-за нехватки памяти|Спектакль|
|CELLSNET-50128|Междустрочный интервал становится уже - преобразование Excel в PDF|Ошибка|
|CELLSNET-50086|Cell цвета исчезают после преобразования в PDF|Ошибка|
|CELLSNET-49996|Форматированные текстовые значения ячеек могут быть потеряны в режиме MemoryPreference.|Ошибка|
|CELLSNET-50042| Название ячеек меняется во время записи|Ошибка|
|CELLSNET-50055|Свойство имени локального диапазона FullText не экранируется, если на родительском листе есть апостроф|Ошибка|
|CELLSNET-50154|GridWeb не удается загрузить/сохранить из кеша файл .csv|Ошибка|
|CELLSNET-50063|При печати файла Excel отображаются две страницы вместо одной страницы|Ошибка|
|CELLSNET-50094|Содержимое листа не отображается должным образом в преобразовании Excel в PDF|Ошибка|
|CELLSNET-50129|Позиция печати повышается по мере перехода к странице - преобразование Excel в PDF|Ошибка|
|CELLSNET-50131|Отсутствуют символы - преобразование Excel в PDF|Ошибка|
|CELLSNET-49578| Неверное максимальное/минимальное значение, рассчитанное по графикам Aspose.Cells|Ошибка|
|CELLSNET-50087|Выходная диаграмма отображается неправильно после изменения типа серии|Ошибка|
|CELLSNET-50197|Легенду в диаграмме водопада нельзя удалить или скрыть.|Ошибка|
|CELLSNET-50065|Различное поведение в отношении свертывания и развертывания многоуровневых групп строк|Ошибка|
|CELLSNET-50137|От XLSX до HTML необъявленная переменная «узел» в скрипте|Ошибка|
|CELLSNET-50157|AutoFitMergedCellsType.EachLine не работает для столбцов с автоматическим подбором|Ошибка|
|CELLSNET-50165|Шрифт фонетического справочника изменен после сохранения файла|Ошибка|
|CELLSNET-50208|Некоторый текст теряется при сохранении в виде HTML|Ошибка|
|CELLSNET-50095|Исключение при открытии файла XSLB|Исключение|
|CELLSNET-50096| StackOverflowException при удалении пустых столбцов|Исключение|
|CELLSNET-50071|Преобразование в исключение HTML "Неподдерживаемая функция: КУБМНОЖ"|Исключение|
|CELLSNET-50097|Исключение при открытии файла XSLX через Aspose.Cells|Исключение|
|CELLSNET-50133|NullReferenceException при сравнении FillFormat|Исключение|
|CELLSNET-50138|Исключение при открытии файла XLSB|Исключение|
|CELLSNET-50016|Диаграмма до EMF неправильные значения оси|Регрессия|
|


## **Public API и обратно несовместимые изменения**

Ниже приведен список любых изменений, внесенных в общедоступный номер API, таких как добавленные, переименованные, удаленные или устаревшие члены, а также любые несовместимые с предыдущими изменениями, внесенные в номер Aspose.Cells for .NET. Если у вас есть сомнения по поводу каких-либо перечисленных изменений, сообщите об этом на форум поддержки Aspose.Cells.

### **Изменяет поведение при удалении внешних ссылок из книги.**

В старых версиях мы не удаляем внешнюю ссылку, URL-адрес которой содержит «AddIns». Такое поведение разработано для особых требований некоторых пользователей. Недостаток такого решения очевиден: пользователи могут указать любое допустимое имя файла или путь для внешних ссылок, и на самом деле большинство из них не хотят, чтобы эти внешние ссылки обрабатывались по-разному. Начиная с этой версии, мы больше не фильтруем эти внешние ссылки. Если у пользователей есть особые требования к некоторым внешним ссылкам, они могут проверять все элементы в коллекции ExternalLinkCollection один за другим и удалять только те, которые они хотят удалить (методом ExternalLinkCollection.RemoveAt(int)).

### **Изменяет поведение Cell.Type для недопустимого значения даты и времени.**

В старых версиях, если одна ячейка запрашивается для форматирования даты и времени, Cell.Type возвращает CellValueType.IsDateTime независимо от того, является ли числовое значение этой ячейки действительным для даты и времени или нет. Это может вызвать исключение, если пользователи зависят только от Cell.Type и пытаются вызвать Cell.DateTimeValue. Начиная с этой версии, мы возвращаем CellValueType.IsNumeric для таких ячеек, чтобы пользователь мог получить правильное значение ячейки API.

### **Изменяет поведение Cells.MaxDisplayRange.**

В старых версиях значение диапазона этого свойства охватывает все ячейки, экземпляры которых были созданы в коллекции ячеек. В этой версии мы исключаем невидимые строки/столбцы из краев отображаемого диапазона, если в этих строках/столбцах есть только экземпляры ячеек.

### **Изменяет методы DataSorter.Sort() для возврата исходных индексов отсортированных строк/столбцов.**

В старых версиях методы DataSorter.Sort() ничего не возвращают. В этой версии мы возвращаем исходные индексы строк/столбцов, соответствующие отсортированному диапазону. Это дает пользователю возможность выполнять расширенную проверку и операции по сортировке.

### **Добавляет свойство TxtLoadOptions.ExtendToNextSheet.**

Поддерживает импорт данных CSV/TSV на несколько рабочих листов, если количество строк или столбцов данных превышает предел MS Excel.

### **Добавляет метод ExternalLinkCollection.Clear().**

Удаляет все внешние ссылки из книги.

### **Добавляет метод ExternalLinkCollection.Clear(bool updateReferencesAsLocal).**

При удалении всех внешних ссылок из книги пользователь может определить, что делать с формулами, в которых есть ссылки на эти внешние ссылки. Если «updateReferencesAsLocal» имеет значение true, то все пользовательские функции во внешних ссылках будут перемещены в саму текущую книгу. Например, формула одной ячейки — «='externalsource.xlam'!customfunction()», после удаления внешней ссылки «externalsource.xlam» формула этой ячейки станет «=customfunction()».

### **Добавляет метод ExternalLinkCollection.RemoveAt(int).**

Удаляет одну указанную внешнюю ссылку из книги.

### **Добавляет метод ExternalLinkCollection.RemoveAt(int, bool updateReferencesAsLocal).**

Подобно методу ExternalLinkCollection.Clear(bool updateReferencesAsLocal), пользователь может определить, как поступить с формулами, ссылающимися на указанную внешнюю ссылку, при удалении ее из книги.

### **Добавляет метод ExternalLinkCollection.GetEnumerator().**

Предоставляет перечислитель для перебора всех внешних ссылок в книге.

### **Устарел метод Workbook.RemoveExternalLinks().**

Вместо этого используйте метод ExternalLinkCollection.Clear().

### **Устарел метод Workbook.HasExernalLinks().**

Используйте ExternalLinkCollection.Count, чтобы проверить наличие внешних ссылок в книге.

### **Удаляет устаревший класс StyleCollection.**

Пожалуйста, используйте Workbook.CreateStyle() и Workbook.GetNamedStyle(string) для управления стилями.

### **Добавляет конструктор PptxSaveOptions(bool saveAsImage).**

Представляет варианты сохранения файла .pptx. Если True, книга будет преобразована в несколько изображений файла .pptx. Если False, рабочая книга будет преобразована в несколько таблиц файла .pptx.

### **Добавляет метод SheetRender.ToPrinter(SettingsprinterSettings, string jobName).**

Отправьте рабочий лист на принтер с настройками принтера и именем задания принтера.

### **Добавляет метод WorkbookRender.ToPrinter(SettingsprinterSettings, string jobName).**

Отправьте книгу на принтер с настройками принтера и именем задания на принтер.

### **Добавляет класс ChartGlobalizationSettings.**

 Представляет параметры глобализации для диаграммы.

### **Добавляет свойство DataLabels.IsNeverOverlap.**

Указывает, не перекрываются ли отображаемые метки данных. (Для круговой диаграммы)

### **Добавляет класс TickLabelItem.**

Включите информацию о элементе Ticklabel.

### **Добавляет свойство TickLabelItem.Height.**

Получает высоту элемента Ticklabel по отношению к высоте диаграммы.

### **Добавляет свойство TickLabelItem.Width.**

Получает ширину элемента Ticklabel по отношению к ширине диаграммы.

### **Добавляет свойство TickLabelItem.X.**

Получает X элемента Ticklabel по отношению к ширине диаграммы.

### **Добавляет свойство TickLabelItem.Y.**

Получает Y элемента Ticklabel в соотношении с высотой диаграммы.

### **Добавляет свойство TickLabels.TickLabelItems.**

Получает элементы TickLabel.

