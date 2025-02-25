﻿---
title: Добавить Cell Формулы
type: docs
weight: 30
url: /ru/net/add-cell-formulas/
---
{{% alert color="primary" %}} 

Самая ценная функция, предлагаемая Aspose.Cells.GridWeb, — это поддержка формул или функций. Aspose.Cells.GridWeb имеет собственный механизм формул, который вычисляет формулы на листах. Aspose.Cells.GridWeb поддерживает как встроенные, так и определяемые пользователем функции или формулы. В этом разделе подробно обсуждается добавление формул в ячейки с помощью Aspose.Cells.GridWeb API.

{{% /alert %}} 
## **Добавление формул в Cells**
### **Как добавить и рассчитать формулу?**
 Можно добавлять, получать доступ и изменять формулы в ячейках, используя свойство Формула ячейки. Aspose.Cells.GridWeb поддерживает пользовательские формулы, начиная от простых и заканчивая сложными. Однако большое количество встроенных функций или формул (аналогичных Microsoft Excel) также поставляется с Aspose.Cells.GridWeb. Полный список встроенных функций см.[список поддерживаемых функций.](/cells/ru/net/list-of-supported-functions/)

{{% alert color="primary" %}} 

Синтаксис формулы должен быть совместим с синтаксисом Excel Microsoft. Например, все формулы должны начинаться со знака равенства (=).

Чтобы добавить формулу динамически, Aspose.Cells.GridWeb распознает ее как формулу, даже если вы не используете знак **=**, но если конечные пользователи работают в графическом интерфейсе, он должен использовать знак "=".

{{% /alert %}} 

{{< gist "aspose-cells-gists" "7c644a93d33d24299a618c1dda1a2385" "Examples.GridWeb-CSharp-Cells-AddFormulas.aspx-AddFormulas.cs" >}}



**Формула добавлена в ячейку B3, но не рассчитана GridWeb** 

![дело:изображение_альтернативный_текст](add-cell-formulas_1.png)

На приведенном выше снимке экрана видно, что формула добавлена в ячейку B3, но еще не рассчитана. Чтобы вычислить все формулы, вызовите метод CalculateFormula элемента управления GridWeb GridWorksheetCollection после добавления формул на листы, как показано ниже.



{{< gist "aspose-cells-gists" "7c644a93d33d24299a618c1dda1a2385" "Examples.GridWeb-CSharp-Cells-AddFormulas.aspx-CalculateFormulas.cs" >}}

{{% alert color="primary" %}} 

 Пользователи также могут вычислять формулы, щелкая**Представлять на рассмотрение**.

**Нажатие кнопки «Отправить» в GridWeb** 

![дело:изображение_альтернативный_текст](add-cell-formulas_2.png)

**ВАЖНЫЙ** : если пользователь щелкает**Сохранять** или же**Отменить** кнопки или вкладки листа, все формулы рассчитываются GridWeb автоматически.

**Результат формулы после расчета** 

![дело:изображение_альтернативный_текст](add-cell-formulas_3.png)

{{% /alert %}} 
### **Ссылка Cells из других рабочих листов**
Используя Aspose.Cells.GridWeb, можно ссылаться на значения, хранящиеся на разных листах, в их формулах, создавая сложные формулы.

Синтаксис для ссылки на значение ячейки из другого листа: SheetName!CellName.



{{< gist "aspose-cells-gists" "7c644a93d33d24299a618c1dda1a2385" "Examples.GridWeb-CSharp-Cells-AddFormulas.aspx-AddComplexFormulas.cs" >}}
