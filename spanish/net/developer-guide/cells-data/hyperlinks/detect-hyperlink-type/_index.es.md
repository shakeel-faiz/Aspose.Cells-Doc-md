﻿---
title: Detectar tipo de hipervínculo
type: docs
weight: 160
url: /es/net/detect-hyperlink-type/
---
## **Detectar tipo de hipervínculo**

 Un archivo de Excel puede tener diferentes tipos de hipervínculos como externo, referencia de celda, ruta de archivo, etc. Aspose.Cells admite la función para detectar el tipo de hipervínculo. Los tipos de hipervínculos están representados por el[**TargetModeType**](https://reference.aspose.com/cells/net/aspose.cells/targetmodetype)Enumeración. Él[**TargetModeType**](https://reference.aspose.com/cells/net/aspose.cells/targetmodetype)La enumeración tiene los siguientes miembros.

- Externo: Enlace externo
- FilePath: Ruta local y completa a archivos\carpetas.
- Correo electrónico: Correo electrónico
- CellReference: enlace a la celda o rango con nombre.

Para comprobar el tipo de hipervínculo, el[**Hipervínculo**](https://reference.aspose.com/cells/net/aspose.cells/hyperlink) la clase proporciona un[**Tipo de enlace**](https://reference.aspose.com/cells/net/aspose.cells/hyperlink/properties/linktype) propiedad con un tipo de retorno de[**TargetModeType**](https://reference.aspose.com/cells/net/aspose.cells/targetmodetype). El siguiente fragmento de código demuestra el uso de la[**Tipo de enlace**](https://reference.aspose.com/cells/net/aspose.cells/hyperlink/properties/linktype)propiedad usando este[archivo fuente excel](94896195.xlsx).

### Código fuente

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Workbook-DetectLinkTypes-1.cs" >}}

El siguiente es el resultado generado por el fragmento de código dado anteriormente.

### Salida de consola
```
LinkTypes.xlsx: FilePath </br>
C:\Windows\System32\cmd.exe: FilePath </br>
C:\Program Files\Common Files: FilePath </br>
'Test Sheet'!B2: CellReference </br>
FullPathExample: CellReference </br>
https://products.aspose.com/cells/ : External </br>
mailto:test@test.com?subject=TestLink: Email </br>
```
