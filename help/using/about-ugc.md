---
title: À propos du contenu généré par l’utilisateur dans Adobe Dynamic Media Classic
description: Présentation du contenu généré par l’utilisateur.
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/user_generated_content
feature: Dynamic Media Classic
role: Admin,User
exl-id: 14729192-7b9d-4f42-99da-6564a3f35959
topic: Content Management
level: Intermediate
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 33%

---

# À propos du contenu généré par l’utilisateur dans Adobe Dynamic Media Classic {#about-user-generated-content}

L’utilisation du contenu créé par l’utilisateur consiste à charger des ressources dans un référentiel de stockage Adobe Dynamic Media Classic dédié et à effectuer les opérations associées.

UGC prend en charge les formats de fichiers d’images pixellisées BMP, GIF, JPG, PNG, PSD et TIFF.

>[!IMPORTANT]
>
>À compter du 1er mai 2023, les ressources UGC dans Dynamic Media pourront être utilisées pendant 60 jours à compter de la date de chargement. Au bout de 60 jours, les ressources seront supprimées.

<!-- * Vector: AI, EPS (EPS files from Adobe Illustrator 2018 are not supported), PDF (only when the PDF file is previously opened and saved in Adobe Illustrator CS6) -->

>[!NOTE]
>
>La prise en charge des ressources d’images vectorielles UGC nouvelles ou existantes dans Adobe Dynamic Media Classic a pris fin le 30 septembre 2021.

Avant de télécharger les fichiers, vous devez obtenir une clé de secret partagé. Cette clé vous permet de récupérer un jeton de téléchargement. Vous envoyez le jeton de téléchargement lorsque vous téléchargez des fichiers et réalisez d’autres tâches sur le contenu généré par l’utilisateur.

Après avoir récupéré une clé de secret partagé et le jeton de téléchargement, vous pouvez réaliser les opérations suivantes pour le contenu généré par l’utilisateur :

* Chargement d’une ressource.
* Obtenez les métadonnées du fichier d’image.
* Supprimer un fichier téléchargé.
* Obtenez des informations sur l’utilisation de l’espace disque d’une entreprise.
