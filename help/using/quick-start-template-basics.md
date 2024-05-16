---
title: "Démarrage rapide : notions de base des modèles"
description: Présentation et démarrage rapide des concepts de base des modèles pour vous aider à démarrer rapidement dans Adobe Dynamic Media Classic.
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

Les concepts de base des modèles sont des fichiers d’images créés dynamiquement et superposés de manière adressable, tels que des fichiers superposés dans des applications de retouche d’images telles qu’Adobe Photoshop. Contrairement à un fichier statique contenant des calques, par exemple un fichier PSD, un modèle peut comporter des paramètres. C’est grâce à ces paramètres que les différents aspects de l’image peuvent être traités et personnalisés.

Un modèle peut contenir n’importe quel nombre de calques d’image et de texte. Vous pouvez convertir un fichier statique contenant des calques, tels qu’un fichier de PSD superposé, en modèle, puis créer des modèles dans Adobe Dynamic Media Classic. Vous pouvez créer des calques de texte dans les modèles à l’aide des polices que vous avez téléchargées dans Adobe Dynamic Media Classic. Après avoir ajouté du texte à un modèle, vous pouvez le mettre en forme en modifiant sa justification, sa police, sa taille et sa couleur.

La page Paramètres vous permet de convertir n’importe quel aspect d’un modèle en paramètre adressable. Ce faisant, vous pouvez modifier l’image superposée à utiliser ou la valeur de texte à utiliser dans votre modèle. Les paramètres sont transmis avec la chaîne URL, ce qui vous permet de modifier n’importe quel paramètre afin que vous puissiez personnaliser dynamiquement l’image de réponse générée à partir du serveur d’images.

Voir aussi [Concepts de base des modèles](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) vidéo de formation.

Ce didacticiel de mise en route est conçu pour vous aider à maîtriser rapidement les opérations liées aux concepts de base des modèles.

## 1. Télécharger les fichiers

Commencez par télécharger le fichier PSD ou le fichier d’image de votre modèle. Adobe Dynamic Media Classic prend en charge de nombreux formats de fichier image en plus du PSD, mais les images TIFF sans perte et PNG sont recommandées pour les modèles, car elles permettent une transparence.

Si vous utilisez un fichier de PSD pour créer votre modèle, sélectionnez **[!UICONTROL Créer un modèle]** dans le **[!UICONTROL Télécharger les options de la tâche]** lorsque vous chargez le fichier de PSD. Sélectionnez également une **[!UICONTROL Nom de calque]** pour qu’Adobe Dynamic Media Classic sache comment nommer les calques de PSD lorsqu’ils sont chargés dans Adobe Dynamic Media Classic.

Si vous utilisez des fichiers image, vous pouvez recadrer les images et créer également un masque à partir des chemins de détourage dans les images au fur et à mesure de leur téléchargement.

Dans la barre de navigation globale, sélectionnez **[!UICONTROL Télécharger]** pour télécharger un fichier de PSD ou d’autres fichiers image de votre ordinateur vers un dossier sur Adobe Dynamic Media Classic. Voir [Chargement des fichiers de modèle](uploading-template-files.md#uploading_template_files).

## 2. Créer un modèle

Pour créer un modèle à partir d’un fichier de PSD, sélectionnez **[!UICONTROL Créer un modèle]** lorsque vous téléchargez le fichier. Pour créer un modèle à partir d’images, dans la barre de navigation globale, accédez à **[!UICONTROL Build]** > **[!UICONTROL Concepts de base des modèles]**, saisissez une mesure de largeur et de hauteur pour la zone de travail. Dans le coin supérieur droit de la page, sélectionnez l’une des options suivantes : **[!UICONTROL Designer]** ou **[!UICONTROL Développeur]**, puis faites glisser les images sur la page Modèle . Vous pouvez également sélectionner les images. *before* vous accédez à **[!UICONTROL Build]** > **[!UICONTROL Concepts de base des modèles]**. La page Modèle contient des outils pour :

* Ajout de calques d’images Pour ajouter un calque, faites glisser une image sur la page Modèle.
* Ajout de calques de texte Sélectionnez la variable **[!UICONTROL Outil Texte]** Icône Faites glisser le pointeur pour créer une zone pour le calque de texte, puis formatez le texte à l’aide des outils de la page Texte.
* Modification de la taille et de la position des calques
* Modification de l’ordre des calques
* Application d’effets d’ombre et d’éclat aux calques d’image et de texte 

Voir [Créer un modèle](creating-template.md#creating_a_template).

## 3. Création de paramètres de modèle

L’étape suivante consiste à paramétrer les propriétés sur les calques pour déterminer les propriétés de calque à inclure dans la chaîne URL. Les paramètres permettent de manipuler les modèles avec une souplesse optimale. Après avoir transformé une propriété de calque en paramètre, vous pouvez le modifier dynamiquement.

Pour paramétrer un calque, ouvrez le modèle dans la page Modèle, puis sélectionnez **[!UICONTROL Paramètres]** en regard d’un nom de calque. Sur la page Paramètres , sélectionnez l’option en regard de chaque paramètre à ajouter. Voir [Créer des paramètres de modèle](creating-template-parameters.md#creating_template_parameters).

## 4. Publier des modèles

Lorsque vous publiez votre modèle, il est placé sur les serveurs d’images Dynamic Media afin de pouvoir être diffusé dynamiquement sur votre site web ou dans votre application. La publication active également l’URL pour appeler le modèle à partir des serveurs Dynamic Media Image Server vers votre site Web ou votre application.

Assurez-vous de publier toutes les images associées à votre modèle.

Pour publier un modèle, marquez-le pour publication puis, sur la barre de navigation globale, sélectionnez **[!UICONTROL Publier]**. Sélectionnez **[!UICONTROL Envoyer la publication]**. Voir [Publication de modèles](publishing-templates.md#publishing_templates).

## 5. Associer un modèle à une page Web

Dynamic Media Classic crée des URL pour les modèles et les active lorsque vous publiez des modèles sur les serveurs d’images Dynamic Media. Vous pouvez copier ces chaînes URL à partir de la page Aperçu du modèle .

Sélectionnez votre modèle dans le panneau Parcourir, puis sélectionnez **[!UICONTROL Aperçu]** pour ouvrir la page Aperçu du modèle . Sélectionnez un paramètre d’image prédéfini pour la diffusion de votre modèle, puis cliquez sur le bouton **[!UICONTROL Copier l’URL]** bouton . Après avoir copié l’URL à partir de la page Aperçu, vous pouvez l’utiliser dans votre site Web ou application. Voir [Associer un modèle à une page Web](linking-template-web-page.md#linking_a_template_to_a_web_page).
