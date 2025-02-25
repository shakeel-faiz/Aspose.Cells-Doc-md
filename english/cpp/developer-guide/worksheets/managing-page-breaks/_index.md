---
title: Managing Page Breaks
type: docs
weight: 30
url: /cpp/managing-page-breaks/
---

{{% alert color="primary" %}} 

According to the definition, a page break is a place in a flow of text where one page ends and the next begins. Microsoft Excel lets users add page breaks into any selected cell of a worksheet.

The location of the cell where the page break is added, the page is ended and all rest of the data after the page break is printed on the next page while printing. In simple words, page breaks divide your worksheet into multiple pages according to your specifications. You can also add page breaks to your worksheets at runtime using Aspose.Cells. Aspose.Cells allows developers to add two kinds of page breaks:

- Horizontal page break
- Vertical page break

In the rest of the discussion, we will describe how can you add horizontal or vertical page breaks into your worksheets using Aspose.Cells.

{{% /alert %}} 
## **Page Breaks**
Aspose.Cells provides a class [IWorkbook](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_workbook) that represents an Excel file. The [IWorkbook](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_workbook) class contains a [Worksheets](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection) collection that allows access to each worksheet in the Excel file.

A worksheet is represented by the [IWorksheet](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet) class. The [IWorksheet](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet) class provides a wide range of methods used to manage a worksheet. To add the page breaks, use the [AddPageBreaks](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet#a5f8dd5624b81e0ee2e7455f2b83380f6) method of the [IWorksheet](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet) class.
### **Adding Page Breaks**
{{< gist "aspose-cells-gists" "6f7d9819d85793c3a3b5d040af42e1a9" "Examples-CellsCPP-Worksheets-ManagingPageBreaks-AddingPageBreaks.cpp" >}}
