---
title: Change the decimal separator from Numeric keypad
type: docs
weight: 150
url: /net/change-the-decimal-separator-from-numeric-keypad/
---

## **Possible Usage Scenarios**
By default, Aspose.Cells.GridWeb displays numeric data accordingly based on the locale/regional settings on the machine. You can change the decimal separator from Numeric keypad programmatically using Aspose.Cells.GridWeb API. So, when a file is imported into GridWeb matrix or you input some numeric data (from the numeric keypad) into a new worksheet cell, it should have your desired decimal separator set visually. 
## **Change the decimal separator from Numeric keypad**
Using the **GridWorksheetCollection.NumberDecimalSeparator** property, you may change the decimal separator from Numeric keypad programmatically. Please see the screenshots that show how it works

![todo:image_alt_text](change-the-decimal-separator-from-numeric-keypad_1.png)

![todo:image_alt_text](change-the-decimal-separator-from-numeric-keypad_2.png)
## **Sample Code**
{{< gist "aspose-cells-gists" "7c644a93d33d24299a618c1dda1a2385" "Worksheets-ChangeDecimalSeparatorFromNumericKeypad.aspx.cs" >}}

{{% alert color="primary" %}} 

Please note, decimal separator change is only for users' visual experience in GridWeb. When you edit and save your workbook, it will still store the numeric values (in the spreadsheet) as per your locale/regional decimal separator.

{{% /alert %}}
