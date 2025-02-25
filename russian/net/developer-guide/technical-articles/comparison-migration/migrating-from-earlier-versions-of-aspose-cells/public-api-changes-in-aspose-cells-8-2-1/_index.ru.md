﻿---
title: Общедоступный API Изменения в Aspose.Cells 8.2.1
type: docs
weight: 80
url: /ru/net/public-api-changes-in-aspose-cells-8-2-1/
---
{{% alert color="primary" %}} 

В этом документе описаны изменения в Aspose.Cells API с версии 8.2.0 до 8.2.1, которые могут представлять интерес для разработчиков модулей/приложений. Он включает в себя не только новые и обновленные общедоступные методы, но и описание любых изменений в поведении за кулисами в Aspose.Cells.

{{% /alert %}} 
## **Добавлен метод GetValidation() для класса Cell.**
Проверка данных — это одна из функций, которую дизайнеры электронных таблиц используют, чтобы запретить пользователям вставлять недопустимые значения в определенную ячейку. С Aspose.Cells for .NET 8.2.1 API представил простой механизм, который определяет, применялась ли проверка данных к ячейке. Используйте метод GetValidation класса Cell для получения любой примененной проверки. Если проверки нет, метод возвращает null. Точно так же вы можете использовать метод GetValidationInCell класса ValidationCollection, чтобы получить проверку, примененную к любой ячейке, предоставив ее индексы строки и столбца.

{{% alert color="primary" %}} 

 Пожалуйста, ознакомьтесь с подробной статьей о[Применить проверку к номеру Cell](/cells/ru/net/get-validation-applied-on-a-cell/) для дополнительной информации.

{{% /alert %}}
## **Добавлен метод GetValidationValue() для класса Cell.**
В дополнение к определению того, применялась ли проверка, вы также можете проверить, удовлетворяет ли заданное значение правилам проверки данных для конкретной ячейки. Эта функция полезна в сценариях, когда вы хотите проверить, удовлетворяет ли введенное в ячейку значение правилам проверки данных на лету. Aspose.Cells API предоставил метод GetValidationValue для класса Cell. Если значение, введенное в ячейку, не удовлетворяет правилам проверки данных, метод GetValidationValue для класса Cell возвращает значение false.

{{% alert color="primary" %}} 

 Пожалуйста, ознакомьтесь с подробной статьей о[Убедитесь, что значение Cell удовлетворяет правилам проверки данных.](/cells/ru/net/verify-that-cell-value-satisfies-data-validation-rules/).

{{% /alert %}}
## **Добавлен перегруженный метод ToPrinter(PrinterSettings printerSettings) для класса WorkbookRender.**
Вы можете использовать перегруженный метод для вывода книги на принтер через PrinterSettings.
