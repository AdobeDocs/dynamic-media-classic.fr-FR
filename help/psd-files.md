---
title: Utilisation de fichiers PSD
seo-title: Utilisation de fichiers PSD
description: 'null'
seo-description: Découvrez comment travailler avec des fichiers PSD.
uuid: 5836 b 660-6 bca -46 e 7-ab 39-1 a 31 d 1 e 0 cff 2
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/master_ files
discoiquuid: 4086 e 3 db -5 aca -41 a 0-8 f 15-302 afbf 67 ddb
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Utilisation de fichiers PSD{#working-with-psd-files}

Les fichiers PSD (Photoshop Document Files) sont généralement utilisés dans Dynamic Media Classic pour créer des modèles. Lorsque vous téléchargez un fichier PSD, vous pouvez créer un modèle Dynamic Media Classic automatiquement à partir du fichier (sélectionnez l'option Créer un modèle sur l'écran Télécharger).

Le système SPS crée plusieurs images à partir d’un fichier PSD avec des calques si vous utilisez le fichier pour créer un modèle. Il crée une image par calque.

## Options de téléchargement des fichiers PSD {#psd-upload-options}

Les options de téléchargement des fichiers PSD sont accessibles via les options Photoshop, dans Télécharger les options de la tâche. Vous pouvez recadrer un fichier, lui associer un profil de couleurs, l’utiliser pour créer un modèle et sélectionner un ancrage.

Les options suivantes sont disponibles au cours du téléchargement des fichiers PSD :

**Recadrage** (situé sous Options de recadrage). Choisissez l’option Rognage pour supprimer automatiquement l’espace blanc des bords d’un fichier PSD. Choisissez l’option Manuel pour rogner les côtés du fichier PSD :

**Rogner** le menu Rogner en fonction de, puis choisissez Couleur ou Transparence.

Si vous optez pour l’option Couleur, sélectionnez le menu Coin, puis choisissez l’angle du fichier PSD présentant la couleur qui représente le mieux la couleur de l’espace blanc à rogner.

Faites glisser le curseur pour définir une valeur de tolérance comprise entre 0 et 1 :

Pour effectuer le rognage en fonction de la couleur, indiquez la valeur 0 pour rogner les pixels seulement s’ils correspondent exactement à la couleur que vous avez sélectionnée dans l’angle du fichier PSD. Les valeurs qui se rapprochent de 1 admettent un plus grand écart des couleurs.

Pour effectuer le rognage en fonction de la transparence, indiquez 0 pour rogner les pixels seulement s’ils sont entièrement transparents. Les valeurs plus proches de 1 permettent une plus grande transparence.

**Manuel** Entrez le nombre de pixels à rogner d'un côté ou de chaque côté de l'image. La proportion de l’image qui est rognée dépend du paramètre ppp (pixels par pouce) défini dans le fichier d’image. Par exemple, si l’image affiche 150 ppp et que vous entrez 75 dans les zones de texte pour les bords supérieur, droit, inférieur et gauche, un demi-pouce est rogné de chaque côté de l’image.

**Profil de couleurs** (situé sous Options de profil de couleurs). Choisissez une option :

**Convertir en srvb (par défaut)** Convertit en srvb (rouge vert vert standard). sRVB est l’espace colorimétrique recommandé pour l’affichage d’images sur les pages Web.

**Conserver l'espace colorimétrique original** Conserve l'espace colorimétrique d'origine de l'image.

**Personnalisé De &gt; Pour** ouvrir les menus, vous pouvez choisir un espace colorimétrique Convertir à partir de et Convertir en couleurs. Vous pouvez choisir un espace colorimétrique Photoshop standard ou un espace colorimétrique téléchargé sur SPS (voir Profils ICC).

**Conserver les calques** pixellise les calques du fichier PSD, le cas échéant, dans des fichiers individuels. Les calques de ces fichiers restent associés au fichier PSD. Pour les afficher, ouvrez le fichier PSD dans l’affichage Détail et sélectionnez le panneau Calque (voir Affichage et modification de calques d’un fichier PSD).

**Créer un modèle** Crée un modèle à partir des calques du fichier PSD.

**Extraire le texte** extrait le texte afin que les utilisateurs puissent rechercher du texte dans une visionneuse.

**Etendre les calques à la taille** d'arrière-plan Etend la taille des calques d'image pixellisés à la taille du calque d'arrière-plan.

**Les** calques de nommage de calques du fichier PSD sont téléchargés sous forme d'images distinctes. Choisissez une option pour nommer ces images dans Scene7 Publishing System :

**Nom de calque** Nomme les images après leur nom de calque dans le fichier PSD. Par exemple, un calque appelé Etiquette de prix dans le fichier PSD d’origine devient une image nommée Etiquette de prix. Cependant, si les calques du fichier PSD portent les noms de calques Photoshop par défaut (Arrière-plan, Calque 1, Calque 2, etc.), les images sont nommées d’après leur numéro de calque dans le fichier PSD, et non leur nom par défaut.

**Photoshop et le numéro de couche** nomme les images après leur numéro de calque dans le fichier PSD, en ignorant les noms de calques d'origine. Le nom des images est composé du nom de fichier Photoshop et d’un numéro de calque. Par exemple, le deuxième calque d’un fichier appelé Pub printemps.psd est nommé Pub printemps_2 même s’il portait un nom dans Photoshop non défini par défaut.

**Nom de Photoshop et de calque** Nom des images après le fichier PSD suivi du nom du calque ou du numéro de calque. Le numéro de calque est utilisé si le nom des calques dans le fichier PSD est un nom de calque Photoshop par défaut. Par exemple, un calque nommé Etiquette de prix dans un fichier PSD appelé PubPrintemps est nommé PubPrintemps_Etiquette de prix. Un calque portant le nom par défaut Calque 2 est nommé Pub Printemps_2.

**Ancrage** de l'ancrage des images dans les modèles générés à partir de la composition superposée produite à partir du fichier PSD. Par défaut, l’ancrage est au centre. Un ancrage au centre permet aux images de remplacement de remplir de manière optimale le même espace, quelles que soient les proportions de l’image de remplacement. Les images qui remplacent cette image et qui présentent un aspect différent occupent le même espace lorsque le modèle est référencé et le paramètre de substitution utilisé. Changez de paramètre si votre application nécessite le remplacement d’images pour occuper l’espace alloué dans le modèle.

## Affichage et modification de calques d’un fichier PSD {#viewing-and-editing-layers-in-a-psd-file}

Si vous avez sélectionné l'option Conserver les calques lorsque vous avez téléchargé votre fichier PSD, Dynamic Media Classic pixellise les calques individuels dans des fichiers. Pour afficher et modifier les calques de fichier appartenant à un fichier PSD, ouvrez le fichier dans le panneau de navigation en mode Affichage des détails.

1. Cliquez deux fois sur le fichier PSD complet dans le panneau de navigation pour l’ouvrir en mode Affichage des détails.

   ***remarque**: Assurez-vous d'ouvrir le fichier complet et non l'un des calques PSD.*

1. Cliquez sur Calques pour ouvrir le panneau Calques. Le panneau Calques affiche tous les calques sous la forme d’images distinctes.
1. Cliquez deux fois sur un calque pour l’ouvrir, puis effectuez l’une des opérations suivantes :

   * Cliquez sur l’icône Zone cliquable pour créer une zone de ce type sur le calque (voir [Création de zones cliquables](creating-image-maps.md#creating_image_maps)).
   * Cliquez sur l’icône Cibles de zoom pour créer de telles cibles sur le calque (voir [Création de cibles de zoom pour un zoom guidé](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom)).
   * Cliquez sur l’icône Recadrer pour recadrer le calque (voir [Recadrage d’une image](cropping-image.md#cropping_an_image)).
   * Cliquez sur Accentuer pour accentuer le calque (voir [Accentuation d’une image](sharpening-image.md#sharpening_an_image)).
   * Cliquez sur Modifier pour régler le calque (voir [Modification d’une image](adjusting-image.md#adjusting_an_image)).

1. Cliquez sur Enregistrer ou Enregistrer sous.
1. Pour afficher ou modifier un autre calque, cliquez sur la flèche située au bas de l’aperçu des calques.
1. Pour quitter le mode Affichage des détails du calque, cliquez sur l’icône Affichage de la grille.

