---
title: Utiliser des fichiers PSD
description: Découvrez comment utiliser les fichiers PSD dans Adobe Dynamic Media Classic.
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

# Utiliser des fichiers PSD{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)**: Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on Web pages. -->

Les PSD (fichiers de document Photoshop) sont le plus souvent utilisés dans Adobe Dynamic Media Classic pour créer des modèles. Lorsque vous chargez un fichier PSD, vous pouvez créer automatiquement un modèle Adobe Dynamic Media Classic à partir de ce fichier (sélectionnez l’option Créer un modèle sur l’écran Charger).

Adobe Dynamic Media Classic crée plusieurs images à partir d’un fichier PSD avec des calques si vous utilisez le fichier pour créer un modèle ; il crée une image pour chaque calque.

## Options de téléchargement des fichiers PSD {#psd-upload-options}

Les options de chargement de fichiers PSD se trouvent sous Options Photoshop dans la boîte de dialogue Charger les options de la tâche. Vous pouvez recadrer un fichier, lui associer un profil de couleurs, l’utiliser pour créer un modèle et sélectionner un ancrage.

Les options suivantes sont disponibles au cours du téléchargement des fichiers PSD :

* **Options de recadrage** : se trouve sous **[!UICONTROL Options de recadrage]**. Sélectionnez **[!UICONTROL Rogner]** afin de recadrer automatiquement l’espace blanc sur les bords d’un fichier PSD. Sélectionnez **[!UICONTROL Manuel]** pour recadrer les côtés du fichier PSD :

   * **[!UICONTROL Rogner]** : sélectionnez le menu **[!UICONTROL Rogner en fonction de]** et choisissez **[!UICONTROL Couleur]** ou **[!UICONTROL Transparence]**.

  Si vous choisissez l’option **[!UICONTROL Couleur]**, sélectionnez le menu Coin et choisissez l’angle du PSD présentant la couleur qui représente le mieux l’espace blanc à rogner.

  Faites glisser le curseur pour définir une valeur de tolérance comprise entre 0 et 1. Pour effectuer le rognage en fonction de la couleur, indiquez la valeur 0 pour rogner les pixels seulement s’ils correspondent exactement à la couleur que vous avez sélectionnée dans l’angle du fichier PSD. Les valeurs qui se rapprochent de 1 admettent un plus grand écart des couleurs. Pour rogner en fonction de la transparence, spécifiez 0 pour rogner les pixels uniquement s’ils sont transparents ; les nombres plus proches de 1 permettent plus de transparence.

   * **[!UICONTROL Manuel]** : saisissez le nombre de pixels à recadrer de n’importe quel côté ou de chaque côté de l’image. La proportion de l’image qui est rognée dépend du paramètre ppp (pixels par pouce) défini dans le fichier d’image. Supposons, par exemple, que l’image affiche 150 ppp. Ensuite, saisissez 75 dans les zones de texte Haut, Droite, Bas et Gauche. Chaque côté de l’image est recadré, 0,5 pouce.

* **Options de profil colorimétrique** : se trouve sous **[!UICONTROL Options de profil colorimétrique]**.

   * **[!UICONTROL Conservation des couleurs par défaut]**

   * **[!UICONTROL Conserver l’espace colorimétrique d’origine]** : conserve l’espace colorimétrique d’origine de l’image.

   * **[!UICONTROL Personnaliser à partir de]** > **[!UICONTROL À]** : ouvre les menus afin que vous puissiez choisir un espace colorimétrique Convertir à partir de et Convertir en . Vous pouvez choisir un espace colorimétrique Photoshop standard ou un espace colorimétrique que vous avez téléchargé sur Adobe Dynamic Media Classic. (voir [Profils ICC](/help/using/icc-profiles.md)).

