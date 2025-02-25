﻿---
title: Aspose.Cells for .NET 8.4.2 Release Notes
type: docs
weight: 80
url: /sv/net/aspose-cells-for-net-8-4-2-release-notes/
---
{{% alert color="primary" %}} 

 Den här sidan innehåller release notes för[Aspose.Cells for .NET 8.4.2](https://downloads.aspose.com/cells/net/new-releases/aspose.cells-for-.net-8.4.2/)

{{% /alert %}} 

 Följande är en lista över förbättringar och ändringar i denna version av Aspose.Cells



\1) Aspose.Cells 


## **Andra förbättringar och förändringar**

## **Nya egenskaper**


 (CELLSNET-43596) - Lägg till ny modul till arbetsbladet VbaProject

(CELLSNET-43569) - Stöd för IFNA-formel/funktion


## **Buggar**


 (CELLSNET-43581) - Text flyttas ut från bannern när Excel-filen konverteras till PDF

 (CELLSNET-43639) - Vattenstämplar visas inte korrekt

 (CELLSNET-43645) - Det går inte att spara inbäddat OLE-objekt från XLSX till HTML

 (CELLSNET-43613) - Anpassat teckensnitt fungerar inte med SheetRender

 (CELLSNET-43573) - Kolumner flyttade till nästa sida vid konvertering till PDF

 (CELLSNET-43571) - Fel sidbrytning i den genererade PDF via Aspose.Cells

 (CELLSNET-43525) - SheetRender.ToImage-genererad bild har text som klipps av

 (CELLSNET-43591) - Felaktigt cirkeldiagrams dataetikettvärde

 (CELLSNET-43574) - Dataetiketternas text överskrider diagramområdet när den konverteras till PDF

 (CELLSNET-43568) - Konvertera diagram till bild och infoga bilden

 (CELLSNET-43502) - Major Grid-linjer försvinner och serielegenden kommer i mitten

(CELLSNET-41716) - X-axeletiketter visas inte korrekt

 (CELLSNET-43641) - Problem med beräkningsformler när iterativ beräkning aktiveras

 (CELLSNET-43637) - Felaktiga formelresultat för PERCENTRANK-funktionen

 (CELLSNET-43630) - Problem med att beräkna LINEST formel/funktion

 (CELLSNET-43628) - Kalkylark försvinner när du klickar på knappen Återställ fönster

 (CELLSNET-43612) - System.ArgumentOutOfRangeException vid laddning av en fil sparad av Aspose.Cells for Java

 (CELLSNET-43604) - ListObjects.DataRange uppdateras inte efter att en rad tagits bort

 (CELLSNET-43603) - Cells.DeleteRows gör kalkylarket skadat

 (CELLSNET-43602) - Vlookup-formeln beräknades inte korrekt

 (CELLSNET-43590) - Xlsx-fil blir korrupt när den öppnas och sparas

 (CELLSNET-43589) - Cell.GetValidationValue fungerar inte för numerisk lista


## **Undantag**


 (CELLSNET-43585) - Aspose.Cells.CellsException vid konvertering av kalkylark till PDF

(CELLSNET-43609) - Undantag för att rendera en Excel-fil till filformatet PDF

 (CELLSNET-43583) - GDI-fel på SheetRender.ToImage-metoden

 (CELLSNET-43565) - CellsException för att spara xlsx till pdf

 (CELLSNET-43631) - SheetRender ctor kastar NullReferenceException undantag

 (CELLSNET-43646) - IndexOutOfRangeException at Workbook.Spara när filsökvägsplatsen inte har ett tillägg

 (CELLSNET-43643) - System.NullReferenceException vid Workbook ctor

 (CELLSNET-43636) - CellsException at Workbook.CalculateFormula

 (CELLSNET-43621) - System.ArgumentException vid Workbook ctor

 (CELLSNET-43614) - Att lägga till modul orsakar undantag för dubbletter av nycklar när arbetsboken sparas

 (CELLSNET-43598) - Undantag vid konvertering av xls till pdf

 (CELLSNET-43572) - System.OverflowException vid Workbook.Save

 (CELLSNET-43570) - ListObject.ConvertToRange kastar NullReferenceException på en tabell

 (CELLSNET-43564) - NullReferenceException när en XLSB-fil sparas tillbaka



 \2) Aspose.Cells Grid Suite


## **Andra förbättringar och förändringar**

## **Buggar**


(CELLSNET-43610) - SaveCommand-händelsen aktiveras inte

 (CELLSNET-43551) - IE8 fungerar inte bra med det anpassade nederländska-belgiska formatet


## **Offentlig API och bakåtinkompatibla ändringar**


 Följande är en lista över alla ändringar som gjorts för allmänheten API, såsom tillagda, bytt namn, borttagna eller utfasade medlemmar samt alla icke-bakåtkompatibla ändringar som gjorts till Aspose.Cells for .NET. Om du har frågor om någon ändring som anges, vänligen ta upp den på supportforumet Aspose.Cells.



 Lägger till VbaModuleCollection.Add metoder

 Lägger till VBA-modul.



 Lägger till åsidosättande Cells.CopyColumns() metoder.

 Kopierar några kolumner.



 Lägger till PasteType.Default och PasteType.DefaultExceptBorders uppräkningar.

Den används för att kopiera intervall som "Alla" och "Alla utom gränser" i MS Excel.


