---
title: Utilisation de fichiers de PSD
description: Découvrez comment utiliser des fichiers de PSD dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
topic: Integrations, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '1023'
ht-degree: 22%

---

# Utilisation de fichiers de PSD{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)**: Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on Web pages. -->

Les PSDs (fichiers de document Photoshop) sont le plus souvent utilisés dans Adobe Dynamic Media Classic pour créer des modèles. Lorsque vous chargez un fichier de PSD, vous pouvez créer automatiquement un modèle Adobe Dynamic Media Classic à partir du fichier (sélectionnez l’option Créer un modèle dans l’écran de téléchargement).

Adobe Dynamic Media Classic crée plusieurs images à partir d’un fichier de PSD avec des calques si vous utilisez le fichier pour créer un modèle ; il crée une image pour chaque calque.

## Options de téléchargement des fichiers PSD {#psd-upload-options}

Les options de téléchargement de fichiers de PSD se trouvent sous Options Photoshop dans la boîte de dialogue Télécharger les options de la tâche . Vous pouvez recadrer un fichier, lui associer un profil de couleurs, l’utiliser pour créer un modèle et sélectionner un ancrage.

Les options suivantes sont disponibles au cours du téléchargement des fichiers PSD :

* **Options de recadrage** : situé sous **[!UICONTROL Options de recadrage]**. Sélectionnez **[!UICONTROL Rogner]** afin de pouvoir automatiquement recadrer l’espace blanc des bords d’un fichier de PSD. Sélectionnez **[!UICONTROL Manuel]** pour recadrer les côtés du fichier de PSD :

   * **[!UICONTROL Rogner]** : sélectionnez le menu **[!UICONTROL Rogner en fonction de]** et choisissez **[!UICONTROL Couleur]** ou **[!UICONTROL Transparence]**.

  Si vous choisissez l’option **[!UICONTROL Color]** , sélectionnez le menu Coin et choisissez l’angle du PSD avec la couleur qui représente le mieux l’espace blanc que vous souhaitez recadrer.

  Faites glisser le curseur pour définir une valeur de tolérance comprise entre 0 et 1. Pour effectuer le rognage en fonction de la couleur, indiquez la valeur 0 pour rogner les pixels seulement s’ils correspondent exactement à la couleur que vous avez sélectionnée dans l’angle du fichier PSD. Les valeurs qui se rapprochent de 1 admettent un plus grand écart des couleurs. Pour effectuer un rognage en fonction de la transparence, indiquez 0 pour rogner les pixels seulement s’ils sont transparents ; les nombres plus proches de 1 permettent une plus grande transparence.

   * **[!UICONTROL Manuel]** : entrez le nombre de pixels à recadrer d’un côté ou de chaque côté de l’image. La proportion de l’image qui est rognée dépend du paramètre ppp (pixels par pouce) défini dans le fichier d’image. Supposons, par exemple, que l’image affiche 150 ppp. Ensuite, saisissez 75 dans les zones de texte Haut, Droite, Bas et Gauche. Chaque côté de l’image est recadré, 0,5 pouces.

* **Options de profil colorimétrique** : situées sous **[!UICONTROL Options de profil colorimétrique]**.

   * **[!UICONTROL Conservation des couleurs par défaut]**

   * **[!UICONTROL Conserver l’espace colorimétrique d’origine]** : conserve l’espace colorimétrique d’origine de l’image.

   * **[!UICONTROL Personnalisé de]** > **[!UICONTROL À]** : ouvre les menus afin que vous puissiez choisir un espace colorimétrique Convertir à partir de et Convertir en. Vous pouvez choisir un espace colorimétrique Photoshop standard ou un espace colorimétrique que vous avez chargé dans Adobe Dynamic Media Classic. (voir [Profils ICC](/help/using/icc-profiles.md)).