* **Options Photoshop**

   * **[!UICONTROL Conserver les calques]** : pixellise les calques du PSD, le cas échéant, en ressources individuelles. Les calques de ces fichiers restent associés au fichier PSD. Vous pouvez les afficher en ouvrant le fichier PSD dans le mode d’affichage Détail et en sélectionnant le panneau Calque. Voir Affichage et modification des calques dans un fichier PSD.

   * **[!UICONTROL Créer un modèle]** : permet de créer un modèle à partir des calques du fichier PSD.

   * **[!UICONTROL Extraire le texte]** : extrait le texte afin que les utilisateurs puissent rechercher du texte dans une visionneuse.

   * **[!UICONTROL Étendre les calques à la taille de l’arrière-plan]** : étend la taille des calques d’image pixellisés à celle du calque d’arrière-plan.

   * **[!UICONTROL Nommage de calque]** : les calques du fichier PSD sont chargés en tant qu’images distinctes. Pour nommer ces images dans Adobe Dynamic Media Classic, choisissez l’une des options suivantes :

      * **[!UICONTROL Nom de calque]** : les images adoptent le nom de leur calque dans le fichier PSD. Par exemple, un calque appelé Etiquette de prix dans le fichier PSD d’origine devient une image nommée Etiquette de prix. Toutefois, si les calques du fichier PSD portent le nom de calque Photoshop par défaut (Arrière-plan, Calque 1, Calque 2, etc.), les images sont nommées en fonction de leur numéro de calque dans le fichier PSD. <!-- not their default layer names -->

      * **[!UICONTROL Photoshop et numéro de calque]** : nomme les images d’après leur numéro de calque dans le fichier PSD, en ignorant les noms de calque d’origine. Le nom des images est composé du nom de fichier Photoshop et d’un numéro de calque. Par exemple, le deuxième calque d’un fichier appelé `Spring Ad.psd` est nommé `Spring Ad_2` même s’il portait un nom personnalisé dans Photoshop.

      * **[!UICONTROL Photoshop et nom de calque]** : nomme les images d’après le fichier PSD suivi du nom ou du numéro du calque. Le numéro de calque est utilisé si le nom des calques dans le fichier PSD est un nom de calque Photoshop par défaut. Par exemple, un calque nommé `Price Tag` dans un fichier PSD nommé `SpringAd` est nommé `Spring Ad_Price Tag`. Un calque portant le nom par défaut Calque 2 est appelé `Spring Ad_2`.

   * **[!UICONTROL Ancrer]** : indiquez comment les images sont ancrées dans les modèles générés à partir de la composition superposée générée à partir du fichier PSD. Par défaut, l’ancrage est au centre. Une ancre centrale permet de remplacer les images qui peuvent remplir au mieux le même espace, quel que soit le format de l’image de remplacement. Les images qui remplacent cette image et qui présentent un aspect différent occupent le même espace lorsque le modèle est référencé et le paramètre de substitution utilisé. Changez de paramètre si votre application nécessite le remplacement d’images pour occuper l’espace alloué dans le modèle.

## Affichage et modification des calques dans un fichier PSD {#viewing-and-editing-layers-in-a-psd-file}

Si vous avez sélectionné l’option **[!UICONTROL Conserver les calques]** lors du chargement de votre PSD, Adobe Dynamic Media Classic a pixellisé les calques individuels dans les ressources. Vous pouvez afficher et modifier les calques de ressources appartenant à un fichier PSD en ouvrant le fichier dans le panneau Parcourir dans l’affichage des détails.

>[!NOTE]
>
>Adobe Dynamic Media Classic prend en charge jusqu’à cinq niveaux dans un groupe de calques imbriqués.

1. Double-cliquez sur le fichier PSD complet dans le panneau Parcourir . Le fichier s’ouvre dans la vue Détail.

   >[!NOTE]
   >
   >veillez à ouvrir le fichier complet et non l’un des calques PSD.

1. Sélectionnez **[!UICONTROL Calques]**. Le panneau Calques affiche tous les calques sous la forme d’images distinctes.
1. Double-cliquez sur un calque et effectuez l’une des opérations suivantes :

   * Pour créer une zone cliquable sur le calque, sélectionnez l’icône **[!UICONTROL Zone cliquable]**. (Voir [Création de zones cliquables](creating-image-maps.md#creating_image_maps).)
   * Pour créer des cibles de zoom sur le calque, sélectionnez l’icône **[!UICONTROL Cibles de zoom]**. (Voir [Création de cibles de zoom pour le zoom guidé](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * Pour recadrer le calque, sélectionnez l’icône **[!UICONTROL Recadrer]**. (Voir [Recadrer une image](cropping-image.md#cropping_an_image).)
   * Pour accentuer le calque, sélectionnez **[!UICONTROL Accentuer]**. (Voir [Accentuer une image](sharpening-image.md#sharpening_an_image).)
   * Pour ajuster le calque, sélectionnez **[!UICONTROL Ajuster]**. (Voir [Réglage d’une image](adjusting-image.md#adjusting_an_image).)

1. Sélectionnez **[!UICONTROL Enregistrer]** ou **[!UICONTROL Enregistrer sous]**.
1. Pour afficher ou modifier un autre calque, sélectionnez une flèche au bas de l’aperçu du calque.
1. Pour quitter l’affichage des détails du calque, sélectionnez l’icône **[!UICONTROL vue Grille]**.
