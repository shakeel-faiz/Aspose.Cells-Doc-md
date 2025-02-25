---
title: Create and Format Table
type: docs
weight: 10
url: /cpp/create-and-format-table/
---

## **Create Table**
One of the advantages of spreadsheets is that they allow you to create different types of lists, for example, phone lists, task lists, lists of transactions, assets or liabilities. Several users can work together to use, create and maintain various lists.

Aspose.Cells supports creating and managing Lists.
### **Advantages of a List Object**
There are quite a few advantages when you convert a list of data to an actual List Object

- New rows and columns are automatically included.
- A total row at the bottom of your list can be easily added to display SUM, AVERAGE, COUNT, etc.
- Columns added to the right are automatically incorporated into the List object.
- Charts based on rows and columns will be expanded automatically.
- Named ranges assigned to rows and columns will be expanded automatically.
- The list is protected from accidental row and column deletion.
### **Creating a List Object using Microsoft Excel**

|**Selecting data range for creating List object**|
| :- |
|![todo:image_alt_text](jHcNq4o.png)|
This displays the Create List dialog.

|**Create List dialog**|
| :- |
|![todo:image_alt_text](kJmukRF.png)|
Implementing the List object for the data and specifying total row (Select **Data**, then **List**, followed by **Total Row**).

|**Creating a list object**|
| :- |
|![todo:image_alt_text](ECSGVdR.png)|
### **Using Aspose.Cells API**
Aspose.Cells provides a class [IWorkbook](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_workbook) that represents a Microsoft Excel file. The [IWorkbook](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_workbook) class contains an [IWorksheets](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection) collection that allows access to each worksheet in an Excel file.

A worksheet is represented by the [IWorksheet](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet) class. The [IWorksheet](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet) class provides a wide range of methods for managing a worksheet. To create an [IListObject](https://reference.aspose.com/cells/cpp/class/aspose.cells.tables.i_list_object) in a worksheet, use the [GetIListObjects](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet#a4356bc4b8cffee624891f10ea49a4705) collection method of the [IWorksheet](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet) class. Each `[IListObject]` is in fact, an object of the [IListObjectCollection](https://reference.aspose.com/cells/cpp/class/aspose.cells.tables.i_list_object_collection) class, which further provides the [Add](https://reference.aspose.com/cells/cpp/class/aspose.cells.tables.i_list_object_collection#ae4afda31b69b75a78558a65bef65ee42) method for adding an `[IListObject]` object and specifying a range of cells for the list.

According to the specified range of cells, the `[IListObject]` object is created by Aspose.Cells. Use attributes (for example [ShowTotals](https://reference.aspose.com/cells/cpp/class/aspose.cells.tables.i_list_object#a9026460927f035f374f5e1ea74e639f2) and [ListColumns](https://reference.aspose.com/cells/cpp/class/aspose.cells.tables.i_list_object#afeeb7bfabd0971e9fe34a09f0b83ae73) etc.) of the `[IListObject]` class to control the list.

In the example given below, we have created the same `[IListObject]` using Aspose.Cells API as we created using Microsoft Excel in the above section.



{{< gist "aspose-cells-gists" "6f7d9819d85793c3a3b5d040af42e1a9" "Examples-C-main-CreatingListObjects.cpp" >}}
## **Format a Table**
To manage and analyze a group of related data, it is possible to turn a range of cells into a list object (also known as an Excel table). A table is a series of rows and columns that contain related data managed independently from the data in other rows and columns. By default, every column in the table has filtering enabled in the header row so that you can filter or sort your list object data quickly. You can add a total row (a special row in a list that provides a selection of aggregate functions useful for working with numerical data) to the list object that provides a drop-down list of aggregate functions for each totals row cell. Aspose.Cells provides options for creating and managing lists (or tables).
### **Formatting a List Object**
Aspose.Cells provides a class [IWorkbook](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_workbook) that represents a Microsoft Excel file. The [IWorkbook](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_workbook) class contains an [IWorksheets](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection) collection that allows access to each worksheet in an Excel file.

A worksheet is represented by the [IWorksheet](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet) class. The [IWorksheet](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet) class provides a wide range of methods for managing worksheets. To create a *ListObject* in a worksheet, use `IListObjectCollection`. Each `[IListObject]` is in fact, an object of the `IListObjectCollection` class, which further provides the [Add](https://reference.aspose.com/cells/cpp/class/aspose.cells.tables.i_list_object_collection#ae4afda31b69b75a78558a65bef65ee42) method for adding an `[IListObject]` object and specify the range of cells it should encompass. According to the specified range of cells, a *ListObject* is created in the worksheet by Aspose.Cells. Use attributes (for example, [TableStyleType](https://reference.aspose.com/cells/cpp/class/aspose.cells.tables.i_list_object#a5de8b5321b0ccb30dfb09cefe6536462)) of the `[IListObject]` class to format the table for your requirements.

The example below adds sample data to a worksheet, adds an `[IListObject]` and applies default styles to it. `[IListObject]` styles are supported by Microsoft Excel 2007/2010.



{{< gist "aspose-cells-gists" "6f7d9819d85793c3a3b5d040af42e1a9" "Examples-C-main-FormatTable.cpp" >}}
