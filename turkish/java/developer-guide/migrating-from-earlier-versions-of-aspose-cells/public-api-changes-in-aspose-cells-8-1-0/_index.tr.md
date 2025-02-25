﻿---
title: Genel API Aspose.Cells 8.1.0'daki değişiklikler
type: docs
weight: 50
url: /tr/java/public-api-changes-in-aspose-cells-8-1-0/
---
{{% alert color="primary" %}} 

Bu belge, Aspose.Cells API sürüm 8.0.2'den 8.1.0'a modül/uygulama geliştiricilerin ilgisini çekebilecek değişiklikleri açıklamaktadır. Yalnızca yeni ve güncellenmiş genel yöntemleri değil, aynı zamanda Aspose.Cells'deki perde arkasındaki davranışlardaki değişikliklerin açıklamasını da içerir.

{{% /alert %}} 
## **HtmlSaveOptions.ExportHiddenWorksheet Özelliği Eklendi**
HtmlSaveOptions sınıfı, gizli çalışma sayfalarının HTML biçiminde dışa aktarılıp aktarılmadığını belirtmek için kullanılabilecek ExportHiddenWorksheet özelliğine sahiptir. Varsayılan değer doğrudur. yanlış olarak ayarlanırsa Aspose.Cells, gizli çalışma sayfası içeriğini dışa aktarmaz.

{{% alert color="primary" %}} 

 Lütfen adresindeki ayrıntılı makaleyi kontrol edin.[Gizli Çalışma Sayfasını Dışa Aktarmayı Önle](/cells/tr/java/prevent-exporting-hidden-worksheet-contents-on-saving-to/)

{{% /alert %}}
## **Cell.StringValueWithoutFormat Özelliği eklendi**
 Cell Sınıfına StringValueWithoutFormat özelliği eklenerek geliştiricilerin herhangi bir biçimlendirme uygulamadan hücre değerini almalarını kolaylaştırılmıştır.

Aşağıda verilen kod parçacığı, sıfırdan bir elektronik tablo oluşturarak ve hücrelerden birine sayı biçimi uygulayarak cell.getDisplayStringValue ile karşılaştırıldığında Cell.getStringValueWithoutFormat yönteminin kullanımını göstermektedir.

**Java**

{{< highlight "csharp" >}}

 //Create an instance of Workbook

Workbook book = new Workbook();

//Access first worksheet

Worksheet sheet = book.getWorksheets().get(0);

//Access A1 cell

Cell cell = sheet.getCells().get("A1");

//Put a value cell and convert it to number

cell.putValue("123456", true);

//Create a new Style object and add it to Workbook's Style Collection

int index = book.getStyles().add();

Style style = book.getStyles().get(index);

//Set Number format for Style object

style.setNumber(3);

//Create an instance of StyleFlag class

//and set NumberFormat to true

StyleFlag flag = new StyleFlag();

flag.setNumberFormat(true);

//Set the style of A1 cell

cell.setStyle(style, flag);

//Get formatted string value 

String formatted = cell.getDisplayStringValue();

System.out.println("Formatted String Value: " +formatted);

//Get un-formatted string value

String unformatted = cell.getStringValueWithoutFormat();

System.out.println("Un-formatted String Value: " + unformatted);

{{< /highlight >}}

{{% alert color="primary" %}} 

Yukarıdaki kodun çıktısı aşağıdaki gibidir

Biçimlendirilmiş Dize Değeri: 123.456
Biçimlendirilmemiş Dize Değeri: 123456

{{% /alert %}}
## **Eski Baytlar, Karakterler, CharactersWithSpaces, Satırlar, Paragraflar Özellikleri**
 Aspose.Cells for .NET 8.1.0'dan başlayarak BuiltInDocumentPropertyCollection sınıfındaki birçok özellik geçersiz olarak işaretlendi. Bu özellikler arasında Bytes, Characters, CharactersWithSpaces, Lines & Paragraphs bulunur. Nedeni, yukarıda belirtilen özelliklerin Excel elektronik tablolarının korunmasında hiçbir faydası yoktur çünkü Excel bunları atlar. Bu özellikler orijinal olarak Word belgeleri ve PowerPoint sunumları için yazılmıştır.
