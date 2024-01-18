---
title: "Démarrage rapide : Media Portal"
description: Présentation et démarrage rapide de Media Portal pour vous aider à maîtriser rapidement les techniques et l’administration de Media Portal dans Adobe Dynamic Media Classic.
uuid: 0dbd6146-b392-4e03-955b-0b323b654b9f
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 1385a092-0b2c-4e05-ad1e-ce3685022300
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: bff613c8-a93b-4cca-94db-8cad1cc36296
topic: Collaboration, Content Management
level: Beginner
source-git-commit: ae7d0c6d3047d68ed3da4187ef516dc51c95de30
workflow-type: tm+mt
source-wordcount: '721'
ht-degree: 56%

---

# Démarrage rapide : Media Portal{#quick-start-media-portal}

Media Portal permet aux entreprises d’acquérir, de contrôler et de distribuer facilement des ressources approuvées à des partenaires et canaux externes, ainsi qu’aux utilisateurs internes d’une entreprise. Cet environnement &quot;libre-service&quot; basé sur un navigateur fournit aux utilisateurs de Media Portal des &quot;vues&quot; contrôlées par l’administrateur dans les ressources Adobe Dynamic Media Classic afin de faciliter l’accès, la navigation, la recherche, la prévisualisation et l’exportation des ressources dans des formats approuvés par l’entreprise.

En tant qu’administrateur, vous contrôlez la manière dont les utilisateurs visualisent, ouvrent et utilisent les fichiers disponibles dans le portail multimédia. Vous pouvez par ailleurs personnaliser l’interface du portail multimédia en fonction de votre site Web et de votre marque. Vous pouvez spécifier la police, la couleur de police, la taille de police et incorporer des éléments de marque tels que des logos dans l’interface de Media Portal.

Consultez les vidéos de formation suivantes :

* [Présentation de Media Portal](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/544_mp_overview1_converted%20renamed_Done-AVS)

* [Visite de Media Portal 1](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/545_mp_tour1_user_converted%20renamed_Done-AVS)

* [Visite de Media Portal 2](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/546_mp_tour2_admin_converted%20renamed_Done-AVS)

Le didacticiel de mise en route suivant est conçu pour vous aider à maîtriser rapidement l’administration de Media Portal. À la fin de chaque étape, sélectionnez le lien de la rubrique pour en savoir plus.

## 1. Compréhension des rôles utilisateur du portail multimédia

Les utilisateurs du portail multimédia se rangent dans trois catégories : utilisateur, contributeur et contributeur-utilisateur. Chaque rôle permet d’effectuer un ensemble de tâches précis. Par exemple, un contributeur est habilité à renommer et à supprimer des fichiers et des dossiers, contrairement à un simple utilisateur. Familiarisez-vous avec ces rôles afin de pouvoir, lors de la création des rôles, bien comprendre les responsabilités que vous octroyez à chacun d’entre eux.

Voir [Rôles utilisateur du portail multimédia](media-portal-user-roles.md#media_portal_user_roles).

## 2. Création de groupes de gestion des utilisateurs

Les groupes déterminent les dossiers et les fichiers auxquels l’utilisateur a accès, les opérations qu’il peut effectuer dans ceux-ci, ainsi que les paramètres d’image prédéfinis disponibles. En tant qu’administrateur, votre première tâche consiste à créer des groupes. Pour chaque groupe, décidez des dossiers, fichiers et paramètres d’image prédéfinis auxquels les membres du groupe pourront accéder. Accordez également aux membres du groupe les autorisations de lecture, d’écriture et de suppression adéquates. Ces autorisations déterminent si les membres du groupe sont habilités à parcourir, modifier, renommer et supprimer les dossiers et fichiers auxquels ils ont accès.

Voir [Création et gestion des groupes Media Portal](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## 3. Ajout des utilisateurs

Lorsque vous ajoutez un utilisateur, vous lui attribuez un rôle (utilisateur, contributeur ou contributeur-utilisateur). Vous affectez également l’utilisateur à un ou plusieurs groupes. Pour accélérer la procédure d’ajout, vous pouvez télécharger une liste d’utilisateurs enregistrée dans un fichier au format CSV. Les nouveaux utilisateurs reçoivent un message électronique de bienvenue accompagné d’instructions de connexion au portail multimédia.

Voir [Ajout et gestion des utilisateurs de Media Portal](adding-media-portal-users.md#adding_and_managing_media_portal_users).

## 4. Gestion des comptes FTP

Vous pouvez avoir des comptes FTP distincts associés à Media Portal et mappés à un dossier spécifique dans votre compte Adobe Dynamic Media Classic. Ce type de fonctionnalité signifie que vous pouvez autoriser les utilisateurs à télécharger des fichiers numériques sur votre compte en utilisant des comptes FTP distincts.

Voir [Gestion des comptes FTP](ftp-accounts.md#managing_ftp_accounts).

>[!NOTE]
>
>Seuls les administrateurs du portail multimédia peuvent administrer ces comptes FTP. En outre, seuls les utilisateurs affectés du rôle de Contributeur-utilisateur Media Portal ou Contributeur Media Portal peuvent télécharger des fichiers.

Voir [Rôles utilisateur du portail multimédia](media-portal-user-roles.md#media_portal_user_roles).

## 5. Configuration des options d’exportation

Les utilisateurs de Media Portal, lorsqu’ils exportent des fichiers, peuvent reformater les fichiers et exporter les fichiers primaires d’origine — si vous leur accordez l’autorisation de le faire. En effet, en tant qu’administrateur, c’est à vous de décider du mode d’exportation des fichiers par les utilisateurs.

Voir [Définition des options d’exportation disponibles pour les utilisateurs de Media Portal](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

## 6. Création de paramètres d’image prédéfinis

Un paramètre d’image prédéfini est un ensemble de paramètres prédéfinis qui modifient la taille, la qualité, le format, la résolution et d’autres aspects de l’apparence d’une image lorsqu’elle est exportée. Les paramètres d’image prédéfinis peuvent servir à contrôler le type de reformatage des images lors de leur exportation.

Voir [Création et activation de paramètres d’image prédéfinis](creating-enabling-image-presets.md#creating_and_enabling_image_presets).

## 7. Création de paramètres prédéfinis des métadonnées et de champs de métadonnées définis par l’utilisateur

Les métadonnées permettent de décrire et d’identifier un fichier ; elles servent à rechercher et à organiser les fichiers. Les paramètres prédéfinis de métadonnées permettent de vous assurer que les métadonnées sont spécifiées correctement et que les champs de métadonnées obligatoires sont bien remplis. Un paramètre prédéfini de métadonnées est un ensemble préétabli d’entrées de métadonnées. Vous pouvez également créer des champs de métadonnées qui décrivent de manière unique les fichiers que vous utilisez.

Voir [Optimisation de l’utilisation des métadonnées](making-efficient-metadata.md#making_more_efficient_use_of_metadata).

## 8. Personnalisation de la page Media Portal

Les paramètres de style Media Portal vous permettent de personnaliser la page Media Portal à l’aide du logo et des couleurs de votre société. Utilisez les paramètres de style pour placer la marque de votre entreprise sur Media Portal.

Voir [Personnalisation de la page Media Portal](customizing-media-portal-screen.md#customizing_the_media_portal_screen).
