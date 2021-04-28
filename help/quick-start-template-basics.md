---
title: '"Démarrage rapide : Concepts de base des modèles"'
description: Une introduction et un Début rapide aux concepts de base des modèles pour vous aider à maîtriser rapidement les opérations.
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
feature: Dynamic Media Classic
role: Business Practitioner
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
translation-type: tm+mt
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 34%

---

# Démarrage rapide : Concepts de base des modèles{#quick-start-template-basics}

Les concepts de base des modèles sont des fichiers d’image créés dynamiquement et superposés de manière adressable, tels que des fichiers superposés dans des applications de retouche d’images telles que Adobe Photoshop. Contrairement à un fichier statique contenant des calques, par exemple un fichier PSD, un modèle peut comporter des paramètres. C’est grâce à ces paramètres que les différents aspects de l’image peuvent être traités et personnalisés.

Un modèle peut contenir n’importe quel nombre de calques d’image et de texte. Vous pouvez convertir un fichier statique contenant des calques, tel qu’un fichier PSD superposé, en modèle et créer des modèles dans Dynamic Media Classic. Vous pouvez créer des calques de texte dans des modèles à l’aide de polices que vous avez téléchargées dans Dynamic Media Classic. Une fois que vous avez ajouté du texte à un modèle, vous pouvez le mettre en forme en modifiant la justification, les polices, le corps des caractères et la couleur.

La page Paramètres vous permet de convertir n’importe quel aspect d’un modèle en paramètre adressable. Ainsi, vous pouvez sélectionner l’image superposée ou la valeur du texte à utiliser dans votre modèle. Les paramètres sont transmis avec la chaîne URL, ce qui vous permet de modifier n’importe quel paramètre afin de personnaliser dynamiquement l’image de réponse générée à partir du serveur d’images.

Cette section de démarrage rapide est conçue pour aider à maîtriser rapidement les opérations liées aux concepts de base des modèles. 

## 1. Téléchargement des fichiers

Commencez par télécharger le fichier PSD ou le fichier d’image de votre modèle. Dynamic Media Classic prend en charge de nombreux formats de fichier d’images en plus du PSD, mais les images TIFF et PNG sans perte sont recommandées pour les modèles car elles permettent la transparence.

Si vous utilisez un fichier PSD pour créer votre modèle, sélectionnez **[!UICONTROL Créer un modèle]** dans la boîte de dialogue **[!UICONTROL Télécharger les options de la tâche]** lorsque vous téléchargez le fichier PSD. Choisissez également une option **[!UICONTROL Affectation de nom de calque]** pour que Dynamic Media Classic sache comment nommer les calques PSD lorsqu’ils sont téléchargés vers Dynamic Media Classic.

Si vous utilisez des fichiers d’images, vous pouvez recadrer les images et créer également un masque à partir des chemins de tracé dans les images au cours du téléchargement.

Sur la barre de navigation globale, cliquez sur **[!UICONTROL Télécharger]** pour télécharger un fichier PSD ou d’autres fichiers d’image depuis votre ordinateur vers un dossier de Dynamic Media Classic. (voir [Téléchargement des fichiers de modèle](uploading-template-files.md#uploading_template_files)).

## 2. Création d’un modèle

Pour créer un modèle à partir d’un fichier PSD, sélectionnez **[!UICONTROL Créer un modèle]** lorsque vous téléchargez le fichier. Pour créer un modèle à partir d’images, sur la barre de navigation globale, cliquez sur **[!UICONTROL Créer]** > **[!UICONTROL Concepts de base des modèles]**, puis entrez une mesure de largeur et de hauteur pour la zone de travail. Près du coin supérieur droit de la page, sélectionnez **[!UICONTROL Designer]** ou **[!UICONTROL Développeur]**, puis faites glisser les images sur la page Modèle. Vous pouvez également sélectionner les images *avant* de cliquer sur **[!UICONTROL Créer]** > **[!UICONTROL Concepts de base des modèles]**. La page Modèle offre les outils pour :

* Ajout de calques d’images Pour ajouter un calque, faites glisser une image dans la page Modèle.
* Ajout de calques de texte Cliquez sur l&#39;icône **[!UICONTROL Outil Texte]**. Faites glisser le pointeur pour créer une zone pour le calque de texte ; puis formater le texte avec des outils sur la page Texte.
* Modification de la taille et de la position des calques
* Modification de l’ordre des calques
* Application d’effets d’ombre et d’éclat aux calques d’image et de texte 

Voir [Création d’un modèle](creating-template.md#creating_a_template).

## 3. Création de paramètres de modèle

L’étape suivante consiste à paramétrer les propriétés sur les calques pour déterminer les propriétés de calque à inclure dans la chaîne URL. Les paramètres permettent de manipuler les modèles avec une souplesse optimale. Après avoir transformé une propriété de calque en paramètre, vous pouvez le modifier dynamiquement.

Pour paramétrer un calque, ouvrez le modèle dans la page Modèle, puis cliquez sur **[!UICONTROL Paramètres]** en regard d’un nom de calque. Sur la page Paramètres, sélectionnez l’option en regard de chaque paramètre à ajouter. (voir [Création de paramètres de modèle](creating-template-parameters.md#creating_template_parameters)).

## 4. Publication de modèles

Lorsque vous publiez votre modèle, il est placé sur les serveurs Dynamic Media Image Server afin de pouvoir être diffusé dynamiquement sur votre site Web ou dans votre application. La publication active également l’URL pour appeler le modèle à partir des serveurs Dynamic Media Image Server vers votre site Web ou votre application.

Assurez-vous de publier toutes les images associées à votre modèle.

Pour publier un modèle, marquez-le pour publication et sur la barre de navigation globale, cliquez sur **[!UICONTROL Publier]**. Cliquez ensuite sur **[!UICONTROL Envoyer la publication]**. (voir [Publication de modèles](publishing-templates.md#publishing_templates)).

## 5. Liaison d’un modèle à une page Web

Dynamic Media Classic crée des URL pour les modèles et les active lorsque vous publiez des modèles sur les serveurs Dynamic Media Image Server. Vous pouvez copier ces chaînes URL à partir de la page Prévisualisation de modèles.

Sélectionnez votre modèle dans le panneau de navigation, puis cliquez sur **[!UICONTROL Prévisualisation]** pour ouvrir la page Prévisualisation de modèles. Choisissez un paramètre d’image prédéfini pour la diffusion de votre modèle, puis cliquez sur **[!UICONTROL Copier l’URL]**. Après avoir copié l’URL à partir de la page de Prévisualisation, vous pouvez l’utiliser sur votre site Web ou dans votre application. (voir [Liaison d’un modèle à une page Web](linking-template-web-page.md#linking_a_template_to_a_web_page)).
