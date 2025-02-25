﻿---
title: Aspose.Cells for .NET 9.0.0 Note di rilascio
type: docs
weight: 40
url: /it/net/aspose-cells-for-net-9-0-0-release-notes/
---
### **1) Aspose.Cells**

|**Chiave** |**Sommario** |**Categoria** |
|:- |:- |:- |
|CELLSNET-40617 | Lettura/scrittura di valori da/a controllo ActiveX ComboBox| Nuova caratteristica|
|CELLSNET-41264 | Utilizzo di Aspose.Cells.GridDesktop nell'applicazione WPF| Nuova caratteristica|
|CELLSNET-44681 | L'importazione di HTML non riesce quando il tag di script utilizza CDATA| Aumento|
|CELLSNET-44693 | Mancano i contenuti durante la conversione da HTML a XLSX| Insetto|
|CELLSNET-44650 | Impossibile convertire i colori di sfondo o in primo piano da HTML| Insetto|
|CELLSNET-44645 | Viene visualizzato un messaggio di errore quando si fa doppio clic su qualsiasi valore della tabella pivot nel file di output| Insetto|
|CELLSNET-44644 |Il file risultante viene danneggiato quando si apre e si salva il file XLS| Insetto|
|CELLSNET-44622 | Il file finale XLSX ha una mancanza degli stili didascalia mentre questi sono presenti nell'input XLSX e intermedio HTML| Insetto|
|CELLSNET-44581 | Problema con la conversione da Spreadsheet a HTML: tag STYLE tra i tag BODY e HTML| Insetto|
|CELLSNET-44718 |ICustomFunction non funziona con [@columnName]| Insetto|
|CELLSNET-44705 | SUM errato visualizzato durante il calcolo delle formule| Insetto|
|CELLSNET-44692 | API calcola in modo errato il valore della formula rispetto a MS Excel| Insetto|
|CELLSNET-44688 | Calcolo errato del valore della cella| Insetto|
|CELLSNET-44684 | Valore errato dalla cella durante il calcolo delle formule| Insetto|
|CELLSNET-44716 | Il risultato PDF non corrisponde a Excel per la stampa delle righe del titolo| Insetto|
|CELLSNET-44713 | I dati sono nascosti nel risultato della conversione di PDF| Insetto|
|CELLSNET-44675 | Il rendering nel file immagine non riesce per un foglio di lavoro| Insetto|
|CELLSNET-44717 | Foglio di calcolo per XPS: il processo non viene mai completato e richiede troppa memoria| Insetto|
|CELLSNET-44678 | I grafici sparkline non vengono visualizzati correttamente durante il rendering del foglio di calcolo su PDF/image| Insetto|
|CELLSNET-44654 | Il metodo Chart.Calculate() rovina l'immagine del grafico| Insetto|
|CELLSNET-44714 |Salvando in memorystream (SpreadsheetML), il processo si blocca e richiede molto tempo| Insetto|
|CELLSNET-44711 | Scoprire la riga nascosta da Aspose.Cells non funziona correttamente in Microsoft Excel| Insetto|
|CELLSNET-44709 | La formula dell'immagine è sparita dopo aver rimosso e reinserito l'immagine| Insetto|
|CELLSNET-44708 | Il reincorporamento della diapositiva della presentazione in XLS comporta la visualizzazione della presentazione con un doppio clic| Insetto|
|CELLSNET-44696 | La linea con la punta della freccia non viene visualizzata completamente nei formati XLSX e PDF| Insetto|
|CELLSNET-44689 | Le impostazioni della stampante vengono modificate all'apertura e al nuovo salvataggio del file XLS di origine| Insetto|
|CELLSNET-44683 | "pane" xml all'interno di "customSheetView" xml non replicato dal foglio di calcolo del progettista| Insetto|
|CELLSNET-44660 | Gli assi Y e X del grafico diventano in grassetto dopo aver caricato e salvato un file XLS| Insetto|
|CELLSNET-44658 | La dimensione del testo delle etichette dell'asse verticale del grafico viene modificata dopo il caricamento e il salvataggio del file XLS| Insetto|
|CELLSNET-44691 | NullReferenceException in Workbook ctor a causa di display:none nell'origine HTML| Eccezione|
|CELLSNET-44685 | Il metodo Workbook.CalculateFormula() genera un'eccezione nel file Excel di origine| Eccezione|
|CELLSNET-44712 | Eccezione: "Testo non valido del nome definito." durante l'apertura di un file Excel| Eccezione|
### **2) Aspose.Cells Griglia Suite**

