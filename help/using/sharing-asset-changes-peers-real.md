---
title: Partage des modifications de ressources avec des pairs en temps réel
description: Découvrez comment partager des modifications de ressources avec des pairs en temps réel dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
topic: Administration, Collaboration
level: Intermediate
source-git-commit: 163eb32112ec6fbefd1dacf48212353ff3053d54
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 26%

---

# Partage des modifications de ressources avec des pairs en temps réel{#sharing-asset-changes-with-peers-in-real-time}

Supposons que plusieurs copies d’Adobe Dynamic Media Classic s’exécutent sur des ordinateurs de la même société. Dans un tel scénario, les actions suivantes de n’importe quel client Dynamic Media Classic sont mises à jour en temps réel avec tous les clients pairs :

* Modification d’une ressource (créateur, éditeur d’image, etc.)
* Modification du nom d’un fichier
* Suppression d’un fichier
* Déplacement d’un fichier
* Téléchargement d’un ou plusieurs fichiers (sur l’ordinateur et le FTP)
* Création, suppression ou modification du nom d’un dossier

Une fois qu’une modification a été apportée au client d’origine, tous les clients pairs connectés à la même société sont mis à jour avec la modification. Les modifications sont appliquées aux pairs sans aucune notification, sauf si un pair modifie un fichier édité dans un éditeur d’images ou une zone de création.

Lorsque vous vous êtes connecté, vous étiez invité à autoriser ou à refuser les mises à jour des pairs. Vous pouvez « mémoriser » votre choix afin que la question ne vous soit plus posée par la suite. Pour annuler votre choix, supprimez le site concerné dans le panneau Mise en réseau coopérative.

Si vous modifiez une ressource modifiée par un pair, vous êtes invité à ingérer la modification dans le créateur ou l’éditeur. Si vous choisissez **[!UICONTROL Oui]**, le créateur ou l’éditeur ignore toutes les modifications apportées à la ressource et importe la ressource mise à jour. Si vous choisissez **[!UICONTROL Non]**, la ressource reste inchangée dans le créateur ou l’éditeur et toutes les modifications que vous avez apportées sont conservées au cours de cette session.

Lorsque vous avez enregistré la ressource, vous avez été informé de l’existence d’une version plus récente et vous avez été invité à la remplacer par vos modifications.
