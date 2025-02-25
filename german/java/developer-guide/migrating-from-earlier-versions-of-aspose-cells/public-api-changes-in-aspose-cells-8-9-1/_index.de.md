﻿---
title: Öffentlich API Änderungen in Aspose.Cells 8.9.1
type: docs
weight: 320
url: /de/java/public-api-changes-in-aspose-cells-8-9-1/
---
{{% alert color="primary" %}} 

Dieses Dokument beschreibt die Änderungen an Aspose.Cells API von Version 8.9.0 zu 8.9.1, die für Modul-/Anwendungsentwickler von Interesse sein könnten. Es enthält nicht nur neue und aktualisierte öffentliche Methoden, hinzugefügte und entfernte Klassen usw., sondern auch eine Beschreibung aller Änderungen im Verhalten hinter den Kulissen in Aspose.Cells.

{{% /alert %}} 
## **APIs hinzugefügt**
### **Konfigurierbare Schriftartquellen**
Aspose.Cells for Java hat eine Reihe von Klassen verfügbar gemacht, um die Unterstützung für konfigurierbare Schriftartquellen zum Rendern von Tabellenkalkulationen bereitzustellen. Hier ist die Liste der Klassen, die mit Aspose.Cells for Java 8.9.1 hinzugefügt wurden.

1. Die FontConfigs-Klasse gibt die Schriftarteinstellungen an.
1. Die FontSourceBase-Klasse ist eine abstrakte Basisklasse für die Klassen, die es dem Benutzer ermöglichen, verschiedene Schriftartquellen anzugeben.
1. Die FileFontSource-Klasse stellt die einzelne TrueType-Schriftartdatei dar, die im Dateisystem gespeichert ist.
1. Die FolderFontSource-Klasse stellt den Ordner dar, der TrueType-Schriftartdateien enthält.
1. Die MemoryFontSource-Klasse stellt die einzelne TrueType-Schriftartdatei dar, die im Arbeitsspeicher gespeichert ist.
1. Die Aufzählung FontSourceType gibt den Typ einer Schriftartquelle an.

Mit den oben genannten Änderungen ermöglicht die Aspose.Cells for Java die Einstellung der Schriftarten wie unten beschrieben.

1. Legen Sie einen benutzerdefinierten Schriftartenordner fest, während Sie die Methode FontConfigs.setFontFolder verwenden.
1. Legen Sie mehrere Ordner für benutzerdefinierte Schriftarten fest, während Sie die Methode FontConfigs.setFontFolders verwenden.
1. Legen Sie Schriftartquellen aus einem benutzerdefinierten Schriftartordner, einer einzelnen Schriftartdatei oder Schriftartdaten aus einem Array von Bytes fest, während Sie die Methode FontConfigs.setFontSources verwenden.

Hier ist ein einfaches Anwendungsszenario der oben genannten Methoden.

**Java**

{{< highlight "csharp" >}}

 //Defining string variables to store paths to font folders & font file

String fontFolder1 = "D:/Arial";

String fontFolder2 = "D:/Calibri";

String fontFile = "D:/Arial/arial.ttf";

//Setting first font folder with setFontFolder method

//Second parameter directs the API to search the sub folders for font files

FontConfigs.setFontFolder(fontFolder1, true);

//Setting both font folders with setFontFolders method

//Second parameter prohibits the API to search the sub folders for font files

FontConfigs.setFontFolders(new String[]{ fontFolder1, fontFolder2 }, false);

//Defining FolderFontSource

FolderFontSource sourceFolder = new FolderFontSource(fontFolder1, false);

//Defining FileFontSource

FileFontSource sourceFile = new FileFontSource(fontFile);

//Defining MemoryFontSource

byte[]bytes = Files.readAllBytes(new File(fontFile).toPath());

MemoryFontSource sourceMemory = new MemoryFontSource(bytes);

//Setting font sources

FontConfigs.setFontSources(new FontSourceBase[]{ sourceFolder, sourceFile, sourceMemory});

{{< /highlight >}}

{{% alert color="primary" %}} 

 Beide FontConfigs.setFontFolder- und FontConfigs.setFontFolders-Methoden akzeptieren einen zweiten Parameter vom Typ Boolean. Die Übergabe von true als zweiten Parameter weist die Aspose.Cells-APIs an, die Unterordner nach den Schriftartdateien zu durchsuchen.

