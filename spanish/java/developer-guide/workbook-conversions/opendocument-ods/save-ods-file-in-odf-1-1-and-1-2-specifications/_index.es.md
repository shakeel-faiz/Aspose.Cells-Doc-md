﻿---
title: Guarde el archivo ODS en ODF 1.1 y 1.2 Especificaciones
type: docs
weight: 170
url: /es/java/save-ods-file-in-odf-1-1-and-1-2-specifications/
---
{{% alert color="primary" %}}

Aspose.Cells admite ahorro (**Hoja de cálculo de OpenDocument**) ODS archivo en (**Formato de documento abierto** ) Especificaciones ODF 1.1 y ODF 1.2. Aspose.Cells ha añadido[**OdsSaveOptions.setStrictSchema11()**](https://reference.aspose.com/cells/java/com.aspose.cells/odssaveoptions#IsStrictSchema11) propiedad para usar la especificación ODF 1.1 para guardar archivos ODS. El valor predeterminado de esta propiedad es**falso**por lo que el archivo ODS guardado sin esta configuración especial utilizará la especificación 1.2.

{{% /alert %}}

El código de muestra a continuación crea el objeto del libro de trabajo, agrega algún valor en la celda A1 de la primera hoja de trabajo y luego guarda el archivo ODS en las especificaciones ODF 1.1 y 1.2. De forma predeterminada, el archivo ODS se guarda en la especificación ODF 1.2.

{{< gist "aspose-cells-gists" "5876dc77e47649b66bdb5deefb4b5639" "Examples-src-main-java-com-aspose-cells-examples-articles-SaveODSfile-SaveODSfile.java" >}}
