﻿---
title: Crittografia dei file Excel utilizzando Aspose.Cells
type: docs
weight: 30
url: /it/net/encrypting-excel-files-using-aspose-cells/
---
{{% alert color="primary" %}} 

Microsoft Excel (97 - 2007) consente di crittografare e proteggere con password i fogli di calcolo. Utilizza algoritmi forniti da un provider di servizi crittografici, o CSP, un insieme di algoritmi crittografici con proprietà diverse. Il CSP predefinito è "Compatibile con Office 97/2000" o "Crittografia debole (XOR)". È importante scegliere la lunghezza corretta della chiave di crittografia. Alcuni CSP non supportano più di 40 o 56 bit. Questa è considerata una crittografia debole. Per una crittografia avanzata, è richiesta una lunghezza minima della chiave di 128 bit. Microsoft Windows contiene CSP che offrono anche tipi di crittografia avanzata, ad esempio "Microsoft Strong Cryptographic Provider". Per darti un'idea, la crittografia a 128 bit è ciò che le banche usano per crittografare la connessione con i loro sistemi di Internet Banking.

Aspose.Cells consente di crittografare e proteggere con password i file Excel Microsoft con il tipo di crittografia desiderato.

{{% /alert %}} 
## **Utilizzando Microsoft Excel**
Per configurare le impostazioni di crittografia dei file in Microsoft Excel (qui Microsoft Excel 2003):

1.  Dal**Utensili** menù, selezionare**Opzioni**.
 Viene visualizzata una finestra di dialogo.
1.  Seleziona il**Sicurezza** scheda.
1.  Immettere una password e fare clic**Avanzate** 
   **Finestra di dialogo Opzioni** 

![cose da fare:immagine_alt_testo](encrypting-excel-files-using-aspose-cells_1.png)




1.  Scegli il tipo di crittografia e conferma la password.

   **Finestra di dialogo Tipo di crittografia** 

![cose da fare:immagine_alt_testo](encrypting-excel-files-using-aspose-cells_2.png)



## **Crittografia con Aspose.Cells**
L'esempio seguente mostra come crittografare e proteggere con password un file excel utilizzando Aspose.Cells API.

**C#**

{{< highlight "csharp" >}}

 string FilePath = @"..\..\..\Sample Files\";

string srcFileName = FilePath + "Encrypting Excel Files.xlsx";

string destFileName = FilePath + "Result Encrypting Excel Files.xlsx";

//Open an excel file.

Workbook workbook = new Workbook(srcFileName);

//Specify XOR encryption type.

workbook.SetEncryptionOptions(EncryptionType.XOR, 40);

//Specify Strong Encryption type (RC4,Microsoft Strong Cryptographic Provider).

workbook.SetEncryptionOptions(EncryptionType.StrongCryptographicProvider, 128);

//Password protect the file.

workbook.Settings.Password = "1234";

//Save the excel file.

workbook.Save(destFileName);

{{< /highlight >}}
## **Scarica il codice in esecuzione**
- [Github](https://github.com/aspose-cells/Aspose.Cells-for-.NET/releases/tag/MissingFeaturesOpenXMLExcelv1.1)
## **Scarica il codice di esempio**
- [Github](https://github.com/aspose-cells/Aspose.Cells-for-.NET/tree/master/Plugins/Aspose.Cells%20Vs%20OpenXML%20Spreadsheets/OpenXML%20Missing%20Features/Encrypting%20Excel%20Files)

