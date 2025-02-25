---
title: Secure PDF Documents
type: docs
weight: 120
url: /net/secure-pdf-documents/
---

{{% alert color="primary" %}}

Sometimes, developers need to work with encrypted PDF files. For example, they need to secure documents with user and owner passwords so not just anyone can open them, or want to restrict whether the document content can be printed or extracted.

This article explains how to pass in PDF security options when saving spreadsheets to PDF.

{{% /alert %}}

Aspose.Cells provides the [**Aspose.Cells.Rendering.PdfSecurity**](https://reference.aspose.com/cells/net/aspose.cells.rendering.pdfsecurity) namespace for working with security. The sample code below describes how to secure PDFs with Aspose.Cells.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Articles-SecurePDFDocuments-1.cs" >}}

{{% alert color="primary" %}}

If the spreadsheet contains formulas, it is best to call [**Workbook.CalculateFormula()**](https://reference.aspose.com/cells/net/aspose.cells/workbook/methods/calculateformula) just before rendering it to PDF. This ensures that formula dependent values are recalculated and the correct values are rendered in the PDF.

{{% /alert %}}
