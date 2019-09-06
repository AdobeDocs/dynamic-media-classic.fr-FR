---
title: Partage de modifications de fichier en temps réel avec des pairs
seo-title: Partage de modifications de fichier en temps réel avec des pairs
description: 'null'
seo-description: Découvrez comment partager des modifications de ressources avec des pairs en temps réel.
uuid: 13 fa 4 f 6 e -66 bf -4682-96 a 9-0 e 7040706 f 53
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/managing_ assets
discoiquuid: ca 7 c 8 a 7 f -76 f 4-4 a 25-8 c 36-617 a 029 e 55 be
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Partage de modifications de fichier en temps réel avec des pairs{#sharing-asset-changes-with-peers-in-real-time}

Avec plusieurs copies de Dynamic Media Classic s'exécutant sur un ou plusieurs ordinateurs de la même société, les actions suivantes de tout client Dynamic Media Classic sont mises à jour en temps réel avec tous les clients pairs :

* Edition d’un fichier (zone de création, éditeur d’images, etc.)
* Modification du nom d’un fichier
* Suppression d’un fichier
* Déplacement d’un fichier
* Téléchargement d’un ou plusieurs fichiers (sur l’ordinateur et le FTP)
* Création, suppression ou modification du nom d’un dossier

Lorsqu’une modification est apportée dans le client d’origine, tous les clients pairs connectés dans la même société sont mis à jour. Les modifications sont appliquées aux pairs sans aucune notification, sauf si un pair modifie un fichier édité dans un éditeur d’images ou une zone de création.

Lorsque vous vous connectez, le lecteur Flash vous invite à accepter ou à rejeter les modifications de pairs. Vous pouvez « mémoriser » votre choix afin que la question ne vous soit plus posée par la suite. Pour annuler votre choix, supprimez le site concerné dans le panneau Mise en réseau coopérative.

Si vous éditez un fichier modifié par un pair, vous êtes invité à intégrer la modification dans la zone de création ou l’éditeur. Si vous acceptez, la zone de création ou l’éditeur ignore toutes vos modifications et importe le fichier modifié par le pair. Si vous refusez, le fichier reste tel quel dans la zone de création ou l’éditeur, et toutes les modifications que vous avez apportées sont conservées au cours de cette session.

Au moment d’enregistrer le fichier, vous êtes informé qu’il existe une nouvelle version et êtes invité à remplacer cette version par la vôtre.
