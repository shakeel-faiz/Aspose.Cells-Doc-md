﻿---
title: Фильтрация данных
type: docs
weight: 85
url: /ru/net/data-filtering/
---
{{% alert color="primary" %}}

Microsoft Excel предоставляет несколько полезных функций для автоматической фильтрации данных рабочего листа. Aspose.Cells полностью поддерживает функции автофильтра Microsoft Excel. В этой статье объясняется, как использовать функции в Microsoft Excel и как кодировать их с помощью Aspose.Cells.

{{% /alert %}}

## **Данные автофильтра**

Автофильтрация — это самый быстрый способ выбрать на листе только те элементы, которые вы хотите отобразить в списке. Функция автофильтра позволяет пользователям фильтровать элементы в списке в соответствии с заданными критериями. Фильтровать по тексту, числам или датам.

### **Автофильтр в Microsoft Excel**

Чтобы активировать функцию автофильтра в Microsoft Excel:

1. Щелкните строку заголовка на листе.
1.  От**Данные** меню, выберите**Фильтр** а потом**Автофильтр**.

Когда вы применяете автофильтр к рабочему листу, переключатели фильтров (черные стрелки) появляются справа от заголовков столбцов.

1. Щелкните стрелку фильтра, чтобы просмотреть список параметров фильтра.

Некоторые параметры автофильтра:

|**Параметры**|**Описание**|
|:- |:- |
|Все|Показать все элементы в списке один раз.|
|Обычай|Настройте критерии фильтра, такие как содержит/не содержит|
|Фильтр по цвету|Фильтры на основе заполненного цвета|
|Фильтры даты|Фильтрует строки по разным критериям по дате|
|Числовые фильтры|Различные типы фильтров по числам, такие как сравнение, средние значения, 10 лучших и т. д.|
|Текстовые фильтры|Различные фильтры, такие как начинается с, заканчивается, содержит и т. д.|
|Пустые/не пустые|Эти фильтры могут быть реализованы с помощью пустого текстового фильтра.|

Пользователи вручную фильтруют данные своих рабочих листов в Microsoft Excel, используя эти параметры.

### **Автофильтр с Aspose.Cells**

Aspose.Cells предоставляет класс Workbook, представляющий файл Excel. Класс Workbook содержит коллекцию Worksheets, которая обеспечивает доступ к каждому рабочему листу в файле Excel.

Рабочий лист представлен классом Worksheet. Класс Worksheet предоставляет широкий набор свойств и методов для управления рабочими листами. Чтобы создать автофильтр, используйте свойство AutoFilter класса Worksheet. Свойство AutoFilter — это объект класса AutoFilter, который предоставляет свойство Range для указания диапазона ячеек, составляющих строку заголовка. Автофильтр применяется к диапазону ячеек, который является строкой заголовка.

На каждом листе можно указать только один диапазон фильтров. Это ограничено Microsoft Excel. Для пользовательской фильтрации данных используйте метод AutoFilter.Custom.

В приведенном ниже примере мы создали тот же автофильтр, используя Aspose.Cells, что и мы, используя Microsoft Excel в предыдущем разделе.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-Processing-FilteringAndValidation-AutofilterData-1.cs" >}}

#### **Различные типы фильтров**

Aspose.Cells предоставляет несколько вариантов для применения различных типов фильтров, таких как цветной фильтр, фильтр даты, числовой фильтр, текстовый фильтр, пустые фильтры и пустые фильтры.

##### **Цвет заливки**

Aspose.Cells предоставляет функцию AddFillColorFilter для фильтрации данных на основе свойства цвета заливки ячеек. В приведенном ниже примере файл шаблона с разными цветами заливки в первом столбце листа используется для проверки функции фильтрации цветов. Образцы файлов можно скачать по следующим ссылкам.

1. [ColoredCells.xlsx](72417315.xlsx)
1. [FilteredColoredCells.xlsx](72417316.xlsx)

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-Processing-Filtering-AutofilterColor-1.cs" >}}

##### **Датировать**

Различные типы фильтров дат могут быть реализованы, например, фильтрация всех строк, имеющих даты в январе 2018 года. Следующий пример кода демонстрирует этот фильтр с использованием функции AddDateFilter. Примеры файлов приведены ниже.

1. [Дата.xlsx](72417317.xlsx)
1. [Фильтредате.xlsx](72417318.xlsx)

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-Processing-Filtering-AutofilterDate-1.cs" >}}

##### **Динамическая дата**

Иногда требуются динамические фильтры на основе даты, например, все ячейки, имеющие даты в январе, независимо от года. В этом случае используется функция DynamicFilter, как показано в следующем примере кода. Примеры файлов приведены ниже.

