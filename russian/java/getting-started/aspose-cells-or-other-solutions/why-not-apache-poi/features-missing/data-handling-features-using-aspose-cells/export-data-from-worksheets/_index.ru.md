﻿---
title: Экспорт данных из рабочих листов
type: docs
weight: 40
url: /ru/java/export-data-from-worksheets/
---
## **Aspose.Cells - Экспорт данных из рабочих листов**
Aspose.Cells не только позволяет своим пользователям импортировать данные в рабочие листы из внешних источников данных, но также позволяет им экспортировать данные рабочего листа в массив.

**Java**

{{< highlight "java" >}}

 //Создание файлового потока, содержащего открываемый файл Excel

FileInputStream fstream = новый FileInputStream (dataDir + "workbook.xls");

//Создание экземпляра объекта Workbook

Книга рабочей книги = новая рабочая книга (fstream);

//Доступ к первому рабочему листу в файле Excel

Рабочий лист = workbook.getWorksheets().get(0);

//Экспорт содержимого 7 строк и 2 столбцов, начиная с 1-й ячейки, в массив.

Объект dataTable [][]= worksheet.getCells().exportArray(4,0,7,8);

 для (int я = 0 ; я< dataTable.length ; i++)

{

	System.out.println("["+ i +"]: "+ Arrays.toString(dataTable[i]));

}

//Closing the file stream to free all resources

fstream.close();

{{< /highlight >}}
## **Скачать рабочий код**

- [Гитхаб](https://github.com/aspose-cells/Aspose.Cells-for-Java/releases/tag/Aspose.Cells_Java_for_Apache_POI_SS-v1.0.0)
## **Скачать пример кода**
- [Гитхаб](https://github.com/aspose-cells/Aspose.Cells-for-Java/blob/master/Plugins/Aspose_Cells_for_Apache_POI/Aspose-Cells-for-Apache-POI-(Maven)/src/main/java/com/aspose/cells/examples/asposefeatures/datahandling/ExportDataFromWorksheets.java)

{{% alert color="primary" %}} 

 Для получения более подробной информации посетите[Экспорт данных из рабочих листов](/java/exporting-data-from-worksheets).

{{% /alert %}}
