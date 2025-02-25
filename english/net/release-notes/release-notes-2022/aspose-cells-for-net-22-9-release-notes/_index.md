---
title: Aspose.Cells for .NET 22.9 Release Notes
type: docs
weight: 4
url: /net/aspose-cells-for-net-22-9-release-notes/
---

{{% alert color="primary" %}}

This page contains release notes for [Aspose.Cells for .NET 22.9](https://www.nuget.org/packages/Aspose.Cells/22.9.0).

{{% /alert %}}

|**Key**|**Summary**|**Category**|
| :- | :- | :- |
|CELLSNET-51935|Support discrete group data for xls file|New Feature
|CELLSNET-51925|Support preset gradient settings for gradient fill|New Feature
|CELLSNET-51740|Support to set table formula for the datatable|Enhancement
|CELLSNET-51853|Support to convert ozm to lbm for CONVERT function|Enhancement
|CELLSNET-51931|Improve the recognization of user's input for Style.Custom to built-in|Enhancement
|CELLSNET-51709|Support multiple tables in a worksheet of .Numbers|Enhancement
|CELLSNET-51810|Support to export empty cells as null to Json|Enhancement
|CELLSNET-51811|Enhance the function of detecting whether the first row is header row|Enhancement
|CELLSNET-51910|Support to apply outline borders with ThemeColor to Range|Enhancement
|CELLSNET-51928|Support reading and writing protected range with SHA-512  algorithm of xlsb|Enhancement
|CELLSNET-51743|Some symbols changed after converting Excel file to PDF|Bug
|CELLSNET-51747|mm becomes "??" in pdf|Bug
|CELLSNET-50960|Re-saved XLSM file (containing a pivot table) got corrupted|Bug
|CELLSNET-51506|External connections are corrupted in genreated file|Bug
|CELLSNET-51735|Wrong text bold style on converting Excel pivot table to PDF|Bug
|CELLSNET-51761|When XLS file with Pivot table is converted to XLSM, the data connections details got deleted|Bug
|CELLSNET-51899|XLS to XLSM conversion - MS Excel could not open the the output XLSM file|Bug
|CELLSNET-51716|Dynamic array formula does not populate spilled cells  |Bug
|CELLSNET-51753|Some formulas are not calculated to update the data across the sheets upon changing selection|Bug
|CELLSNET-51800|Values from XLSX are incorrect in the output PDF|Bug
|CELLSNET-51801|Recalculation of a workbook is slow after calculating with calculation chain|Bug
|CELLSNET-51897|HLOOKUP value is incorrect|Bug
|CELLSNET-51187|Vertical dotted lines misaligned with labels on axis in chart to SVG rendering|Bug
|CELLSNET-51734|System.Security.Cryptography.Pkcs 6.0.1 dependency requires .NET Core 3.1|Bug
|CELLSNET-51912|When converting Excel To PDF, the resultant PDF does not show axis correctly|Bug
|CELLSNET-51744|Gridweb keeps jumping back|Bug
|CELLSNET-51608|Number is hidden behind red/green circle when exporting Excel to HTML on docker (Azure cloud kubernetes)|Bug
|CELLSNET-51864|Issue with calculating "PageSetup.Zoom" with HorizontalPageBreaks|Bug
|CELLSNET-51938|XLSX to PDF: Character spacing is wrong|Bug
|CELLSNET-51226|Add identifier attribute for chart/group in Excel Workbook|Bug
|CELLSNET-51461|Unnecessary borders are added for the data in Excel to DOCX conversion|Bug
|CELLSNET-51736|Cell borders got lost in the resultant PDF |Bug
|CELLSNET-51738|Invalid record for single cell caused generated file corrupted|Bug
|CELLSNET-51760|Worksheet.AutoFitColumns is not working right|Bug
|CELLSNET-51770|Merged Cells does not work fine when saving as PowerPoint file|Bug
|CELLSNET-51771|Afer cells are merged some data are lost in the generaed PowerPoint file|Bug
|CELLSNET-51772|Connection info is getting changed when converting XLS file to XLSM|Bug
|CELLSNET-51778|Converting an XLS file to XLSM is deleting few chars at the end of the link in named ranges|Bug
|CELLSNET-51785|DOCX >> Html table >> Excel sheet does not convert properly |Bug
|CELLSNET-51825|AutoFit worked differently in v22.1.0 and v22.8.0|Bug
|CELLSNET-51829|XLS to XLSM file conversion caused some custom properties lost|Bug
|CELLSNET-51830|Input document stream is prematurely disposed after creating Workbook for particular file|Bug
|CELLSNET-51865|XLS worksheet has no data while you can see filled rows in Excel|Bug
|CELLSNET-51880|XLSB to XLSM conversion - the output XLSM file is corrupted|Bug
|CELLSNET-51898|XLS to XLSM conversion - the output XLSM file is corrupted|Bug
|CELLSNET-51921|Cannot apply a copied style without setting its flags to explicit or using a flag|Bug
|CELLSNET-51922|Cell protection is lost after opening and re-saving the XLSX file|Bug
|CELLSNET-51923|DataTable Column Caption property is not honored and rendered in the output Excel when importing data|Bug
|CELLSNET-51924|Incorrect locale in chart text elements|Bug
|CELLSNET-51944|The name of built-in styles does not automaitcally change according to region|Bug
|CELLSNET-51848|Calculating workbook throws Stackoverflow exception|Exception
|CELLSNET-51965|Exception when importing an XLSX file with Accounting formatting into Aspose.Cells.GridDesktop|Exception
|CELLSNET-51961|Exception "Index was out of range" when rendering an ODS to PDF|Exception
|CELLSNET-51863|System.StackOverflowException in CollectionBase.Exists|Exception

## **Public API and Backwards Incompatible Changes**

The following is a list of any changes made to the public API such as added, renamed, removed or deprecated members as well as any non-backward compatible change made to Aspose.Cells for .NET. If you have concerns about any change listed, please raise it on the Aspose.Cells support forum.

### **Adds Cell.SetTableFormula(...) methods**

Support to set formulas for range of cells to create two-variable data table and one-variable data table.

### **Adds Cell.SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, object[][] values, bool calculateRange, bool calculateValue, CalculationOptions copts) method**

Support to set dynamic array formula with custom options for calculation, especially when there are functions which need user's custom engine for calculation in the formula.

### **Adds Workbook.RefreshDynamicArrayFormulas(bool calculate, CalculationOptions copts) method**

Support to refresh dynamic array formulas with custom options for calculation, especially when there are functions which need user's custom engine for calculation functions in the dynamic array formulas.

### **Adds ChartFrame.TextOptions property.**

Represents the font options of the chart's text.

### **Adds ExportRangeToJsonOptions.ExportEmptyCells property.**

Indicates whether exporting null if the cells are empty.

### **Add NumbersLoadOptions constructor.**

Represents the options of loading numbers.

### **Adds enum LoadNumbersTableType.**

Represnts the type of loading multi tables in a worksheet of the Mac .numbers.

### **Adds ProtectedRange.IsProtectedWithPassword property.**

Inidicates whether the range is protected with password.

### **Adds ImportTableOptions.ExportCaptionAsFieldName properties**

Indicates whether exporting caption as field name when importing data table.

### **Adds TextOptions.LanguageCode property.**

Gets and sets the language code of the font.

### **Adds enum PresetThemeGradientType.**

Represents the preset theme gradient type.

### **Adds GradientFill.SetPresetThemeGradient() method.**

Sets the preset theme gradient type.

### **Adds override Style.SetBorder() methods.**

Sets the borders with various kinds of color.

### **Adds Range.SetOutlineBorder() and Range.SetOutlineBorders() methods**

Sets the borders of the range with various kinds of color.
