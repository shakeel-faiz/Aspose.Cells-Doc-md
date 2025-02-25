﻿---
title: Geben Sie an, wie die Zeichenfolge in Ausgabe HTML mit HtmlCrossType gekreuzt werden soll
type: docs
weight: 140
url: /de/net/specify-how-to-cross-string-in-output-html-using-htmlcrosstype/
---
## **Mögliche Nutzungsszenarien**

Wenn die Zelle Text oder eine Zeichenfolge enthält, aber größer als die Breite der Zelle ist, läuft die Zeichenfolge über, wenn die nächste Zelle in der nächsten Spalte null oder leer ist. Wenn Sie Ihre Excel-Datei in HTML speichern, können Sie diesen Überlauf kontrollieren, indem Sie den Kreuztyp mit angeben[**HtmlCrossType**](https://reference.aspose.com/cells/net/aspose.cells/htmlcrosstype) Aufzählung. Es hat die folgenden Werte

- **HtmlCrossType.Default**: Darstellung wie MS Excel, abhängig von der nächsten Zelle. Wenn die nächste Zelle null ist, kreuzt sich die Zeichenfolge oder sie wird abgeschnitten.

- **HtmlCrossType.MSExport**: Zeigen Sie die Zeichenfolge wie MS Excel beim Exportieren von HTML an.

- **HtmlCrossType.Cross**: Kreuzzeichenfolge HTML anzeigen, ist die Leistung beim Erstellen großer HTML-Dateien mehr als zehnmal schneller als beim Festlegen des Werts auf Standard oder FitToCell.

- **HtmlCrossType.FitToCell**: Die Zeichenfolge wird nur innerhalb der Zellenbreite angezeigt.

## **Geben Sie an, wie die Zeichenfolge in Ausgabe HTML mit HtmlCrossType gekreuzt werden soll**

 Der folgende Beispielcode lädt die[Beispiel-Excel-Datei](51740732.xlsx) und speichert es im Format HTML, indem Sie different angeben[**HtmlCrossType**](https://reference.aspose.com/cells/net/aspose.cells/htmlcrosstype) . Bitte laden Sie die herunter[HTML ausgeben](51740734.zip) mit diesem Code generiert. Die Beispiel-Excel-Datei enthält das rot umrandete Bild, wie in diesem Screenshot gezeigt, der die Wirkung von zeigt[**HtmlCrossType**](https://reference.aspose.com/cells/net/aspose.cells/htmlcrosstype) Werte am Ausgang HTML.

![todo: Bild_alt_Text](specify-how-to-cross-string-in-output-html-using-htmlcrosstype_1.png)

## **Beispielcode**

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-LoadingSavingConvertingAndManaging-SpecifyHtmlCrossTypeInOutputHTML.cs" >}}
