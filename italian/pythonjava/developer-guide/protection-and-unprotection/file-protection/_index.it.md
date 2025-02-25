﻿---
title: Crittografare e decrittografare i file Excel
type: docs
weight: 10
url: /it/python-java/encrypt-and-decrypt-excel-files/
description: Come crittografare e decrittografare i file Excel utilizzando Python. Bloccare e sbloccare i file Excel.
---
{{% alert color="primary" %}}

Microsoft Excel (97 - 365) consente di crittografare e proteggere con password i fogli di calcolo. Utilizza algoritmi forniti da un provider di servizi crittografici, o CSP, un insieme di algoritmi crittografici con proprietà diverse. Il CSP predefinito è "Compatibile con Office 97/2000" o "Crittografia debole (XOR)". È importante scegliere la lunghezza corretta della chiave di crittografia. Alcuni CSP non supportano più di 40 o 56 bit. Questa è considerata una crittografia debole. Per una crittografia avanzata, è richiesta una lunghezza minima della chiave di 128 bit. Microsoft Windows contiene CSP che offrono anche tipi di crittografia avanzata, ad esempio "Microsoft Strong Cryptographic Provider". Per darti un'idea, la crittografia a 128 bit è ciò che le banche usano per crittografare la connessione con i loro sistemi di Internet Banking.

Aspose.Cells for Python consente di crittografare e proteggere con password i file Excel Microsoft con il tipo di crittografia desiderato.

{{% /alert %}}

## **Utilizzando Microsoft Excel**

Per configurare le impostazioni di crittografia dei file in Microsoft Excel (qui Microsoft Excel 2003):

1.  Dal**Utensili** menù, selezionare**Opzioni**Apparirà una finestra di dialogo.
1.  Seleziona il**Sicurezza** scheda.
1.  Immettere una password e fare clic**Avanzate**
1. Scegli il tipo di crittografia e conferma la password.

## **Crittografia file Excel con Aspose.Cells**

L'esempio seguente mostra come crittografare e proteggere con password un file excel utilizzando Aspose.Cells API.

{{< gist "aspose-cells-gists" "32e50c6aabc547111966569f3fd39694" "Examples-CSharp-Files-Utility-EncryptingFiles-1.py" >}}

## **Decrittografia file Excel con Aspose.Cells**
È molto utile aprire il file excel protetto da password e decrittografarlo utilizzando Aspose.Cells API come i seguenti codici:

{{< gist "aspose-cells-gists" "32e50c6aabc547111966569f3fd39694" "Decrypt-Excel-File.py" >}}


