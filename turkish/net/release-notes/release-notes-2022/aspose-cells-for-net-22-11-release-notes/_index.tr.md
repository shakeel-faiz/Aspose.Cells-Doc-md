﻿---
title: Aspose.Cells for .NET 22.11 Sürüm Notları
type: docs
weight: 2
url: /tr/net/aspose-cells-for-net-22-11-release-notes/
---
{{% alert color="primary" %}}

 Bu sayfa için sürüm notları içerir[Aspose.Cells for .NET 22.11](https://www.nuget.org/packages/Aspose.Cells/22.11.0).

{{% /alert %}}

|**Anahtar**|**Özet**|**Kategori**|
|:- |:- |:- |
|CELLSNET-52026|Destek kopyalama zaman çizelgesi|
|CELLSNET-52022|CSE eski dizi formülünü ve normal dizi formülünü ayırt edin veya ayırt edin|
|CELLSNET-52156|XLSX'i HTML'e kaydederken birleştirilmiş tablo hücrelerini devre dışı bırakın|
|CELLSNET-52159|Html'yi excel'e dönüştürürken daraltılmış özelliği ayrıştırma desteği|
|CELLSNET-51939|XLSX - PDF: İçerik yanlış hizalama|
|CELLSNET-51940|XLS ila PDF: Hücrelerde içerik yanlış hizalama|
|CELLSNET-52068|XLSX - PDF: Eksik şekiller/Düzen çökmesi|
|CELLSNET-52092|Excel'deki rakamlarda karakter baskısı ve boşluklar kesildi|
|CELLSNET-52186|XLSX belgesi PDF'e dönüştürülürken şekiller/kutular boş|
|CELLSNET-52225|XLSX - PDF Metin kutularındaki karakterler tersine çevrildi|
|CELLSNET-52086|Oluşturulan dosyada bozuk dış bağlantılar|
|CELLSNET-52133|Excel formülleri, yeniden kaydedilen xlsb dosyasında kaşlı ayraçlarla sarılır|
|CELLSNET-52158|Yanlış dairesel referans tespiti|
|CELLSNET-52174|Cell.IsArrayFormula, xlsb şablon dosyasından okunduktan sonra dizi formülü için yanlıştır|
|CELLSNET-52217|Bazı büyük sayılar için arama işlevleri yanlış hesaplandı|
|CELLSNET-52221|XLOOKUP için dinamik dizi formülü doğru şekilde dökülmedi|
|CELLSNET-52232|Harici bağlantının sayfa adından tek tırnak kaldırılır|
|CELLSNET-52198|Grafikleri görüntü dosyaları olarak dönüştürürken çakışma sorunu|
|CELLSNET-52043|HorizontalPageBreaks ile "PageSetup.Zoom" hesaplanırken sorun|
|CELLSNET-52157|Sayfa kenarlığı, pdf'ye dönüştürülürken metinle çakışıyor|
|CELLSNET-52118|OpenOffice ve LibreCalc'ta html hücreye ayarlandığında farklı biçimlerde tutarsız sonuç|
|CELLSNET-52125|İndeks, range.copy with resim için aralığın dışındaydı|
|CELLSNET-52143| XLS dosyası XLSM'e dönüştürülürken bağlantının ilişki türü değişiyor|
|CELLSNET-52144|XLS - XLSM dönüştürme bağlantı ilişkisi türünü değiştirme|
|CELLSNET-52151|xlsb'nin kaydedilmesi, tüm yorumları son yorumla değiştirdi|
|CELLSNET-52152|Aspose.Cells ile AutoFit satır işlemi uygulandığında satır yüksekliği değeri yanlış|
|CELLSNET-52155|Aralık kopyasından sonra koşullu biçimlendirme kayboldu|
|CELLSNET-52181|XLSX - HTML: Cells aralığı doğru şekilde dışa aktarılmamış|
|CELLSNET-52214|Çıktı Excel dosyasında son satır içeriği kesiliyor|
|CELLSNET-52236| Akıllı işaretçi (grup:birleştirme) birleştirilmiş hücreler için çalışmıyor|
|CELLSNET-52241|Belgedeki kutular (şekiller) çıktıda görünmüyor PDF|
|CELLSNET-52243|VBA projesini değiştirmek, çalışma kitabı kaydedildiğinde bir hata verir|

## **Herkese Açık API ve Geriye Dönük Uyumsuz Değişiklikler**

Aşağıda, API numaralı telefon numarasına eklenen, yeniden adlandırılan, kaldırılan veya kullanımdan kaldırılan üyeler gibi genele açık olarak yapılan tüm değişikliklerin ve Aspose.Cells for .NET numaralı telefona yapılan geriye dönük uyumlu olmayan değişikliklerin bir listesi bulunmaktadır. Listelenen herhangi bir değişiklikle ilgili endişeleriniz varsa lütfen şu adrese bildirin: Aspose.Cells destek forumu.

### **Cell.IsDynamicArrayFormula özelliğini ekler**

Hücre formülünün dinamik dizi formülü(true) veya eski dizi formülü(false) olduğunu gösterir.

### **SparklineGroup.SparklineCollection özelliğini geçersiz kılar ve SparklineGroup.Sparklines özelliğini ekler**

Bunun yerine SparklineGroup.Sparklines özelliğini kullanın.

### **Worksheet.SparklineGroupCollection özelliğini geçersiz kılar ve Worksheet.SparklineGroups özelliğini ekler**

Bunun yerine Worksheet.SparklineGroups özelliğini kullanın.
