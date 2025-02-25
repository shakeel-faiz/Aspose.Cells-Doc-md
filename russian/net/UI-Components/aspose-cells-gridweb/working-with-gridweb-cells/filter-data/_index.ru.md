﻿---
title: Данные фильтра
type: docs
weight: 80
url: /ru/net/filter-data/
---
{{% alert color="primary" %}} 

Aspose.Cells.GridWeb предоставляет функции автоматического фильтра и настраиваемого фильтра данных. Эти функции дают вам возможность выбирать только те элементы на листе, которые вы хотите отобразить в списке. Кроме того, вы можете фильтровать элементы в списке в соответствии с заданными критериями. Фильтруйте текст, числа или даты с помощью функций фильтрации.

{{% /alert %}} 
## **Работа с фильтрами**
Используйте метод рабочего листа AddAutoFilter, чтобы включить автофильтр для рабочего листа. Этот метод принимает индексы строки, начала и конца столбца.

Чтобы включить настраиваемый фильтр, используйте метод рабочего листа AddCustomFilter, который принимает индекс строки, к которой необходимо применить фильтр, и настраиваемые критерии фильтрации.

В приведенном ниже примере реализованы как автоматические, так и пользовательские фильтры данных. В этом примере функция автоматической фильтрации включена, и поиск отфильтрованных строк осуществляется на основе некоторых критериев.

**Вход: список данных на первом листе.** 

![дело:изображение_альтернативный_текст](filter-data_1.jpg)

**Вывод: включить функцию автофильтра** 

![дело:изображение_альтернативный_текст](filter-data_2.jpg)
### **Автофильтр**
{{< gist "aspose-cells-gists" "7c644a93d33d24299a618c1dda1a2385" "Examples.GridWeb-CSharp-Cells-SetAutoFilter.aspx-SetAutoFilter.cs" >}}
### **Пользовательский фильтр данных**
**Пользовательские отфильтрованные данные на основе критериев** 

![дело:изображение_альтернативный_текст](filter-data_3.jpg)



{{< gist "aspose-cells-gists" "7c644a93d33d24299a618c1dda1a2385" "Examples.GridWeb-CSharp-Cells-SetCustomFilter.aspx-SetCustomFilter.cs" >}}
