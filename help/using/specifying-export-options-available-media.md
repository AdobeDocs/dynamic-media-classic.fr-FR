---
title: Définition d’options d’exportation disponibles pour les utilisateurs de Media Portal
description: Découvrez comment spécifier les options d’exportation disponibles pour les utilisateurs de Media Portal dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: c27df6c2-76f4-441c-bd26-cee98203291e
topic: Collaboration, Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 42%

---

# Définition d’options d’exportation disponibles pour les utilisateurs de Media Portal {#specifying-export-options-available-to-media-portal-users}

Sous réserve que l’administrateur les y autorise, les utilisateurs du portail multimédia peuvent reformater des images lors de leur exportation. Par exemple, il est possible de modifier la taille et le format du fichier, ainsi que la qualité de l’image. Le reformatage automatique des images au cours de l’exportation évite d’avoir à effectuer cette opération séparément, ce qui permet de gagner du temps. De plus, les administrateurs peuvent créer un paramètre prédéfini, c’est-à-dire une sélection préétablie de paramètres de format d’image. Vous pouvez ainsi utiliser un paramètre prédéfini lors de l’exportation d’images afin de les reformater selon les spécifications de l’entreprise.

Les deux restrictions suivantes s’appliquent si vous exportez des ressources d’image par le biais d’une conversion définie par l’utilisateur ou si vous exportez des images principales d’origine :

* La taille du fichier d’exportation zip compressé ne doit pas dépasser 1 Go pour la tâche d’exportation.
* Une tâche d’exportation peut contenir un maximum de 500 fichiers.

Voir aussi [Exportation de ressources à partir d’Adobe Dynamic Media Classic](exporting-assets-from-dmc.md#exporting-assets-from_dmc).

**Pour spécifier les options d’exportation disponibles pour les utilisateurs du portail multimédia :**

1. Sur la barre de navigation globale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres d’image prédéfinis]**.
1. Dans la fenêtre Paramètres d’image prédéfinis, sélectionnez l’une des options suivantes :

   * **Activer la conversion définie par l’utilisateur** : lorsque cette option est sélectionnée, les utilisateurs peuvent choisir une autre option dans la liste déroulante **[!UICONTROL Taille]** de la fenêtre Exporter l’Assets sélectionnée. Les utilisateurs peuvent ensuite choisir une unité de mesure, comme les pixels ou les centimètres, puis spécifier la largeur et la hauteur souhaitées. Lors de l’exportation ou du téléchargement de ces fichiers, les fichiers image sont reformatés.

     Lorsque **[!UICONTROL pixels]** sont sélectionnés dans la liste déroulante **[!UICONTROL Taille]**, la largeur × hauteur de l’image obtenue ne peut pas dépasser 100 millions de pixels. Cette taille équivaut à 10 000 × 10 000 pixels pour une image carrée, soit environ 8 000 × 12 000 pixels pour une image de rapport 2x3. Cette limitation de taille ne s’applique pas si vous exportez des images primaires d’origine.

     Désélectionnez cette option pour que les utilisateurs téléchargent les fichiers sans les reformater au fur et à mesure de leur téléchargement.

   * **Activer l’exportation originale** : permet d’exporter les images primaires d’origine. Dans le panneau **[!UICONTROL Exporter l’Assets sélectionnée]** , les utilisateurs peuvent ouvrir le menu déroulant **[!UICONTROL Conversion]** et choisir **[!UICONTROL Exporter l’original]** pour exporter les fichiers d’origine. Désélectionnez cette option si vous souhaitez obliger les utilisateurs à appliquer un paramètre d’image prédéfini ou des options de conversion spécifiques lorsqu’ils exportent des images.

>[!MORELIKETHIS]
>
>* [Paramètres d’image prédéfinis](application-setup.md#image_presets)
>* [Choisir les autorisations d’accès des paramètres d’image prédéfinis pour un groupe](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)
