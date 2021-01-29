---
title: '"Démarrage rapide : Zoom"'
description: Une introduction et un Début rapide pour effectuer un zoom pour vous aider à maîtriser rapidement les opérations.
uuid: 31eda632-3469-4f90-885b-e90c6a2e5e75
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 559c986d-313d-46df-a5ff-0b49316ad3a7
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 64%

---


# Démarrage rapide : Zoom{#quick-start-zoom}

Le zoom vous permet de vue interactive des détails haute résolution dans les images. Vous pouvez, par exemple, voir les couleurs, les options, les angles et les détails d’une image dans une visionneuse intégrée, entièrement configurable et dynamique. Cette visionneuse peut être incorporée à une page Web ou s’afficher dans une fenêtre contextuelle. Vous pouvez examiner des images de près et effectuer un panoramique à des résolutions élevées pour les inspecter en détail. La fonction de zoom permet à vos clients de bénéficier d’une expérience de visualisation plus interactive, instructive et dynamique. 

Dynamic Media Classic offre également le zoom guidé, qui vous permet de mettre en évidence les fonctions importantes d’une image. Vous pouvez par exemple créer une cible de zoom pour un logo afin d’attirer l’attention des utilisateurs sur ce dernier. Lorsque les utilisateurs cliquent sur cette cible de zoom, ils effectuent un zoom sur le logo.

Toutes les images de zoom sont créées et servies à partir d’images originales uniques, de graphiques et d’attributs gérés par des bases de données. La fonction de zoom de Dynamic Media Classic réduit considérablement le temps et les coûts de production et de diffusion des images. Vous pouvez utiliser les visionneuses de zoom pour effectuer un zoom avant ou arrière sur les images. La visionneuse de zoom comporte des boutons sur lesquels il suffit de cliquer pour effectuer un zoom et un panoramique ; à cela s’ajoute la possibilité d’effectuer un panoramique par glissement sur l’écran. Des paramètres prédéfinis de visionneuse de zoom permettent de configurer la visionneuse utilisée pour effectuer un zoom sur les images.

**Début rapide**

Ce Début de zoom rapide est conçu pour vous aider à maîtriser rapidement les techniques de zoom dans Dynamic Media Classic. Suivez les étapes 1 à 6. Chaque étape se termine par un renvoi à une rubrique contenant de plus amples informations.

**1. Téléchargement des images de zoom**

Début en téléchargeant vos images de zoom vers Dynamic Media Classic. Pour un zoom optimal, Dynamic Media Classic recommande que les images fassent au moins 2 000 pixels dans la dimension la plus longue.

Sélectionnez le bouton Télécharger de la barre de navigation globale pour télécharger des images depuis votre ordinateur ou votre réseau vers un dossier de Dynamic Media Classic. (voir [Téléchargement des images de zoom](uploading-zoom-images.md#uploading_zoom_images)).

**2. Création de cibles de zoom pour un zoom guidé**

Les cibles de zoom vous permettent de mettre en valeur des sections particulières d’une image. Vous pouvez, par exemple, attirer l’attention des utilisateurs sur les sections d’une image qui la caractérisent ou la distinguent. Les cibles de zoom s’affichent sous la forme de miniatures, à côté de l’image, dans la fenêtre de la visionneuse de zoom. La sélection d’une de ces miniatures de cible de zoom permet d’effectuer un zoom automatique sur la section de l’image que vous définissez.

Pour créer une cible de zoom, cliquez sur le bouton de modification en survol et choisissez Cibles de zoom ou ouvrez une image dans le panneau de navigation de la vue de détails, puis cliquez sur Cibles de zoom. Utilisez ensuite les outils de zoom disponibles sur l’écran de l’éditeur de cible de zoom pour définir une partie de l’image comme cible (voir [Création de cibles de zoom pour un zoom guidé](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom)).

**Cookie. Configuration des paramètres prédéfinis de la visionneuse de zoom**

Les paramètres prédéfinis de visionneuse de zoom déterminent le style et le comportement des visionneuses de zoom. Vous pouvez configurer des paramètres prédéfinis de visionneuse de zoom si vous êtes administrateur ; Dynamic Media Classic est également fourni avec les paramètres prédéfinis par défaut de la visionneuse de zoom &quot;Meilleure pratique&quot;.

Pour créer un paramètre prédéfini de visionneuse de zoom, cliquez sur le bouton Configuration dans la barre de navigation globale et choisissez Paramètres prédéfinis de la visionneuse. Ensuite, sur l’écran Paramètres prédéfinis de la visionneuse, cliquez sur le bouton Ajouter, choisissez une plate-forme, choisissez une visionneuse de zoom, puis cliquez sur Ajouter. Ensuite, sélectionnez des options sur l’écran Configurer la visionneuse 

Les options de paramètre prédéfini de visionneuse de zoom des offres Dynamic Media Classic vous permettent de sélectionner le style de bouton et l’aspect général de la visionneuse. Vous avez également la possibilité de personnaliser les paramètres de zoom pour votre site Web (voir [Configuration des paramètres prédéfinis de la visionneuse de zoom](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets)).

**4. Prévisualisation des images avec la visionneuse de zoom**

Vous pouvez prévisualiser des images dans une visionneuse de zoom afin de vérifier le résultat obtenu lorsque vous effectuez un zoom sur les images.

Pour faire des essais avec divers paramètres prédéfinis de visionneuse de zoom, choisissez une image dans le panneau de navigation, puis cliquez sur le bouton Prévisualiser. L’écran Prévisualiser s’ouvre. Choisissez la commande Paramètres prédéfinis > Zoom, puis sélectionnez un paramètre prédéfini avec les menus Zoom.

Les boutons de zoom apparaissent. Vous pouvez alors vérifier l’aspect des images de zoom sur votre site Web. Sélectionnez les boutons de zoom (et les cibles de zoom) pour tester le paramètre prédéfini de visionneuse de zoom choisi (voir [Prévisualisation d’images avec différentes visionneuses de zoom](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers)).

**5. Publication des images de zoom**

Lorsque vous publiez vos images de zoom, elles sont placées sur les serveurs Dynamic Media Image Server afin d’être diffusées sur votre site Web et dans votre application. Dans le cadre du processus de publication, Dynamic Media Classic active les chaînes URL. Ces chaînes URL appellent des images de zoom des serveurs Dynamic Media Image Server vers votre site Web ou votre application.

Cliquez sur le bouton Publier de la barre de navigation globale pour lancer une publication. Dans l’écran de publication qui s’affiche, cliquez sur le bouton Lancer publication (voir [Publication des images de zoom](publishing-zoom-images.md#publishing_zoom_images)).

**6. Liaison des visionneuses de zoom à une page Web**

Dynamic Media Classic crée les chaînes d’appel URL nécessaires pour zoomer sur les images et les active lorsque vous publiez des images sur les serveurs Dynamic Media Image Server. Vous pouvez copier ces chaînes URL depuis l’écran Prévisualiser. Une fois copiées, les chaînes URL peuvent être utilisées dans vos applications et sur vos sites Web (voir [Liaison des visionneuses de zoom à une page Web](linking-zoom-viewers-web-pages.md#linking_zoom_viewers_to_your_web_pages)).
