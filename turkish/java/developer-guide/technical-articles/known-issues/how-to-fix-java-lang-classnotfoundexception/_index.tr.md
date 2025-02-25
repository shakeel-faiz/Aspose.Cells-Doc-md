﻿---
title: Java.lang.ClassNotFoundException nasıl düzeltilir?
type: docs
weight: 30
url: /tr/java/how-to-fix-java-lang-classnotfoundexception/ 
---
Aspose.Cells for Java API bazı ek kütüphanelere bağlıdır, eğer eksiklerse "java.lang.ClassNotFoundException" olarak bir istisna atılabilir.
Bu makale, bu tür istisnaları listeler ve bunları çözmek için hangi kitaplıkların kurulu olduğunu açıklar.

## ClassNotFoundException nasıl düzeltilir: org.bouncycastle.jce.provider.BouncyCastleProvider
### **Özet**
Aspose.Cells for Java API, şifreleme ve şifre çözme özellikleri için Bouncy Castle'a bağlıdır, yani programın şifreli elektronik tabloları yüklemesi veya kaydetmesi gerekiyorsa, projenin sınıf yoluna bcprov-jdk16-146.jar referansını eklemesi gerekir.
### **belirtiler**
 Java.lang.ClassNotFoundException'ı alabilirsiniz: org.bouncycastle.jce.provider.BouncyCastleProvider.
### **Çözüm**
Çözüm aslında aşağıda detaylandırıldığı gibi çok basit.

1. herhangi bir büyük sürümünü indirin[Aspose.Cells for Java](https://downloads.aspose.com/cells/java).
1. İndirilen arşivi çıkartın ve \JDK 1.6\aspose-cells-xx0-java\lib dizinine gidin.
1. Projenin sınıf yolunda bcprov-jdk16-146.jar dosyasına başvurun.

Alternatif olarak, bağımlılığı pom.xml dosyasına ekleyebilir ve projenin bağımlılığı maven aracılığıyla çözmesine izin verebilirsiniz.

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

