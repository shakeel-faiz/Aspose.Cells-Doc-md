﻿---
title: Trova se il valore della cella inizia con virgolette singole
type: docs
weight: 270
url: /it/net/find-if-the-cell-value-starts-with-single-quote-mark/
---
{{% alert color="primary" %}}

 Aspose.Cells ora fornisce il[**Style.QuotePrefix**](https://reference.aspose.com/cells/net/aspose.cells/style/properties/quoteprefix) proprietà per trovare se il valore della cella inizia con una singola virgoletta. Prima di questa proprietà, non c'era modo di distinguere tra stringhe come sample e 'sample etc.

{{% /alert %}}

Il seguente codice di esempio spiega che le stringhe come sample e 'sample non possono essere differenziate con[**Cell.StringValue**](https://reference.aspose.com/cells/net/aspose.cells/cell/properties/stringvalue) proprietà. Pertanto dobbiamo usare[**Style.QuotePrefix**](https://reference.aspose.com/cells/net/aspose.cells/style/properties/quoteprefix)proprietà per distinguerli.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Articles-FindIfCellValueStartsWithSingleQuote-FindIfCellValueStartsWithSingleQuote.cs" >}}
