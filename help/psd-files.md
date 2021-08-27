---
title: Utilisation de fichiers PSD
description: Découvrez comment utiliser des fichiers PSD dans Adobe Dynamic Media Classic.
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
source-git-commit: ad5270545be502d3aaabba574353787622ab0445
workflow-type: tm+mt
source-wordcount: '990'
ht-degree: 29%

---

# Utilisation de fichiers PSD{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)** - Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages. -->

Les fichiers PSD (Photoshop Document) sont le plus souvent utilisés dans Adobe Dynamic Media Classic pour créer des modèles. Lorsque vous chargez un fichier PSD, vous pouvez créer automatiquement un modèle Adobe Dynamic Media Classic à partir du fichier (sélectionnez l’option Créer un modèle dans l’écran de téléchargement).

Adobe Dynamic Media Classic crée plusieurs images à partir d’un fichier PSD avec des calques si vous utilisez le fichier pour créer un modèle ; il crée une image pour chaque calque.

## Options de téléchargement des fichiers PSD {#psd-upload-options}

Les options de téléchargement de fichiers PSD se trouvent sous Options Photoshop dans la boîte de dialogue Télécharger les options de la tâche . Vous pouvez recadrer un fichier, lui associer un profil de couleurs, l’utiliser pour créer un modèle et sélectionner un ancrage.

Les options suivantes sont disponibles au cours du téléchargement des fichiers PSD :

* **Options de recadrage**  : situées sous les options de  **[!UICONTROL recadrage]**. Sélectionnez **[!UICONTROL Rogner]** pour supprimer automatiquement l’espace blanc des bords d’un fichier PSD ; sélectionnez **[!UICONTROL Manuel]** pour recadrer les côtés du fichier PSD :

   * **[!UICONTROL Rogner]**  : sélectionnez le  **[!UICONTROL menu]** Rogner en fonction de la position, puis choisissez  ****  **[!UICONTROL Transparence]** de la couleur.

      Si vous choisissez l’option **[!UICONTROL Couleur]**, sélectionnez le menu Coin et choisissez l’angle du fichier PSD avec la couleur qui représente le mieux l’espace blanc que vous souhaitez recadrer.

      Faites glisser le curseur pour définir une valeur de tolérance comprise entre 0 et 1. Pour effectuer le rognage en fonction de la couleur, indiquez la valeur 0 pour rogner les pixels seulement s’ils correspondent exactement à la couleur que vous avez sélectionnée dans l’angle du fichier PSD. Les valeurs qui se rapprochent de 1 admettent un plus grand écart des couleurs. Pour effectuer un rognage en fonction de la transparence, spécifiez 0 pour rogner les pixels uniquement s’ils sont transparents. Les valeurs plus proches de 1 permettent une plus grande transparence.

   * **[!UICONTROL Manuel]**  : permet d’entrer le nombre de pixels à recadrer d’un côté ou de chaque côté de l’image. La proportion de l’image qui est rognée dépend du paramètre ppp (pixels par pouce) défini dans le fichier d’image. Par exemple, si l’image affiche 150 ppp et que vous entrez 75 dans les zones de texte pour les bords supérieur, droit, inférieur et gauche, un demi-pouce est rogné de chaque côté de l’image.

* **Options de profil de couleurs**  : situées sous Options de profil de  **[!UICONTROL couleurs]**.

   * **[!UICONTROL Conservation des couleurs par défaut]**

   * **[!UICONTROL Conserver l’espace colorimétrique d’origine]**  : conserve l’espace colorimétrique d’origine de l’image.

   * **[!UICONTROL Personnaliser à partir de]**  >  **[!UICONTROL vers]**  : ouvre les menus afin que vous puissiez sélectionner un espace colorimétrique Convertir à partir de et Convertir en. Vous pouvez choisir un espace colorimétrique Photoshop standard ou un espace colorimétrique que vous avez chargé dans Adobe Dynamic Media Classic. (voir [Profils ICC](/help/icc-profiles.md)).

* **Options Photoshop**

   * **[!UICONTROL Conserver les calques]**  : extrait les calques du fichier PSD, le cas échéant, dans des ressources individuelles. Les calques de ces fichiers restent associés au fichier PSD. Vous pouvez les afficher en ouvrant le fichier PSD dans la vue Détails et en sélectionnant le panneau Calque. (voir Affichage et modification de calques d’un fichier PSD).

   * **[!UICONTROL Créer un modèle]**  : crée un modèle à partir des calques du fichier PSD.

   * **[!UICONTROL Extraire le texte]**  : extrait le texte afin que les utilisateurs puissent rechercher du texte dans une visionneuse.

   * **[!UICONTROL Etendre les calques à la taille de l’arrière-plan]**  : permet d’étendre la taille des calques d’image pixellisés à celle du calque d’arrière-plan.

   * **[!UICONTROL Affectation de nom de calque]**  : les calques du fichier PSD sont téléchargés en tant qu’images distinctes. Pour nommer ces images dans Adobe Dynamic Media Classic, choisissez l’une des options suivantes :

      * **[!UICONTROL Nom de calque]**  : nomme les images à la suite de leur nom de calque dans le fichier PSD. Par exemple, un calque appelé Etiquette de prix dans le fichier PSD d’origine devient une image nommée Etiquette de prix. Cependant, si les noms de calque dans le fichier PSD sont des noms de calque Photoshop par défaut (Arrière-plan, Calque 1, Calque 2, etc.), les images sont nommées d’après leurs numéros de calque dans le fichier PSD. <!-- not their default layer names -->

      * **[!UICONTROL Photoshop et numéro de calque]**  : attribue un nom aux images en fonction de leur numéro de calque dans le fichier PSD, en ignorant les noms de calque d’origine. Le nom des images est composé du nom de fichier Photoshop et d’un numéro de calque. Par exemple, le deuxième calque d’un fichier appelé `Spring Ad.psd` est nommé `Spring Ad_2` même s’il portait un nom autre que celui par défaut dans Photoshop.

      * **[!UICONTROL Photoshop et nom du calque]**  : nomme les images à la suite du fichier PSD suivi du nom ou du numéro du calque. Le numéro de calque est utilisé si le nom des calques dans le fichier PSD est un nom de calque Photoshop par défaut. Par exemple, un calque nommé `Price Tag` dans un fichier PSD nommé `SpringAd` est nommé `Spring Ad_Price Tag`. Un calque portant le nom par défaut Calque 2 est appelé `Spring Ad_2`.
   * **[!UICONTROL Ancre]**  : spécifiez le mode d’ancrage des images dans les modèles qui sont générés à partir de la composition en couches produite à partir du fichier PSD. Par défaut, l’ancrage est au centre. Un ancrage au centre permet aux images de remplacement de remplir de manière optimale le même espace, quelles que soient les proportions de l’image de remplacement. Les images qui remplacent cette image et qui présentent un aspect différent occupent le même espace lorsque le modèle est référencé et le paramètre de substitution utilisé. Changez de paramètre si votre application nécessite le remplacement d’images pour occuper l’espace alloué dans le modèle.


## Affichage et modification de calques dans un fichier PSD {#viewing-and-editing-layers-in-a-psd-file}

Si vous avez sélectionné l’option Conserver les calques lors du transfert de votre fichier PSD, Adobe Dynamic Media Classic les a tronqués dans des ressources. Vous pouvez afficher et modifier les calques de ressources appartenant à un fichier PSD en ouvrant le fichier dans le panneau de navigation de la vue Détails.

1. Double-cliquez sur le fichier PSD complet dans le panneau de navigation. Le fichier s’ouvre dans la vue Détails.

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
