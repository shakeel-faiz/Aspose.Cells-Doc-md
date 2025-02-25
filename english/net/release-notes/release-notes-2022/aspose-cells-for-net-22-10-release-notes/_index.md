---
title: Aspose.Cells for .NET 22.10 Release Notes
type: docs
weight: 3
url: /net/aspose-cells-for-net-22-10-release-notes/
---

{{% alert color="primary" %}}

This page contains release notes for [Aspose.Cells for .NET 22.10](https://www.nuget.org/packages/Aspose.Cells/22.10.0).

{{% /alert %}}

|**Key**|**Summary**|**Category**|
| :- | :- | :- |
|CELLSNET-42037|PivotTable Timeline Filter disappears after loading excel document and updating|New Feature
|CELLSNET-51963|Support for CRTX files|New Feature
|CELLSNET-51952|MAXIFS formulas take long time to be calculated|Enhancement
|CELLSNET-52064|It's not allowed to push non-empty cells off the end of the worksheet error when using Cells.InsertRows method|Enhancement
|CELLSNET-52029|Translate legend entries labels in accordance with locale/regional settings|Enhancement
|CELLSNET-51419|External Link of Pivot table got deleted when converting XLS file to XLSM|Bug
|CELLSNET-51984|XLSX file with PivotTable file is corrupted after re-save|Bug
|CELLSNET-51987|Issue with some Smart Markers (inserted) in the PivotTable and Pivot chart|Bug
|CELLSNET-52065|Wrong external data connections when converting external connections|Bug
|CELLSNET-52088|Extra row is added when creating classic pivot table |Bug
|CELLSNET-52018|GetValidationValue incorrect using NotBetween operator |Bug
|CELLSNET-52069|Decimal values in the result of Cell.Formula may be different from what ms excel shows|Bug
|CELLSNET-52078|Style.SetPatternColor(BackgroundType,Color,Color) does not take effect|Bug
|CELLSNET-52105|LightCellsDataHandler.StartSheet(Worksheet) cannot skip the sheet when returning false for xlsb template file|Bug
|CELLSNET-46764|Missing chart title on convert to pdf|Bug
|CELLSNET-52049|XLSX to PDF: Text not formatted properly|Bug
|CELLSNET-52073|Issue regarding Arial Tur font in Excel to PDF rendering|Bug
|CELLSNET-52083|Some cells with the Accounting number format are rendered as #####.|Bug
|CELLSNET-52091|When setting the worksheet contents to black and white, it is still printed in color & borders are displayed unnecessarily|Bug
|CELLSNET-51972|Worksheet containing button objects are not recognized properly when copying the sheet|Bug
|CELLSNET-51973|Html table to Excel sheet not converted properly |Bug
|CELLSNET-52001|Re-saving an XLSX file generated corrupt file|Bug
|CELLSNET-52015|Unable to load power query formula from Excel file|Bug
|CELLSNET-52054|Style corruption after saving and reopening an Aspose.Cells-generated workbook |Bug
|CELLSNET-52056|Hyperlink Duplication Issue |Bug
|CELLSNET-52071|Excel to XML conversion - Element Names are Not Escaped |Bug
|CELLSNET-52074|HTML to XLSX: Missing cell content|Bug
|CELLSNET-52084|The position of the "Northwind Traders" text is incorrect (the left indent value is not interpreted correctly).|Bug
|CELLSNET-52063|PivotTable.CalculateData caused NullReferenceException|Exception
|CELLSNET-51986|Calculating workbook twice with enabled calculation chain caused exception|Exception
|CELLSNET-52081|Opening XLSX file whose styles have been removed throws exception|Exception
|CELLSNET-52044|Exception raised while importing the customer's file in GridWeb|Exception
|CELLSNET-52002|Exception is thrown when trying to open unprotected document with a password|Exception

## **Public API and Backwards Incompatible Changes**

The following is a list of any changes made to the public API such as added, renamed, removed or deprecated members as well as any non-backward compatible change made to Aspose.Cells for .NET. If you have concerns about any change listed, please raise it on the Aspose.Cells support forum.

### **Changed the limit of moving cells out of the sheet for inserting rows**

In old versions, if there are cells that have formatting settings but has no value?and will be moved out of the sheet, insert operation is not allowed. From 22.10, insert operation is allowed for such kind of situation and such behavior is same with ms excel now.

### **Adds DataModelConnection class**

Specifies a data model connection.

### **Adds Chart.ChangeTemplate(byte[]) methods**

Change chart type with preset template file.

### **Adds ChartCollection.Add(byte[] data, string dataRange, bool isVertical, int topRow, int leftColumn,int rightRow, int bottomColumn) method.**

Adds chart with preset template file.
