﻿---
title: Добавить рабочие листы
type: docs
weight: 20
url: /ru/net/add-worksheets/
---
{{% alert color="primary" %}} 

Рабочие листы являются неотъемлемой частью Aspose.Cells.GridWeb. Все данные управляются и хранятся в виде рабочих листов. Aspose.Cells.GridWeb позволяет разработчикам добавлять один или несколько рабочих листов в элемент управления Aspose.Cells.GridWeb. В этом разделе показаны простые подходы к добавлению рабочих листов в Aspose.Cells.GridWeb.

{{% /alert %}} 
## **Добавление рабочего листа**
### **Без указания имени листа**
Самый простой способ добавить рабочий лист в Aspose.Cells.GridWeb — вызвать метод Add коллекции GridWorksheetCollection в элементе управления GridWeb. При этом создаются рабочие листы с именами по умолчанию (то есть Лист1, Лист2, Лист3 и т. д.) и добавляются в элемент управления GridWeb.

**Вывод: рабочий лист с именем по умолчанию добавлен в GridWeb.** 

![дело:изображение_альтернативный_текст](add-worksheets_1.png)



{{< gist "aspose-cells-gists" "7c644a93d33d24299a618c1dda1a2385" "Examples.GridWeb-CSharp-Worksheets-AddWorksheets.aspx-AddWorksheetWithoutName.cs" >}}

{{% alert color="primary" %}} 

 Метод Add возвращает индекс нового рабочего листа, который можно использовать для доступа к экземпляру этого рабочего листа. Подробнее о том, как получить доступ к рабочим листам, см.[Доступ к рабочим листам](/cells/ru/net/access-worksheets/).

{{% /alert %}} 
### **С указанным именем листа**
Чтобы добавить рабочий лист с определенным именем в элемент управления GridWeb вместо использования схемы именования по умолчанию, вызовите перегруженную версию метода Add, который принимает указанное имя листа. Например, в приведенном ниже примере добавляется рабочий лист с именем Invoice.

**Вывод: рабочий лист с указанным именем добавлен в GridWeb.** 

![дело:изображение_альтернативный_текст](add-worksheets_2.png)



{{< gist "aspose-cells-gists" "7c644a93d33d24299a618c1dda1a2385" "Examples.GridWeb-CSharp-Worksheets-AddWorksheets.aspx-AddWorksheetWithName.cs" >}}

{{% alert color="primary" %}} 

Метод Add, принимающий имя рабочего листа в виде строки, возвращает экземпляр GridWorksheet.

{{% /alert %}}
