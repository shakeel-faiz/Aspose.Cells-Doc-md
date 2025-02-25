﻿---
title: Daten aus Arbeitsblättern exportieren
type: docs
weight: 40
url: /de/java/export-data-from-worksheets/
---
## **Aspose.Cells – Exportieren von Daten aus Arbeitsblättern**
Aspose.Cells ermöglicht seinen Benutzern nicht nur den Import von Daten in Arbeitsblätter aus externen Datenquellen, sondern auch den Export von Arbeitsblattdaten in ein Array.

**Java**

{{< highlight "java" >}}

 //Erstellen eines Dateistroms, der die zu öffnende Excel-Datei enthält

FileInputStream fstream = new FileInputStream(dataDir + "workbook.xls");

//Instanziieren eines Workbook-Objekts

Arbeitsmappe Arbeitsmappe = neue Arbeitsmappe (fstream);

//Auf das erste Arbeitsblatt in der Excel-Datei zugreifen

Arbeitsblatt Arbeitsblatt = workbook.getWorksheets().get(0);

// Exportieren des Inhalts von 7 Zeilen und 2 Spalten beginnend mit der 1. Zelle in Array.

Objekt dataTable [][]= worksheet.getCells().exportArray(4,0,7,8);

 für (int i = 0 ; i< dataTable.length ; i++)

{

	System.out.println("["+ i +"]: "+ Arrays.toString(dataTable[i]));

}

//Closing the file stream to free all resources

fstream.close();

{{< /highlight >}}
## **Laufcode herunterladen**

- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-Java/releases/tag/Aspose.Cells_Java_for_Apache_POI_SS-v1.0.0)
## **Beispielcode herunterladen**
- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-Java/blob/master/Plugins/Aspose_Cells_for_Apache_POI/Aspose-Cells-for-Apache-POI-(Maven)/src/main/java/com/aspose/cells/examples/asposefeatures/datahandling/ExportDataFromWorksheets.java)

{{% alert color="primary" %}} 

 Weitere Informationen finden Sie unter[Exportieren von Daten aus Arbeitsblättern](/java/exporting-data-from-worksheets).

{{% /alert %}}