1. [Дата.xlsx](72417317.xlsx)
1. [FilteredDynamicDate.xlsx](72417319.xlsx)

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-Processing-Filtering-AutofilterDynamicFilter-1.cs" >}}

##### **Число**

Пользовательские фильтры можно применять с помощью Aspose.Cells, например, выбирать ячейки с номером в заданном диапазоне. В следующем примере показано использование функции Custom() для фильтрации чисел. Примеры файлов приведены ниже.

1. [Номер.xlsx](72417320.xlsx)
1. [Фильтредномер.xlsx](72417321.xlsx)

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-Processing-Filtering-AutofilterNumber-1.cs" >}}

##### **Текст**

Если столбец содержит текст и должны быть выбраны ячейки, содержащие определенный текст, можно использовать функцию Filter(). В следующем примере файл шаблона содержит список стран, и необходимо выбрать строку, содержащую название конкретной страны. Следующий код демонстрирует фильтрацию текста. Примеры файлов приведены ниже.

1. [Текст.xlsx](72417322.xlsx)
1. [Фильтрованный текст.xlsx](72417323.xlsx)

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-Processing-Filtering-AutofilterText-1.cs" >}}

##### **Бланки**

Если столбец содержит текст, так что несколько ячеек пусты, и фильтр требуется для выбора только тех строк, в которых присутствуют пустые ячейки, можно использовать функцию MatchBlanks(), как показано ниже. Примеры файлов приведены ниже.

1. [Пустой.xlsx](72417324.xlsx)
1. [FilteredBlank.xlsx](72417325.xlsx)

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-Processing-Filtering-AutofilterBlank-1.cs" >}}

##### **Не пустые**

Когда необходимо отфильтровать ячейки с любым текстом, используйте функцию фильтра MatchNonBlanks, как показано ниже. Примеры файлов приведены ниже.

1. [Пустой.xlsx](72417324.xlsx)
1. [Фильтреднонбланк.xlsx](72417326.xlsx)

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-Processing-Filtering-AutofilterNonBlank-1.cs" >}}

##### **Пользовательский фильтр с содержит**

Excel предоставляет настраиваемые фильтры, такие как строки фильтра, которые содержат определенную строку. Эта функция доступна в версии Aspose.Cells и демонстрируется ниже путем фильтрации имен в образце файла. Примеры файлов приведены ниже.

1. [sourceSampleCountryNames.xlsx](sourseSampleCountryNames.xlsx)
1. [аутсаурсесамплекатринамес.xlsx](outSourseSampleCountryNames.xlsx).

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-Processing-Filtering-AutofilterCustom-Contains-1.cs" >}}

##### **Пользовательский фильтр с NotContains**

Excel предоставляет настраиваемые фильтры, такие как строки фильтра, которые не содержат какой-либо конкретной строки. Эта функция доступна в Aspose.Cells и демонстрируется ниже путем фильтрации имен в образце файла, приведенном ниже.

1. [sourceSampleCountryNames.xlsx](sourseSampleCountryNames.xlsx).

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-Processing-Filtering-AutofilterCustom-NotContains-1.cs" >}}

##### **Пользовательский фильтр с BeginsWith**

Excel предоставляет настраиваемые фильтры, такие как строки фильтра, которые начинаются с определенной строки. Эта функция доступна в Aspose.Cells и демонстрируется ниже путем фильтрации имен в образце файла, приведенном ниже.

1. [sourceSampleCountryNames.xlsx](sourseSampleCountryNames.xlsx).

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-Processing-FilteringAndValidation-AutofilterBeginsWith-1.cs" >}}

##### **Пользовательский фильтр с EndsWith**

Excel предоставляет настраиваемые фильтры, такие как строки фильтра, которые заканчиваются определенной строкой. Эта функция доступна в Aspose.Cells и демонстрируется ниже путем фильтрации имен в образце файла, приведенном ниже.

1. [sourceSampleCountryNames.xlsx](sourseSampleCountryNames.xlsx).

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-Processing-FilteringAndValidation-AutofilterEndsWith-1.cs" >}}

## **Предварительные темы**
- [Применить расширенный фильтр Microsoft Excel для отображения записей, отвечающих сложным критериям](/cells/ru/net/apply-advanced-filter-of-microsoft-excel-to-display-records-meeting-complex-criteria/)
- [Получить все индексы скрытых строк после обновления автофильтра](/cells/ru/net/get-all-hidden-rows-indices-after-refreshing-autofilter/)
