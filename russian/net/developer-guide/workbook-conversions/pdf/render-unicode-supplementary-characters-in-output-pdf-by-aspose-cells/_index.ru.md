﻿---
title: Визуализация дополнительных символов Unicode в выводе PDF по Aspose.Cells
type: docs
weight: 350
url: /ru/net/render-unicode-supplementary-characters-in-output-pdf-by-aspose-cells/
---
{{% alert color="primary" %}}

Обычные символы Unicode имеют длину 2 байта, а дополнительные символы Unicode имеют длину 4 байта. Aspose.Cells теперь поддерживает отрисовку этих 4-байтовых символов Unicode.

В стандарте символов Unicode дополнительные символы — это символы, которым присвоены кодовые точки от U+10000 до U+10FFFF. Другими словами, это символы Unicode больше, чем U+FFFF.

- В UTF-8 эти символы имеют длину 4 байта.
- В UTF-16 для этих символов требуется 2 суррогата (16-битные единицы).

{{% /alert %}}

## Визуализация дополнительных символов Unicode в выводе PDF по Aspose.Cells

 На следующем снимке экрана показано, как Aspose.Cells визуализировал[исходный файл excel](5115563.xlsx) в[вывод PDF](5115564.pdf). Как вы можете видеть, все три дополнительных символа Unicode были отображены точно так же, как это было сделано Microsoft Excel.

![дело:изображение_альтернативный_текст](output.png)

## Образец кода

 Вы можете использовать этот пример кода для преобразования[исходный файл excel](5115563.xlsx) в[вывод PDF](5115564.pdf).

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Articles-RenderUnicodeInOutput-RenderUnicodeInOutput.cs" >}}
