﻿---
title: Oluştur Kaldır ve GridCell Yorumları Al
type: docs
weight: 10
url: /tr/java/create-remove-and-get-gridcell-comments/
---
## **Olası Kullanım Senaryoları**
Aşağıdaki makale, GridWeb çalışma sayfası içinde GridCell yorumlarının nasıl oluşturulacağını, kaldırılacağını ve alınacağını açıklamaktadır. Bu ekran görüntüsünde gösterildiği gibi fareyi hücrenin üzerine getirdiğinizde GridWeb'in MS-Excel gibi bir Araç İpucu olarak yorum görüntülediğini belirtmekte fayda var.

![yapılacaklar:resim_alternatif_metin](create-remove-and-get-gridcell-comments_1.png)
## **Cell içinde Yorum nesnesi oluştur**
Lütfen hücre içinde bir yorum nesnesi oluşturmak için GridCell.CreateComment yöntemini kullanın. Aşağıdaki örnek kod, GridWeb'in ilk çalışma sayfasının B4 hücresinde örnek bir açıklama oluşturur.

{{< highlight "java" >}}

 // Access first worksheet of GridWeb

GridWorksheet sheet = GridWeb1.getWorkSheets().get(0);

// Access cell B4

GridCell cell = sheet.getCells().get("B4");

// Create comment with these parameters

// i.e. note, author, isvisible

cell.createComment("This is a B4 note.", "Peter", true);

{{< /highlight >}}
## **Yorum nesnesini Cell'den kaldır**
Bir yorum nesnesini hücreden kaldırmak için lütfen GridCell.RemoveComment yöntemini kullanın. Aşağıdaki örnek kod, GridWeb'in ilk çalışma sayfasındaki B4 hücresi açıklamasını kaldırır.



{{< highlight "java" >}}

 // Access first worksheet of GridWeb

GridWorksheet sheet = GridWeb1.getWorkSheets().get(0);

// Access cell B4

GridCell cell = sheet.getCells().get("B4");

// Remove the comment object from this cell.

cell.removeComment();

{{< /highlight >}}
## **Cell'den Yorum nesnesini al**
Lütfen hücreden yorum nesnesi almak için GridCell.GetComment() yöntemini kullanın. Aşağıdaki örnek kod, yorum nesnesini B4 hücresinden alır ve ardından Yazar, Not, Görünürlük vb. gibi çeşitli özelliklerine erişir.

{{< highlight "java" >}}

 // Access first worksheet of GridWeb

GridWorksheet sheet = GridWeb1.getWorkSheets().get(0);

// Access cell B4

GridCell cell = sheet.getCells().get("B4");

// Get comment of this cell

GridComment gridComm = cell.getComment();

// Access its various properties

String strAuth = gridComm.getAuthor();

String strNote = gridComm.getNote();

boolean isVis = gridComm.isVisible();


{{< /highlight >}}




