﻿---
title: نسخ أوراق العمل ونقلها في جايثون
type: docs
weight: 20
url: /ar/java/copying-and-moving-worksheets-in-jython/
---
## **Aspose.Cells - نسخ ونقل أوراق العمل**
 لإلحاق المستندات باستخدام**Aspose.Cells Java لـ Jython**. هنا يمكنك أن ترى رمز المثال.

**كود جايثون**

{{< highlight "java" >}}

 from aspose-cells import Settings

from com.aspose.cells import Workbook

from com.aspose.cells import SaveFormat


class CopyingAndMovingWorksheets:

    def __init__(self):

        # Copy Worksheets within a Workbook

        self.copy_worksheet()

        # Move Worksheets within Workbook

        self.move_worksheet()



    def copy_worksheet(dataDir):  



        dataDir = Settings.dataDir + 'WorkingWithWorksheets/CopyingAndMovingWorksheets/'



         # Instantiating a Workbook object by excel file path

        workbook = Workbook(dataDir + "Book1.xls")



        # Create a Worksheets object with reference to the sheets of the Workbook.

        sheets = workbook.getWorksheets()

        # Copy data to a new sheet from an existing sheet within the Workbook.

        sheets.addCopy("Sheet1")

        # Saving the modified Excel file in default (that is Excel 2003) format

        workbook.save(dataDir + "Copy Worksheet.xls")

        print "Copy worksheet, please check the output file."



    def move_worksheet(dataDir):



        dataDir = Settings.dataDir + 'WorkingWithWorksheets/CopyingAndMovingWorksheets/'



         # Instantiating a Workbook object by excel file path

        workbook = Workbook(dataDir + "Book1.xls")



        # Get the first worksheet in the book.

        sheet = workbook.getWorksheets().get(0)

        # Move the first sheet to the third position in the workbook.

        sheet.moveTo(2)

        # Saving the modified Excel file in default (that is Excel 2003) format

        workbook.save(dataDir + "Move Worksheet.xls")

        print "Move worksheet, please check the output file."



if __name__ == '__main__':        

    CopyingAndMovingWorksheets()

{{< /highlight >}}
## **قم بتنزيل كود التشغيل**
 تحميل**إرفاق المستندات (Aspose.Cells)** من أي من الترميز الاجتماعي المذكور أدناه

- [جيثب](https://github.com/aspose-cells/Aspose.Cells-for-Java/blob/master/Plugins/Aspose-Cells-Java-for-Jython/asposecells/WorkingWithWorksheets/CopyingAndMovingWorksheets.py)
