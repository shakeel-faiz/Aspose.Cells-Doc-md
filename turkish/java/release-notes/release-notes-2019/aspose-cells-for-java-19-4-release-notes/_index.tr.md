﻿---
title: Aspose.Cells for Java 19.4 Sürüm Notları
type: docs
weight: 90
url: /tr/java/aspose-cells-for-java-19-4-release-notes/
---
{{% alert color="primary" %}} 

Bu sayfa Aspose.Cells for Java 19.4 için sürüm notları içerir.

{{% /alert %}} 

|**Anahtar**|**Özet**|**Kategori**|
|:- |:- |:- |
|CELLSJAVA-42838|Otomatik göster görev bölmesi özelliği devre dışı bırakılıyor.|Yeni özellik|
|CELLSJAVA-42853|XLSX'i HTML'e dönüştürürken performans sorunu|Artırma|
|CELLSJAVA-42852|Her iki eksendeki etiket gösterilmiyor|Böcek|
|CELLSJAVA-42856|Excel'den HTML'e dönüştürme sorunu|Böcek|
|CELLSJAVA-42872|Sayfanın resmi, sağ ve alt satırlar eksik|Böcek|
|CELLSJAVA-42873|Önceden hazırlanmış Sayfada birkaç hücre arka planı ve metin eksik ve gizli.|Böcek|
|CELLSJAVA-42874|Dosyayı HTML'e aktarırken sütun kaybı|Böcek|
|CELLSJAVA-42875|Genişlik yanlış ve ekran şekilsiz|Böcek|
|CELLSJAVA-42878|Formül hesaplama sonucu doğru değil|Böcek|
|CELLSJAVA-40419|Excel'den PDF'e dışa aktarırken etiketli PDF oluşturulamıyor|Böcek|
|CELLSJAVA-40570|Farklı boyutlardaki sayfalar için PDF ve JPG'ye yanlış dönüştürme|Böcek|
|CELLSJAVA-42833|Aynı PDF dosyasını bir çalışma kitabındaki birden çok sayfaya eklerken sorun|Böcek|
|CELLSJAVA-42858|Picture:FitToCell seçeneğiyle akıllı işaretçileri kullanarak birleştirilmiş hücrelere görüntü eklerken sorun|Böcek|
|CELLSJAVA-42862|CSV içe aktarma işleminden sonra formüllerde sayfa adı yeniden adlandırılıyor|Böcek|
|CELLSJAVA-42865|ODS dosyasındaki bir hücreden yanlış zaman okundu|Böcek|
|CELLSJAVA-42879|Excel dosyası Aspose.Cells tarafından kaydedildikten sonra bozuluyor|Böcek|
|CELLSJAVA-42860|ODS dosya biçimini yüklerken java.lang.NullPointerException|İstisna|
|CELLSJAVA-42871|java.lang.Exception: XLSX'i PDF'e dönüştürürken yedeklenen akış için desteklenmeyen klon|İstisna|

## **Herkese Açık API ve Geriye Dönük Uyumsuz Değişiklikler**
Aşağıda, API numaralı telefon numarasına eklenen, yeniden adlandırılan, kaldırılan veya kullanımdan kaldırılan üyeler gibi genele açık olarak yapılan tüm değişikliklerin ve Aspose.Cells for Java numaralı telefona yapılan geriye dönük uyumlu olmayan değişikliklerin bir listesi bulunmaktadır. Listelenen herhangi bir değişiklikle ilgili endişeleriniz varsa lütfen şu adrese bildirin: Aspose.Cells destek forumu.
### **Markdown belgesini kaydetmek için API'ler ekler: SaveFormat.Markdown, FileFormatType.Markdown, MarkdownSaveOptions**
Hücre içeriğini işaretleme tablosu olarak kaydetmeyi destekler. Workbook.Save() yöntemiyle, etkin sayfadaki tüm hücre içerikleri, işaretleme belgesinde bir tablo olarak dışa aktarılacaktır.
### **TxtLoadOptions'ın eski özelliklerini kaldırır**
Lütfen KeepExactFormat yerine LoadStyleStrategy özelliğini kullanın.
### **Eski sınıf LoadDataOption'ı kaldırır**
Lütfen bunun yerine LoadFilter sınıfını ve LoadOptions.LoadFilter özelliğini kullanın.
### **LoadOptions'ın eski özelliklerini kaldırır**
LoadOptions.ConvertNumericData: Lütfen bu özelliği, TxtLoadOptions gibi ilgili LoadOptions alt sınıfıyla birlikte kullanın.
LoadOptions.LoadDataOptions: Lütfen özel LoadFilter uygulamasıyla LoadOptions.LoadFilter özelliğini kullanın.
LoadOptions.LoadDataFilterOptions: lütfen bunun yerine LoadOptions.LoadFilter.LoadDataFilterOptions kullanın.
LoadOptions.OnlyLoadDocumentProperties: lütfen LoadOptions.LoadFilter.LoadDataFilterOptions=LoadDataFilterOptions.DocumentProperties'i kullanın.
LoadOptions.LoadDataAndFormatting/LoadDataOnly: lütfen LoadOptions.LoadFilter.LoadDataFilterOptions=LoadDataFilterOptions.CellData'yı kullanın | LoadDataFilterOptions.DefinedNames.
### **PdfSaveOptions.ExportDocumentStructure özelliğini ekler**
Belge yapısının dışa aktarılıp aktarılmayacağını belirleyen bir değer alır veya ayarlar.
### **Aspose.Cells.WebExtensions ad alanının sınıflarını ekler**
WebExtensions ve WebExtensionTasks'ı temsil eder.
### **WorksheetCollection.WebExtensions ve WorksheetCollection.WebExtensionTaskPanes özelliklerini ekler.**
Tüm WebExtensions ve WebExtensionTasks'ı temsil eder.
### **WebExtensionShape sınıfını ekler.**
WebExtension şeklini temsil eder.
### **Cells.InsertCutCells() yöntemini ekler.**
Kesilmiş hücreleri ekler.
### **Cells.SetViewColumnWidthPixel yöntemini ekler.**
Sütunun görünüm genişliğini ayarlar.
### **ThreadedCommentCollection ve ThreadedComment sınıflarını ekler.**
Zincirleme açıklamayı temsil eder.
### **WorksheetCollection.ThreadedCommentAuthors özelliğini ekler.**
Zincirleme yorumların yazarlarını alır ve ayarlar.
### **Comment.ThreadedComments özelliğini ekler.**
Yorumdaki zincirleme açıklamaları temsil eder.
### **CommentCollection.AddThreadedComment() ve CommentCollection.GetThreadedComments() yöntemlerini ekler.**
Zincirleme yorumları ekler ve alır.
### **Chart.SubTitle özelliğini ekler.**
Grafiğin alt başlığını alır. Yalnızca ODS biçim dosyası için.
