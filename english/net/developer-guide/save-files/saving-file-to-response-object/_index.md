---
title: Saving File to Response Object
type: docs
weight: 50
url: /net/saving-file-to-response-object/
---

{{% alert color="primary" %}}

Aspose.Cells makes it possible to manipulate files. This article explains the various ways in which files can be saved to a response object.

{{% /alert %}}

## **Saving File to Response Object**

It is also possible to generate a file dynamically and send it directly to a client browser. In order to do so, use a special overloaded version of the **[Save](https://reference.aspose.com/cells/net/aspose.cells.workbook/save/methods/5)** method that accepts the following parameters:

- ASP.NET **[HttpResponse](https://docs.microsoft.com/en-gb/dotnet/api/system.web.httpresponse?view=netframework-4.8)** object.
- File name.
- **[ContentDisposition](https://reference.aspose.com/cells/net/aspose.cells/contentdisposition)**, the content-disposition type of the output file.
- **[SaveOptions](https://reference.aspose.com/cells/net/aspose.cells/saveoptions)**, the file format type

The **[ContentDisposition](https://reference.aspose.com/cells/net/aspose.cells/contentdisposition)** enumeration determines whether the file being sent to the browser provides the option to open by itself directly in the browser or in an application associated with .xls/.xlsx or another extension.

The enumeration contains the following pre-defined save types:

|**Type**|**Description**|
| :- | :- |
|Attachment|Sends the spreadsheet to the browser and opens in an application as an attachment associated with .xls/.xlsx or other extensions|
|Inline|Sends the document to the browser and presents an option to save the spreadsheet to disk or open inside the browser|

### **XLS Files**

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Files-Handling-SaveXLSFile-1.cs" >}}

### **XLSX Files**

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Files-Handling-SaveXLSXFile-1.cs" >}}

### **PDF Files**

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Files-Handling-SaveInPdfFormat-1.cs" >}}

### **Note**

Due to the object "System.Web.HttpResponse" does not contained in .NET5 and .Netstandard,
So this function does not exist in Aspose.Cells .NET5 and .Netstandard version, you can refer to the following code to save the file to the stream, then do operation to the stream.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Files-Handling-SavingFiletoStream-1.cs" >}}

