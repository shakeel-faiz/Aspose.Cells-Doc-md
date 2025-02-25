﻿---
title: Speichern Sie die Arbeitsmappe im Text- oder CSV-Format mit Aspose.Cells
type: docs
weight: 80
url: /de/net/save-workbook-to-text-or-csv-format-using-aspose-cells/
---
{{% alert color="primary" %}} 

Manchmal möchten Sie eine Arbeitsmappe mit mehreren Arbeitsblättern in das Textformat konvertieren oder speichern. Bei Textformaten (z. B. TXT, TabDelim, CSV usw.) speichern sowohl Microsoft Excel als auch Aspose.Cells standardmäßig nur den Inhalt des aktiven Arbeitsblatts.

{{% /alert %}} 

Im folgenden Codebeispiel wird erläutert, wie eine gesamte Arbeitsmappe im Textformat gespeichert wird. Laden Sie die Quellarbeitsmappe, die eine beliebige Microsoft Excel- oder OpenOffice-Tabellendatei sein kann (also XLS, XLSX, XLSM, XLSB, ODS usw.) mit einer beliebigen Anzahl von Arbeitsblättern.

Wenn der Code ausgeführt wird, konvertiert er die Daten aller Blätter in der Arbeitsmappe in das Format TXT.

Sie können dasselbe Beispiel ändern, um Ihre Datei im Format CSV zu speichern. TxtSaveOptions.Separator ist standardmäßig ein Komma, geben Sie also kein Trennzeichen an, wenn Sie im Format CSV speichern.

**C#**

{{< highlight "csharp" >}}

string FilePath = @"..\..\..\Beispieldateien\";

string FileName = FilePath + "Save Workbook to Text or CSV Format.xlsx";

string destFileName = FilePath + "Save Workbook to Text or CSV Format.txt";

//Laden Sie Ihre Quellarbeitsmappe

Arbeitsmappe Arbeitsmappe = neue Arbeitsmappe (Dateiname);

//0-Byte-Array

byte[]workbookData = new byte[0];

//Optionen zum Speichern von Text. Sie können jede Art von Trennzeichen verwenden

TxtSaveOptions opts = neue TxtSaveOptions();

opts.Trennzeichen = '\t';

// Alle Arbeitsblattdaten im Textformat in das Datenarray der Arbeitsmappe kopieren

 für (int idx = 0; idx< workbook.Worksheets.Count; idx++)

{

    //Save the active worksheet into text format

    MemoryStream ms = new MemoryStream();

    workbook.Worksheets.ActiveSheetIndex = idx;

    workbook.Save(ms, opts);

    //Save the worksheet data into sheet data array

    ms.Position = 0;

    byte[] sheetData = ms.ToArray();

    //Combine this worksheet data into workbook data array

    byte[] combinedArray = new byte[workbookData.Length + sheetData.Length];

    Array.Copy(workbookData, 0, combinedArray, 0, workbookData.Length);

    Array.Copy(sheetData, 0, combinedArray, workbookData.Length, sheetData.Length);

    workbookData = combinedArray;

}

//Save entire workbook data into file

File.WriteAllBytes(destFileName, workbookData);

{{< /highlight >}}
## **Beispielcode herunterladen**
- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-.NET/tree/master/Plugins/Aspose.Cells%20Vs%20OpenXML%20Spreadsheets/OpenXML%20Missing%20Features/Save%20Workbook%20to%20Text%20or%20CSV%20Format)

## **Laufendes Beispiel herunterladen**
- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-.NET/releases/tag/MissingFeaturesOpenXMLExcelv1.1)