{{% /alert %}} 

Aspose.Cells for Java ermöglicht auch die Konfiguration der Schriftersetzung. Dieser Mechanismus ist hilfreich, wenn eine erforderliche Schriftart auf dem Computer, auf dem die Konvertierung stattfinden soll, nicht verfügbar ist. Benutzer können eine Liste mit Schriftartnamen als Alternative zur ursprünglich erforderlichen Schriftart bereitstellen. Um dies zu erreichen, haben die Aspose.Cells-APIs die Methode FontConfigs.setFontSubstitutes verfügbar gemacht, die zwei Parameter akzeptiert. Der erste Parameter ist vom Typ string, der der Name der Schriftart sein sollte, die ersetzt werden muss. Der zweite Parameter ist ein Array vom Typ String. Benutzer können eine Liste mit Schriftartnamen als Ersatz für den ursprünglichen Schriftartnamen (angegeben im ersten Parameter) bereitstellen.

Hier ist ein einfaches Nutzungsszenario der Methode FontConfigs.SetFontSubstitutes.

**Java**

{{< highlight "csharp" >}}

 //Substituting the Arial font with Times New Roman & Calibri

FontConfigs.setFontSubstitutes("Arial", new String[]{ "Times New Roman", "Calibri" });

{{< /highlight >}}

Die Aspose.Cells for Java hat auch Mittel bereitgestellt, um Informationen darüber zu sammeln, welche Quellen und Substitutionen eingestellt wurden.

1. Die Methode FontConfigs.getFontSources gibt ein Array vom Typ FontSourceBase zurück, das die Liste der angegebenen Schriftartquellen enthält. Falls keine Quellen festgelegt wurden, gibt die Methode FontConfigs.getFontSources ein leeres Array zurück.
1. Die Methode „FontConfigs.getFontSubstitutes“ akzeptiert einen Parameter vom Typ „String“, mit dem der Schriftartname angegeben werden kann, für den eine Ersetzung festgelegt wurde. Falls für den angegebenen Schriftartnamen keine Ersetzung festgelegt wurde, gibt die Methode FontConfigs.getFontSubstitutes null zurück.

{{% alert color="primary" %}} 

 Weitere Einzelheiten zu FontConfigs finden Sie im Artikel unter[Konfigurieren von Schriftarten zum Rendern von Tabellenkalkulationen](/cells/de/java/configuring-fonts-for-rendering-spreadsheets/).

{{% /alert %}} 
### **IFilePathProvider Interface & HtmlSaveOptions.FilePathProvider-Eigenschaft hinzugefügt**
Aspose.Cells for Java 8.9.1 ermöglicht das Abrufen/Setzen des IFilePathProvider zum Exportieren von Arbeitsblättern in separate HTML-Dateien. Diese neuen APIs sind in Szenarien hilfreich, in denen Hyperlinks in einem Arbeitsblatt auf eine Position in einem anderen Arbeitsblatt verweisen, in denen die Anwendungsanforderung darin besteht, jedes Arbeitsblatt in eine separate HTML-Datei zu rendern. Die Implementierung des IFilePathProvider ermöglicht es, die oben genannten Hyperlinks intakt zu halten, unabhängig davon, ob sie auf einen Ort in einer separaten resultierenden HTML-Datei verweisen.

Im Folgenden ist das einfache Verwendungsszenario der HtmlSaveOptions.FilePathProvider-Eigenschaft dargestellt.

**Java**

{{< highlight "csharp" >}}

 //Eine Tabelle in eine Instanz von Workbook laden

Arbeitsmappenbuch = neue Arbeitsmappe (dir + "sample.xlsx");

// Speichern Sie jedes Arbeitsblatt in einer separaten HTML-Datei

 für (int i = 0; i< book.getWorksheets().getCount(); i++)

{

	book.getWorksheets().setActiveSheetIndex(i);

	//Create an instance of HtmlSaveOptions & set FilePathProvider property

	HtmlSaveOptions options = new HtmlSaveOptions();

	options.setExportActiveWorksheetOnly(true);

	options.setFilePathProvider(new IFilePathProvider() 

	{ 

		public String getFullName(String sheetName)

		{

		    if ("Sheet2".equals(sheetName))

		    {

		        return "sheet1.html";

		    }

		    else if ("Sheet3".equals(sheetName))

		    {

		        return "sheet2.html";

		    }



		    return "";

		}

	});



	 //Write HTML file to disc

	 book.save(dir + "sheet"+ i +".html", options);

}

