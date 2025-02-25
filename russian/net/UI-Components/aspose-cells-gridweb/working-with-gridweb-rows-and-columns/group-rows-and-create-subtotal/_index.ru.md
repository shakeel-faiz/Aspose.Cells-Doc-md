﻿---
title: Сгруппируйте строки и создайте промежуточный итог
type: docs
weight: 70
url: /ru/net/group-rows-and-create-subtotal/
---
{{% alert color="primary" %}} 

Aspose.Cells.GridWeb может создать схему для ваших данных. Это позволяет отображать и скрывать уровни детализации, щелкая символы схемы «+» и «-», чтобы отобразить только строки, содержащие сводки или заголовки для разделов на листе. Вы можете использовать символы, чтобы увидеть подробности под отдельной сводкой или заголовком.

При группировании строк важно выбирать только те строки сведений, которые составляют группу. Не включайте связанную сводную строку. Например, если строка 6 содержит итоги для данных в строках с 3 по 5, выберите только строки с 3 по 5, чтобы определить группу. Элемент управления Aspose.Cells.GridWeb отображает**Показать детали** (+) и**скрыть детали** Символы (-) рядом с заголовками строк, определяющие группы на листе.

Aspose.Cells.GridWeb также позволяет создавать промежуточные итоги на основе любого поля данных. Промежуточный итог не обязательно является суммой: это может быть среднее значение, количество, минимум, максимум или другое статистическое вычисление.

В этом разделе обсуждается группировка строк и создание промежуточных итогов с помощью Aspose.Cells.GridWeb API. Разработчики могут группировать строки с любым уровнем вложенности и легко создавать промежуточные итоги.

{{% /alert %}} 
## **Группировка строк**
Чтобы сгруппировать определенное количество строк:

1. Добавьте элемент управления Aspose.Cells.GridWeb в веб-форму.
1. Доступ к рабочему листу.
1. Выберите нужное количество ячеек в строках.
1. Сгруппируйте строки.

Когда строки сгруппированы, кнопка развертывания/свертывания отображается в верхней части сводной строки строк. Вы можете изменить настройку направления. Свойство WebWorksheet.IsSummaryRowBelow является логическим свойством. Установите для него значение false (по умолчанию), и итоговая строка будет над строками сведений. Установите для него значение true, и итоговая строка будет ниже строк с подробными сведениями. Нажмите кнопку «Развернуть/свернуть», чтобы развернуть или свернуть сгруппированные строки.

В следующем примере строки группируются со 2-й по 10-ю.

**Группировка строк** 

![дело:изображение_альтернативный_текст](group-rows-and-create-subtotal_1.png)



{{< highlight "java" >}}

 // Accessing the reference of the worksheet that is currently active

GridWorksheet sheet = GridWeb1.WorkSheets[GridWeb1.ActiveSheetIndex];

// Group the rows

sheet.Cells.GroupRows(1, 9);

{{< /highlight >}}
### **Вложение сгруппированных строк**
Вы можете создавать уровни организации при группировании набора строк. Вы можете группировать строки среди сгруппированных строк. В следующем примере показано вложение сгруппированных строк.

**Группировка строк** 

![дело:изображение_альтернативный_текст](group-rows-and-create-subtotal_2.png)



{{< highlight "java" >}}

 // Accessing the reference of the worksheet that is currently active

GridWorksheet sheet = GridWeb1.WorkSheets[GridWeb1.ActiveSheetIndex];

// Group the rows

sheet.Cells.GroupRows(1, 9);

// Create nested group of rows

sheet.Cells.GroupRows(4, 6);

{{< /highlight >}}
### **Внутренний процесс: как работает контроль?**
Каждая строка листа имеет номер схемы. По умолчанию номер контура равен нулю. Каждый раз, когда вы группируете строки, номер схемы увеличивается на 1. Номер структуры можно получить, вызвав метод GridWorksheet.Cells.GetRowOutlineLevel().
## **Разгруппировать строки**
Aspose.Cells.GridWeb позволяет разгруппировать сгруппированные строки.

Чтобы разгруппировать определенное количество строк:

1. Выберите несколько ячеек в строках листа, чтобы разгруппировать их.
1. Разгруппируйте строки.

В следующем примере строки со 2-й по 10-ю разгруппированы.



{{< highlight "java" >}}

 // Accessing the reference of the worksheet that is currently active

