﻿---
title: Aspose.Cells for .NET 20.4 Примечания к выпуску
type: docs
weight: 40
url: /ru/net/aspose-cells-for-net-20-4-release-notes/
---
{{% alert color="primary" %}} 

 Эта страница содержит примечания к выпуску для[Aspose.Cells for .NET 20.4](https://www.nuget.org/packages/Aspose.Cells/20.4.0).

{{% /alert %}} 

|**Ключ**|**Резюме**|**Категория**|
|:- |:- |:- |
|CELLSNET-47276|От XLSX до CSV, запятые требуются для пустых ячеек, также как в MS Excel|Новая особенность|
|CELLSNET-47054|Поддержка объединения нескольких ячеек в виде диапазона|Новая особенность|
|CELLSNET-47091|Возможность обновления исходного поля PowerQueryFormulaItems|Новая особенность|
|CELLSNET-47273|Установите латинский текстовый шрифт и азиатский текстовый шрифт для оси категории диаграммы|Улучшение|
|CELLSNET-47217|Поддержка панели данных, цветовой шкалы и условного форматирования набора иконок ODS.|Улучшение|
|CELLSNET-47201|Откройте защищенный паролем файл с помощью Aspose.Cells.GridDesktop.|Улучшение|
|CELLSNET-47254|Поддержка ввода новой строки, как в MS-EXCEL в строке формул|Улучшение|
|CELLSNET-47224|Улучшите производительность обновления сводных данных.|Спектакль|
|CELLSNET-47243|Зависание GetDisplayStyle для рабочего листа со строками 65536|Спектакль|
|CELLSNET-47289|CalculateFormula() никогда не возвращает значение|Спектакль|
|CELLSNET-47263|Зависание при попытке открыть документ ODP в конструкторе рабочей книги|Спектакль|
|CELLSNET-42556|Сортировка PivotField не работает|Ошибка|
|CELLSNET-47046|Неоткрытые разделители кавычек в атрибутах IMG HTML в сгенерированной разметке HTML|Ошибка|
|CELLSNET-47208|Сводная таблица не поддерживает формат последней версии|Ошибка|
|CELLSNET-47219|Неверная формула в столбце таблицы после вставки строки и ее обновления|Ошибка|
|CELLSNET-47261|Рендеринг Excel в HTML - неправильный размер шрифта в экспортированной таблице|Ошибка|
|CELLSNET-47279|Текст первого столбца во всех строках не индексируется при экспорте файла в HTML.|Ошибка|
|CELLSNET-47163|Проблема со вставкой столбца и ссылки на обновление|Ошибка|
|CELLSNET-47244|Формулы (ОКРУГЛЫЙ, МИН) рассчитаны неправильно|Ошибка|
|CELLSNET-47250|Удаление дубликатов работает для первого столбца только при указании параметра columnOffsets|Ошибка|
|CELLSNET-47267|Формулы не рассчитываются в файле шаблона|Ошибка|
|CELLSNET-47268|Несоответствие TrimLeadingBlankRowAndColumn|Ошибка|
|CELLSNET-47269|Преобразование XLSX в CSV - отсутствует запятая в выводе|Ошибка|
|CELLSNET-47200|Проблема с перекрытием кнопок навигации при установке скрытого листа в качестве активного листа|Ошибка|
|CELLSNET-47274|Фоновое изображение не задано в GridWeb|Ошибка|
|CELLSNET-47179|Подпись VBA с библиотекой Bouncy Castle|Ошибка|
|CELLSNET-47258|Проблема с изображениями штрих-кода в рендеринге Sheet to TIFF|Ошибка|
|CELLSNET-47216|PowerQueries исчезли после замены исходного кода|Ошибка|
|CELLSNET-47241|ODS файл ломается при установке стиля шрифта и сохранении|Ошибка|
|CELLSNET-47252|Числовой интеллектуальный маркер, вставляющий значение ячейки в виде текста|Ошибка|
|CELLSNET-47262|Проблема со 100% Stacked Bar, а также с основным и второстепенным блоками|Ошибка|
|CELLSNET-47271|Сохранение XLSX со встроенным Visio приводит к повреждению файла.|Ошибка|
|CELLSNET-47282|Aspose.Cells 20.3: проблема преобразования XLSB в XLS|Ошибка|
|CELLSNET-47291|Неправильный символ маркера, прочитанный из файла Excel|Ошибка|
|CELLSNET-47096|Проблема с панелью формул GridDesktop с SplitterPane|Ошибка|
|CELLSNET-47247|Исключение возникает при вызове Cell.R1C1Formula.|Исключение|
|CELLSNET-47235|NullPointerException при обновлении PivotData|Исключение|
|CELLSNET-47246|Исключение «Не удается получить доступ к закрытому потоку» при сохранении файла Excel в PDF|Исключение|
|CELLSNET-47086|Исключение выдается при рендеринге диаграммы|Исключение|
|CELLSNET-47242|FormatException при загрузке файла|Исключение|
|CELLSNET-47266|Исключение «Индекс аргумента выходит за пределы диапазона массива» при загрузке всех вложенных файлов|Исключение|
### **Public API и обратно несовместимые изменения**
Ниже приведен список любых изменений, внесенных в общедоступный номер API, таких как добавленные, переименованные, удаленные или устаревшие члены, а также любые несовместимые с предыдущими изменениями, внесенные в номер Aspose.Cells for .NET. Если у вас есть сомнения по поводу каких-либо перечисленных изменений, сообщите об этом на форум поддержки Aspose.Cells.
#### **Добавляет свойство ChartTextFrame.DirectionType.**
Получает и задает направление текста на диаграмме.
#### **Добавляет ChartTextFrame.ReadingOrder и устаревает свойство ChartTextFrame.TextDirection.**
Вместо этого используйте свойство ChartTextFrame.ReadingOrder.
#### **Добавляет классы для расширенной функции Revisions.**
Получает информацию о редакции.
#### **Изменяет значение по умолчанию свойства TxtSaveOptions.TrimLeadingBlankRowAndColumn.**
Чтобы поведение по умолчанию при сохранении CSV было одинаковым с MS Excel, мы изменили значение по умолчанию и поведение этого свойства. Для старых версий его значение по умолчанию было "**ЛОЖЬ**". С версии 20.4 его значение по умолчанию становится "**истинный**".
#### **Изменяет поведение при обнаружении пустых строк/столбцов для сохранения CSV.**
Для старых версий мы считали пустыми те строки/столбцы, которые не содержат данных, но имеют пользовательские настройки (видимость, форматирование и т. д.). Начиная с версии 20.4 мы больше не считаем их пустыми, новое поведение такое же, как и в MS Excel.
#### **Добавляет свойство TxtSaveOptions.ExportArea.**
Задает диапазон данных ячеек для экспорта. Пользователи могут использовать эту опцию, чтобы получить тот же результат со старыми версиями для измененного поведения TxtSaveOptions.TrimLeadingBlankRowAndColumn и пустых строк/столбцов.
#### **Добавляет класс UnionRange.**
Представляет диапазон объединения.
#### **Удаляет устаревшее свойство DrawObject.Image.**
Вместо этого используйте свойство DrawObject.ImageBytes.
#### **Добавляет свойство Bullet.FontName**
Получает и задает имя шрифта маркера.
#### **Добавляет метод WorksheetCollection.CreateUnionRange().**
Создает диапазон объединения.
#### **Удаляет устаревшее перечисление SaveType.**
Он не используется.
#### **Удаляет устаревшие свойства OleObject.ImageFormat и Picture.ImageFormat.**
Вместо этого используйте свойства OleObject.ImageType и Picture.ImageType.
