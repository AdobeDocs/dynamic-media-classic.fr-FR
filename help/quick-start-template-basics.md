---
title: '"Démarrage rapide : Concepts de base des modèles"'
description: Présentation et démarrage rapide des concepts de base des modèles pour vous aider à démarrer rapidement.
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
feature: Dynamic Media Classic
role: Business Practitioner
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 34%

---

# Démarrage rapide : Concepts de base des modèles{#quick-start-template-basics}

Les concepts de base des modèles sont des fichiers d’images créés dynamiquement et superposés de manière adressable, tels que des fichiers superposés dans des applications de retouche d’images telles qu’Adobe Photoshop. Contrairement à un fichier statique contenant des calques, par exemple un fichier PSD, un modèle peut comporter des paramètres. C’est grâce à ces paramètres que les différents aspects de l’image peuvent être traités et personnalisés.

Un modèle peut contenir n’importe quel nombre de calques d’image et de texte. Vous pouvez convertir un fichier statique contenant des calques, tels qu’un fichier PSD superposé, en modèle, puis créer des modèles dans Dynamic Media Classic. Vous pouvez créer des calques de texte dans les modèles à l’aide des polices que vous avez téléchargées dans Dynamic Media Classic. Une fois que vous avez ajouté du texte à un modèle, vous pouvez le mettre en forme en modifiant la justification, les polices, le corps des caractères et la couleur.

La page Paramètres vous permet de convertir n’importe quel aspect d’un modèle en paramètre adressable. Ainsi, vous pouvez sélectionner l’image superposée ou la valeur du texte à utiliser dans votre modèle. Les paramètres sont transmis avec la chaîne URL, ce qui vous permet de modifier n’importe quel paramètre afin de personnaliser dynamiquement l’image de réponse générée à partir du serveur d’images.

Cette section de démarrage rapide est conçue pour aider à maîtriser rapidement les opérations liées aux concepts de base des modèles. 

## 1. Télécharger les fichiers

Commencez par télécharger le fichier PSD ou le fichier d’image de votre modèle. Dynamic Media Classic prend en charge de nombreux formats de fichier image en plus du PSD, mais les formats sans perte TIFF et PNG sont recommandés pour les modèles car ils permettent une transparence.

Si vous utilisez un fichier PSD pour créer votre modèle, sélectionnez **[!UICONTROL Créer un modèle]** dans la boîte de dialogue **[!UICONTROL Télécharger les options de tâche]** lorsque vous chargez le fichier PSD. Choisissez également une option **[!UICONTROL Affectation de nom de calque]** pour que Dynamic Media Classic sache comment nommer les calques PSD lorsqu’ils sont chargés vers Dynamic Media Classic.

Si vous utilisez des fichiers d’images, vous pouvez recadrer les images et créer également un masque à partir des chemins de tracé dans les images au cours du téléchargement.

Dans la barre de navigation globale, cliquez sur **[!UICONTROL Télécharger]** pour télécharger un fichier PSD ou d’autres fichiers image de votre ordinateur vers un dossier de Dynamic Media Classic. (voir [Téléchargement des fichiers de modèle](uploading-template-files.md#uploading_template_files)).

## 2. Créer un modèle

Pour créer un modèle à partir d’un fichier PSD, sélectionnez **[!UICONTROL Créer un modèle]** lorsque vous chargez le fichier. Pour créer un modèle à partir d’images, dans la barre de navigation globale, cliquez sur **[!UICONTROL Créer]** > **[!UICONTROL Concepts de base des modèles]**, saisissez une mesure de largeur et de hauteur pour la zone de travail. Près du coin supérieur droit de la page, sélectionnez **[!UICONTROL Designer]** ou **[!UICONTROL Développeur]**, puis faites glisser les images sur la page Modèle. Vous pouvez également sélectionner les images *avant* cliquer sur **[!UICONTROL Créer]** > **[!UICONTROL Concepts de base des modèles]**. La page Modèle contient des outils pour :

* Ajout de calques d’images Pour ajouter un calque, faites glisser une image sur la page Modèle.
* Ajout de calques de texte Cliquez sur l’icône **[!UICONTROL Outil de texte]** . Faites glisser le pointeur pour créer une zone pour le calque de texte ; mettez ensuite le texte en forme à l’aide des outils de la page Texte .
* Modification de la taille et de la position des calques
* Modification de l’ordre des calques
* Application d’effets d’ombre et d’éclat aux calques d’image et de texte 

Voir [Création d’un modèle](creating-template.md#creating_a_template).

## 3. Création de paramètres de modèle

L’étape suivante consiste à paramétrer les propriétés sur les calques pour déterminer les propriétés de calque à inclure dans la chaîne URL. Les paramètres permettent de manipuler les modèles avec une souplesse optimale. Après avoir transformé une propriété de calque en paramètre, vous pouvez le modifier dynamiquement.

Pour paramétrer un calque, ouvrez le modèle dans la page Modèle, puis cliquez sur **[!UICONTROL Paramètres]** en regard d’un nom de calque. Sur la page Paramètres , sélectionnez l’option en regard de chaque paramètre à ajouter. (voir [Création de paramètres de modèle](creating-template-parameters.md#creating_template_parameters)).

## 4. Publier des modèles

Lorsque vous publiez votre modèle, il est placé sur les serveurs d’images Dynamic Media afin de pouvoir être diffusé dynamiquement sur votre site web ou dans votre application. La publication active également l’URL pour appeler le modèle à partir des serveurs Dynamic Media Image Server vers votre site web ou votre application.

Assurez-vous de publier toutes les images associées à votre modèle.

Pour publier un modèle, marquez-le pour publication puis, sur la barre de navigation globale, cliquez sur **[!UICONTROL Publier]**. Cliquez ensuite sur **[!UICONTROL Envoyer la publication]**. (voir [Publication de modèles](publishing-templates.md#publishing_templates)).

## 5. Associer un modèle à une page web

Dynamic Media Classic crée des URL pour les modèles et les active lorsque vous publiez des modèles sur les serveurs d’images Dynamic Media. Vous pouvez copier ces chaînes URL à partir de la page Aperçu du modèle .

Sélectionnez votre modèle dans le panneau de navigation, puis cliquez sur **[!UICONTROL Aperçu]** pour ouvrir la page Aperçu du modèle. Sélectionnez un paramètre d’image prédéfini pour la diffusion de votre modèle, puis cliquez sur **[!UICONTROL Copier l’URL]**. Après avoir copié l’URL à partir de la page Aperçu, vous pouvez l’utiliser sur votre site web ou dans votre application. (voir [Liaison d’un modèle à une page Web](linking-template-web-page.md#linking_a_template_to_a_web_page)).
