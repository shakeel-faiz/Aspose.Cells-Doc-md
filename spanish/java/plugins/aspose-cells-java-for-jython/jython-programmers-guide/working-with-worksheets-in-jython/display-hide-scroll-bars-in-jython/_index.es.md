﻿---
title: Mostrar ocultar barras de desplazamiento en Jython
type: docs
weight: 40
url: /es/java/display-hide-scroll-bars-in-jython/
---
## **Aspose.Cells - Mostrar ocultar barras de desplazamiento**
 Para anexar documentos usando**Aspose.Cells Java para Jython**. Aquí puedes ver el código de ejemplo.

**Código Jython**

{{< highlight "java" >}}

 from aspose-cells import Settings

from com.aspose.cells import Workbook


class DisplayHideScrollBars:

    def __init__(self):

        dataDir = Settings.dataDir + 'WorkingWithWorksheets/DisplayHideScrollBars/'



        workbook = Workbook(dataDir + "Book1.xls")



        #Hiding the vertical scroll bar of the Excel file

        workbook.getSettings().setVScrollBarVisible(False)

        #Hiding the horizontal scroll bar of the Excel file

        workbook.getSettings().setHScrollBarVisible(False)

        #Saving the modified Excel file in default (that is Excel 2003) format

        workbook.save(dataDir + "output.xls")

        # Print message

        print "Scroll bars are now hidden, please check the output document."



if __name__ == '__main__':        

    DisplayHideScrollBars()

{{< /highlight >}}
## **Descargar código de ejecución**
 Descargar**Adjuntar Documentos (Aspose.Cells)**de cualquiera de los sitios de codificación social mencionados a continuación:

- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-Java/blob/master/Plugins/Aspose-Cells-Java-for-Jython/asposecells/WorkingWithWorksheets/DisplayHideScrollBars.py)
