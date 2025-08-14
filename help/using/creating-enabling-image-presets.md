---
title: Création et activation des paramètres d’image prédéfinis
description: Découvrez comment créer et activer des paramètres d’image prédéfinis dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Image Presets,Asset Management
role: Admin,User
exl-id: 94c6c388-226b-4172-a6c7-a8dcf9c0f0cf
topic: Content Management
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 48%

---

# Création et activation des paramètres d’image prédéfinis{#creating-and-enabling-image-presets}

Lors de l’exportation de fichiers d’image via le portail multimédia, les utilisateurs peuvent choisir un paramètre d’image prédéfini dans la boîte de dialogue Exporter les fichiers sélectionnés. Un paramètre d’image prédéfini est un ensemble de paramètres prédéfinis. Ces paramètres peuvent modifier la taille, la qualité de l’image, le format, la résolution et d’autres aspects de l’aspect d’une image lors de son exportation.

Les administrateurs du portail multimédia peuvent créer des paramètres d’image prédéfinis permettant de contrôler le type de reformatage des images lors de leur exportation. Les paramètres d’image prédéfinis reformatent les images selon les spécifications de votre société lorsque les utilisateurs exportent des images à partir d’Adobe Dynamic Media Classic. Au lieu de reformater les images selon leurs préférences, les utilisateurs les exportent en respectant les spécifications exactes d’un paramètre d’image prédéfini.

Les restrictions suivantes s’appliquent lorsque vous exportez des fichiers d’image :

* La largeur × la hauteur doivent être inférieures ou égales à 100 Mo par image. Par exemple, l’image ne peut pas dépasser 10 K × 10 K, ni aucune variation d’aspect inférieure, comme 8 K × 12 K.
* La taille de fichier totale maximale est de 1 Go par tâche d’exportation.
* Il peut y avoir un maximum de 500 fichiers par tâche d’exportation.

>[!NOTE]
>
>Ces restrictions s’appliquent uniquement à l’exportation de ressources d’images dérivées, et non à l’exportation de fichiers principaux.

Pour plus d’informations sur la création d’un paramètre d’image prédéfini, voir [Paramètres d’image prédéfinis](application-setup.md#image_presets).

Pour permettre aux utilisateurs de choisir des paramètres d’image prédéfinis lors de l’exportation de leurs fichiers, voir [Définition d’options d’exportation disponibles pour les utilisateurs du portail multimédia](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

Pour choisir les paramètres d’image prédéfinis accessibles par les membres d’un groupe, voir [Choix des autorisations d’accès de paramètres d’image prédéfinis pour un groupe](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).
