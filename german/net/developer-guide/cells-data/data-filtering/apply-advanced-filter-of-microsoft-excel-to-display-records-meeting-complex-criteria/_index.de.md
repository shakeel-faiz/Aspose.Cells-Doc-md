﻿---
title: Wenden Sie den erweiterten Filter von Microsoft Excel an, um Datensätze anzuzeigen, die komplexe Kriterien erfüllen
type: docs
weight: 280
url: /de/net/apply-advanced-filter-of-microsoft-excel-to-display-records-meeting-complex-criteria/
---
## **Mögliche Nutzungsszenarien**

 Microsoft Excel ermöglicht Ihnen die Bewerbung*Erweiterter Filter* auf Arbeitsblattdaten, um Datensätze anzuzeigen, die komplexe Kriterien erfüllen. Sie können den erweiterten Filter mit Microsoft Excel über dessen anwenden*Daten > Erweitert*Befehl wie in diesem Screenshot gezeigt.

![todo: Bild_alt_Text](apply-advanced-filter-of-microsoft-excel-to-display-records-meeting-complex-criteria_1.png)

Aspose.Cells ermöglicht es Ihnen auch, den erweiterten Filter mit anzuwenden[**Arbeitsblatt.AdvancedFilter()**](https://reference.aspose.com/cells/net/aspose.cells/worksheet/methods/advancedfilter)Methode. Genau wie Microsoft Excel akzeptiert es die folgenden Parameter.

**istFilter**

Gibt an, ob die Liste gefiltert wird.

**listRange**

Der Listenbereich.

**Kriterienbereich**

Die Kriterien reichen.

**Kopieren nach**

Der Bereich, in den Daten kopiert werden.

**uniqueRecordOnly**

Nur Anzeigen oder Kopieren eindeutiger Zeilen.

## **Wenden Sie den erweiterten Filter von Microsoft Excel an, um Datensätze anzuzeigen, die komplexe Kriterien erfüllen**

Der folgende Beispielcode wendet den erweiterten Filter auf die an[Beispiel-Excel-Datei](48496692.xlsx) und generiert die[Excel-Datei ausgeben](48496691.xlsx). Der Screenshot zeigt beide Dateien zum Vergleich. Wie Sie im Screenshot sehen können, wurden die Daten in der Excel-Ausgabedatei nach komplexen Kriterien gefiltert.

![todo: Bild_alt_Text](apply-advanced-filter-of-microsoft-excel-to-display-records-meeting-complex-criteria_2.png)

## **Beispielcode**

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Data-ApplyAdvancedFilterOfMicrosoftExcel.cs" >}}