|**Chiave** |**Sommario** |**Categoria** |
|:- |:- |:- |
|CELLSNET-44667 |L'ombreggiatura Cell dovuta alla formattazione condizionale non viene visualizzata sull'interfaccia GridWeb| Insetto|
### **Pubblico API e modifiche incompatibili con le versioni precedenti**
Di seguito è riportato un elenco di eventuali modifiche apportate al pubblico API come membri aggiunti, rinominati, rimossi o deprecati, nonché qualsiasi modifica non compatibile con le versioni precedenti apportata a Aspose.Cells for .NET. In caso di dubbi su qualsiasi modifica elencata, si prega di segnalarlo su il forum di supporto Aspose.Cells.
#### **Aggiunge la proprietà Shape.TextOptions**
Rappresenta le opzioni di testo della forma.
#### **Metodo Worksheet.SetBackground obsoleto**
Utilizzare invece la proprietà Worksheet.BackgroundImage.
#### **LineShape.BeginArrowheadStyle e ArcShape.BeginArrowheadStyle obsoleti**
Utilizzare invece la proprietà Shape.Line.BeginArrowheadStyle.
#### **LineShape.BeginArrowheadWidth e ArcShape.BeginArrowheadWidth obsoleti**
Utilizzare invece la proprietà Shape.Line.BeginArrowheadWidth.
#### **LineShape.BeginArrowheadLength e ArcShape.BeginArrowheadLength obsoleti**
Utilizzare invece la proprietà Shape.Line.BeginArrowheadLength.
#### **LineShape.EndArrowheadStyle e ArcShape.EndArrowheadStyle obsoleti**
Utilizzare invece la proprietà Shape.Line.EndArrowheadStyle.
#### **LineShape.EndArrowheadWidth e ArcShape.EndArrowheadWidth obsoleti**
Utilizzare invece la proprietà Shape.Line.EndArrowheadWidth.
#### **LineShape.EndArrowheadLength e ArcShape.EndArrowheadLength obsoleti**
Utilizzare invece la proprietà Shape.Line.EndArrowheadLength.
#### **Elimina il metodo Worksheet.CopyConditionalFormatting() obsoleto**
#### **Elimina il metodo Workbook.CheckWriteProtectedPassword() obsoleto**
Utilizzare invece il metodo WorkbookSettings.WriteProtection.ValidatePassword.
#### **Rinomina Workbook.RemoveDigitallySign come metodo Workbook.RemoveDigitalSignature**
Il metodo Workbook.RemoveDigitallySign è stato rinominato in Workbook.RemoveDigitalSignature.
#### **Aggiunge la proprietà ChartSplitType.Auto**
Rappresenta i punti dati che devono essere divisi utilizzando il meccanismo predefinito per questo tipo di grafico.
#### **Aggiunge la proprietà ChartPoint.IsInSecondaryPlot**
Ottiene o imposta un valore che indica se questi punti dati si trovano nella seconda torta o barra di un grafico a torta o a barre del grafico a torta.
#### **Aggiunge la proprietà OleObject.ClassIdentifier**
Ottiene o imposta l'identificatore di classe dell'oggetto incorporato.
#### **Aggiunge la proprietà LoadOptions.CultureInfo**
Ottiene o imposta le informazioni sulle impostazioni cultura del sistema al momento del caricamento del file.
