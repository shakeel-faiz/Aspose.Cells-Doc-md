﻿---
title: Ändern Sie einen vorhandenen Stil
type: docs
weight: 90
url: /de/net/modify-an-existing-style/
---
{{% alert color="primary" %}}

Um dieselben Formatierungsoptionen auf Zellen anzuwenden, erstellen Sie ein neues Formatierungsstilobjekt. Ein Formatierungsstilobjekt ist eine Kombination aus Formatierungsmerkmalen wie Schriftart, Schriftgröße, Einzug, Zahl, Rahmen, Muster usw., die als Satz benannt und gespeichert werden. Bei der Anwendung werden alle Formatierungen in diesem Stil angewendet.

Sie können auch einen vorhandenen Stil verwenden, ihn mit der Arbeitsmappe speichern und verwenden, um Informationen mit denselben Attributen zu formatieren.

 Wenn Zellen nicht explizit formatiert sind, wird die**Normal** Stil (der Standardstil der Arbeitsmappe) wird angewendet. Microsoft Excel definiert zusätzlich zum normalen Stil mehrere Stile vor, einschließlich Komma, Währung und Prozent.

Aspose.Cells ermöglicht das Ändern jedes dieser Stile oder jedes anderen Stils, den Sie mit Ihren gewünschten Attributen definieren.

{{% /alert %}}

## **Mit Microsoft Excel**

So aktualisieren Sie einen Stil in Microsoft Excel 97-2003:

1.  Auf der**Format** Menü, klicken**Stil**.
1.  Wählen Sie den Stil aus, den Sie ändern möchten**Stilname** aufführen.
1.  Klicken**Ändern**.
1. Wählen Sie die gewünschten Stiloptionen mithilfe der Registerkarten im Dialogfeld Format Cells aus.
1.  Klicken**OK**.
1.  Unter**Stil beinhaltet**, geben Sie die gewünschten Stilmerkmale an.
1.  Klicken**OK** , um den Stil zu speichern und auf den ausgewählten Bereich anzuwenden.

## **Mit Aspose.Cells**

 Die folgenden Beispiele demonstrieren die Verwendung[**Style.Update**](https://reference.aspose.com/cells/net/aspose.cells/style/methods/update)Methode.

### **Erstellen und Ändern eines Stils**

 Dieses Beispiel erstellt eine[**Stil**](https://reference.aspose.com/cells/net/aspose.cells/style) Objekt, wendet es auf eine Reihe von Zellen an und ändert die[**Stil**](https://reference.aspose.com/cells/net/aspose.cells/style)Objekt. Die Änderungen werden automatisch auf die Zelle und den Bereich angewendet, auf den der Stil angewendet wurde.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Articles-ModifyExistingStyle-ModifyThroughStyleObject-1.cs" >}}

### **Ändern eines vorhandenen Stils**

In diesem Beispiel wird eine einfache Excel-Vorlagendatei verwendet, in der ein Stil namens „Prozent“ bereits auf einen Bereich angewendet wurde. Das Beispiel:

1. bekommt den Stil,
1. erstellt ein Stilobjekt und
1. ändert die Stilformatierung.

Die Änderungen werden automatisch auf den Bereich angewendet, auf den der Stil angewendet wurde.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Articles-ModifyExistingStyle-ModifyThroughSampleExcelFile-1.cs" >}}
