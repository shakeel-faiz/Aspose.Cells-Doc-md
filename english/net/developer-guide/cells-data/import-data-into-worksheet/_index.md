---
title: Import Data into Worksheet
type: docs
weight: 170
url: /net/import-data-into-worksheet/
---

{{% alert color="primary" %}}

This article discusses some data import techniques that developers have access to through Aspose.Cells.

{{% /alert %}}

## **Import Data into Worksheet**

When you open an Excel file with Aspose.Cells, all data in the file is automatically imported. Aspose.Cells can also import data from other data sources.

Aspose.Cells provides a [**Workbook**](https://reference.aspose.com/cells/net/aspose.cells/workbook) class that represents a Microsoft Excel file. The [**Workbook**](https://reference.aspose.com/cells/net/aspose.cells/workbook) class contains a [**Worksheets**](https://reference.aspose.com/cells/net/aspose.cells/workbook/properties/worksheets) collection that allows access to each worksheet in an Excel file. A worksheet is represented by the [**Worksheet**](https://reference.aspose.com/cells/net/aspose.cells/worksheet) class. The [**Worksheet**](https://reference.aspose.com/cells/net/aspose.cells/worksheet) class provides a [**Cells**](https://reference.aspose.com/cells/net/aspose.cells/worksheet/properties/cells) collection. [**Cells**](https://reference.aspose.com/cells/net/aspose.cells/worksheet/properties/cells) collection provides useful methods to import data from different data sources. This article explains how these methods can be used.

## **Importing data int Excel with ICellsDataTable interface**
Implement [ICellsDataTable](https://reference.aspose.com/cells/net/aspose.cells/icellsdatatable) to wrap your various data sources, then use [Cells.ImportData()](https://reference.aspose.com/cells/net/aspose.cells/cells/importdata/#importdata) to import data to Excel worksheet.
### **Sample Code**
{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "ImportICellsDataTableIntoWorksheet.cs" >}}

The implementation of *CustomerDataSource*, *Customer*, and *CustomerList* classes is given below

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Workbook-ICellsDataTableDataSourceForWorkbookDesigner-2.cs" >}}


## **Importing from Array**

To import data to a spreadsheet from an array, call the [**ImportArray**](https://reference.aspose.com/cells/net/aspose.cells/cells/methods/importarray/index) method of the [**Cells**](https://reference.aspose.com/cells/net/aspose.cells/worksheet/properties/cells) collection. There are many overloaded versions of the [**ImportArray**](https://reference.aspose.com/cells/net/aspose.cells/cells/methods/importarray/index) method but a typical overload takes the following parameters:

- **Array**, the array object that you're importing content from.
- **Row number**, the row number of the first cell that the data will be imported to.
- **Column number**, the column number of the first cell that the data will be imported to.
- **Is vertical**, a Boolean value that specifies whether to import data vertically or horizontally.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-Handling-Importing-ImportingFromArray-1.cs" >}}

## **Importing from ArrayList**

To import data from an *ArrayList* to worksheets, call the [**Cells**](https://reference.aspose.com/cells/net/aspose.cells/worksheet/properties/cells) collection's [**ImportArrayList**](https://reference.aspose.com/cells/net/aspose.cells/cells/methods/importarraylist) method. The ImportArray method takes the following parameters:

- **Array list**, represents the *ArrayList* object you're importing.
- **Row number**, represents the row number of the first cell that the data will be imported to.
- **Column number**, represents the column number of the first cell that the data will be imported to.
- **Is vertical**, a Boolean value that specifies whether to import data vertically or horizontally.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-Handling-Importing-ImportingFromArrayList-1.cs" >}}

## **Importing from Custom Objects**

To import data from a collection of objects to a worksheet, use [**ImportCustomObjects**](https://reference.aspose.com/cells/net/aspose.cells/cells/methods/importcustomobjects/index). Provide a list of columns/properties to the method to display your desired list of objects.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-Handling-Importing-ImportingFromCustomObject-1.cs" >}}

## **Importing from Custom Objects to merged area**

To import data from a collection of objects to a worksheet containing merged cells, use [**ImportTableOptions.CheckMergedCells**](https://reference.aspose.com/cells/net/aspose.cells/importtableoptions/properties/checkmergedcells) property. If the Excel template has merged cells, set the value of[**ImportTableOptions.CheckMergedCells**](https://reference.aspose.com/cells/net/aspose.cells/importtableoptions/properties/checkmergedcells) property to true. Pass the [**ImportTableOptions**](https://reference.aspose.com/cells/net/aspose.cells/importtableoptions) object along with the list of columns/properties to the method to display your desired list of objects. The following code sample demonstrates the use of [**ImportTableOptions.CheckMergedCells**](https://reference.aspose.com/cells/net/aspose.cells/importtableoptions/properties/checkmergedcells) property to import data from Custom Objects to merged cells. Please see the attached [source Excel](90112033.xlsx) file and the [output Excel](90112034.xlsx) file for reference.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-Handling-Importing-ImportCustomObjectsToMergedArea-1.cs" >}}

## **Importing from DataTable**

To import data from a *DataTable*, call the [**Cells**](https://reference.aspose.com/cells/net/aspose.cells/worksheet/properties/cells) collection's [**ImportDataTable**](https://reference.aspose.com/cells/net/aspose.cells/cells/methods/importdatatable/index) method. There are many overloaded versions of the [**ImportDataTable**](https://reference.aspose.com/cells/net/aspose.cells/cells/methods/importdatatable/index) method but a typical overload takes the following parameters:

- **Data table**, the *DataTable* object that you're importing the content from.
- **Is field name shown**, specifies whether the names of the *DataTable* columns should be imported to the worksheet as a first row or not.
- **Start cell**, represents the name of the start cell (for example "A1") from where to import the contents of the *DataTable*.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-Handling-Importing-ImportingFromDataTable-1.cs" >}}

## **Importing from dynamic object as data source**

Aspose.Cells provides features to work with dynamic objects as datasource. It helps in using datasource where properties are added dynamically to the objects. Once the properties are added to the object, Aspose.Cells considers the first entry as the template and handles the rest accordingly. It means if some dynamic property is added to a first item only and not to other objects, Aspose.Cells considers that all items in the collection should be the same.

In this example, a template model is used which initially contains two variables only. This List is converted to List of dynamic objects. Then some additional field is added into it and finally loaded into the workbook. The workbook picks only those values which are in the template XLSX file. This template workbook uses Smart Markers which also contain parameters. Parameters allow you to modify how the information is laid out. Details about the Smart Markers can be obtained from the following article:

[Using Smart Markers](/cells/net/using-smart-markers/)

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-Handling-Importing-ImportingFromDynamicDataTable-1.cs" >}}

## **Importing from DataColumn (.NET)**

A *DataTable* or *DataView* object is composed of one or more columns. Developers can also import data from any Column/Columns of the *DataTable* or *DataView* by calling the [**ImportData**](https://reference.aspose.com/cells/net/aspose.cells/cells/methods/importdata/index) method of the [**Cells**](https://reference.aspose.com/cells/net/aspose.cells/worksheet/properties/cells) collection. The [**ImportData**](https://reference.aspose.com/cells/net/aspose.cells/cells/methods/importdata/index) method accepts a parameter of type [**ImportTableOptions**](https://reference.aspose.com/cells/net/aspose.cells/importtableoptions). The [**ImportTableOptions**](https://reference.aspose.com/cells/net/aspose.cells/importtableoptions) class provides a [**ColumnIndexes**](https://reference.aspose.com/cells/net/aspose.cells/importtableoptions/properties/columnindexes) property that accepts an array of columns indexes.

The sample code given below demonstrates the use of [**ImportTableOptions.ColumnIndexes**](https://reference.aspose.com/cells/net/aspose.cells/importtableoptions/properties/columnindexes) to import selective columns.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-Handling-Importing-ImportingFromDataColumn-1.cs" >}}

## **Importing from DataView (.NET)**

To import data from a *DataView*, call the [**Cells**](https://reference.aspose.com/cells/net/aspose.cells/worksheet/properties/cells) collection's [**ImportData**](https://reference.aspose.com/cells/net/aspose.cells/cells/methods/importdata/index) method. There are many overloaded versions of the [**ImportData**](https://reference.aspose.com/cells/net/aspose.cells/cells/methods/importdata/index) method but the one for DataView takes the following parameters:

- **DataView:** The *DataView* object that you're about to import content from.
- **First Row:** the row number of the first cell that the data will be imported to.
- **First Column:** the column number of the first cell that the data will be imported to.
- **ImportTableOptions:** The import options.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-Handling-Importing-ImportingFromDataView-1.cs" >}}

## **Importing from DataGrid (.NET)**

It is possible to import data from a *DataGrid* by calling the [**ImportDataGrid**](https://reference.aspose.com/cells/net/aspose.cells/cells/methods/importdatagrid/index) method of the [**Cells**](https://reference.aspose.com/cells/net/aspose.cells/worksheet/properties/cells) collection. There are many overloaded versions of the [**ImportDataGrid**](https://reference.aspose.com/cells/net/aspose.cells/cells/methods/importdatagrid/index) method but a typical overload takes the following parameters:

- **Data grid**, the *DataGrid* object that you're importing content from.
- **Row Number**, the row number of the first cell that the data will be imported to.
- **Column Number**, the column number of the first cell that the data will be imported to.
- **Insert Rows**, a Boolean property that indicates whether extra rows should be added to the worksheet to fit data or not.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-Handling-Importing-ImportingFromDataGrid-1.cs" >}}

## **Importing from GridView**

To import data from a *GridView* control, call the [**ImportGridView**](https://reference.aspose.com/cells/net/aspose.cells/cells/methods/importgridview) method of the [**Cells**](https://reference.aspose.com/cells/net/aspose.cells/worksheet/properties/cells) collection.

Aspose.Cells allows us to respect HTML formatted values while importing data to the spreadsheet. When HTML parsing is enabled while importing data, Aspose.Cells converts the HTML into corresponding cell formatting.

## **Importing HTML formatted data**

Aspose.Cells provides a [**Cells**](https://reference.aspose.com/cells/net/aspose.cells/cells) class that provides very useful methods for importing data from external data sources. This article shows how to parse HTML formatted text while importing data and convert the HTML into formatted cell values.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-Handling-Importing-ImportHtmlFormattedData-1.cs" >}}

## **Importing Data from JSON**

Aspose.Cells provides a [**JsonUtility**](https://reference.aspose.com/cells/net/aspose.cells.utility/jsonutility) class for processing JSON. [**JsonUtility**](https://reference.aspose.com/cells/net/aspose.cells.utility/jsonutility) class has an [**ImportData**](https://reference.aspose.com/cells/net/aspose.cells.utility/jsonutility/methods/importdata) method for importing JSON data. Aspose.Cells also provides a [**JsonLayoutOptions**](https://reference.aspose.com/cells/net/aspose.cells.utility/jsonlayoutoptions) class that represents the options of JSON layout. The [**ImportData**](https://reference.aspose.com/cells/net/aspose.cells.utility/jsonutility/methods/importdata) method accepts [**JsonLayoutOptions**](https://reference.aspose.com/cells/net/aspose.cells.utility/jsonlayoutoptions) as a parameter. The [**JsonLayoutOptions**](https://reference.aspose.com/cells/net/aspose.cells.utility/jsonlayoutoptions) class provides the following properties.

- [**ArrayAsTable**](https://reference.aspose.com/cells/net/aspose.cells.utility/jsonlayoutoptions/properties/arrayastable): Indicates in the array should be processed as a table or not.
- [**ConvertNumericOrDate**](https://reference.aspose.com/cells/net/aspose.cells.utility/jsonlayoutoptions/properties/convertnumericordate): Gets or sets a value that indicates whether the string in JSON is to be converted to numeric or date.
- [**DateFormat**](https://reference.aspose.com/cells/net/aspose.cells.utility/jsonlayoutoptions/properties/dateformat): Gets and sets the format of the date value.
- [**IgnoreArrayTitle**](https://reference.aspose.com/cells/net/aspose.cells.utility/jsonlayoutoptions/properties/ignorearraytitle): Indicates whether to ignore the title if the property of the object is an array
- [**IgnoreNull**](https://reference.aspose.com/cells/net/aspose.cells.utility/jsonlayoutoptions/properties/ignorenull): Indicates whether the null value should be ignored or not.
- [**IgnoreObjectTitle**](https://reference.aspose.com/cells/net/aspose.cells.utility/jsonlayoutoptions/properties/ignoreobjecttitle): Indicates whether to ignore the title if the property of the object is an object.
- [**NumberFormat**](https://reference.aspose.com/cells/net/aspose.cells.utility/jsonlayoutoptions/properties/numberformat): Gets and sets the format of numeric value.
- [**TitleStyle**](https://reference.aspose.com/cells/net/aspose.cells.utility/jsonlayoutoptions/properties/titlestyle): Gets and sets the style of the title.

The sample code given below demonstrates the use of the [**JsonUtility**](https://reference.aspose.com/cells/net/aspose.cells.utility/jsonutility) and [**JsonLayoutOptions**](https://reference.aspose.com/cells/net/aspose.cells.utility/jsonlayoutoptions) classes to import JSON data.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-Handling-Importing-ImportingFromJson-1.cs" >}}

## **Advance topics**
- [Specify Formula Fields while Importing Data to Worksheet](/cells/net/specify-formula-fields-while-importing-data-to-worksheet/)
- [Shift First Row down when inserting Cells Data Table Rows](/cells/net/shift-first-row-down-when-inserting-cells-data-table-rows/)