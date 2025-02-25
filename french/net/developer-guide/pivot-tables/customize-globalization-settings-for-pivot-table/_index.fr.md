﻿---
title: Personnaliser les paramètres de globalisation pour le tableau croisé dynamique
type: docs
weight: 50
url: /fr/net/customize-globalization-settings-for-pivot-table/
---
## **Scénarios d'utilisation possibles**

 Parfois, vous voulez personnaliser le*Total croisé dynamique, sous-total, total général, tous les éléments, plusieurs éléments, étiquettes de colonne, étiquettes de ligne, valeurs vides*texte selon vos besoins. Aspose.Cells vous permet de personnaliser les paramètres de globalisation du tableau croisé dynamique pour faire face à de tels scénarios. Vous pouvez également utiliser cette fonction pour changer les étiquettes en d'autres langues comme l'arabe, l'hindi, le polonais, etc.

## **Personnaliser les paramètres de globalisation pour le tableau croisé dynamique**

 L'exemple de code suivant explique comment personnaliser les paramètres de globalisation du tableau croisé dynamique. Il crée une classe*CustomPivotTableGlobalizationSettingsCustomPivotTableGlobalizationSettingsCustomPivotTableGlobalizationSettingsCustomPivotTableGlobalizationSettings* dérivé d'une classe de base[**GlobalizationSettings**](https://reference.aspose.com/cells/net/aspose.cells/globalizationsettings) et remplace toutes ses méthodes nécessaires. Ces méthodes renvoient le texte personnalisé pour le*Total croisé dynamique, sous-total, total général, tous les éléments, plusieurs éléments, étiquettes de colonne, étiquettes de ligne, valeurs vides*. Ensuite, il affecte l'objet de cette classe à[**WorkbookSettings.GlobalizationSettingsWorkbookSettings.GlobalizationSettings**](https://reference.aspose.com/cells/net/aspose.cells/workbooksettings/properties/globalizationsettings) la propriété. Le code charge le[fichier excel source](40468488.xlsx) qui contient le tableau croisé dynamique, actualise et calcule ses données et l'enregistre sous[sortie PDF](40468487.pdf)dossier. La capture d'écran suivante montre l'effet de l'exemple de code sur la sortie PDF. Comme vous pouvez le voir dans la capture d'écran, différentes parties du tableau croisé dynamique ont maintenant un texte personnalisé renvoyé par les méthodes remplacées de[**GlobalizationSettings**](https://reference.aspose.com/cells/net/aspose.cells/globalizationsettings)classe.

![tâche : image_autre_texte](customize-globalization-settings-for-pivot-table_1.png)

## **Exemple de code**

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-PivotTable-CustomizePivotTableGlobalSettings-CustomizePivotTableGlobalSettings.cs" >}}
