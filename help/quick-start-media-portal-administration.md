---
title: '"Démarrage rapide : Media Portal"'
description: Présentation et démarrage rapide de Media Portal pour vous aider à maîtriser rapidement les techniques et l’administration de Media Portal.
uuid: 0dbd6146-b392-4e03-955b-0b323b654b9f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 1385a092-0b2c-4e05-ad1e-ce3685022300
feature: Dynamic Media Classic,Collaboration,Gestion des ressources
role: Administrator,Business Practitioner
exl-id: bff613c8-a93b-4cca-94db-8cad1cc36296
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 73%

---

# Démarrage rapide :  du portail multimédia{#quick-start-media-portal}

Media Portal permet aux entreprises d’acquérir, de contrôler et de distribuer facilement des ressources approuvées à des partenaires et canaux externes, ainsi qu’aux utilisateurs internes d’une entreprise. Cet environnement en libre-service basé sur un navigateur fournit aux utilisateurs de Media Portal des &quot;vues&quot; contrôlées par l’administrateur des ressources Dynamic Media Classic pour un accès facile aux ressources, leur navigation, leur recherche, leur prévisualisation et leur exportation dans des formats approuvés par l’entreprise.

En tant qu’administrateur, vous contrôlez la manière dont les utilisateurs visualisent, ouvrent et utilisent les fichiers disponibles dans le portail multimédia. Vous pouvez par ailleurs personnaliser l’interface du portail multimédia en fonction de votre site Web et de votre marque. Vous pouvez spécifier la police, la couleur de la police, la taille de la police et incorporer des éléments de marque tels que des logos dans l’interface de Media Portal.

Cette section de démarrage rapide est conçue pour vous aider à maîtriser rapidement les opérations liées à l’administration du portail multimédia. À la fin de chaque étape, cliquez sur le lien de la rubrique pour en savoir plus.

## 1. Compréhension des rôles utilisateur du portail multimédia

Les utilisateurs du portail multimédia se rangent dans trois catégories : utilisateur, contributeur et contributeur-utilisateur. Chaque rôle permet d’effectuer un ensemble de tâches précis. Par exemple, un contributeur est habilité à renommer et à supprimer des fichiers et des dossiers, contrairement à un simple utilisateur. Familiarisez-vous avec ces rôles afin de pouvoir, lors de la création des rôles, bien comprendre les responsabilités que vous octroyez à chacun d’entre eux.

Voir [Rôles utilisateur du portail multimédia](media-portal-user-roles.md#media_portal_user_roles).

## 2. Création de groupes de gestion des utilisateurs

Les groupes déterminent les dossiers et les fichiers auxquels l’utilisateur a accès, les opérations qu’il peut effectuer dans ceux-ci, ainsi que les paramètres d’image prédéfinis disponibles. En tant qu’administrateur, votre première tâche consiste à créer des groupes. Pour chaque groupe, décidez des dossiers, fichiers et paramètres d’image prédéfinis auxquels les membres du groupe pourront accéder. Accordez également aux membres du groupe les autorisations de lecture, d’écriture et de suppression adéquates. Ces autorisations déterminent si les membres du groupe sont habilités à parcourir, modifier, renommer et supprimer les dossiers et fichiers auxquels ils ont accès.

Voir [Création et gestion des groupes du portail multimédia](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## 3. Ajout des utilisateurs

Lorsque vous ajoutez un utilisateur, vous lui attribuez un rôle (utilisateur, contributeur ou contributeur-utilisateur). Vous affectez également l’utilisateur à un ou plusieurs groupes. Pour accélérer la procédure d’ajout, vous pouvez télécharger une liste d’utilisateurs enregistrée dans un fichier au format CSV. Les nouveaux utilisateurs reçoivent un message électronique de bienvenue accompagné d’instructions de connexion au portail multimédia.

Voir [Ajout et gestion des utilisateurs du portail multimédia](adding-media-portal-users.md#adding_and_managing_media_portal_users).

## 4. Gestion des comptes FTP

Vous pouvez disposer de comptes FTP distincts associés à Media Portal et mappés à un dossier spécifique dans votre compte Dynamic Media Classic. Ce type de fonctionnalité signifie que vous pouvez autoriser les utilisateurs à télécharger des fichiers numériques sur votre compte en utilisant des comptes FTP distincts.

Voir [Gestion des comptes FTP](ftp-accounts.md#managing_ftp_accounts).

>[!NOTE]
>
>seuls les administrateurs du portail multimédia peuvent gérer ces comptes FTP. En outre, seuls les utilisateurs affectés du rôle de Contributeur-utilisateur Media Portal ou Contributeur Media Portal peuvent télécharger des fichiers.

Voir [Rôles utilisateur du portail multimédia](media-portal-user-roles.md#media_portal_user_roles).

## 5. Configuration des options d’exportation

Lors de l’exportation de fichiers, les utilisateurs du portail multimédia ont la possibilité de reformater les fichiers en vue d’exporter les fichiers originaux, sous réserve d’y être autorisés par vous (l’administrateur). En effet, en tant qu’administrateur, c’est à vous de décider du mode d’exportation des fichiers par les utilisateurs.

Voir [Définition d’options d’exportation disponibles pour les utilisateurs du portail multimédia](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

## 6. Création de paramètres d’image prédéfinis

Un paramètre d’image prédéfini désigne un ensemble de paramètres préétablis qui permettent de modifier la taille, la qualité d’image, le format, la résolution et d’autres attributs de l’apparence d’une image au moment de l’exportation. Les paramètres d’image prédéfinis peuvent servir à contrôler le type de reformatage des images lors de leur exportation.

Voir [Création et activation des paramètres d’image prédéfinis](creating-enabling-image-presets.md#creating_and_enabling_image_presets).

## 7. Création de paramètres prédéfinis des métadonnées et de champs de métadonnées définis par l’utilisateur

Les métadonnées permettent de décrire et d’identifier un fichier ; elles servent à rechercher et à organiser les fichiers. Les paramètres prédéfinis de métadonnées permettent de vous assurer que les métadonnées sont spécifiées correctement et que les champs de métadonnées obligatoires sont bien remplis. Un paramètre prédéfini de métadonnées est un ensemble préétabli d’entrées de métadonnées. Vous pouvez également créer des champs de métadonnées qui décrivent de manière unique les fichiers que vous utilisez.

Voir [Optimisation de l’utilisation des métadonnées](making-efficient-metadata.md#making_more_efficient_use_of_metadata).

## 8. Personnalisation de la page Media Portal

Les paramètres de style Media Portal vous permettent de personnaliser la page Media Portal avec le logo et les couleurs de votre entreprise. Utilisez les paramètres de style pour placer la marque de votre entreprise sur Media Portal.

Voir [Personnalisation de la page Media Portal](customizing-media-portal-screen.md#customizing_the_media_portal_screen).
