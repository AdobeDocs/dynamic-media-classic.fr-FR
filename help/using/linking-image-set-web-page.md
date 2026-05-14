---
title: Liaison d’une visionneuse d’images à une page web
description: Découvrez comment lier une visionneuse d’images à une page web dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: df4e5218-2a66-413c-b247-b2a16d884041
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T20:02:41.296Z'
TQID: 'https://experienceleague.adobe.com/d1hGtQAgf1wwjIAbeRJ-kQW4kfglXNu5VSIGxRTgxnc'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 703
ht-degree: 18%

---

# Liaison d’une visionneuse d’images à une page web{#linking-an-image-set-to-a-web-page}

Après avoir publié une visionneuse d’images, vous pouvez copier son URL associée ou son code intégré pour l’utiliser dans votre site web ou application. Vous pouvez ensuite déployer l’URL ou coller le code incorporé si nécessaire afin que les utilisateurs puissent afficher la visionneuse d’images sur votre site web ou application.

>[!NOTE]
>
>l’URL n’est activée qu’une fois le fichier publié.

## Copie d’une URL de visionneuse d’images {#copying-an-image-set-url}

1. Dans le panneau Exploration des ressources, dans la liste déroulante Afficher, sélectionnez **[!UICONTROL Visionneuse d’images]**.
1. Dans le panneau Bibliothèque de fichiers sur la gauche, accédez au dossier Fichiers qui contient la visionneuse d’images dont vous voulez copier le code incorporé.
1. Au-dessus de panneau de navigation des fichiers, sur le côté droit de la barre d’outils, exécutez l’une des opérations suivantes :

   * Sélectionnez **[!UICONTROL Vue Grille]**. Dans le panneau de navigation des fichiers, cliquez deux fois sur un fichier pour l’ouvrir dans le mode Affichage des détails. Dans le panneau **[!UICONTROL URL et code intégré]** à droite, sélectionnez **[!UICONTROL Copier l’URL]** à droite de la visionneuse souhaitée.
   * Sélectionnez **[!UICONTROL Vue Grille]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis, sous l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Sur la page Liste des visionneuses, dans la colonne Actions du tableau, sélectionnez **[!UICONTROL Copier l’URL]**.

   * Sélectionnez **[!UICONTROL Vue Liste]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis à droite de l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste de visionneuses]**.

     Sur la page Liste des visionneuses, dans la colonne Actions du tableau, sélectionnez **[!UICONTROL Copier l’URL]**.

   * Sélectionnez **[!UICONTROL Vue Grille]**, **[!UICONTROL Vue Liste]** ou **[!UICONTROL Vue Détail]**. Dans la même barre d’outils, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Sur la page Liste des visionneuses, dans la colonne Actions du tableau, sélectionnez **[!UICONTROL Copier l’URL]**.

## Ajout d’URL de visionneuse d’images à une page web {#adding-image-set-urls-to-your-web-page}

La méthode la plus courante pour déployer une visionneuse d’images consiste à placer un lien (au moyen d’une icône de navigation) sur votre page web. Lorsque ce lien est sélectionné, il lance une page dynamique (JSP) qui affiche la visionneuse d’images dans une fenêtre pop-up zoom. Le lien de zoom affiche une fenêtre contextuelle contenant l’affichage agrandi proprement dit.

Pour plus d’informations et d’exemples de code, consultez la section [Visionneuse zoom HTML5 intégrée](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/zoom/c-html5-20-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2) du Guide de référence des visionneuses Adobe.

## Copie du code incorporé d’une visionneuse d’images {#copying-the-embed-code-of-an-image-set-viewer}

Grâce à la fonction de code incorporé, vous pouvez réviser le code de visionneuse de la visionneuse d’images sélectionnée. Vous pouvez également copier le code dans le presse-papiers afin de le coller dans vos pages web pour le déploiement de la visionneuse. Vous ne pouvez pas modifier le code dans la boîte de dialogue Code incorporé.

**Pour copier le code incorporé d’une visionneuse d’images, procédez comme suit**

1. Dans le panneau Exploration des ressources, dans la liste déroulante Afficher, sélectionnez **[!UICONTROL Visionneuse d’images]**.
1. dans le panneau Bibliothèque de ressources sur le côté gauche, accédez au dossier de ressources contenant la visionneuse d’images dont vous souhaitez copier le code incorporé.
1. Au-dessus de panneau de navigation des fichiers, sur le côté droit de la barre d’outils, exécutez l’une des opérations suivantes :

   * Sélectionnez **[!UICONTROL Vue Grille]**. Dans le panneau de navigation des fichiers, cliquez deux fois sur un fichier pour l’ouvrir dans le mode Affichage des détails. Dans le panneau URL à droite, sélectionnez **[!UICONTROL Code intégré]**.
   * Sélectionnez **[!UICONTROL Vue Grille]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis, sous l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, dans la colonne Actions du tableau, sélectionnez **[!UICONTROL Code incorporé]**.

   * Sélectionnez **[!UICONTROL Vue Liste]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis à droite de l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste de visionneuses]**.

     Dans la page Liste des visionneuses, dans la colonne Actions du tableau, sélectionnez **[!UICONTROL Code incorporé]**.

   * Sélectionnez **[!UICONTROL Vue Grille]**, **Vue Liste** ou **Vue Détail**. Dans la même barre d’outils, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, dans la colonne Actions du tableau, sélectionnez **[!UICONTROL Code incorporé]**.

1. Dans la boîte de dialogue **[!UICONTROL Code incorporé]**, sélectionnez **[!UICONTROL Copier dans le presse-papiers]**.

   La modification du code n’est pas autorisée dans la boîte de dialogue **[!UICONTROL Code intégré]**.

1. Sélectionnez **[!UICONTROL Fermer]**.

>[!MORELIKETHIS]
>
>* [Publier](publishing-files.md#publishing_files)
