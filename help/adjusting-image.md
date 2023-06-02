---
title: Modification d’une image
description: Découvrez comment ajuster une image dans Adobe Dynamic Media Classic.
uuid: c052acd3-e8c1-4134-ad21-b9c41578097f
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 47a23980-2886-4da3-ab2d-6cd50e00d188
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 880ee6d0-cb0a-4d53-9056-f0b8b292136e
source-git-commit: 358284e6c9888e5188bec35eb7b5408563a71bad
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 52%

---

# Modification d’une image{#adjusting-an-image}

Adobe Dynamic Media Classic propose différentes commandes pour modifier l’aspect d’une image. Vous pouvez retourner, faire pivoter, rendre flou, modifier et coloriser une image ou modifier l’équilibre de ses couleurs. Faites des essais avec ces commandes pour constater leurs effets sur l’image en cours de traitement.

Voir aussi [Création d’un alias pour une image](adjusting-image.md#creating_an_alias_for_an_image).

**Pour ajuster une image :**

1. Sélectionnez le bouton de survol Modifier de l’image et choisissez Ajuster. Dans le panneau de navigation, double-cliquez sur l’image pour l’ouvrir dans la vue Détails.
1. Sélectionnez une taille et un paramètre prédéfini d’image (dans la partie inférieure de la fenêtre).
1. Utilisez les commandes situées sur le côté droit de la fenêtre Editeur de modification pour régler l’image :

   * Utilisez les options de retournement (Retourner) pour faire pivoter une image sur le plan horizontal ou vertical. 
   * Utilisez le curseur de rotation (Pivoter) pour faire pivoter l’image. Vous pouvez saisir des valeurs dans le champ Pivoter pour appliquer une rotation à une image. Les valeurs positives appliquent une rotation horaire et les valeurs négatives, une rotation antihoraire.
   * Utilisez le curseur Estomper ou la zone correspondante pour rendre une image floue. Plus la valeur est élevée, plus l’image devient floue.
   * Utilisez les options Contraste, Luminosité, Saturation, Teinte et Equilibre des couleurs pour régler la couleur et la luminosité. Ces effets sont cumulatifs. Par exemple, les modifications apportées aux paramètres Magenta/Vert s’ajoutent aux modifications des paramètres Teinte.
   * Utilisez les options Coloriser pour coloriser une image tout en conservant ses zones foncées et ses zones claires. Les modifications effectuées à l’aide des options Coloriser sont également cumulatives. Dans le menu Luminosité, choisissez **[!UICONTROL Aucune compensation]** vous désactivez donc la compensation automatique de la luminosité. Définissez la valeur de contraste sur 0 pour conserver la plage de contraste de l’image originale, ou spécifiez une plage de contraste avec une valeur supérieure à 0. Une valeur égale à 100 produit le contraste maximum. Les valeurs types se situent entre 30 et 70.

1. Une fois le réglage de l’image terminé, procédez de l’une des manières suivantes :

   * Sélectionner **[!UICONTROL Enregistrer]**.

   * Pour remplacer l’original de l’image, sélectionnez **[!UICONTROL Enregistrer sous]**.

      Dans la liste déroulante, sélectionnez **[!UICONTROL Remplacer l’original]**, puis sélectionnez **[!UICONTROL Enregistrer]**.

   * Pour enregistrer l’image en tant que nouvelle image maître, sélectionnez **[!UICONTROL Enregistrer sous]**.

      Dans la liste déroulante, sélectionnez **[!UICONTROL Enregistrer en tant que nouvelle image originale]**.
Dans le **[!UICONTROL Nom du dossier]** , sélectionnez le dossier dans lequel vous souhaitez enregistrer la nouvelle image Principale.
Sélectionner **[!UICONTROL Enregistrer]**.

   * Pour enregistrer l’image comme une autre vue de la Principale image. créez un alias pour cette image. Sélectionner **[!UICONTROL Enregistrer sous]**.

      Dans le **[!UICONTROL Enregistrer sous]** dans la liste déroulante, sélectionnez **[!UICONTROL Enregistrer comme une autre vue du gabarit]**.
Dans le **[!UICONTROL Nom du dossier]** , sélectionnez le dossier dans lequel vous souhaitez enregistrer la nouvelle image Principale.
Sélectionner **[!UICONTROL Enregistrer]**.

## Création d’un alias pour une image {#creating-an-alias-for-an-image}

Une fois une image ajustée, vous pouvez l’enregistrer en tant qu’autre vue de la Principale image. Pour ce faire, créez un alias de l’image en utilisant la fonction **[!UICONTROL Enregistrer une vue supplémentaire de l’image originale]**.

**Pour créer un alias pour une image :**

1. En mode d’affichage Grille ou Liste, en mode **[!UICONTROL Modifier]** , sélectionnez la liste déroulante en regard d’une image pour laquelle vous souhaitez créer un alias. **[!UICONTROL Ajuster]**.
1. Dans le coin inférieur droit de la page, sélectionnez **[!UICONTROL Enregistrer sous]**.
1. Dans le **[!UICONTROL Enregistrer sous]** dans la liste déroulante, sélectionnez **[!UICONTROL Enregistrer en tant que vue supplémentaire du gabarit]**.
1. Dans la zone de liste **[!UICONTROL Nom de dossier]**, sélectionnez le dossier où enregistrer l’alias de l’image.
1. Dans le champ **[!UICONTROL Nom de fichier]**, entrez le nom à utiliser pour l’alias.
1. Sélectionner **[!UICONTROL Enregistrer]**.
