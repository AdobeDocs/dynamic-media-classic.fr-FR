---
title: 'Démarrage rapide : portail multimédia'
description: Cette section présente et démarre rapidement le portail multimédia pour vous aider à maîtriser rapidement les techniques et l’administration du portail multimédia dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: bff613c8-a93b-4cca-94db-8cad1cc36296
topic: Collaboration, Content Management
level: Beginner
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 45%

---

# Démarrage rapide : portail multimédia{#quick-start-media-portal}

Media Portal permet aux entreprises d’acquérir, de contrôler et de distribuer facilement des ressources approuvées à des partenaires et des canaux externes, ainsi qu’aux utilisateurs internes d’une entreprise. Cet environnement de navigateur en « libre-service » fournit aux utilisateurs du portail multimédia des « vues » contrôlées par l’administrateur dans les ressources Adobe Dynamic Media Classic pour un accès, une navigation, une recherche, une prévisualisation et une exportation faciles des ressources dans des formats approuvés par l’entreprise.

En tant qu’administrateur, vous contrôlez la manière dont les utilisateurs visualisent, ouvrent et utilisent les fichiers disponibles dans le portail multimédia. De plus, vous pouvez personnaliser l’interface du portail multimédia pour qu’elle corresponde à votre site web et à votre marque. Vous pouvez spécifier la police, la couleur et la taille de la police, et incorporer des éléments de branding tels que des logos dans l’interface de Media Portal.

Regardez les vidéos de formation suivantes :

* [Présentation du portail multimédia](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/544_mp_overview1_converted%20renamed_Done-AVS)

* [Visite guidée du portail multimédia 1](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/545_mp_tour1_user_converted%20renamed_Done-AVS)

* [Visite guidée du portail multimédia 2](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/546_mp_tour2_admin_converted%20renamed_Done-AVS)

Le didacticiel de mise en route suivant est conçu pour vous aider à démarrer rapidement l’administration de Media Portal. À la fin de chaque étape, sélectionnez le lien de la rubrique pour en savoir plus.

## &#x200B;1. Compréhension des rôles utilisateur du portail multimédia

Les utilisateurs de Media Portal peuvent jouer trois rôles : utilisateur, contributeur et utilisateur-contributeur. Chaque rôle permet d’effectuer un ensemble de tâches précis. Par exemple, un contributeur est habilité à renommer et à supprimer des fichiers et des dossiers, contrairement à un simple utilisateur. Familiarisez-vous avec ces rôles afin de pouvoir, lors de la création des rôles, bien comprendre les responsabilités que vous octroyez à chacun d’entre eux.

Voir [Rôles utilisateur du portail multimédia](media-portal-user-roles.md#media_portal_user_roles).

## &#x200B;2. Création de groupes de gestion des utilisateurs

Les groupes déterminent les dossiers et les fichiers auxquels l’utilisateur a accès, les opérations qu’il peut effectuer dans ceux-ci, ainsi que les paramètres d’image prédéfinis disponibles. En tant qu’administrateur, votre première tâche consiste à créer des groupes. Pour chaque groupe, décidez des dossiers, fichiers et paramètres d’image prédéfinis auxquels les membres du groupe pourront accéder. Accordez également aux membres du groupe les autorisations de lecture, d’écriture et de suppression adéquates. Ces autorisations déterminent si les membres du groupe sont habilités à parcourir, modifier, renommer et supprimer les dossiers et fichiers auxquels ils ont accès.

Voir [Création et gestion des groupes du portail multimédia](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## &#x200B;3. Ajout des utilisateurs

Lorsque vous ajoutez un utilisateur, vous lui attribuez un rôle (utilisateur, contributeur ou contributeur-utilisateur). Vous pouvez également affecter l’utilisateur à un ou plusieurs groupes. Pour accélérer la procédure d’ajout, vous pouvez télécharger une liste d’utilisateurs enregistrée dans un fichier au format CSV. Les nouveaux utilisateurs reçoivent un message électronique de bienvenue accompagné d’instructions de connexion au portail multimédia.

Voir [ Ajouter et gérer des utilisateurs du portail multimédia ](adding-media-portal-users.md#adding_and_managing_media_portal_users).

## &#x200B;4. Gestion des comptes FTP

Vous pouvez avoir des comptes FTP distincts associés au portail multimédia. Ils peuvent être mappés à un dossier spécifique dans votre compte Adobe Dynamic Media Classic. Ce type de fonctionnalité signifie que vous pouvez autoriser les utilisateurs à télécharger des fichiers numériques sur votre compte en utilisant des comptes FTP distincts.

Voir [ Gestion des comptes FTP ](ftp-accounts.md#managing_ftp_accounts).

>[!NOTE]
>
>Seuls les administrateurs du portail multimédia peuvent administrer ces comptes FTP. En outre, seuls les utilisateurs affectés du rôle de Contributeur-utilisateur Media Portal ou Contributeur Media Portal peuvent télécharger des fichiers.

Voir [Rôles utilisateur du portail multimédia](media-portal-user-roles.md#media_portal_user_roles).

## &#x200B;5. Configuration des options d’exportation

Les utilisateurs de Media Portal, lorsqu’ils exportent des fichiers, peuvent reformater les fichiers et exporter les fichiers principaux d’origine, si vous leur donnez l’autorisation de le faire. En effet, en tant qu’administrateur, c’est à vous de décider du mode d’exportation des fichiers par les utilisateurs.

Voir [Définition des options d’exportation disponibles pour les utilisateurs du portail multimédia](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

## &#x200B;6. Création de paramètres d’image prédéfinis

Un paramètre d’image prédéfini est un ensemble de paramètres prédéfinis. Ces paramètres peuvent modifier la taille, la qualité de l’image, le format, la résolution et d’autres aspects de l’aspect d’une image lors de son exportation. Les paramètres d’image prédéfinis peuvent servir à contrôler le type de reformatage des images lors de leur exportation.

Voir [Création et activation des paramètres d’image prédéfinis](creating-enabling-image-presets.md#creating_and_enabling_image_presets).

## &#x200B;7. Création de paramètres prédéfinis des métadonnées et de champs de métadonnées définis par l’utilisateur

Les métadonnées décrivent et identifient un fichier. Il est utilisé pour rechercher et organiser des ressources. Vous pouvez créer des paramètres prédéfinis de métadonnées pour vous assurer de saisir correctement les métadonnées et de remplir tous les champs de métadonnées qui nécessitent des données. Un paramètre prédéfini de métadonnées est un ensemble préétabli d’entrées de métadonnées. Vous pouvez également créer des champs de métadonnées qui décrivent de manière unique les fichiers que vous utilisez.

Voir [Optimisation de l’utilisation des métadonnées](making-efficient-metadata.md#making_more_efficient_use_of_metadata).

## &#x200B;8. Personnalisation de la page du portail multimédia

Les paramètres de style du portail multimédia vous permettent d’étiqueter la page du portail multimédia avec le logo et les couleurs de votre entreprise. Utilisez les paramètres de style pour placer l’image de marque de votre entreprise sur le portail multimédia.

Voir [Personnalisation de la page du portail multimédia](customizing-media-portal-screen.md#customizing_the_media_portal_screen).
