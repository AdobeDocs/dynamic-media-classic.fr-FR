---
title: Création et activation des paramètres d’image prédéfinis
description: Découvrez comment créer et activer des paramètres d’image prédéfinis.
uuid: 62cfc6fa-da91-4c42-a3ed-10956384d633
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 84257b2a-681c-4fe9-a6e5-3633c1d61d8c
feature: Dynamic Media Classic,Collaboration,paramètres d’image prédéfinis,Gestion des ressources
role: Admin,User
exl-id: 94c6c388-226b-4172-a6c7-a8dcf9c0f0cf
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 81%

---

# Création et activation des paramètres d’image prédéfinis{#creating-and-enabling-image-presets}

Lors de l’exportation de fichiers d’image via le portail multimédia, les utilisateurs peuvent choisir un paramètre d’image prédéfini dans la boîte de dialogue Exporter les fichiers sélectionnés. Un paramètre d’image prédéfini désigne un ensemble de paramètres préétablis qui permettent de modifier la taille, la qualité d’image, le format, la résolution et d’autres attributs de l’apparence d’une image au moment de l’exportation. 

Les administrateurs du portail multimédia peuvent créer des paramètres d’image prédéfinis permettant de contrôler le type de reformatage des images lors de leur exportation. Les paramètres d’image prédéfinis reformatent les images selon les spécifications de votre entreprise lorsque les utilisateurs exportent des images à partir de Dynamic Media Classic. Au lieu de reformater les images selon leurs préférences, les utilisateurs les exportent en respectant les spécifications exactes d’un paramètre d’image prédéfini.

Les restrictions suivantes s’appliquent lorsque vous exportez des fichiers d’image :

* La largeur x hauteur doit être inférieure ou égale à 100 Mo par image. Par exemple, l’image ne doit pas dépasser 10 K x 10 K, ou toute variation de rapport telle que 8 K x 12 K.
* La taille totale du fichier par tâche d’exportation ne peut pas dépasser 1 Go.
* Il peut y avoir un maximum de 500 fichiers par tâche d’exportation.

>[!NOTE]
>
>ces restrictions s’appliquent uniquement à l’exportation de fichiers d’image dérivés, et non à celle de fichiers maître.

Pour plus d’informations sur la création d’un paramètre d’image prédéfini, voir [Paramètres d’image prédéfinis](application-setup.md#image_presets).

Pour permettre aux utilisateurs de choisir des paramètres d’image prédéfinis lors de l’exportation de leurs fichiers, voir [Définition d’options d’exportation disponibles pour les utilisateurs du portail multimédia](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

Pour choisir les paramètres d’image prédéfinis accessibles par les membres d’un groupe, voir [Choix des autorisations d’accès de paramètres d’image prédéfinis pour un groupe](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).
