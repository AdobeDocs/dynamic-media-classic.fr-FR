---
title: Partager les modifications de ressources avec des clients homologues en temps réel
description: Découvrez comment partager les modifications de ressources avec des homologues en temps réel dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
topic: Administration, Collaboration
level: Intermediate
autotag-review: '2026-05-13T20:12:54.992Z'
TQID: 'https://experienceleague.adobe.com/Yn5GsnQ4cM3Byk18iEB8Z4uGsTt9FjEZOBP17Yt-K8M'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 4c8d0e861708e8931bbefe55260c7704c43e0ce6
workflow-type: tm+mt
source-wordcount: 285
ht-degree: 14%

---

# Partager en temps réel les modifications apportées aux ressources avec des clients homologues{#sharing-asset-changes-with-peers-in-real-time}

Plusieurs instances d’Adobe Dynamic Media Classic s’exécutent sur des ordinateurs au sein de la même organisation. Dans un tel scénario, les actions suivantes de n’importe quel client Dynamic Media Classic sont mises à jour en temps réel sur tous les clients pairs :

* Modifier une ressource (créateur, éditeur d’image, etc.)
* Modification du nom d’un fichier
* Suppression d’un fichier
* Déplacement d’un fichier
* Téléchargement d’un ou plusieurs fichiers (sur l’ordinateur et le FTP)
* Création, suppression ou modification du nom d’un dossier

Une fois qu’une modification a été apportée au client d’origine, tous les clients homologues connectés dans la même société sont mis à jour avec la modification. Les modifications sont automatiquement appliquées aux homologues, à condition que l’homologue ne modifie pas la ressource dans l’un des éditeurs ou créateurs d’images.

Lorsque vous vous connectez, vous êtes invité à autoriser ou refuser les mises à jour d’homologues. Vous pouvez enregistrer le choix pour n’être invité qu’une seule fois. Pour annuler votre choix, supprimez le site concerné dans le panneau Mise en réseau coopérative.

Si vous étiez en train de modifier une ressource modifiée par un homologue, vous êtes invité à ingérer la modification dans le créateur ou l’éditeur. Si vous choisissez **[!UICONTROL Oui]**, le créateur ou l’éditeur ignore les modifications apportées à la ressource et importe la ressource mise à jour. Si vous choisissez **[!UICONTROL Non]**, la ressource reste inchangée dans le créateur ou l’éditeur et toutes les modifications que vous avez apportées sont conservées au cours de cette session.

Lorsque vous enregistrez la ressource, vous êtes averti qu’une version plus récente existe. Vous êtes ensuite invité à confirmer si vous souhaitez remplacer la ressource par vos modifications.
