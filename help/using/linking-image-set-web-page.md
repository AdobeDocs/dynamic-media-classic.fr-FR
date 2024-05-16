---
title: Liaison d’une visionneuse d’images à une page Web
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
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 24%

---

# Liaison d’une visionneuse d’images à une page Web{#linking-an-image-set-to-a-web-page}

Une fois que vous avez publié une visionneuse d’images, vous pouvez copier l’URL associée ou son code intégré en vue de l’utiliser dans votre site web ou dans votre application. Vous pouvez ensuite déployer l’URL ou coller le code incorporé si nécessaire afin que les utilisateurs puissent afficher la visionneuse d’images sur votre site Web ou dans votre application.

>[!NOTE]
>
>l’URL n’est activée qu’une fois le fichier publié.

## Copie d’une URL de visionneuse d’images {#copying-an-image-set-url}

1. Dans la liste déroulante Afficher du panneau de navigation des ressources, sélectionnez **[!UICONTROL Visionneuse d’images]**.
1. Dans le panneau Bibliothèque de fichiers sur la gauche, accédez au dossier Fichiers qui contient la visionneuse d’images dont vous voulez copier le code incorporé.
1. Au-dessus du panneau de navigation des fichiers, sur le côté droit de la barre d’outils, exécutez l’une des opérations suivantes :

   * Sélectionner **[!UICONTROL Affichage de la grille]**. Dans le panneau de navigation des fichiers, cliquez deux fois sur un fichier pour l’ouvrir dans le mode Affichage des détails. Dans le panneau URL et code intégré à droite, sélectionnez **[!UICONTROL Copier l’URL]** à droite de la visionneuse que vous souhaitez.
   * Sélectionner **[!UICONTROL Affichage de la grille]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis sous l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, sous la colonne Actions du tableau, sélectionnez **[!UICONTROL Copier l’URL]**.

   * Sélectionner **[!UICONTROL Mode Liste]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis, à droite de l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, sous la colonne Actions du tableau, sélectionnez **[!UICONTROL Copier l’URL]**.

   * Sélectionner **[!UICONTROL Affichage de la grille]**, **[!UICONTROL Mode Liste]**, ou **[!UICONTROL Affichage des détails]**. Dans la même barre d’outils, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, sous la colonne Actions du tableau, sélectionnez **[!UICONTROL Copier l’URL]**.

## Ajout d’URL de visionneuse d’images à une page web {#adding-image-set-urls-to-your-web-page}

La méthode la plus courante pour déployer une visionneuse d’images consiste à placer un lien (au moyen d’une icône de navigation) sur votre page Web. Lorsque cette option est sélectionnée, le lien lance une page dynamique (JSP) qui affiche la visionneuse d’images dans une fenêtre de zoom contextuelle. Le lien de zoom ouvre une fenêtre contextuelle qui contient la fonction de zoom réelle.

Pour plus d’informations et d’exemples de code, voir [Incorporer la visionneuse de zoom HTML5 dans le guide de référence des visionneuses d’Adobes](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/zoom/c-html5-20-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2).

## Copie du code incorporé d’une visionneuse d’images {#copying-the-embed-code-of-an-image-set-viewer}

L’utilisation de la fonction Code incorporé permet de vérifier le code de la visionneuse d’images sélectionnée. Vous pouvez également copier le code dans le Presse-papiers afin de le coller dans vos pages web pour le déploiement de la visionneuse. Vous ne pouvez pas modifier le code dans la boîte de dialogue Code incorporé.

**Pour copier le code incorporé d’une visionneuse d’images :**

1. Dans la liste déroulante Afficher du panneau de navigation des ressources, sélectionnez **[!UICONTROL Visionneuse d’images]**.
1. Dans le panneau Bibliothèque de fichiers sur la gauche, accédez au dossier Fichiers qui contient la visionneuse d’images dont vous voulez copier le code incorporé.
1. Au-dessus du panneau de navigation des fichiers, sur le côté droit de la barre d’outils, exécutez l’une des opérations suivantes :

   * Sélectionner **[!UICONTROL Affichage de la grille]**. Dans le panneau de navigation des fichiers, cliquez deux fois sur un fichier pour l’ouvrir dans le mode Affichage des détails. Dans le panneau URL situé à droite, sélectionnez **[!UICONTROL Code incorporé]**.
   * Sélectionner **[!UICONTROL Affichage de la grille]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis sous l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, sous la colonne Actions du tableau, sélectionnez **[!UICONTROL Code incorporé]**.

   * Sélectionner **[!UICONTROL Mode Liste]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis, à droite de l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, sous la colonne Actions du tableau, sélectionnez **[!UICONTROL Code incorporé]**.

   * Sélectionner **[!UICONTROL Affichage de la grille]**, **Mode Liste**, ou **Affichage des détails**. Dans la même barre d’outils, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, sous la colonne Actions du tableau, sélectionnez **[!UICONTROL Code incorporé]**.

1. Dans la boîte de dialogue Code incorporé, sélectionnez **[!UICONTROL Copier dans le Presse-papiers]**.

   Vous ne pouvez pas modifier le code dans la boîte de dialogue Code incorporé.

1. Sélectionner **[!UICONTROL Fermer]**.

>[!MORELIKETHIS]
>
>* [Publier](publishing-files.md#publishing_files)
