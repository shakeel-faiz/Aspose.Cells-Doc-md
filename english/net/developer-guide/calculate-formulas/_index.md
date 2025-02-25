﻿---
title: Calculate Formulas
type: docs
weight: 125
url: /net/calculate-formulas/
---

## **Adding Formulas & Calculating Results**

Aspose.Cells has an embedded formula calculation engine. Not only it can re-calculate formulas imported from designer templates but also it supports to calculate the results of formulas added at runtime.

Aspose.Cells supports most of the formulas or functions that are part of Microsoft Excel(Read [a list of the functions supported by the calculation engine](/cells/net/supported-formula-functions/)). Those functions can be used through the APIs or designer spreadsheets. Aspose.Cells supports a huge set of mathematical, string, boolean, date/time, statistical, database, lookup, and reference formulas.

Use the [**Formula**](https://reference.aspose.com/cells/net/aspose.cells/cell/properties/formula) property or [**SetFormula(...)**](https://reference.aspose.com/cells/net/aspose.cells.cell/setformula/methods/2) methods of the [**Cell**](https://reference.aspose.com/cells/net/aspose.cells/cell) class to add a formula to a cell. When applying a formula, always begin the string with an equal sign (=) as you do when creating a formula in Microsoft Excel and use a comma (,) to delimit function parameters.

To calculate the results of formulas, user may call the [**CalculateFormula**](https://reference.aspose.com/cells/net/aspose.cells.workbook/calculateformula/methods/1) method of the [**Workbook**](https://reference.aspose.com/cells/net/aspose.cells/workbook) class which processes all formulas embedded in an Excel file. Or, user may call the [**CalculateFormula**](https://reference.aspose.com/cells/net/aspose.cells/worksheet/methods/calculateformula) method of the [**Worsheet**](https://reference.aspose.com/cells/net/aspose.cells/worksheet) class which processes all formulas embedded in a sheet. Or, user also may call the [**Calculate**](https://reference.aspose.com/cells/net/aspose.cells/cell/methods/calculate) method of the [**Cell**](https://reference.aspose.com/cells/net/aspose.cells/cell) class which processes the  formula of one Cell:

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Formulas-CalculatingFormulas-1.cs" >}}

### **Important to Know**

{{% alert color="primary" %}}

The **Formula** property and **SetFormula(...)** methods of the [**Cell**](https://reference.aspose.com/cells/net/aspose.cells/cell) class work differently from the **Calculate** methods of the [**Workbook**](https://reference.aspose.com/cells/net/aspose.cells/workbook), [**Worksheet**](https://reference.aspose.com/cells/net/aspose.cells/worksheet) and [**Cell**](https://reference.aspose.com/cells/net/aspose.cells/cell) classes. The **Formula** property and **SetFormula(...)** methods simply add the formula to a cell but do not calculate the result at runtime. To get the result of the formulas, please call **Calculate** methods.

{{% /alert %}}

## **Direct Calculation of Formula**

Aspose.Cells has an embedded formula calculation engine. As well as calculating formulas imported from a designer file, Aspose.Cells can calculate formula results directly.

Sometimes, you need to calculate formula results directly without adding them into a worksheet. The values of the cells used in the formula already exist in a worksheet and all you need is to find the result of those values based on some Microsoft Excel formula without adding the formula in a worksheet.

You can use Aspose.Cells' formula calculation engine APIs for [**Worksheet**](https://reference.aspose.com/cells/net/aspose.cells/worksheet) to [**calculate**](https://reference.aspose.com/cells/net/aspose.cells.worksheet/calculateformula/methods/3) the results of such formulas without adding them to the worksheet:

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Formulas-DirectCalculationFormula-1.cs" >}}

Above code produces the following output:
{{< highlight net >}}
Value of A1: 20
Value of A2: 30
Result of Sum(A1:A2): 50.0
{{< /highlight >}}

## **Calculating Formulas repeatedly**

When there are lots of formulas in the workbook and user needs to calculate them repeatedly with modifying only a small part of them, it may be helpful for performance to enable the formula calculation chain: [**FormulaSettings.EnableCalculationChain**](https://reference.aspose.com/cells/net/aspose.cells/formulasettings/properties/enablecalculationchain).

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Formulas-CalculatingFormulasOnce-1.cs" >}}

### **Important to Know**

{{% alert color="primary" %}}

By default the calculation chain is disabled. Because creating the chain also needs extra time, the first time of calculating formulas([**Workbook.CalculateFormula(...)**](https://reference.aspose.com/cells/net/aspose.cells.workbook/calculateformula/methods/1)) may consume more CPU processing time and memory when comparing with calculating formulas without chain. If user does not need to calculate formulas repeatedly, the default behavior(calculating formula directly without creating calculation chain) should be the better way.

{{% /alert %}}


## **Advance topics**
- [Add Cells to Microsoft Excel Formula Watch Window](/cells/net/add-cells-to-microsoft-excel-formula-watch-window/)
- [Calculating IFNA function using Aspose.Cells](/cells/net/calculating-ifna-function-using-aspose-cells/)
- [Calculation of Array Formula of Data Tables](/cells/net/calculation-of-array-formula-of-data-tables/)
- [Calculation of Excel 2016 MINIFS and MAXIFS functions](/cells/net/calculation-of-excel-2016-minifs-and-maxifs-functions/)
- [Decrease the Calculation Time of Cell.Calculate method](/cells/net/decrease-the-calculation-time-of-cell-calculate-method/)
- [Detecting Circular Reference](/cells/net/detecting-circular-reference/)
- [Direct calculation of custom function without writing it in a worksheet](/cells/net/direct-calculation-of-custom-function-without-writing-it-in-a-worksheet/)
- [Implement Custom Calculation Engine to extend the Default Calculation Engine of Aspose.Cells](/cells/net/implement-custom-calculation-engine-to-extend-the-default-calculation-engine-of-aspose-cells/)
- [Interrupt or Cancel the Formula Calculation of Workbook](/cells/net/interrupt-or-cancel-the-formula-calculation-of-workbook/)
- [Returning a Range of Values using AbstractCalculationEngine](/cells/net/returning-a-range-of-values-using-abstractcalculationengine/)
- [Returning a Range of Values using ICustomFunction](/cells/net/returning-a-range-of-values-using-icustomfunction/)
- [Setting Formula Calculation Mode of Workbook](/cells/net/setting-formula-calculation-mode-of-workbook/)
- [Using FormulaText function in Aspose.Cells](/cells/net/using-formulatext-function-in-aspose-cells/)
- [Using ICustomFunction Feature](/cells/net/using-icustomfunction-feature/)
