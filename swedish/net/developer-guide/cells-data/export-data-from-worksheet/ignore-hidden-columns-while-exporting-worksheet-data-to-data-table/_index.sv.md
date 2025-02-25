﻿---
title: Ignorera dolda kolumner när du exporterar kalkylbladsdata till datatabell
type: docs
weight: 330
url: /sv/net/ignore-hidden-columns-while-exporting-worksheet-data-to-data-table/
---
{{% alert color="primary" %}}

 Ibland vill du ignorera dolda kolumner när du exporterar kalkylbladsdata till en datatabell. Du kan uppnå det med Aspose.Cells genom att ställa in[**ExportTableOptions.PlotVisibleColumns**](https://reference.aspose.com/cells/net/aspose.cells/exporttableoptions/properties/plotvisiblecolumns) till**Sann** . Som standard är dess värde**falsk** , så du måste ställa in den**Sann** för att ignorera de dolda kolumnerna.

{{% /alert %}}

 Följande exempelkod förklarar användningen av[**ExportTableOptions.PlotVisibleColumns**](https://reference.aspose.com/cells/net/aspose.cells/exporttableoptions/properties/plotvisiblecolumns)egenskapen att ignorera de dolda kolumnerna samtidigt som kalkylbladets hela data exporteras till datatabellen.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Articles-IgnoreHiddenColumnsDataTable-1.cs" >}}
