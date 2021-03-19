---
title: '"Début rapide : Media Portal"'
description: Présentation et Début rapide sur Media Portal pour vous aider à maîtriser rapidement les techniques et l’administration du portail multimédia.
uuid: 0dbd6146-b392-4e03-955b-0b323b654b9f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 1385a092-0b2c-4e05-ad1e-ce3685022300
feature: Dynamic Media Classic,Collaboration,Gestion des ressources
role: Administrateur, Professionnel
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 84%

---


# Démarrage rapide :  du portail multimédia{#quick-start-media-portal}

Media Portal permet aux sociétés d’acquérir, de contrôler et de distribuer facilement des ressources créatives approuvées à des partenaires et canaux externes, ainsi qu’à des utilisateurs internes de l’entreprise. Cet environnement en libre-service basé sur un navigateur fournit aux utilisateurs du portail multimédia des &quot;vues&quot; contrôlées par l’administrateur dans les ressources Dynamic Media Classic pour un accès facile aux ressources Classic, la navigation, la recherche, la prévisualisation et l’exportation dans des formats approuvés par l’entreprise.

En tant qu’administrateur, vous contrôlez la manière dont les utilisateurs visualisent, ouvrent et utilisent les fichiers disponibles dans le portail multimédia. Vous pouvez par ailleurs personnaliser l’interface du portail multimédia en fonction de votre site Web et de votre marque. Vous avez la possibilité de spécifier la police et ses attributs (couleur et taille), de même que d’incorporer des éléments d’identification de la marque (tels que des logos) dans l’interface du portail multimédia.

**Début rapide**

Cette section de démarrage rapide est conçue pour vous aider à maîtriser rapidement les opérations liées à l’administration du portail multimédia. A la fin de chaque étape figure une référence croisée pointant vers une rubrique présentant des informations complémentaires sur le sujet.

**1. Compréhension des rôles utilisateur du portail multimédia**

Les utilisateurs du portail multimédia se rangent dans trois catégories : utilisateur, contributeur et contributeur-utilisateur. Chaque rôle permet d’effectuer un ensemble de tâches précis. Par exemple, un contributeur est habilité à renommer et à supprimer des fichiers et des dossiers, contrairement à un simple utilisateur. Familiarisez-vous avec ces rôles afin de pouvoir, lors de la création des rôles, bien comprendre les responsabilités que vous octroyez à chacun d’entre eux.

Voir [Rôles utilisateur du portail multimédia](media-portal-user-roles.md#media_portal_user_roles).

**2. Création de groupes de gestion des utilisateurs**

Les groupes déterminent les dossiers et les fichiers auxquels l’utilisateur a accès, les opérations qu’il peut effectuer dans ceux-ci, ainsi que les paramètres d’image prédéfinis disponibles. En tant qu’administrateur, votre première tâche consiste à créer des groupes. Pour chaque groupe, décidez des dossiers, fichiers et paramètres d’image prédéfinis auxquels les membres du groupe pourront accéder. Accordez également aux membres du groupe les autorisations de lecture, d’écriture et de suppression adéquates. Ces autorisations déterminent si les membres du groupe sont habilités à parcourir, modifier, renommer et supprimer les dossiers et fichiers auxquels ils ont accès.

Voir [Création et gestion des groupes du portail multimédia](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

**Cookie. Ajout des utilisateurs**

Lorsque vous ajoutez un utilisateur, vous lui attribuez un rôle (utilisateur, contributeur ou contributeur-utilisateur). Vous affectez également l’utilisateur à un ou plusieurs groupes. Pour accélérer la procédure d’ajout, vous pouvez télécharger une liste d’utilisateurs enregistrée dans un fichier au format CSV. Les nouveaux utilisateurs reçoivent un message électronique de bienvenue accompagné d’instructions de connexion au portail multimédia.

Voir [Ajout et gestion des utilisateurs du portail multimédia](adding-media-portal-users.md#adding_and_managing_media_portal_users).

**4. Gestion des comptes FTP**

Vous pouvez disposer de comptes FTP distincts associés au portail multimédia et mappés à un dossier spécifique dans votre compte Dynamic Media Classic. Ce type de fonctionnalité signifie que vous pouvez autoriser les utilisateurs à télécharger des fichiers numériques sur votre compte en utilisant des comptes FTP distincts.

Voir [Gestion des comptes FTP](ftp-accounts.md#managing_ftp_accounts).

>[!NOTE]
>
>seuls les administrateurs du portail multimédia peuvent gérer ces comptes FTP. En outre, seuls les utilisateurs affectés du rôle de Contributeur-utilisateur Media Portal ou Contributeur Media Portal peuvent télécharger des fichiers.

Voir [Rôles utilisateur du portail multimédia](media-portal-user-roles.md#media_portal_user_roles).

**5. Configuration des options d’exportation**

Lors de l’exportation de fichiers, les utilisateurs du portail multimédia ont la possibilité de reformater les fichiers en vue d’exporter les fichiers originaux, sous réserve d’y être autorisés par vous (l’administrateur). En effet, en tant qu’administrateur, c’est à vous de décider du mode d’exportation des fichiers par les utilisateurs.

Voir [Définition d’options d’exportation disponibles pour les utilisateurs du portail multimédia](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

**6. Création de paramètres d’image prédéfinis**

Un paramètre d’image prédéfini désigne un ensemble de paramètres préétablis qui permettent de modifier la taille, la qualité d’image, le format, la résolution et d’autres attributs de l’apparence d’une image au moment de l’exportation. Les paramètres d’image prédéfinis peuvent servir à contrôler le type de reformatage des images lors de leur exportation.

Voir [Création et activation des paramètres d’image prédéfinis](creating-enabling-image-presets.md#creating_and_enabling_image_presets).

**7. Création de paramètres prédéfinis des métadonnées et de champs de métadonnées définis par l’utilisateur**

Les métadonnées permettent de décrire et d’identifier un fichier ; elles servent à rechercher et à organiser les fichiers. Les paramètres prédéfinis de métadonnées permettent de vous assurer que les métadonnées sont spécifiées correctement et que les champs de métadonnées obligatoires sont bien remplis. Un paramètre prédéfini de métadonnées est un ensemble préétabli d’entrées de métadonnées. Vous pouvez également créer des champs de métadonnées qui décrivent de manière unique les fichiers que vous utilisez.

Voir [Optimisation de l’utilisation des métadonnées](making-efficient-metadata.md#making_more_efficient_use_of_metadata).

**8. Personnalisation de l’écran du portail multimédia**

Les paramètres de style du portail multimédia vous permettent de faire apparaître la marque de votre entreprise sur l’écran du portail multimédia sous forme de logo et de couleurs personnalisés. Grâce aux paramètres de style, vous pouvez faire figurer le tampon de votre société sur le portail multimédia. 

Voir [Personnalisation de l’écran du portail multimédia](customizing-media-portal-screen.md#customizing_the_media_portal_screen).
