﻿---
title: Enregistrer le classeur au format texte ou CSV dans Aspose.Cells
type: docs
weight: 110
url: /fr/net/save-workbook-to-text-or-csv-format-in-aspose-cells/
---
{{% alert color="primary" %}} 

Parfois, vous souhaitez convertir ou enregistrer un classeur avec plusieurs feuilles de calcul au format texte. Pour les formats de texte (par exemple TXT, TabDelim, CSV etc.), par défaut, Microsoft Excel et Aspose.Cells enregistrent uniquement le contenu de la feuille de calcul active.

{{% /alert %}} 

L'exemple de code suivant explique comment enregistrer un classeur entier au format texte. Chargez le classeur source qui peut être n'importe quel fichier de feuille de calcul Excel ou OpenOffice Microsoft (donc XLS, XLSX, XLSM, XLSB, ODS, etc.) avec n'importe quel nombre de feuilles de calcul.

Lorsque le code est exécuté, il convertit les données de toutes les feuilles du classeur au format TXT.

Vous pouvez modifier le même exemple pour enregistrer votre fichier au format CSV. Par défaut, TxtSaveOptions.Separator est une virgule, ne spécifiez donc pas de séparateur si vous enregistrez au format CSV.

**C#**

{{< highlight "csharp" >}}

 chaîne filePath = "source.xlsx" ;

// Chargez votre classeur source

Classeur classeur = nouveau classeur (filePath);

// tableau de 0 octet

octet[]workbookData = nouvel octet[0] ;

//Options d'enregistrement de texte. Vous pouvez utiliser n'importe quel type de séparateur

TxtSaveOptions opts = new TxtSaveOptions();

opts.Separator = '\t';

// Copiez chaque donnée de feuille de calcul au format texte dans le tableau de données du classeur

 pour (int idx = 0; idx< workbook.Worksheets.Count; idx++)

{

    //Save the active worksheet into text format

    MemoryStream ms = new MemoryStream();

    workbook.Worksheets.ActiveSheetIndex = idx;

    workbook.Save(ms, opts);

    //Save the worksheet data into sheet data array

    ms.Position = 0;

    byte[] sheetData = ms.ToArray();

    //Combine this worksheet data into workbook data array

    byte[] combinedArray = new byte[workbookData.Length + sheetData.Length];

    Array.Copy(workbookData, 0, combinedArray, 0, workbookData.Length);

    Array.Copy(sheetData, 0, combinedArray, workbookData.Length, sheetData.Length);

    workbookData = combinedArray;

}

//Save entire workbook data into file

File.WriteAllBytes(filePath + ".out.txt", workbookData);


{{< /highlight >}}
## **Télécharger le code d'exécution**
- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-.NET/tree/master/Plugins/Aspose.Cells%20Vs%20VSTO%20Spreadsheets/Aspose.Cells%20Features%20missing%20in%20VSTO/Save%20Workbook%20to%20Text%20or%20CSV%20Format)
## **Télécharger l'exemple de code**
- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-.NET/releases/tag/MissingFeaturesAsposeCellsForVSTO1.1)
