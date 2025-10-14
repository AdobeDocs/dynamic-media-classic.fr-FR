---
title: 'Démarrage rapide : Concepts de base des modèles'
description: Une introduction et un démarrage rapide des bases des modèles pour vous aider à démarrer rapidement dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 17%

---

# Démarrage rapide : Concepts de base des modèles{#quick-start-template-basics}

Les fichiers de base de modèle sont créés et adressables dynamiquement à l’aide de fichiers image superposés, comme les fichiers superposés dans les applications d’édition d’images telles qu’Adobe Photoshop. Contrairement à un fichier statique contenant des calques, par exemple un fichier PSD, un modèle peut comporter des paramètres. C’est grâce à ces paramètres que les différents aspects de l’image peuvent être traités et personnalisés.

Un modèle peut contenir n’importe quel nombre de calques d’image et de texte. Vous pouvez convertir un fichier statique contenant des calques, tel qu’un fichier PSD superposé, en modèle, puis créer des modèles dans Adobe Dynamic Media Classic. Vous pouvez créer des calques de texte dans les modèles à l’aide des polices que vous avez chargées dans Adobe Dynamic Media Classic. Après avoir ajouté du texte à un modèle, vous pouvez le mettre en forme en modifiant sa justification, sa police, sa taille de police et sa couleur.

La page Paramètres vous permet de convertir n’importe quel aspect d’un modèle en paramètre adressable. Ce faisant, vous pouvez modifier l’image superposée à utiliser ou la valeur de texte à utiliser dans votre modèle. Les paramètres sont transmis avec la chaîne d’URL, ce qui vous permet de modifier n’importe quel paramètre afin de personnaliser dynamiquement l’image de réponse générée à partir du serveur d’images.

Consultez également la vidéo de formation [Principes de base des modèles](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS).

Ce démarrage rapide est conçu pour vous aider à maîtriser rapidement les bases des modèles.

## &#x200B;1. Chargez les fichiers

Commencez par télécharger le fichier PSD ou le fichier d’image de votre modèle. Adobe Dynamic Media Classic prend en charge de nombreux formats de fichiers image en plus de PSD, mais les images TIFF et PNG sans perte sont recommandées pour les modèles, car elles assurent la transparence.

Si vous utilisez un fichier PSD pour créer votre modèle, sélectionnez **[!UICONTROL Créer un modèle]** dans la boîte de dialogue **[!UICONTROL Charger les options de la tâche]** lorsque vous chargez le fichier PSD. Choisissez également une option **[!UICONTROL Dénomination de calque]** afin qu’Adobe Dynamic Media Classic sache comment nommer les calques PSD lorsqu’ils sont chargés vers Adobe Dynamic Media Classic.

Si vous utilisez des fichiers d’image, vous pouvez recadrer les images et également créer un masque à partir des tracés d’écrêtage des images au fur et à mesure de leur chargement.

Sur la barre de navigation générale, sélectionnez **[!UICONTROL Télécharger]** pour télécharger un fichier PSD ou d’autres fichiers image de votre ordinateur vers un dossier d’Adobe Dynamic Media Classic. Voir [Charger des fichiers de modèle](uploading-template-files.md#uploading_template_files).

## &#x200B;2. Créer un modèle

Pour créer un modèle à partir d’un fichier PSD, sélectionnez **[!UICONTROL Créer un modèle]** lorsque vous chargez le fichier. Pour créer un modèle à partir d’images, sur la barre de navigation globale, accédez à **[!UICONTROL Créer]** > **[!UICONTROL Principes de base des modèles]**, puis saisissez une mesure de largeur et de hauteur pour la zone de travail. Dans le coin supérieur droit de la page, sélectionnez **[!UICONTROL Designer]** ou **[!UICONTROL Développeur]**, puis faites glisser les images sur la page Modèle. Vous pouvez également sélectionner les images *avant* vous accédez à **[!UICONTROL Créer]** > **[!UICONTROL Principes de base des modèles]**. La page Modèle propose des outils pour :

* Ajout de calques d’images Pour ajouter un calque, faites glisser une image dans la page Modèle.
* Ajout de calques de texte Sélectionnez l’icône **[!UICONTROL Outil Texte]**. Faites glisser le pointeur pour créer une zone pour le calque de texte, puis mettez en forme le texte avec des outils sur la page de texte.
* Modification de la taille et de la position des calques
* Modification de l’ordre des calques
* Application d’effets d’ombre et d’éclat aux calques d’image et de texte 

Voir [Création d’un modèle](creating-template.md#creating_a_template).

## &#x200B;3. Créer des paramètres de modèle

L’étape suivante consiste à paramétrer les propriétés sur les calques pour déterminer les propriétés de calque à inclure dans la chaîne URL. Les paramètres permettent de manipuler les modèles avec une souplesse optimale. Après avoir transformé une propriété de calque en paramètre, vous pouvez le modifier dynamiquement.

Pour paramétrer un calque, ouvrez le modèle dans la page Modèle, puis sélectionnez **[!UICONTROL Paramètres]** en regard d’un nom de calque. Sur la page Paramètres , sélectionnez l’option en regard de chaque paramètre à ajouter. Voir [Création de paramètres de modèle](creating-template-parameters.md#creating_template_parameters).

## &#x200B;4. Publier des modèles

La publication de votre modèle le place sur les serveurs d’images Dynamic Media afin qu’il puisse être diffusé dynamiquement sur votre site web ou application. La publication active également l’URL pour appeler le modèle depuis les serveurs d’images Dynamic Media vers votre site web ou application.

Assurez-vous de publier toutes les images associées à votre modèle.

Pour publier un modèle, marquez-le pour publication et, sur la barre de navigation générale, sélectionnez **[!UICONTROL Publier]**. Sélectionnez ensuite **[!UICONTROL Envoyer la publication]**. Voir [&#x200B; Publication de modèles &#x200B;](publishing-templates.md#publishing_templates).

## &#x200B;5. Lier un modèle à une page Web

Dynamic Media Classic crée des URL pour les modèles et les active lorsque vous publiez des modèles sur les serveurs d’images Dynamic Media. Vous pouvez copier ces chaînes d’URL à partir de la page d’aperçu du modèle.

Sélectionnez votre modèle dans le panneau de navigation, puis sélectionnez **[!UICONTROL Aperçu]** pour ouvrir la page d’aperçu du modèle. Sélectionnez un paramètre d’image prédéfini pour diffuser votre modèle, puis cliquez sur le bouton **[!UICONTROL Copier l’URL]**. Après avoir copié l’URL à partir de la page d’aperçu, vous pouvez l’utiliser dans votre site web ou application. Voir [Lier un modèle à une page web](linking-template-web-page.md#linking_a_template_to_a_web_page).
