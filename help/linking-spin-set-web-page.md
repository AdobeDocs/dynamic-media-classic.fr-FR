---
title: Liaison d’une visionneuse à 360° à une page Web
description: Découvrez comment lier une visionneuse à 360° à une page Web.
uuid: d3c5773e-60c4-4e8b-9c48-e1e3eb8028d0
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 651b21ef-e322-4e6d-8e37-45ffd56f7a58
feature: Dynamic Media Classic, Visionneuses, Visionneuses à 360°
role: Business Practitioner
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
translation-type: tm+mt
source-git-commit: 38d09bb78834c6b3614bf2b96fd6aee5661e0a5a
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 86%

---

# Liaison d’une visionneuse à 360° à une page Web{#linking-a-spin-set-to-a-web-page}

Les sites Web et applications accèdent au contenu du serveur Dynamic Media Image Server, y compris aux visionneuses à 360°, au moyen de chaînes URL ou de code incorporé. Ces chaînes URL sont activées au cours du processus de publication. Pour placer la chaîne URL ou le code incorporé de votre visionneuse à 360° dans vos pages Web et applications, copiez-la depuis Dynamic Media Classic.

>[!NOTE]
>
>l’URL n’est activée qu’une fois le fichier publié.

## Copie de l’URL d’une visionneuse à 360°  {#copying-a-spin-set-url}

1. Dans la liste déroulante Afficher du panneau de navigation des fichiers, cliquez sur **[!UICONTROL Visionneuse à 360°]**.
1. Dans le panneau Bibliothèque de fichiers sur la gauche, accédez au dossier Fichiers qui contient la visionneuse à 360° dont vous voulez copier le code incorporé.
1. Au-dessus du panneau de navigation des fichiers, sur le côté droit de la barre d’outils, exécutez l’une des opérations suivantes :

   * Cliquez sur **[!UICONTROL Affichage de la grille]**. Dans le panneau de navigation des fichiers, cliquez deux fois sur un fichier pour l’ouvrir dans le mode Affichage des détails. Dans le panneau des URL et d’intégration du code, sur la droite, cliquez sur **[!UICONTROL Copier l’URL]** à droite de la visionneuse appropriée.
   * Cliquez sur **[!UICONTROL Affichage de la grille]**. Dans le panneau de navigation des fichiers, sélectionnez un fichier, puis sous l’image miniature, cliquez sur **[!UICONTROL Prévisualiser]** > **[!UICONTROL Liste des visionneuses]**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **[!UICONTROL Copier l’URL]**.

   * Cliquez sur **[!UICONTROL Affichage par liste]**. Dans le panneau de navigation des fichiers, sélectionnez un fichier, puis à droite de l’image miniature, cliquez sur **[!UICONTROL Prévisualiser]** > **[!UICONTROL Liste des visionneuses]**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **[!UICONTROL Copier l’URL]**.

   * Cliquez sur **[!UICONTROL Affichage de la grille]**, **[!UICONTROL Affichage par liste]** ou **[!UICONTROL Affichage des détails]**. Dans la même barre d’outils, cliquez sur **[!UICONTROL Prévisualiser]** > **[!UICONTROL Liste des visionneuses]**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **[!UICONTROL Copier l’URL]**.

## Ajout d’URL de visionneuse à 360° à une page Web  {#adding-spin-set-urls-to-your-web-page}

Les visionneuses à 360° sont déployées comme toutes les visionneuses de zoom par le biais d’une page dynamique (ASP ou JSP) qui affiche la visionneuse à 360° dans une fenêtre de zoom. L’appel d’URL vers la plate-forme Dynamic Media Classic suit le même protocole sur la visionneuse de zoom. Cependant, le nom du paramètre prédéfini de visionneuse dépend du paramètre prédéfini que l’administrateur a défini comme paramètre prédéfini de visionneuse à 360° par défaut. Par exemple, la syntaxe de l’URL en différé suivante contient le nom de paramètre prédéfini `viewer.jsp` et le paramètre SKU est désormais le nom de la visionneuse à 360° :

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

Dans cet exemple de syntaxe d’URL (le lien n’est pas en direct), notez le numéro SKU ( `sku=backpack_spin`). La chaîne située après `sku=` correspond au nom de la visionneuse à 360° ( `backpack spin`).

## Copie du code incorporé d’une visionneuse à 360°{#copying-the-embed-code-of-a-spin-set-viewer}

La fonction Code incorporé permet de vérifier le code de la visionneuse à 360° sélectionnée. Vous pouvez aussi copier le code dans le Presse-papiers afin de le coller dans vos pages Web pour le déploiement de la visionneuse. Vous ne pouvez pas modifier le code dans la boîte de dialogue Intégrer le code.

**Pour copier le code incorporé d’une visionneuse à 360° :**

1. Dans la liste déroulante Afficher du panneau de navigation des fichiers, cliquez sur **[!UICONTROL Visionneuse à 360°]**.
1. Dans le panneau Bibliothèque de fichiers sur la gauche, accédez au dossier Fichiers qui contient la visionneuse à 360° dont vous voulez copier le code incorporé.
1. Au-dessus du panneau de navigation des fichiers, sur le côté droit de la barre d’outils, exécutez l’une des opérations suivantes :

   * Cliquez sur **[!UICONTROL Affichage de la grille]**. Dans le panneau de navigation des fichiers, cliquez deux fois sur un fichier pour l’ouvrir dans le mode Affichage des détails. Dans le panneau des URL et du code incorporé sur la droite, cliquez sur **[!UICONTROL Code incorporé]** sur la droite de la visionneuse appropriée.
   * Cliquez sur **[!UICONTROL Affichage de la grille]**. Dans le panneau de navigation des fichiers, sélectionnez un fichier, puis sous l’image miniature, cliquez sur **[!UICONTROL Prévisualiser]** > **[!UICONTROL Liste des visionneuses]**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **[!UICONTROL Code incorporé]**.

   * Cliquez sur **[!UICONTROL Affichage par liste]**. Dans le panneau de navigation des fichiers, sélectionnez un fichier, puis à droite de l’image miniature, cliquez sur **[!UICONTROL Prévisualiser]** > **[!UICONTROL Liste des visionneuses]**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **[!UICONTROL Code incorporé]**.

   * Cliquez sur **[!UICONTROL Affichage de la grille]**, **[!UICONTROL Affichage par liste]** ou **[!UICONTROL Affichage des détails]**. Dans la même barre d’outils, cliquez sur **[!UICONTROL Prévisualiser]** > **[!UICONTROL Liste des visionneuses]**.

      Dans la page Liste des visionneuses, dans la colonne Actions du tableau, cliquez sur **[!UICONTROL Code incorporé]**.

1. Dans la boîte de dialogue Code incorporé, cliquez sur **[!UICONTROL Copier dans le Presse-papiers]**.

   Vous ne pouvez pas modifier le code dans la boîte de dialogue Code intégré.

1. Cliquez sur **[!UICONTROL Fermer]**.