{{< /highlight >}}

{{% alert color="primary" %}} 

 Weitere Einzelheiten zu dieser Verbesserung finden Sie im Artikel auf[Implementieren der IFilePathProvider-Schnittstelle](/cells/de/java/provide-exported-worksheet-html-file-path-via-ifilepathprovider-interface/).

{{% /alert %}} 
### **CopyOptions.ReferToDestinationSheet-Eigenschaft und Überladung für Cells.copyRows-Methode hinzugefügt**
Aspose.Cells for Java API hat die CopyOptions.ReferToDestinationSheet-Eigenschaft des booleschen Typs zusammen mit einer Überladung der Cells.copyRows-Methode verfügbar gemacht, um den Vorgang zum Kopieren von Zeilen zu vereinfachen, wenn zu kopierende Zeilen auch ein Diagramm und seine Datenquelle enthalten. Entwickler können diese neuen APIs verwenden, um die Datenquelle des Diagramms auf die Quell- oder Zielarbeitsblätter zu verweisen.

Es folgt das einfache Nutzungsszenario.

**Java**

{{< highlight "csharp" >}}

 //Load a sample spreadsheet in an instance of Workbook

Workbook book = new Workbook(dir + "sample.xlsx");

//Access the worksheet containing the chart & its data source

Worksheet source = book.getWorksheets().get(0);

//Add a new worksheet to the collection

Worksheet destination = book.getWorksheets().get(book.getWorksheets().add());

//Initialize CopyOptions and set its ReferToDestinationSheet property to true

CopyOptions options = new CopyOptions();

options.setReferToDestinationSheet(true);

//Copy the rows

destination.getCells().copyRows(source.getCells(), 0, 0, source.getCells().getMaxDisplayRange().getRowCount(), options);

//Save the result on disc

book.save(dir + "output.xlsx");

{{< /highlight >}}

{{% alert color="primary" %}} 

 Weitere Einzelheiten zu dieser Funktion finden Sie im Artikel auf[Steuern Sie die Datenquelle des Diagramms beim Kopieren von Zeilen](/cells/de/java/change-data-source-of-the-chart-to-destination-worksheet-while-copying-rows-or-range/).

{{% /alert %}} 
### **CalculationOptions.Recursive-Eigenschaft hinzugefügt**
Aspose.Cells for Java 8.9.1 hat die CalculationOptions.Recursive-Eigenschaft des booleschen Typs verfügbar gemacht. Durch Festlegen der Eigenschaft „CalculationOptions.Recursive“ auf „true“ und Übergeben des Objekts an die Methode „Workbook.calculateFormula“ werden die Aspose.Cells-APIs angewiesen, die abhängigen Zellen rekursiv zu berechnen, wenn Zellen berechnet werden, die von anderen Zellen abhängen.

Es folgt das einfache Nutzungsszenario.

**Java**

{{< highlight "csharp" >}}

 //Load a sample spreadsheet in an instance of Workbook

Workbook book = new Workbook(dir + "sample.xlsx");

//Initialize CalculationOptions & set Recursive property to true

CalculationOptions options = new CalculationOptions();

options.setRecursive(true);

//Recalculate formulas

book.calculateFormula(options);

{{< /highlight >}}

{{% alert color="primary" %}} 

 Weitere Einzelheiten zu dieser Funktion finden Sie im Artikel auf[Berechnungszeit optimieren](/cells/de/java/decrease-the-calculation-time-of-cell-calculate-method/).

{{% /alert %}}
## **Veraltete APIs**
### **Veraltete CellsHelper.FontDir-Eigenschaft**
Es wird empfohlen, stattdessen die Methode FontConfigs.setFontFolder(String, boolean) zu verwenden, wobei der Ordner rekursiv zu false ist.
### **Veraltete CellsHelper.FontDirs-Eigenschaft**
Verwenden Sie stattdessen die Methode „FontConfigs.setFontFolders(String[], boolean)“, wobei der Ordner rekursiv zu „false“ wird.
### **Veraltete CellsHelper.FontFiles-Eigenschaft**
Verwenden Sie stattdessen die Methode FontConfigs.setFontSources(FontSourceBase[]).
