﻿---
title: Aspose.Cells for .NET 22.11 Notes de mise à jour
type: docs
weight: 2
url: /fr/net/aspose-cells-for-net-22-11-release-notes/
---
{{% alert color="primary" %}}

 Cette page contient des notes de version pour[Aspose.Cells for .NET 22.11](https://www.nuget.org/packages/Aspose.Cells/22.11.0).

{{% /alert %}}

|**Clé**|**Résumé**|**Catégorie**|
|:- |:- |:- |
|CELLSNET-52026|Prise en charge de la chronologie de copie|
|CELLSNET-52022|Distinguer ou différencier la formule matricielle héritée du CSE de la formule matricielle normale|
|CELLSNET-52156|Désactiver les cellules de tableau fusionnées lors de l'enregistrement de XLSX à HTML|
|CELLSNET-52159|Prise en charge de l'analyse de la propriété réduite lors de la conversion de HTML en Excel|
|CELLSNET-51939|XLSX à PDF : désalignement du contenu|
|CELLSNET-51940|XLS à PDF : Désalignement du contenu dans les cellules|
|CELLSNET-52068|XLSX à PDF : Formes manquantes/Effondrement de la mise en page|
|CELLSNET-52092|L'impression et l'espacement des caractères dans les chiffres d'Excel sont coupés|
|CELLSNET-52186|Les formes/boîtes sont vides lors de la conversion du document XLSX en PDF|
|CELLSNET-52225|XLSX à PDF Caractères dans les zones de texte inversés|
|CELLSNET-52086|Connexions externes corrompues dans le fichier généré|
|CELLSNET-52133|Les formules Excel sont entourées d'accolades dans le fichier xlsb réenregistré|
|CELLSNET-52158|Détection de référence circulaire incorrecte|
|CELLSNET-52174|Cell.IsArrayFormula est faux pour la formule matricielle après avoir été lu à partir du fichier de modèle xlsb|
|CELLSNET-52217|Les fonctions de recherche ont été calculées de manière incorrecte pour certains grands nombres|
|CELLSNET-52221|La formule de tableau dynamique n'a pas été renversée correctement pour XLOOKUP|
|CELLSNET-52232|Les guillemets simples sont supprimés du nom de la feuille de lien externe|
|CELLSNET-52198|Problème de chevauchement lors de la conversion de graphiques en fichiers image|
|CELLSNET-52043|Problème lors du calcul de "PageSetup.Zoom" avec HorizontalPageBreaks|
|CELLSNET-52157|La bordure de page chevauche le texte lors de la conversion en pdf|
|CELLSNET-52118|Résultat incohérent dans différents formats lorsque html est défini sur cellule dans OpenOffice et LibreCalc|
|CELLSNET-52125|L'index était hors limites pour range.copy with picture|
|CELLSNET-52143| Le type de relation du lien est modifié lors de la conversion d'un fichier XLS en XLSM|
|CELLSNET-52144|Conversion XLS à XLSM modification du type de relation de lien|
|CELLSNET-52151|L'enregistrement de xlsb a remplacé tous les commentaires par le dernier commentaire|
|CELLSNET-52152|La valeur de hauteur de ligne est incorrecte lorsque l'opération de ligne AutoFit est appliquée via Aspose.Cells|
|CELLSNET-52155|Mise en forme conditionnelle perdue après la copie de la plage|
|CELLSNET-52181|XLSX à HTML : la plage Cells n'est pas exportée correctement|
|CELLSNET-52214|Le contenu de la dernière ligne est tronqué dans le fichier Excel de sortie|
|CELLSNET-52236| Le marqueur intelligent (group:merge) ne fonctionne pas pour les cellules fusionnées|
|CELLSNET-52241|Les cases (formes) du document n'apparaissent pas dans la sortie PDF|
|CELLSNET-52243|La modification du projet VBA générera une erreur lors de l'enregistrement du classeur|

## **Public API et modifications incompatibles avec les versions antérieures**

Voici une liste de toutes les modifications apportées au public API, telles que les membres ajoutés, renommés, supprimés ou obsolètes, ainsi que toute modification non rétrocompatible apportée à Aspose.Cells for .NET. Si vous avez des inquiétudes concernant l'un des changements répertoriés, veuillez le signaler sur le forum d'assistance Aspose.Cells.

### **Ajoute la propriété Cell.IsDynamicArrayFormula**

Indique si la formule de la cellule est une formule matricielle dynamique (true) ou une formule matricielle héritée (false).

### **Obsolète la propriété SparklineGroup.SparklineCollection et ajoute la propriété SparklineGroup.Sparklines**

Utilisez plutôt la propriété SparklineGroup.Sparklines.

### **Obsolète la propriété Worksheet.SparklineGroupCollection et ajoute la propriété Worksheet.SparklineGroups**

Utilisez plutôt la propriété Worksheet.SparklineGroups.
