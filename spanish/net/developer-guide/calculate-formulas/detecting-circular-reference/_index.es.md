﻿---
title: Detección de referencia circular
type: docs
weight: 70
url: /es/net/detecting-circular-reference/
---
## **Introducción**

Los libros de trabajo pueden tener referencias circulares y, a veces, es necesario detectar si hay referencias circulares o no.

## **Concepto detrás de la detección de la referencia circular**

Las referencias circulares solo se pueden detectar cuando se calcula la fórmula porque las referencias de una fórmula comúnmente dependen del resultado calculado de otras partes u otras fórmulas. Por lo tanto, proporcionamos nuevas API para este requisito (para recopilar celdas con referencias circulares) en el proceso de cálculo de fórmulas:

[**CalculationCell**](https://reference.aspose.com/cells/net/aspose.cells/calculationcell): Representa el cálculo de datos relevantes sobre una celda que se está calculando

[**AbstractCalculationMonitor.OnCircular(IEnumerator circularCellsData)**](https://reference.aspose.com/cells/net/aspose.cells/abstractcalculationmonitor/methods/oncircular): será invocado por el motor de cálculo de fórmulas cuando encuentre referencias circulares, el elemento en el enumerador es[**CalculationCell**](https://reference.aspose.com/cells/net/aspose.cells/calculationcell) objetos que representan todas las celdas en un círculo. El valor devuelto indica si el motor de fórmulas necesita calcular esas celdas en circular después de esta llamada.

 El usuario podrá recoger dichas referencias circulares en la ejecución de[**AbstractCalculationMonitor.OnCircular()**](https://reference.aspose.com/cells/net/aspose.cells/abstractcalculationmonitor/methods/oncircular) método.

El archivo de muestra de origen se puede descargar desde el siguiente enlace:

[Fórmulas circulares.xls](77496332.xls)

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Formulas-DetectCircularReference-1.cs" >}}

Definicion de*Monitor circular* clase que se deriva de[**ResumenCálculoMonitor**](https://reference.aspose.com/cells/net/aspose.cells/abstractcalculationmonitor) clase es la siguiente:

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Formulas-DetectCircularReference-2.cs" >}}
