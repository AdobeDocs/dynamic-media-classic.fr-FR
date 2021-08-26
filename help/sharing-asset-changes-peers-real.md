---
title: Partage de modifications de fichier en temps réel avec des pairs
description: Découvrez comment partager des modifications de ressources avec des pairs en temps réel.
uuid: 13fa4f6e-66bf-4682-96a9-0e7040706f53
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: ca7c8a7f-76f4-4a25-8c36-617a029e55be
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 50%

---

# Partage de modifications de fichier en temps réel avec des pairs{#sharing-asset-changes-with-peers-in-real-time}

Avec plusieurs copies d’Adobe Dynamic Media Classic exécutées sur un ou plusieurs ordinateurs de la même société, les actions suivantes de n’importe quel client Dynamic Media Classic d’Adobe sont mises à jour en temps réel avec tous les clients pairs :

* Modification d’une ressource (créateur, éditeur d’image, etc.)
* Modification du nom d’un fichier
* Suppression d’un fichier
* Déplacement d’un fichier
* Téléchargement d’un ou plusieurs fichiers (sur l’ordinateur et le FTP)
* Création, suppression ou modification du nom d’un dossier

Une fois qu’une modification a été apportée au client d’origine, tous les clients pairs connectés à la même société sont mis à jour avec la modification. Les modifications sont appliquées aux pairs sans aucune notification, sauf si un pair modifie un fichier édité dans un éditeur d’images ou une zone de création.

Lorsque vous vous connectez, vous êtes invité à autoriser ou à refuser les mises à jour des pairs. Vous pouvez « mémoriser » votre choix afin que la question ne vous soit plus posée par la suite. Pour annuler votre choix, supprimez le site concerné dans le panneau Mise en réseau coopérative.

Si vous éditez un fichier modifié par un pair, vous êtes invité à intégrer la modification dans la zone de création ou l’éditeur. Si vous sélectionnez **[!UICONTROL Oui]**, le créateur ou l’éditeur ignore toutes les modifications apportées à la ressource et importe la ressource mise à jour. Si vous choisissez **[!UICONTROL Non]**, la ressource reste inchangée dans le créateur ou l’éditeur et toutes les modifications que vous avez apportées sont conservées au cours de cette session.

Au moment d’enregistrer le fichier, vous êtes informé qu’il existe une nouvelle version et êtes invité à remplacer cette version par la vôtre.
