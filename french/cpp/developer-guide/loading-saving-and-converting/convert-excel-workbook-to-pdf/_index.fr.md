﻿---
title: Convertir le classeur Excel en PDF
type: docs
weight: 80
url: /fr/cpp/convert-excel-workbook-to-pdf/
---
## **Conversion du classeur Excel en PDF**
Les fichiers PDF sont largement utilisés pour échanger des documents entre les organisations, les secteurs gouvernementaux et les particuliers. Il s'agit d'un format de document standard et les développeurs de logiciels sont souvent invités à trouver un moyen de convertir des fichiers Excel Microsoft en documents PDF.

Aspose.Cells prend en charge la conversion de fichiers Excel en PDF et maintient une haute fidélité visuelle lors de la conversion.

{{% alert color="primary" %}} 

 Aspose.Cells écrit directement les informations sur API et le numéro de version dans les documents de sortie. Par exemple, lors du rendu du document à PDF, Aspose.Cells for C++ remplit le**Application** champ avec la valeur 'Aspose.Cells' et**PDF Producteur** champ avec valeur, par exemple 'Aspose.Cells v18.5.0'.

Veuillez noter que vous ne pouvez pas demander au Aspose.Cells for C++ de modifier ou de supprimer ces informations des documents de sortie.

{{% /alert %}} 
### **Conversion directe**
Aspose.Cells prend en charge la conversion de feuilles de calcul en PDF indépendamment des autres logiciels. Enregistrez simplement un fichier Excel au PDF en utilisant le[IClasseur](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_workbook)classe'[Sauver](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349)méthode. Le[Sauver](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349)méthode fournit la[EnregistrerFormat_Pdf](https://reference.aspose.com/cells/cpp/namespace/aspose.cells#a11cae527e4e68f1adcac8f47ea64481a)membre d'énumération qui convertit les fichiers Excel natifs au format PDF.

Suivez les étapes ci-dessous pour convertir directement les feuilles de calcul Excel au format PDF :

1.  Instancier un objet de la[IClasseur](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_workbook)classe en appelant son constructeur vide.
1. Vous pouvez ouvrir/charger un fichier de modèle existant ou ignorer cette étape si vous créez le classeur à partir de rien.
1. Effectuez n'importe quel travail (saisir des données, appliquer une mise en forme, définir des formules, insérer des images ou d'autres objets de dessin, etc.) sur la feuille de calcul à l'aide des API Aspose.Cells.
1.  Lorsque le code de la feuille de calcul est terminé, appelez le[IClasseur](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_workbook)classe'[Sauver](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_workbook#a77072cfb929787df9ad1f38b02f58349)méthode pour enregistrer la feuille de calcul.

Le format de fichier doit être PDF, sélectionnez donc PDF pertinent (une valeur prédéfinie) dans l'énumération SaveFormat pour générer le document final PDF

 Veuillez consulter l'exemple de code suivant, son[exemple de fichier Excel](67338368.xlsx) et[sortie PDF](67338369.pdf) pour votre référence.

{{< gist "aspose-cells-gists" "6f7d9819d85793c3a3b5d040af42e1a9" "LoadingSavingAndConverting-ConvertExcelWorkbookToPDF_DirectConversion.cpp" >}}
### **Conversion avancée**
Vous pouvez également choisir d'utiliser le[IPdfSaveOptionsIPdfSaveOptionsIPdfSaveOptions](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_pdf_save_options)class pour définir différents attributs pour la conversion. Définition de différentes propriétés du**IPdfSaveOptionsIPdfSaveOptionsIPdfSaveOptions** La classe vous permet de contrôler les paramètres d'impression, de police, de sécurité et de compression pour la sortie PDF. La propriété la plus importante est[Définir la conformité](https://reference.aspose.com/cells/cpp/class/aspose.cells.i_pdf_save_options#a2158ff23d7c071f8224b1cd063233c07)qui vous permet d'enregistrer les fichiers Excel dans des fichiers PDF/A conformes à la norme PDF.
#### **Enregistrement du classeur dans des fichiers conformes PDF/A**
L'extrait de code suivant montre comment utiliser le**IPdfSaveOptionsIPdfSaveOptionsIPdfSaveOptions**class pour enregistrer les fichiers Excel au format PDF/A conforme PDF

 Veuillez consulter l'exemple de code suivant et son[sortie PDF](67338370.pdf) pour votre référence.

{{< gist "aspose-cells-gists" "6f7d9819d85793c3a3b5d040af42e1a9" "LoadingSavingAndConverting-ConvertExcelWorkbookToPDF_A_CompliedFiles.cpp" >}}
#### **Définir l'heure de création PDF**
Avec le**IPdfSaveOptionsIPdfSaveOptionsIPdfSaveOptions** classe, vous pouvez obtenir ou définir l'heure de création PDF.

 Veuillez consulter l'exemple de code suivant et son[sortie PDF](67338371.pdf) pour votre référence.

{{< gist "aspose-cells-gists" "6f7d9819d85793c3a3b5d040af42e1a9" "LoadingSavingAndConverting-ConvertExcelWorkbookToPDF_SetPDFCreationTime.cpp" >}}
