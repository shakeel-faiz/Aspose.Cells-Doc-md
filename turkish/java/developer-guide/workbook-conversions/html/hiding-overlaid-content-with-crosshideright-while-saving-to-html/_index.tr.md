﻿---
title: HTML'e kaydederken CrossHideRight ile Yer Paylaşımlı İçeriği Gizleme
type: docs
weight: 100
url: /tr/java/hiding-overlaid-content-with-crosshideright-while-saving-to-html/
---
## **Olası Kullanım Senaryoları**

Excel dosyanızı HTML'e kaydettiğinizde, hücre dizileri için farklı çapraz tipler belirleyebilirsiniz. Varsayılan olarak, Aspose.Cells, Microsoft Excel'e göre HTML'i oluşturur, ancak değiştirdiğinizde[**HtmlSaveOptions.HtmlCrossStringType**](https://reference.aspose.com/cells/java/com.aspose.cells/htmlsaveoptions#HtmlCrossStringType)ile[**CROSS_HIDE_RIGHT**](https://reference.aspose.com/cells/java/com.aspose.cells/htmlcrosstype#CROSS_HIDE_RIGHT)daha sonra hücrenin sağ tarafında, hücre dizisiyle örtüşen veya örtüşen tüm dizileri gizler.

## **HTML'e kaydederken CrossHideRight ile Yer Paylaşımlı İçeriği Gizleme**

Aşağıdaki örnek kod,[örnek excel dosyası](64716916.xlsx)ve onu kaydeder[çıkış HTML](64716915.zip)ayarladıktan sonra[**HtmlSaveOptions.HtmlCrossStringType**](https://reference.aspose.com/cells/java/com.aspose.cells/htmlsaveoptions#HtmlCrossStringType)olarak[**CROSS_HIDE_RIGHT**](https://reference.aspose.com/cells/java/com.aspose.cells/htmlcrosstype#CROSS_HIDE_RIGHT). Ekran görüntüsü nasıl olduğunu açıklıyor[**CROSS_HIDE_RIGHT**](https://reference.aspose.com/cells/java/com.aspose.cells/htmlcrosstype#CROSS_HIDE_RIGHT)varsayılan çıkıştan HTML çıkışını etkiler.

![yapılacaklar:resim_alternatif_metin](hiding-overlaid-content-with-crosshideright-while-saving-to-html_1.png)

## **Basit kod**

{{< gist "aspose-cells-gists" "5876dc77e47649b66bdb5deefb4b5639" "HTML-HidingOverlaidContentWithCrossHideRightWhileSavingToHtml.java" >}}
