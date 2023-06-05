---
title: Définition d’options d’exportation disponibles pour les utilisateurs de Media Portal
description: Découvrez comment spécifier les options d’exportation disponibles pour les utilisateurs de Media Portal dans Adobe Dynamic Media Classic.
uuid: 5258b8a4-0704-43cd-97d1-c9af2e4e298b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 9bfd95da-3714-4e38-98af-331a04c685f5
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: c27df6c2-76f4-441c-bd26-cee98203291e
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 61%

---

# Définition d’options d’exportation disponibles pour les utilisateurs de Media Portal {#specifying-export-options-available-to-media-portal-users}

Sous réserve que l’administrateur les y autorise, les utilisateurs du portail multimédia peuvent reformater des images lors de leur exportation. Par exemple, il est possible de modifier la taille et le format du fichier, ainsi que la qualité de l’image. Le reformatage automatique des images au cours de l’exportation évite d’avoir à effectuer cette opération séparément, ce qui permet de gagner du temps. De plus, les administrateurs peuvent créer un paramètre prédéfini, c’est-à-dire une sélection préétablie de paramètres de format d’image. Vous pouvez ainsi utiliser un paramètre prédéfini lors de l’exportation d’images afin de les reformater selon les spécifications de l’entreprise.

Les deux restrictions suivantes s’appliquent si vous exportez des ressources d’image par le biais d’une conversion définie par l’utilisateur ou si vous exportez des images Principales d’origine :

* La taille du fichier d’exportation zip compressé ne doit pas dépasser 1 Go pour la tâche d’exportation.
* Une tâche d’exportation peut contenir un maximum de 500 fichiers.

Voir aussi [Exportation de ressources à partir d’Adobe Dynamic Media Classic](exporting-assets-from-dmc.md#exporting-assets-from_dmc).

**Pour définir les options d’exportation disponibles pour les utilisateurs du portail multimédia:**

1. Dans la barre de navigation globale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres d’image prédéfinis]**.
1. Dans la fenêtre Paramètres d’image prédéfinis, sélectionnez l’une des options suivantes :

   * **Activer la conversion définie par l’utilisateur** : lorsque cette option est sélectionnée, les utilisateurs peuvent choisir d’autres options parmi les options **[!UICONTROL Taille]** liste déroulante dans la fenêtre Exporter les ressources sélectionnées . Les utilisateurs peuvent ensuite choisir une unité de mesure, pixels ou centimètres, puis spécifier la largeur et la hauteur souhaitée. Lors de l’exportation ou du téléchargement de ces fichiers, les fichiers image sont reformatés.

      Lorsque vous choisissez **[!UICONTROL pixels]** dans la liste déroulante **[!UICONTROL Taille]**, la largeur x hauteur de l’image obtenue ne doit pas dépasser 100 millions de pixels. Cette taille équivaut à 10 000 x 10 000 pixels pour une image carrée ou à environ 8 000 x 12 000 pixels pour une image 2x3. Cette limitation de taille ne s’applique pas si vous exportez des images Principales d’origine.

      Désélectionnez cette option si vous souhaitez que les utilisateurs téléchargent les fichiers sans les reformater pendant le téléchargement.

   * **Activer Exporter l’original** - Permet d’exporter des images Principales originales. Dans le **[!UICONTROL Exportation des ressources sélectionnées]** , les utilisateurs peuvent ouvrir le panneau **[!UICONTROL Conversion]** menu déroulant et choisissez **[!UICONTROL Exporter l’original]** pour exporter les fichiers originaux. Désélectionnez cette option si vous souhaitez forcer les utilisateurs à choisir un paramètre d’image prédéfini ou des options de conversion lorsqu’ils exportent des images.

>[!MORELIKETHIS]
>
>* [Paramètres d’image prédéfinis](application-setup.md#image_presets)
>* [Choix des autorisations d’accès de paramètres d’image prédéfinis pour un groupe](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)