GridWorksheet sheet = GridWeb1.WorkSheets[GridWeb1.ActiveSheetIndex];

// Ungroup the rows

sheet.Cells.UngroupRows(1, 9); 

{{< /highlight >}}

{{% alert color="primary" %}} 

При вызове метода GridWorksheet.Cells.UngroupRows() номер структуры сгруппированных строк устанавливается равным нулю.

{{% /alert %}} 
## **Создание промежуточного итога**
Функция промежуточного итога элемента управления может группировать строки на листе с указанным столбцом и вычислять сводку по столбцам. Aspose.Cells.GridWeb может автоматически вычислять промежуточные итоговые значения для списка. Когда вы реализуете промежуточные итоги, элемент управления обрисовывает список, чтобы вы могли отображать и скрывать строки сведений для каждого промежуточного итога. Прежде чем добавлять промежуточные итоги, выполните сортировку по полю, в котором вы хотите получить промежуточные итоги. Для создания промежуточных итогов используйте любую версию перегруженного метода WebWorksheet.CreateSubtotal.



{{< highlight "java" >}}

 public void CreateSubtotal

(

           int columnNameRowIndex,

           int dataRows,

           int groupByColumnIndex,

           SubtotalFunction subtotalFunction,

           int[]subtotalColumnIndexList

);

{{< /highlight >}}
### **Список параметров**

|**Нет.**|**Имя параметра**|**Описание**|
|:- |:- |:- |
|1|столбецNameRowIndex|Индекс строки имени столбца row.|
|2|dataRows|Количество строк данных.|
|3|groupByColumnIndex|Индекс столбца для группируемого столбца.|
|4|промежуточный итогФункция|Перечисление типа функции промежуточного итога.|
|5|subtotalColumnIndexList|Индексы столбца для промежуточного итога.|
### **Список сводных функций**
Существует несколько типов сводных функций, поддерживаемых перечислением {[SubtotalFunction}}:

|**Нет.**|**Имя функции**|**Описание**|
|:- |:- |:- |
|1|СРЕДНИЙ|Вычисляет среднее значение.|
|2|СЧИТАТЬ|Подсчитывает числовые значения в ячейках.|
|3|СЧЁТ|Подсчитывает нечисловые данные в ячейках.|
|4|МАКСИМУМ|Вычисляет наибольшее значение.|
|5|МИН.|Вычисляет наименьшее значение.|
|6|ТОВАР|Вычисляет произведение значений.|
|7|СУММА|Вычисляет сумму значений.|
В следующем примере создаются промежуточные итоги, которые вычисляют нечисловые значения, сгруппированные по второму столбцу на листе.

**Итоги** 

![дело:изображение_альтернативный_текст](group-rows-and-create-subtotal_3.png)



{{< highlight "java" >}}

 sheet.CreateSubtotal(0, sheet.Cells.MaxRow, 1, SubtotalFunction.COUNTA, new int[]{ 1, 2, 3, 4, 5 });

{{< /highlight >}}
## **Удаление промежуточного итога**
Чтобы удалить промежуточный итог, используйте метод WebWorksheet.RemoveSubtotal. В следующем примере удаляются промежуточные итоги.



{{< highlight "java" >}}

 // Accessing the reference of the worksheet that is currently active

GridWorksheet sheet = GridWeb1.WorkSheets[GridWeb1.ActiveSheetIndex];

//Remove the subtotals

sheet.RemoveSubtotal();

{{< /highlight >}}
## **О функции ПРОМЕЖУТОЧНЫЙ ИТОГ**
Элемент управления GridWeb использует функцию формулы ПРОМЕЖУТОЧНЫЙ ИТОГ для вычисления значения промежуточного итога.

Синтаксис: ПРОМЕЖУТОЧНЫЕ.ИТОГИ(номер_функции, ссылка1, ссылка2, ...)

номер_функции — число, указывающее тип функции, используемой при расчете промежуточного итога.

|**1**|**СРЕДНИЙ**|
|:- |:- |
|2|СЧИТАТЬ|
|3|СЧЁТ|
|4|МАКСИМУМ|
|5|МИН.|
|6|ТОВАР|
|7|СУММА|
ref1, ref2 — области для подсчета. Если ref1, ref2, ... содержат другие функции промежуточных итогов, указанные ячейки игнорируются, чтобы избежать дублирования вычислений.
