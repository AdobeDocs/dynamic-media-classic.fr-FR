---
title: Liaison d’une visionneuse à 360° à une page Web
seo-title: Liaison d’une visionneuse à 360° à une page Web
description: 'null'
seo-description: Découvrez comment lier une visionneuse à 360 ° à une page Web.
uuid: d 3 c 5773 e -60 c 4-4 e 8 b -9 c 48-e 1 e 3 eb 8028 d 0
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/spin_ sets
discoiquuid: 651 b 21 ef-e 322-4 e 6 d -8 e 37-45 ffd 56 f 7 a 58
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Liaison d’une visionneuse à 360° à une page Web{#linking-a-spin-set-to-a-web-page}

Les sites Web et applications accèdent au contenu du serveur Dynamic Media Image Server, y compris aux visionneuses à 360 °, au moyen de chaînes URL ou de code incorporé. Ces chaînes URL sont activées au cours du processus de publication. Pour placer la chaîne URL ou le code incorporé de la visionneuse à 360° dans vos pages Web ou applications, copiez-la ou le depuis Scene7 Publishing System.

>[!NOTE]
>
>l’URL n’est activée qu’une fois le fichier publié.

## Copie de l’URL d’une visionneuse à 360° {#copying-a-spin-set-url}

1. Dans la liste déroulante Afficher du panneau de navigation des fichiers, cliquez sur **Visionneuse à 360°**.
1. Dans le panneau Bibliothèque de fichiers sur la gauche, accédez au dossier Fichiers qui contient la visionneuse à 360° dont vous voulez copier le code incorporé.
1. Au-dessus du panneau de navigation des fichiers, sur le côté droit de la barre d’outils, exécutez l’une des opérations suivantes :

   * Cliquez sur **Affichage de la grille**. Dans le panneau de navigation des fichiers, cliquez deux fois sur un fichier pour l’ouvrir dans le mode Affichage des détails. Dans le panneau des URL et d’intégration du code, sur la droite, cliquez sur **Copier l’URL** à droite de la visionneuse appropriée.
   * Cliquez sur **Affichage de la grille**. Dans le panneau de navigation des fichiers, sélectionnez un fichier, puis sous l’image miniature, cliquez sur **Prévisualiser** &gt; **Liste des visionneuses**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Copier l’URL**.

   * Cliquez sur **Affichage par liste**. Dans le panneau de navigation des fichiers, sélectionnez un fichier, puis à droite de l’image miniature, cliquez sur **Prévisualiser** &gt; **Liste des visionneuses**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Copier l’URL**.

   * Cliquez sur **Affichage de la grille**, **Affichage par liste** ou **Affichage des détails**. Dans la même barre d’outils, cliquez sur **Prévisualiser** &gt; **Liste des visionneuses**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Copier l’URL**.

## Ajout d’URL de visionneuse à 360° à une page Web {#adding-spin-set-urls-to-your-web-page}

Les visionneuses à 360° sont déployées comme toutes les visionneuses de zoom par le biais d’une page dynamique (ASP ou JSP) qui affiche la visionneuse à 360° dans une fenêtre de zoom. L'appel d'URL vers la plate-forme Dynamic Media Classic suit le même protocole sur la visionneuse de zoom. Cependant, le nom du paramètre prédéfini de visionneuse dépend du paramètre prédéfini que l’administrateur a défini comme paramètre prédéfini de visionneuse à 360° par défaut. Par exemple, la syntaxe de l’URL en différé suivante contient le nom de paramètre prédéfini `viewer.jsp` et le paramètre SKU est désormais le nom de la visionneuse à 360° :

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

Dans cet exemple de syntaxe d’URL (le lien n’est pas en direct), notez le numéro SKU ( `sku=backpack_spin`). The string after `sku=` is the Spin Set name ( `backpack spin`).

## Copie du code incorporé d’une visionneuse à 360°{#copying-the-embed-code-of-a-spin-set-viewer}

La fonction Code incorporé permet de vérifier le code de la visionneuse à 360° sélectionnée. Vous pouvez aussi copier le code dans le Presse-papiers afin de le coller dans vos pages Web pour le déploiement de la visionneuse. Vous ne pouvez pas modifier le code dans la boîte de dialogue Code incorporé.

**Copie du code incorporé d’une visionneuse à 360°**

1. Dans la liste déroulante Afficher du panneau de navigation des fichiers, cliquez sur **Visionneuse à 360°**.
1. Dans le panneau Bibliothèque de fichiers sur la gauche, accédez au dossier Fichiers qui contient la visionneuse à 360° dont vous voulez copier le code incorporé.
1. Au-dessus du panneau de navigation des fichiers, sur le côté droit de la barre d’outils, exécutez l’une des opérations suivantes :

   * Cliquez sur **Affichage de la grille**. Dans le panneau de navigation des fichiers, cliquez deux fois sur un fichier pour l’ouvrir dans le mode Affichage des détails. Dans le panneau des URL et du code incorporé sur la droite, cliquez sur **Code incorporé** sur la droite de la visionneuse appropriée.
   * Cliquez sur **Affichage de la grille**. Dans le panneau de navigation des fichiers, sélectionnez un fichier, puis sous l’image miniature, cliquez sur **Prévisualiser** &gt; **Liste des visionneuses**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Code incorporé**.

   * Cliquez sur **Affichage par liste**. Dans le panneau de navigation des fichiers, sélectionnez un fichier, puis à droite de l’image miniature, cliquez sur **Prévisualiser** &gt; **Liste des visionneuses**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Code incorporé**.

   * Cliquez sur **Affichage de la grille**, **Affichage par liste** ou **Affichage des détails**. Dans la même barre d’outils, cliquez sur **Prévisualiser** &gt; **Liste des visionneuses**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **Code incorporé**.

1. Dans la boîte de dialogue Code incorporé, cliquez sur **Copier dans le Presse-papiers**.

   Vous ne pouvez pas modifier le code dans la boîte de dialogue Code incorporé.

1. Cliquez sur Fermer.