* **Options Photoshop**

   * **[!UICONTROL Conserver les calques]** : extrait les calques du PSD, le cas échéant, dans des ressources individuelles. Les calques de ces fichiers restent associés au fichier PSD. Vous pouvez les afficher en ouvrant le fichier de PSD dans la vue Détails et en sélectionnant le panneau Calque. Voir Affichage et modification de calques dans un fichier de PSD.

   * **[!UICONTROL Créer un modèle]** : crée un modèle à partir des calques du fichier de PSD.

   * **[!UICONTROL Extract Text]** : extrait le texte afin que les utilisateurs puissent rechercher du texte dans une visionneuse.

   * **[!UICONTROL Étendre les calques à la taille de l’arrière-plan]** : permet d’étendre la taille des calques d’image pixellisés à celle du calque d’arrière-plan.

   * **[!UICONTROL Nom de calque]** : les calques du fichier de PSD sont téléchargés en tant qu’images distinctes. Pour nommer ces images dans Adobe Dynamic Media Classic, choisissez l’une des options suivantes :

      * **[!UICONTROL Nom de calque]** : nomme les images après leurs noms de calque dans le fichier de PSD. Par exemple, un calque appelé Etiquette de prix dans le fichier PSD d’origine devient une image nommée Etiquette de prix. Cependant, si les noms de calque dans le fichier de PSD sont des noms de calque Photoshop par défaut (Arrière-plan, Calque 1, Calque 2, etc.), les images sont nommées d’après leur numéro de calque dans le fichier de PSD. <!-- not their default layer names -->

      * **[!UICONTROL Photoshop et numéro de calque]** : nomme les images après leur numéro de calque dans le fichier de PSD, en ignorant les noms de calque d’origine. Le nom des images est composé du nom de fichier Photoshop et d’un numéro de calque. Par exemple, la deuxième couche d’un fichier appelé `Spring Ad.psd` est nommée `Spring Ad_2` même s’il portait un nom différent de celui par défaut dans Photoshop.

      * **[!UICONTROL Photoshop et nom du calque]** : nomme les images après le fichier de PSD suivi du nom du calque ou du numéro du calque. Le numéro de calque est utilisé si le nom des calques dans le fichier PSD est un nom de calque Photoshop par défaut. Par exemple, un calque nommé `Price Tag` dans un fichier de PSD nommé `SpringAd` est nommé `Spring Ad_Price Tag`. Un calque portant le nom par défaut Layer 2 est appelé `Spring Ad_2`.

   * **[!UICONTROL Ancre]** : spécifiez le mode d’ancrage des images dans les modèles qui sont générés à partir de la composition superposée produite à partir du fichier de PSD. Par défaut, l’ancrage est au centre. Une ancre centrale permet aux images de remplacement de remplir le mieux le même espace, quel que soit le rapport L/H de l’image de remplacement. Les images qui remplacent cette image et qui présentent un aspect différent occupent le même espace lorsque le modèle est référencé et le paramètre de substitution utilisé. Changez de paramètre si votre application nécessite le remplacement d’images pour occuper l’espace alloué dans le modèle.

## Affichage et modification des calques dans un fichier de PSD {#viewing-and-editing-layers-in-a-psd-file}

Si vous avez sélectionné l’option **[!UICONTROL Conserver les calques]** lors du chargement de votre PSD, Adobe Dynamic Media Classic les a tronqués dans des ressources. Vous pouvez afficher et modifier les calques de ressources appartenant à un fichier de PSD en ouvrant le fichier dans le panneau Parcourir de la vue Détails.

>[!NOTE]
>
>Adobe Dynamic Media Classic prend en charge jusqu’à cinq niveaux dans un groupe de calques imbriqués.

1. Double-cliquez sur le fichier de PSD complet dans le panneau Parcourir . Le fichier s’ouvre dans la vue Détails.

   >[!NOTE]
   >
   >veillez à ouvrir le fichier complet et non l’un des calques PSD.

1. Sélectionnez **[!UICONTROL Calques]**. Le panneau Calques affiche tous les calques sous la forme d’images distinctes.
1. Double-cliquez sur un calque et effectuez l’une des opérations suivantes :

   * Pour créer une zone cliquable sur le calque, sélectionnez l’icône **[!UICONTROL Zone cliquable]** . (Voir [Création de zones cliquables](creating-image-maps.md#creating_image_maps).)
   * Pour créer des cibles de zoom sur le calque, sélectionnez l’icône **[!UICONTROL Cibles de zoom]** . (Voir [Création de cibles de zoom pour un zoom guidé](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * Pour recadrer le calque, sélectionnez l’icône **[!UICONTROL Recadrer]** . (Voir [Recadrage d’une image](cropping-image.md#cropping_an_image).)
   * Pour accentuer le calque, sélectionnez **[!UICONTROL Accentuer]**. (Voir [Accentuer une image](sharpening-image.md#sharpening_an_image).)
   * Pour ajuster le calque, sélectionnez **[!UICONTROL Ajuster]**. (Voir [Ajuster une image](adjusting-image.md#adjusting_an_image).)

1. Sélectionnez **[!UICONTROL Enregistrer]** ou **[!UICONTROL Enregistrer sous]**.
1. Pour afficher ou modifier un autre calque, sélectionnez une flèche au bas de l’aperçu du calque.
1. Pour quitter le mode Détails du calque, sélectionnez l’icône **[!UICONTROL Affichage de la grille]** .
