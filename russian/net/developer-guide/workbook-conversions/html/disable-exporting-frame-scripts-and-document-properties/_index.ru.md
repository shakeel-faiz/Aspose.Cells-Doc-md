﻿---
title: Отключить экспорт сценариев фреймов и свойств документа
type: docs
weight: 310
url: /ru/net/disable-exporting-frame-scripts-and-document-properties/
---
{{% alert color="primary" %}}

Aspose.Cells экспортирует сценарии фреймов и свойства документа при преобразовании рабочей книги в HTML. Версия 8.6.0 Aspose.Cells for .NET представляет параметр, который позволяет при необходимости отключить экспорт сценариев фреймов и свойств документа. Используйте свойство HtmlSaveOptions.ExportFrameScriptsAndProperties, чтобы отключить экспорт.

{{% /alert %}}

## **Отключить экспорт скриптов фреймов и свойств документа**

Следующий пример кода позволяет отключить экспорт сценариев фреймов и свойств документа. После преобразования рабочей книги в формат HTML выходной файл не будет содержать никаких сценариев фреймов и свойств документа.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Articles-HtmlExportFrameScripts-1.cs" >}}
