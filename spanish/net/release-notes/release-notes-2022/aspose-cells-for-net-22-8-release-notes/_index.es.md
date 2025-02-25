﻿---
title: Aspose.Cells for .NET 22.8 Notas de la versión
type: docs
weight: 5
url: /es/net/aspose-cells-for-net-22-8-release-notes/
---
{{% alert color="primary" %}}

 Esta página contiene notas de la versión para[Aspose.Cells for .NET 22.8](https://www.nuget.org/packages/Aspose.Cells/22.8.0).

{{% /alert %}}

|**Llave**|**Resumen**|**Categoría**|
|:- |:- |:- |
|CELLSNET-51589|Admite el estilo de botón expandir/contraer para tabla dinámica|
|CELLSNET-51473|Convertir comentarios encadenados a html|
|CELLSNET-51570|Copie la altura de la fila al procesar marcadores inteligentes de una tabla|
|CELLSNET-51590|Eliminar formas agrupadas del grupo|
|CELLSNET-51595|Alineación vertical incorrecta del texto de la celda al convertir a PDF desde un archivo de Excel con tabla dinámica|
|CELLSNET-51621|Las fórmulas compartidas se copiaron incorrectamente para diferentes formatos de archivo|
|CELLSNET-51524|Ajuste de palabra incorrecto al convertir a PDF desde un archivo de Excel con tabla dinámica|
|CELLSNET-51675|La forma se pierde al convertir a pdf|
|CELLSNET-51435|Se agregan nuevas relaciones de hoja de trabajo al convertir un libro de trabajo XLSB a XLSM|
|CELLSNET-51545|El libro de trabajo con hojas de diálogo de MS Excel 5.0 no se pudo cargar antes de Aspose.Cells|
|CELLSNET-51546|Los gráficos se duplican después de abrirlos y guardarlos con las celdas Aspose y luego verlos en Excel|
|CELLSNET-51550|Los enlaces en rangos con nombre se eliminan en la conversión XLS a XLSM|
|CELLSNET-51551|Los archivos se corrompieron y el enlace externo cambió a enlace DDE al convertir archivos XLS a XLSM|
|CELLSNET-51558|La conversión de archivos XLS con enlace de tipo xlAlternateStartup a XLSM genera archivos dañados|
|CELLSNET-51564|Datos duplicados del marcador inteligente|
|CELLSNET-51574|Un cuadro de texto que tiene dos columnas se representa con una sola columna cuando se vuelve a guardar un archivo XLSX|
|CELLSNET-51580|Un enlace externo de tipo xlPathMissing se cambia al tipo externalLinkPath normal en la conversión XLS a XLSM|
|CELLSNET-51599|Nombres muy largos para recursos de tipo de imagen mientras se guardan como Html|
|CELLSNET-51627|No se puede cargar el archivo XLSM específico|
|CELLSNET-51632|RibbonXml no funciona|
|CELLSNET-51696|Convertir XLS a XLSM está cambiando la propiedad de definición de conexión de datos "Guardar contraseña"|
|CELLSNET-51559|Convertir un archivo XLSB a XLSM arrojando la excepción "startIndex no puede ser mayor que la longitud de la cadena"|

## **Public API y cambios incompatibles con versiones anteriores**

La siguiente es una lista de los cambios realizados al público API, como miembros agregados, renombrados, eliminados o obsoletos, así como cualquier cambio no compatible con versiones anteriores realizado en Aspose.Cells for .NET. Si tiene inquietudes sobre cualquier cambio enumerado, plantéelo en el foro de soporte Aspose.Cells.

### **Agregue el método FontSettingCollection.Replace().**

Reemplace el texto de la forma.

### **Agregue la propiedad ShapeTextAlignment.NumberOfColumns.**

Obtiene y establece el número de columnas del texto de la forma.

### **Agregue la propiedad HtmlSaveOptions.ExportCommentsType.**

Obtiene y establece el tipo de comentarios de exportación a html.

### **Agregue la clase base PaginatedSaveOptions para PdfSaveOptions y XpsSaveOptions.**

Representa las opciones de paginación.

### **Agregue la clase SheetSet.**

Describe un juego de hojas.

### **Agregue la propiedad PaginatedSaveOptions.SheetSet.**

Obtiene o establece las hojas para representar.

### **Agregue la propiedad ImageOrPrintOptions.SheetSet.**

Obtiene o establece las hojas para representar.

### **Agregue la propiedad GridWeb.IgnoreStyleWithNoData.**

Obtiene o establece si GridWeb ignora mostrar filas o columnas que no contienen valores de celda pero aún tienen estilo

### **Propiedad ImageOrPrintOptions.SaveFormat obsoleta.**

Para Tiff/Svg, utilice ImageType; Para Xps, utilice Workbook.Save(string, SaveOptions) con XpsSaveOptions.

### **Constructor obsoleto XpsSaveOptions(Aspose.Cells.SaveFormat saveFormat).**

Utilice el constructor XpsSaveOptions() en su lugar.

### **Constructor obsoleto SvgSaveOptions(Aspose.Cells.SaveFormat saveFormat).**

Utilice el constructor SvgSaveOptions() en su lugar.

### **Quite el constructor PdfSaveOptions(Aspose.Cells.SaveFormat saveFormat).**

Utilice el constructor PdfSaveOptions() en su lugar.
