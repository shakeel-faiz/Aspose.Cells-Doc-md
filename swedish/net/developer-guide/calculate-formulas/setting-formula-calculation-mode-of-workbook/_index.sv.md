﻿---
title: Ställa in formelberäkningsläge för arbetsbok
type: docs
weight: 110
url: /sv/net/setting-formula-calculation-mode-of-workbook/
---
{{% alert color="primary" %}}

Microsoft Excel låter dig ställa in formelberäkningsläget, det vill säga hur formler beräknas. Det finns tre möjliga värden:

- Automatiskt - räkna om när något ändras och varje gång en arbetsbok öppnas.
- Automatisk utom för datatabeller - räkna om när något ändras, men utelämna datatabeller.
- Manuell - räkna om endast när användaren uttryckligen begär det genom att trycka på F9 eller CTRL+ALT+F9, eller när arbetsboken sparas.

{{% /alert %}}

Så här ställer du in formelberäkningsläget i Microsoft Excel:

1.  Välj**Formler** och då**Beräkningsalternativ**.
1. Välj ett av alternativen.

 Aspose.Cells låter dig också ställa in**Formelberäkningsläge** använder sig av[**FormulaSettings.CalculationMode**](https://reference.aspose.com/cells/net/aspose.cells/formulasettings/properties/calculationmode) lägesegenskap. Du kan tilldela den[**CalcModeType**](https://reference.aspose.com/cells/net/aspose.cells/calcmodetype)uppräkning som har ett av följande värden:

- CalcModeType.Automatic
- CalcModeType.AutomaticExceptTable
- CalcModeType.Manual

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Articles-WorkingWithCalculationEngine-SettingFormulaCalculationModeWorkbook-1.cs" >}}
