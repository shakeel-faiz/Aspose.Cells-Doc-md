﻿---
title: Cómo arreglar java.lang.ClassNotFoundException
type: docs
weight: 30
url: /es/java/how-to-fix-java-lang-classnotfoundexception/ 
---
Aspose.Cells for Java API depende de algunas bibliotecas adicionales, si faltan, se puede generar una excepción como "java.lang.ClassNotFoundException".
Este artículo enumera este tipo de excepciones y explica qué bibliotecas se instalan para resolverlas.

## Cómo solucionar ClassNotFoundException: org.bouncycastle.jce.provider.BouncyCastleProvider
### **Resumen**
Aspose.Cells for Java API depende de Bouncy Castle para las funciones de cifrado y descifrado, es decir, si se requiere que el programa cargue o guarde hojas de cálculo cifradas, se requiere agregar la referencia de bcprov-jdk16-146.jar en la ruta de clase del proyecto.
### **Síntomas**
 Puede obtener la java.lang.ClassNotFoundException: org.bouncycastle.jce.provider.BouncyCastleProvider.
### **Solución**
La solución es realmente muy simple como se detalla a continuación.

1. Descargue cualquier versión importante de[Aspose.Cells for Java](https://downloads.aspose.com/cells/java).
1. Extraiga el archivo descargado y busque el directorio \JDK 1.6\aspose-cells-xx0-java\lib.
1. Haga referencia a bcprov-jdk16-146.jar en la ruta de clases del proyecto.

Alternativamente, puede agregar la dependencia en pom.xml y dejar que el proyecto resuelva la dependencia a través de maven.

{{< highlight "java" >}}

 <dependencies>

	<dependency>

		<groupId>org.bouncycastle</groupId>

		<artifactId>bcprov-jdk16</artifactId>

		<version>1.46</version>

		<type>jar</type>

	</dependency>

</dependencies>

{{< /highlight >}}

