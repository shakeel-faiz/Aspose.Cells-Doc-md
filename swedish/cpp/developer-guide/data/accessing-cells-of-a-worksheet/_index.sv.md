﻿---
title: Åtkomst till Cells i ett arbetsblad
type: docs
weight: 10
url: /sv/cpp/accessing-cells-of-a-worksheet/
---
{{% alert color="primary" %}} 

Vi vet att alla kalkylblad kan innehålla data som i princip lagras i celler (som ett kalkylblad är uppbyggt av). En cell är en grundläggande del av ett kalkylblad som används för att konstruera hela kalkylbladet som en sekvens av rader och kolumner. Innan vi försöker komma åt data från ett kalkylblad skulle vi behöva få tillgång till dess celler. Så i det här ämnet kommer vi att diskutera några grundläggande metoder för att komma åt kalkylbladsceller vid körning med Aspose.Cells.

{{% /alert %}} 
## **Tillgång till Cells**
 Aspose.Cells tillhandahåller en klass[IArbetsbok](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_workbook) som representerar en Excel-fil. De[IArbetsbok](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_workbook) klass innehåller en[Arbetsblad](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet_collection)samling som gör det möjligt att komma åt varje kalkylblad i Excel-filen. Ett arbetsblad representeras av[IArbetsblad](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet) klass. De[IArbetsblad](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet) klass ger en[Cells](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_cell)samling som representerar alla celler i kalkylbladet.

 Vi kan använda[Cells](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_cell)samling för att komma åt celler i ett kalkylblad. Aspose.Cells tillhandahåller tre grundläggande metoder för att komma åt celler i ett kalkylblad:

1. Använder cellnamn.
1. Använda en cells rad- och kolumnindex.
1.  Använda ett cellindex i[Cells](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_cell)samling

{{% alert color="primary" %}} 

Vi har nämnt att den tredje inflygningen är den snabbaste och den första är den långsammaste. Prestandaskillnaden mellan tillvägagångssätten är mycket liten, så oroa dig inte för prestandaförsämring, vilket tillvägagångssätt du än använder.

{{% /alert %}} 
### **Använder Cell Namn**
 Utvecklare kan komma åt vilken specifik cell som helst genom att skicka dess cellnamn till[Cells](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_cell) samling av[IArbetsblad](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet)klass som ett index.

 Om du skapar ett tomt kalkylblad vid start kommer antalet[Cells](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_cell)samlingen är noll. När du använder det här tillvägagångssättet för att komma åt en cell, kommer den att kontrollera om denna cell finns i samlingen eller inte. Om ja, returnerar den cellobjektet i samlingen annars skapar den ett nytt[ICell](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_cell) objekt, lägger till objektet till[Cells](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_cell)samling och returnerar sedan objektet. Detta tillvägagångssätt är det enklaste sättet att komma åt cellen om du är bekant med Microsoft Excel, men det är det långsammaste sättet jämfört med andra metoder.

{{< gist "aspose-cells-gists" "6f7d9819d85793c3a3b5d040af42e1a9" "Examples-CellsCPP-Data-AccessingCellsOfWorksheet-AccessingCellsUsingCellName.cpp" >}}
### **Använda rad- och kolumnindex för Cell**
 Utvecklare kan komma åt vilken specifik cell som helst genom att skicka indexen för dess rad och kolumn till[Cells](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_cell) samling av[IArbetsblad](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_worksheet)klass. Detta tillvägagångssätt fungerar på samma sätt som det första tillvägagångssättet.

{{< gist "aspose-cells-gists" "6f7d9819d85793c3a3b5d040af42e1a9" "Examples-CellsCPP-Data-AccessingCellsOfWorksheet-AccessingCellsUsingRowAndColumnIndexOfTheCell.cpp" >}}
## **Få åtkomst till maximalt visningsområde för arbetsblad**
Aspose.Cells tillåter utvecklare att komma åt ett kalkylblads maximala visningsområde. Det maximala visningsintervallet - cellintervallet mellan den första och sista cellen med innehåll - är användbart när du behöver kopiera, markera eller visa hela innehållet i ett kalkylblad i en bild.

 Du kan komma åt ett kalkylblads maximala visningsområde med[MaxDisplayIRange](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_cell#ad351277ccaa0a4e1e8cd0693a1e2e988) metod för[Cells](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_cell)samling.

{{< gist "aspose-cells-gists" "6f7d9819d85793c3a3b5d040af42e1a9" "Examples-CellsCPP-Data-AccessingCellsOfWorksheet-AccessingMaximumDisplayRangeOfWorksheet.cpp" >}}
