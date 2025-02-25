﻿---
title: Aspose.Cells for .NET 19.5 Примечания к выпуску
type: docs
weight: 80
url: /ru/net/aspose-cells-for-net-19-5-release-notes/
---
{{% alert color="primary" %}} 

 Эта страница содержит примечания к выпуску для[Aspose.Cells for .NET 19.5](https://www.nuget.org/packages/Aspose.Cells/19.5.0).

{{% /alert %}} 

|**Ключ**|**Резюме**|**Категория**|
|:- |:- |:- |
|CELLSNET-46703|Новый японский календарь отображается неправильно|Новая особенность|
|CELLSNET-46693|Фон поддержки ODS|Новая особенность|
|CELLSNET-46695|Установить фон файла ODS|Новая особенность|
|CELLSNET-46706|Неверный порядок номеров при преобразовании арабского шрифта в PDF.|Улучшение|
|CELLSNET-46692|Контролируйте все внешние данные с помощью интерфейса IStreamProvider|Улучшение|
|CELLSNET-46711|ImportCustomObjects в объединенную область прерывает слияние|Улучшение|
|CELLSNET-46713|Метод «String.StartsWith("\0")» всегда возвращает значение true в macOS.|Улучшение|
|CELLSNET-46719|Исключение при установке строки HTML с использованием цветовой модели RGBA|Улучшение|
|CELLSNET-46701|Обработка пузырьковых диаграмм зависает в версии 19.4|Ошибка|
|CELLSNET-46682|Опция «Скрыть элементы без данных» в настройках слайсера не отмечена.|Ошибка|
|CELLSNET-46707|PivotTable.GetChildren() возвращает неправильное количество зависимостей|Ошибка|
|CELLSNET-46689|Сохранение книги как PDF отличается от собственного вывода Excel|Ошибка|
|CELLSNET-46704|Результат преобразования Excel в PDF с использованием Aspose.Cells отличается от Excel.|Ошибка|
|CELLSNET-46720|Структура страницы повреждена на последней странице преобразования Excel в PDF|Ошибка|
|CELLSNET-46727|Неправильная нумерация страниц при сохранении книги как PDF|Ошибка|
|CELLSNET-46700|Метки данных круговой диаграммы перекрываются друг с другом|Ошибка|
|CELLSNET-46696|Преобразование XLS с графической диаграммой Microsoft в XLSX и XLSM приводит к ошибке нечитаемого содержимого.|Ошибка|
|CELLSNET-46697|Преобразование XLSM с объектом OLE в XLS вызывает ошибку|Ошибка|
|CELLSNET-46712|Преобразование XLS с графической диаграммой Microsoft в XLSX и XLSM приводит к ошибке нечитаемого содержимого.|Ошибка|
|CELLSNET-46715|Cells.InsertCutCells() Проблема|Ошибка|
|CELLSNET-46725|"_х000а_" добавлена строка в описание альтернативного текста многолинейного графика|Ошибка|
|CELLSNET-46683|Исключение при рендеринге файла Excel на PDF|Исключение|
|CELLSNET-46690|Возникает исключение при загрузке книги Excel из Shape.ForeignData (Diagram)|Исключение|
|CELLSNET-46728|Исключение при сохранении потока как книги|Исключение|
### **Public API и обратно несовместимые изменения**
Ниже приведен список любых изменений, внесенных в общедоступный номер API, таких как добавленные, переименованные, удаленные или устаревшие члены, а также любые несовместимые с предыдущими изменениями, внесенные в номер Aspose.Cells for .NET. Если у вас есть сомнения по поводу каких-либо перечисленных изменений, сообщите об этом на форум поддержки Aspose.Cells.
#### **Добавляет конструктор StreamProviderOptions**
Новые параметры StreamProvider.
#### **Добавляет перечисление FileFormatType.GraphChart**
Представляет файл встроенной графической диаграммы.
#### **Добавляет свойства ImportTableOptions.CheckMergedCells.**
Указывает, проверяются ли объединенные ячейки при импорте данных.
#### **Добавляет ODSCellFieldCollection, классы ODSCellField и перечисление ODSCellFieldType.**
Представляет поле ячейки ODS.
#### **Добавляет свойства Cells.ODSCellFields.**
Получает список полей ячеек ODS.
#### **Добавляет класс ODSPageBackground и свойство PageSetup.ODSPageBackground.**
Представляет фон ODS.
