﻿---
title: Отключить проверку совместимости в Excel
type: docs
weight: 170
url: /ru/net/disable-compatibility-checker-in-excel/
keywords: c# excel disable compatibility checke
---
## Отключить средство проверки совместимости в листах Excel в C#

{{% alert color="primary" %}}

Microsoft Флаги средства проверки совместимости Excel при сохранении файла в более раннем формате файла могут вызвать проблемы с функциональностью или потерю точности. Средство проверки совместимости — это функция Microsoft Office Excel 2007 и Microsoft Excel 2010.

Когда вы сохраняете книгу в предыдущей версии, от Excel 97 до Excel 2003, из Excel 2007 или Excel 2010, средство проверки совместимости сканирует книгу, чтобы определить, содержит ли она функции, которые не поддерживаются в более ранней версии. Чтобы помочь вам принять решение о том, как справляться с проблемами совместимости, средство проверки совместимости отображает диалоговые окна с параметрами. Его также можно использовать для создания отчета о любых проблемах в книге или отключения этой функции.

Иногда вам нужно отключить средство проверки совместимости для определенной электронной таблицы. С помощью API-интерфейсов Aspose.Cells' вы можете сделать это программно, чтобы пользователи не расстраивались и не сбивались с толку из-за всплывающего диалогового окна средства проверки совместимости, когда они повторно сохраняют файл в Microsoft Excel вручную.

{{% /alert %}}

## **Использование Microsoft Excel**

Чтобы отключить средство проверки совместимости в Microsoft Excel (например, Microsoft Excel 2007/2010):

-  (Excel 2007) На кнопке Office щелкните**Подготовить** , тогда**Запустить проверку совместимости** , а затем очистите**Проверяйте совместимость при сохранении этой книги** вариант.
-  (Excel 2010) На вкладке «Файл» щелкните**Информация** , тогда**Проверить наличие проблем** , нажмите**Проверить совместимость** , и, наконец, очистить**Проверяйте совместимость при сохранении этой книги** вариант.

## **Использование API Aspose.Cells**

 Установить[**Workbook.Settings.CheckComptiliblity**](https://reference.aspose.com/cells/net/aspose.cells/workbooksettings/properties/checkcompatibility) собственность на**ЛОЖЬ** чтобы отключить Microsoft средство проверки совместимости Excel.

### **Примеры кода**

В приведенных ниже примерах кода показано, как отключить средство проверки совместимости с помощью Aspose.Cells for .NET.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Articles-DisableCompatibilityChecker-1.cs" >}}
