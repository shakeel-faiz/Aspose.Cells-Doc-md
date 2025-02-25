﻿---
title: Convertir libro de Excel a PDF
type: docs
weight: 80
url: /es/cpp/convert-excel-workbook-to-pdf/
---
## **Conversión de libro de Excel a PDF**
Los archivos PDF se utilizan ampliamente para intercambiar documentos entre organizaciones, sectores gubernamentales e individuos. Es un formato de documento estándar y a menudo se les pide a los desarrolladores de software que encuentren una forma de convertir archivos Excel Microsoft en documentos PDF.

Aspose.Cells admite la conversión de archivos de Excel a PDF y mantiene una alta fidelidad visual en la conversión.

{{% alert color="primary" %}} 

 Aspose.Cells escribe directamente la información sobre API y el número de versión en los documentos de salida. Por ejemplo, al representar el Documento en PDF, Aspose.Cells for C++ rellena el**Solicitud** campo con valor 'Aspose.Cells' y**PDF Productor** campo con valor, por ejemplo, 'Aspose.Cells v18.5.0'.

Tenga en cuenta que no puede indicar al Aspose.Cells for C++ que cambie o elimine esta información de los documentos de salida.

{{% /alert %}} 
### **Conversión Directa**
Aspose.Cells admite la conversión de hojas de cálculo a PDF independientemente de otro software. Simplemente guarde un archivo de Excel en PDF usando el[ILibro de trabajo](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_workbook)clase'[Ahorrar](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349)método. Él[Ahorrar](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349)método proporciona la[GuardarFormato_Pdf](https://reference.aspose.com/cells/cpp/namespace/aspose.cells#a11cae527e4e68f1adcac8f47ea64481a)miembro de enumeración que convierte los archivos nativos de Excel al formato PDF.

Siga los pasos a continuación para convertir directamente las hojas de cálculo de Excel al formato PDF:

1.  Instanciar un objeto de la[ILibro de trabajo](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_workbook)clase llamando a su constructor vacío.
1. Puede abrir/cargar un archivo de plantilla existente u omitir este paso si está creando el libro de trabajo desde cero.
1. Realice cualquier trabajo (ingresar datos, aplicar formato, establecer fórmulas, insertar imágenes u otros objetos de dibujo, etc.) en la hoja de cálculo utilizando las API Aspose.Cells.
1.  Cuando el código de la hoja de cálculo esté completo, llame al[ILibro de trabajo](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_workbook)clase'[Ahorrar](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349)método para guardar la hoja de cálculo.

El formato de archivo debe ser PDF, así que seleccione PDF relevante (un valor predefinido) de la enumeración SaveFormat para generar el documento final PDF

 Consulte el siguiente código de ejemplo, su[ejemplo de archivo de Excel](67338368.xlsx) y[salida PDF](67338369.pdf) para tu referencia.

{{< gist "aspose-cells-gists" "6f7d9819d85793c3a3b5d040af42e1a9" "LoadingSavingAndConverting-ConvertExcelWorkbookToPDF_DirectConversion.cpp" >}}
### **Conversión avanzada**
También puede optar por utilizar el[IPdfSaveOptions](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_pdf_save_options)class para establecer diferentes atributos para la conversión. Configuración de diferentes propiedades del**IPdfSaveOptions** class le da control sobre la configuración de impresión, fuente, seguridad y compresión para la salida PDF. La propiedad más importante es[Establecer Cumplimiento](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_pdf_save_options#a2158ff23d7c071f8224b1cd063233c07)que le permite guardar los archivos de Excel en archivos compatibles con PDF/A PDF.
#### **Guardar libro de trabajo en PDF/A Archivos cumplidos**
El siguiente fragmento de código demuestra cómo usar el**IPdfSaveOptions**clase para guardar archivos de Excel en formato PDF/A compatible con PDF

 Consulte el siguiente código de ejemplo y su[salida PDF](67338370.pdf) para tu referencia.

{{< gist "aspose-cells-gists" "6f7d9819d85793c3a3b5d040af42e1a9" "LoadingSavingAndConverting-ConvertExcelWorkbookToPDF_A_CompliedFiles.cpp" >}}
#### **Establecer la hora de creación PDF**
Con el**IPdfSaveOptions** clase, puede obtener o establecer la hora de creación PDF.

 Consulte el siguiente código de ejemplo y su[salida PDF](67338371.pdf) para tu referencia.

{{< gist "aspose-cells-gists" "6f7d9819d85793c3a3b5d040af42e1a9" "LoadingSavingAndConverting-ConvertExcelWorkbookToPDF_SetPDFCreationTime.cpp" >}}
