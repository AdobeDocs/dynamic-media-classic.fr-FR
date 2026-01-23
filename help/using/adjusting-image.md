---
title: Modification d’une image
description: Découvrez comment ajuster une image dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 880ee6d0-cb0a-4d53-9056-f0b8b292136e
topic: Content Management
level: Intermediate
source-git-commit: c4613c78347c4bda3d84747a72146617158c03b6
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 37%

---

# Modification d’une image{#adjusting-an-image}

Adobe Dynamic Media Classic propose différentes commandes pour ajuster l’aspect d’une image. Vous pouvez inverser, faire pivoter, rendre floue, modifier la balance des couleurs et colorer une image. Faites des essais avec ces commandes pour constater leurs effets sur l’image en cours de traitement.

Voir aussi [Créer un alias pour une image](adjusting-image.md#creating_an_alias_for_an_image).

**Pour ajuster une image :**

1. Sélectionnez le bouton Modifier de survol de l’image et choisissez Ajuster, ou, dans le panneau Parcourir , double-cliquez sur l’image pour l’ouvrir dans l’affichage des détails.
1. Sélectionnez une taille et un paramètre prédéfini d’image (dans la partie inférieure de la fenêtre).
1. Utilisez les commandes situées sur le côté droit de la fenêtre de `Adjust Editor` pour ajuster l’image :

   * Utilisez les options de retournement (Retourner) pour faire pivoter une image sur le plan horizontal ou vertical. 
   * Utilisez le curseur **[!UICONTROL Rotateur]** pour faire pivoter l’image. Vous pouvez saisir des valeurs dans le champ **[!UICONTROL Rotateur]** pour faire pivoter une image. Les valeurs positives appliquent une rotation horaire et les valeurs négatives, une rotation antihoraire.
   * Utilisez le curseur Estomper ou la zone correspondante pour rendre une image floue. Plus la valeur est élevée, plus l’image devient floue.
   * Utilisez les options Contraste, Luminosité, Saturation, Teinte et Equilibre des couleurs pour régler la couleur et la luminosité. Ces effets sont cumulatifs. Par exemple, les modifications apportées aux paramètres Magenta/Vert s’ajoutent aux modifications des paramètres Teinte.
   * Utilisez les options `Colorize` pour colorer une image tout en conservant les ombres et les tons clairs. Les modifications effectuées à l’aide des options Coloriser sont également cumulatives. Dans le menu Luminosité , choisissez **[!UICONTROL Aucune compensation]** afin de désactiver la compensation automatique de la luminosité. Définissez la valeur de contraste sur 0 pour conserver la plage de contraste de l’image originale, ou spécifiez une plage de contraste avec une valeur supérieure à 0. Une valeur égale à 100 produit le contraste maximum. Les valeurs habituelles sont comprises entre 30 et 70.

1. Une fois le réglage de l’image terminé, procédez de l’une des manières suivantes :

   * Sélectionnez **[!UICONTROL Enregistrer]**.

   * Pour remplacer l’original de l’image, sélectionnez **[!UICONTROL Enregistrer sous]**.

     Dans la liste déroulante, sélectionnez **[!UICONTROL Remplacer l’original]**, puis sélectionnez **[!UICONTROL Enregistrer]**.

   * Pour enregistrer l’image en tant que nouvelle image principale, sélectionnez **[!UICONTROL Enregistrer sous]**.

     Dans la liste déroulante, sélectionnez **[!UICONTROL Enregistrer en tant que nouvelle instance principale]**.
Dans la zone de liste **[!UICONTROL Nom du dossier]**, sélectionnez le dossier dans lequel vous souhaitez enregistrer la nouvelle image principale.
Sélectionnez **[!UICONTROL Enregistrer]**.

   * Pour enregistrer l’image en tant qu’autre affichage de l’image principale. créez un alias pour cette image. Sélectionnez **[!UICONTROL Enregistrer sous]**.

     Dans la liste déroulante de la boîte de dialogue **[!UICONTROL Enregistrer sous]**, sélectionnez **[!UICONTROL Enregistrer en tant qu’autre vue de la vue principale]**.
Dans la zone de liste **[!UICONTROL Nom du dossier]**, sélectionnez le dossier dans lequel vous souhaitez enregistrer la nouvelle image principale.
Sélectionnez **[!UICONTROL Enregistrer]**.

## Création d’un alias pour une image {#creating-an-alias-for-an-image}

Lorsque vous avez ajusté une image, vous pouvez l’enregistrer en tant qu’autre vue de l’image principale. Pour ce faire, vous pouvez créer un alias pour l’image à l’aide de la fonction **[!UICONTROL Enregistrer en tant qu’autre vue de l’image principale]**.

**Pour créer un alias pour une image :**

1. Dans la vue Grille ou Liste, dans la liste déroulante **[!UICONTROL Modifier]** en regard d’une image pour laquelle vous souhaitez créer un alias, sélectionnez **[!UICONTROL Ajuster]**.
1. Dans le coin inférieur droit de la page, sélectionnez **[!UICONTROL Enregistrer sous]**.
1. Dans la liste déroulante de la boîte de dialogue **[!UICONTROL Enregistrer sous]**, sélectionnez **[!UICONTROL Enregistrer en tant qu’autre vue de la vue principale]**.
1. Dans la zone de liste **[!UICONTROL Nom de dossier]**, sélectionnez le dossier où enregistrer l’alias de l’image.
1. Dans le champ **[!UICONTROL Nom de fichier]**, entrez le nom à utiliser pour l’alias.
1. Sélectionnez **[!UICONTROL Enregistrer]**.
