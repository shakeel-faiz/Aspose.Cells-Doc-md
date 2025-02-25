﻿---
title: Copier une feuille de calcul
type: docs
weight: 50
url: /fr/net/copy-a-worksheet/
---
{{% alert color="primary" %}} 

[Ajouter des feuilles de calcul](/cells/fr/net/add-worksheets/) décrit comment ajouter de nouvelles feuilles de calcul à Aspose.Cells.GridWeb. Il est également possible d'ajouter une copie (ou réplique) d'une autre feuille de calcul au contrôle Aspose.Cells.GridWeb. Cette fonctionnalité peut être utile lorsque des données identiques ou similaires dans une feuille de calcul sont également requises dans une autre feuille de calcul. Lorsque c'est le cas, il est plus facile de copier une feuille de calcul existante et de l'ajouter à Aspose.Cells.GridWeb en tant que nouvelle feuille de calcul au lieu de la créer à partir de zéro.

{{% /alert %}} 
## **Copier une feuille de calcul**
### **Utilisation de l'index de feuille**
L'exemple de code ci-dessous montre comment ajouter une copie d'une feuille de calcul au contrôle GridWeb en spécifiant l'index de la feuille de calcul dans la méthode AddCopy de GridWorksheetCollection.



{{< gist "aspose-cells-gists" "7c644a93d33d24299a618c1dda1a2385" "Examples.GridWeb-CSharp-Worksheets-CopyWorksheets.aspx-CopyWorksheetUsingIndex.cs" >}}
### **Utilisation du nom de la feuille**
L'exemple de code ci-dessous montre comment ajouter une copie d'une feuille de calcul au contrôle GridWeb en spécifiant le nom de la feuille de calcul dans la méthode AddCopy de GridWorksheetCollection.



{{< gist "aspose-cells-gists" "7c644a93d33d24299a618c1dda1a2385" "Examples.GridWeb-CSharp-Worksheets-CopyWorksheets.aspx-CopyWorksheetUsingName.cs" >}}

{{% alert color="primary" %}} 

 La méthode AddCopy renvoie l'index de la feuille de calcul nouvellement ajoutée qui peut être utilisée pour accéder à l'instance de la feuille de calcul. Pour plus de détails sur la façon d'accéder aux feuilles de calcul, lisez[Accéder aux feuilles de travail](/cells/fr/net/access-worksheets/).

{{% /alert %}}
