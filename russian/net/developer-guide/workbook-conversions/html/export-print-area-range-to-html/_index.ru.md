﻿---
title: Экспорт диапазона области печати в HTML
type: docs
weight: 60
url: /ru/net/export-print-area-range-to/
---
## **Возможные сценарии использования**

 Это распространенный сценарий, когда нам нужно экспортировать только область печати, т.е. выбранный диапазон ячеек, а не весь лист в HTML. Эта функция уже доступна для рендеринга PDF, однако теперь вы можете выполнить эту задачу и для HTML. Сначала установите область печати в объекте настройки страницы рабочего листа. В дальнейшем используйте[**Хтмлсавеоптионс. Экспортпринтареаонли**](https://reference.aspose.com/cells/net/aspose.cells/htmlsaveoptions/properties/exportprintareaonly) флаг, чтобы экспортировать только выбранный диапазон.

## Образец кода

Следующий пример кода загружает книгу, а затем экспортирует область печати в HTML. Пример файла для тестирования этой функции можно загрузить по следующей ссылке:

[образецInlineCharts.xlsx](79527946.xlsx)

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-HTML-ExportPrintAreaToHtml-1.cs" >}}
