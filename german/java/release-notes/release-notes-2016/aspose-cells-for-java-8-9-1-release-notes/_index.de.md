﻿---
title: Aspose.Cells for Java 8.9.1 Versionshinweise
type: docs
weight: 60
url: /de/java/aspose-cells-for-java-8-9-1-release-notes/
---
## **1) Aspose.Cells**

|**Taste**|**Zusammenfassung**|**Kategorie**|
|:- |:- |:- |
|CELLSJAVA-41925|Die Berechnungszeit hat sich mit den letzten API-Revisionen erhöht|Neue Funktion|
|CELLSJAVA-40958|Ein vom Benutzer konfigurierbarer Ersatzmechanismus für Schriftarten ist erforderlich|Neue Funktion|
|CELLSJAVA-41936|Die Workbook.calculateFormula()-Methode wird für die Excel-Quelldatei nie beendet|Erweiterung|
|CELLSJAVA-41928|Bildressource kann nicht erfasst werden, während die Tabelle mit IStreamProvider auf HTML gerendert wird|Insekt|
|CELLSJAVA-41841|Problem beim Rendern von Kontrollkästchen auf HTML|Insekt|
|CELLSJAVA-41932|Problem mit getDisplayStringValue() für Werte im Datumsformat|Insekt|
|CELLSJAVA-41930|Bei Verwendung von Light Cells-APIs zum Verarbeiten einer XLS-Datei wird immer die erste Zelle des ersten Blatts verarbeitet|Insekt|
|CELLSJAVA-41931|Zeichenabstand und -umbruch für vertikalen Text beim Rendern der Tabelle auf PDF nicht korrekt|Insekt|
|CELLSJAVA-41709|Spaltenbreiten sind auf CentOS anders als auf Windows|Insekt|
|CELLSJAVA-41933|Der Diagrammmaßstab hat sich beim Rendern der Tabelle auf PDF verschoben|Insekt|
|CELLSJAVA-41934|Ausrichtungsproblem beim Rendern einer Excel-Datei auf PDF|Insekt|
|CELLSJAVA-41935|Die Formatierung von Legendeneinträgen wird beim Rendern der Tabelle auf PDF gestört|Insekt|
|CELLSJAVA-41943|Die horizontalen Achsenbeschriftungen wurden nicht vollständig gerendert, das heißt; Bei allen Beschriftungen fehlen einige Inhalte im gerenderten Bild.|Insekt|
|CELLSJAVA-41940|Datei ist nach Formelberechnung und Speichern beschädigt|Insekt|
|CELLSJAVA-41927|Ausnahme: "java.lang.OutOfMemoryError" beim Speichern im Dateiformat HTML|Ausnahme|
|CELLSJAVA-41945|CellsException: Fehler beim Berechnen von Cell[0Sheet1!E5]in Workbook.CalculateFormula beim Berechnen der TREND-Funktion|Ausnahme|
|CELLSJAVA-41946|Das Öffnen einer Excel-Datei verursacht eine java.lang.NumberFormatException: Für die Eingabezeichenfolge: „80000020“|Ausnahme|
|CELLSJAVA-41922|IndexOutOfBoundsException beim Kopieren von Zellen|Ausnahme|
## **Öffentliche API und rückwärts inkompatible Änderungen**
Im Folgenden finden Sie eine Liste aller Änderungen, die an der öffentlichen API vorgenommen wurden, z. B. hinzugefügte, umbenannte, entfernte oder veraltete Mitglieder, sowie alle nicht abwärtskompatiblen Änderungen, die an Aspose.Cells for Java vorgenommen wurden das Aspose.Cells Support-Forum.
### **Fügt die Eigenschaft CopyOptions.ReferToDestinationSheet und die Methode Cells.CopyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions) hinzu**
Gibt an, ob beim Kopieren von Zeilen/Bereichen auf das Zielarbeitsblatt (als Datenquelle für das Diagramm) verwiesen werden soll.
Wenn der Bereich kopiert wird und das Diagramm auf das Quellblatt verweist, bedeutet False, dass die Datenquelle des kopierten Diagramms nicht geändert wird. True bedeutet, dass die Datenquelle des kopierten Diagramms auf das Zielblatt verweist.
### **Fügt die HtmlSaveOptions.FilePathProvider-Eigenschaft hinzu**
Ruft den IFilePathProvider zum separaten Exportieren von Arbeitsblättern in HTML ab oder legt diesen fest.
### **Fügt die IFilePathProvider-Schnittstelle hinzu**
Stellt den exportierten Dateipfadanbieter dar.
### **Fügt die FontConfigs-Klasse hinzu**
Gibt Schriftarteinstellungen an.
### **Fügt die FontSourceBase-Klasse hinzu**
Dies ist eine abstrakte Basisklasse für die Klassen, die es dem Benutzer ermöglichen, verschiedene Schriftartquellen anzugeben.
### **Fügt die FileFontSource-Klasse hinzu**
Stellt die einzelne TrueType-Schriftartdatei dar, die im Dateisystem gespeichert ist.
### **Fügt die FolderFontSource-Klasse hinzu**
Stellt den Ordner dar, der TrueType-Schriftartdateien enthält.
### **Fügt die MemoryFontSource-Klasse hinzu**
Stellt die einzelne TrueType-Schriftartdatei dar, die im Arbeitsspeicher gespeichert ist.
### **Fügt FontSourceType-Aufzählung hinzu**
Gibt den Typ einer Schriftartquelle an.
### **Fügt die CalculationOptions.Recursive-Eigenschaft hinzu**
Gibt an, ob die abhängigen Zellen bei der Berechnung einer Zelle rekursiv berechnet werden und von anderen Zellen abhängen.
### **Veraltet die CellsHelper.FontDir-Eigenschaft**
Verwenden Sie stattdessen die Methode „FontConfigs.SetFontFolder(string, bool)“, wobei der Ordner rekursiv zu „false“ wird.
### **Veraltet die CellsHelper.FontDirs-Eigenschaft**
Verwenden Sie stattdessen die Methode „FontConfigs.SetFontFolders(string[], bool)“, wobei der Ordner rekursiv zu „false“ wird.
### **Veraltet die CellsHelper.FontFiles-Eigenschaft**
Verwenden Sie stattdessen FontConfigs.SetFontSources(FontSourceBase[]).

{{% alert color="primary" %}} 

Da die Codebasis von Aspose.Cells for Java mit dem Code der relevanten .NET-Version übereinstimmt, sind die meisten Änderungen, Erweiterungen und Korrekturen, die in Aspose.Cells for .NET v8.9.1 enthalten sind, auch in dieser Aspose.Cells for Java v8.9.1 enthalten.

{{% /alert %}}
