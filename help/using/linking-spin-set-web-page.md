---
title: Liaison d’une visionneuse à 360° à une page web
description: Découvrez comment lier une visionneuse à 360° à une page web dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
topic: Content Management
level: Intermediate
source-git-commit: c4613c78347c4bda3d84747a72146617158c03b6
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 21%

---

# Liaison d’une visionneuse à 360° à une page web{#linking-a-spin-set-to-a-web-page}

Les sites web et les applications accèdent au contenu du serveur d’images Dynamic Media, y compris les visionneuses à 360°, par le biais de chaînes URL ou de code incorporé. Ces chaînes URL sont activées au cours du processus de publication. Pour placer la chaîne d’URL ou le code intégré de la visionneuse à 360° dans vos pages web et applications, vous devez le copier depuis Adobe Dynamic Media Classic.

>[!NOTE]
>
>l’URL n’est activée qu’une fois le fichier publié.

## Copie d’une URL de visionneuse à 360° {#copying-a-spin-set-url}

1. Dans le panneau de navigation des ressources, dans la liste déroulante Afficher, sélectionnez **[!UICONTROL Visionneuse à 360°]**.
1. dans le panneau Bibliothèque de ressources sur le côté gauche, accédez au dossier de ressources contenant la visionneuse à 360° dont vous souhaitez copier le code intégré.
1. Au-dessus de panneau de navigation des fichiers, sur le côté droit de la barre d’outils, exécutez l’une des opérations suivantes :

   * Sélectionnez **[!UICONTROL Vue Grille]**. Dans le panneau de navigation des fichiers, cliquez deux fois sur un fichier pour l’ouvrir dans le mode Affichage des détails. Dans le panneau URL et code intégré à droite, sélectionnez **[!UICONTROL Copier l’URL]** à droite de la visionneuse souhaitée.
   * Sélectionnez **[!UICONTROL Vue Grille]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis, sous l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Sur la page Liste des visionneuses, dans la colonne Actions du tableau, sélectionnez **[!UICONTROL Copier l’URL]**.

   * Sélectionnez **[!UICONTROL Vue Liste]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis à droite de l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste de visionneuses]**.

     Sur la page Liste des visionneuses, dans la colonne Actions du tableau, sélectionnez **[!UICONTROL Copier l’URL]**.

   * Sélectionnez **[!UICONTROL Vue Grille]**, **[!UICONTROL Vue Liste]** ou **[!UICONTROL Vue Détail]**. Dans la même barre d’outils, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Sur la page Liste des visionneuses, dans la colonne Actions du tableau, sélectionnez **[!UICONTROL Copier l’URL]**.

## Ajout d’URL de visionneuse à 360° à une page web {#adding-spin-set-urls-to-your-web-page}

Les visionneuses à 360° sont déployées comme toutes les visionneuses de zoom par le biais d’une page dynamique (ASP ou JSP) qui affiche la visionneuse à 360° dans une fenêtre de zoom. L’appel de l’URL à la plateforme Adobe Dynamic Media Classic suit le même protocole sur la visionneuse zoom. Cependant, le nom du paramètre prédéfini de visionneuse dépend du paramètre prédéfini que l’administrateur a défini comme paramètre prédéfini de visionneuse à 360° par défaut. Par exemple, l’exemple de syntaxe d’URL non active suivant inclut un nom de paramètre prédéfini appelé `viewer.jsp` et le paramètre SKU est désormais le nom de la visionneuse à 360° :

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

Dans cet exemple de syntaxe d’URL (le lien n’est pas actif), notez un numéro de SKU ( `sku=backpack_spin`). La chaîne après `sku=` est le nom de la visionneuse à 360° ( `backpack spin`).

## Copie du code incorporé d’une visionneuse à 360° {#copying-the-embed-code-of-a-spin-set-viewer}

Grâce à la fonction Code incorporé , vous pouvez réviser le code de la visionneuse pour la visionneuse à 360° sélectionnée. Vous pouvez également copier le code dans le presse-papiers afin de le coller dans vos pages web pour le déploiement de la visionneuse. Vous ne pouvez pas modifier le code dans la boîte de dialogue Code incorporé.

**Pour copier le code incorporé d’une visionneuse à 360°, procédez comme suit**

1. Dans le panneau de navigation des ressources, dans la liste déroulante Afficher, sélectionnez **[!UICONTROL Visionneuse à 360°]**.
1. dans le panneau Bibliothèque de ressources sur le côté gauche, accédez au dossier de ressources contenant la visionneuse à 360° dont vous souhaitez copier le code intégré.
1. Au-dessus de panneau de navigation des fichiers, sur le côté droit de la barre d’outils, exécutez l’une des opérations suivantes :

   * Sélectionnez **[!UICONTROL Vue Grille]**. Dans le panneau de navigation des fichiers, cliquez deux fois sur un fichier pour l’ouvrir dans le mode Affichage des détails. Dans le panneau URL et code intégré à droite, sélectionnez **[!UICONTROL Code intégré]** à droite de la visionneuse de votre choix.
   * Sélectionnez **[!UICONTROL Vue Grille]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis, sous l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, dans la colonne Actions du tableau, sélectionnez **[!UICONTROL Code incorporé]**.

   * Sélectionnez **[!UICONTROL Vue Liste]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis à droite de l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste de visionneuses]**.

     Dans la page Liste des visionneuses, dans la colonne Actions du tableau, sélectionnez **[!UICONTROL Code incorporé]**.

   * Sélectionnez **[!UICONTROL Vue Grille]**, **[!UICONTROL Vue Liste]** ou **[!UICONTROL Vue Détail]**. Dans la même barre d’outils, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, dans la colonne Actions du tableau, sélectionnez **[!UICONTROL Code incorporé]**.

1. Dans la boîte de dialogue Code incorporé, sélectionnez **[!UICONTROL Copier dans le presse-papiers]**.

   Vous ne pouvez pas modifier le code dans la boîte de dialogue Code incorporé.

1. Sélectionnez **[!UICONTROL Fermer]**.
