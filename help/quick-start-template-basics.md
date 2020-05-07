---
title: '"Démarrage rapide : Concepts de base des modèles"'
seo-title: '"Démarrage rapide : Concepts de base des modèles"'
description: 'null'
seo-description: Une introduction et un Début rapide aux concepts de base des modèles pour vous aider à maîtriser rapidement les opérations.
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
translation-type: tm+mt
source-git-commit: df0c2897b9fceddde648be53b23e25b13388d6b9
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 77%

---


# Démarrage rapide : Concepts de base des modèles{#quick-start-template-basics}

Les concepts de base des modèles sont des fichiers d’images créés dynamiquement et superposés de manière adressable, tels que des fichiers superposés dans des applications de retouche d’images telles qu’Adobe Photoshop. Contrairement à un fichier statique contenant des calques, par exemple un fichier PSD, un modèle peut comporter des paramètres. C’est grâce à ces paramètres que les différents aspects de l’image peuvent être traités et personnalisés.

Un modèle peut contenir n’importe quel nombre de calques d’image et de texte. Vous pouvez convertir un fichier statique contenant des calques, tel qu’un fichier PSD superposé, en modèle, ainsi que créer des modèles dans Contenu multimédia dynamique classique. Vous pouvez créer des calques de texte dans les modèles à l’aide des polices que vous avez téléchargées dans SPS. Une fois que vous avez ajouté du texte à un modèle, vous pouvez le mettre en forme en modifiant la justification, les polices, le corps des caractères et la couleur.

Sur l’écran Paramètres, vous pouvez convertir n’importe quel aspect d’un modèle en paramètre adressable. Ainsi, vous pouvez sélectionner l’image superposée ou la valeur du texte à utiliser dans votre modèle. Les paramètres sont transmis avec la chaîne URL, ce qui vous permet de modifier n’importe quel paramètre afin de personnaliser dynamiquement l’image de réponse générée à partir du serveur d’images.

**Début rapide**

Cette section de démarrage rapide est conçue pour aider à maîtriser rapidement les opérations liées aux concepts de base des modèles. 

**1. Téléchargement des fichiers**

Commencez par télécharger le fichier PSD ou le fichier d’image de votre modèle. Dynamic Media Classic prend en charge de nombreux formats de fichier d’images en plus du PSD, mais les images TIFF et PNG sans perte sont recommandées pour les modèles car elles permettent la transparence.

Si vous utilisez un fichier PSD pour créer votre modèle, sélectionnez l’option Créer un modèle dans la boîte de dialogue Télécharger les options de la tâche lorsque vous téléchargez le fichier PSD. Choisissez également une option de dénomination de calque pour indiquer à Dynamic Media Classic comment nommer les calques PSD lorsqu’ils sont téléchargés vers Scene7 Publishing System.

Si vous utilisez des fichiers d’images, vous pouvez recadrer les images et créer également un masque à partir des chemins de tracé dans les images au cours du téléchargement.

Sélectionnez le bouton Télécharger de la barre de navigation globale pour télécharger un fichier PSD ou d’autres fichiers d’images de votre ordinateur dans un dossier SPS (voir [Téléchargement des fichiers de modèle](uploading-template-files.md#uploading_template_files)).

**2. Création d’un modèle**

Pour créer un modèle à partir d’un fichier PSD, sélectionnez l’option Créer un modèle lorsque vous téléchargez le fichier. Pour créer un modèle depuis des images, choisissez Créer > Concepts de base des modèles, entrez la largeur et la hauteur de la zone de travail, puis faites glisser des images sur l’écran Modèle. Vous pouvez également sélectionner les images avant de choisir la commande Créer > Concepts de base des modèles. L’écran Modèle contient des outils permettant d’effectuer les opérations suivantes :

* Ajout de calques d’images (pour ajouter un calque, faites glisser une image sur l’écran Modèle)
* Ajout de calques de texte Sélectionnez l’outil Texte , faites glisser la souris pour tracer le cadre de délimitation du calque de texte, puis formatez le texte à l’aide des outils de l’écran Texte.
* Modification de la taille et de la position des calques
* Modification de l’ordre des calques
* Application d’effets d’ombre et d’éclat aux calques d’image et de texte 

Voir [Création d’un modèle](creating-template.md#creating_a_template).

**Cookie. Création de paramètres de modèle**

L’étape suivante consiste à paramétrer les propriétés sur les calques pour déterminer les propriétés de calque à inclure dans la chaîne URL. Les paramètres permettent de manipuler les modèles avec une souplesse optimale. Après avoir transformé une propriété de calque en paramètre, vous pouvez le modifier dynamiquement.

Pour paramétrer un calque, ouvrez le modèle sur l’écran Modèle, puis sélectionnez le bouton Paramètres situé en regard du nom du calque. Sur l’écran Paramètres, sélectionnez l’option située en regard de chacun des paramètres à ajouter (voir [Création de paramètres de modèle](creating-template-parameters.md#creating_template_parameters)).

**4. Publication de modèles**

Lorsque vous publiez votre modèle, il est placé sur les serveurs Dynamic Media Image Server afin de pouvoir être diffusé de manière dynamique sur votre site Web ou dans votre application. La publication active également l’URL pour appeler le modèle à partir des serveurs d’images de Contenu multimédia dynamique vers votre site Web ou votre application.

Assurez-vous de publier toutes les images associées à votre modèle.

Pour publier un modèle, marquez-le pour publication, puis sélectionnez le bouton Publier dans la barre de navigation globale. Sélectionnez ensuite le bouton Lancer publication (voir [Publication de modèles](publishing-templates.md#publishing_templates)).

**5. Liaison d’un modèle à une page Web**

Dynamic Media Classic crée des URL pour les modèles et les active lorsque vous publiez des modèles sur des serveurs d’images Contenu multimédia dynamique. Vous pouvez copier ces chaînes URL depuis l’écran Prévisualisation du modèle.

Sélectionnez votre modèle dans le panneau de navigation, puis cliquez sur le bouton Prévisualiser pour accéder à l’écran Prévisualisation du modèle. Ensuite, choisissez un paramètre d’image prédéfini pour la diffusion de votre modèle, puis sélectionnez le bouton Copier l’URL. Après avoir copié l’URL à partir de l’écran de prévisualisation, vous pouvez l’utiliser sur votre site Web ou dans votre application (voir [Liaison d’un modèle à une page Web](linking-template-web-page.md#linking_a_template_to_a_web_page)).
