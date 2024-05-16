---
title: Liaison des visionneuses de zoom à des pages web
description: Découvrez comment lier les visionneuses de zoom à vos pages web dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: 2073d95b-1600-481f-8038-d29e8acacf7d
topic: Administration, Content Management, Development
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 23%

---

# Liaison des visionneuses de zoom à des pages web{#linking-zoom-viewers-to-your-web-pages}

Vos sites Web et applications accèdent au contenu du serveur d’images Dynamic Media au moyen de chaînes d’URL ou de code incorporé. Cet accès inclut les images principales et les cibles de zoom associées. Elle comprend également des paramètres prédéfinis de visionneuse de zoom. Ces chaînes URL sont activées au cours du processus de publication. Pour placer ces chaînes URL ou le code incorporé dans vos pages Web et applications, vous devez les copier depuis Adobe Dynamic Media Classic.

>[!NOTE]
>
>l’URL n’est activée qu’une fois le fichier publié.

## Copie de l’URL d’une visionneuse de zoom {#copying-a-zoom-viewer-url}

1. Dans le panneau Bibliothèque de fichiers sur la gauche, accédez au dossier Fichiers qui contient la visionneuse de zoom dont vous voulez copier le code incorporé.
1. Au-dessus du panneau de navigation des fichiers, sur le côté droit de la barre d’outils, exécutez l’une des opérations suivantes :

   * Sélectionner **[!UICONTROL Affichage de la grille]** ou **[!UICONTROL Mode Liste]**. Dans le panneau de navigation des fichiers, cliquez deux fois sur un fichier pour l’ouvrir dans le mode Affichage des détails. Dans le panneau URL et code intégré à droite, sélectionnez **[!UICONTROL Copier l’URL]** à droite de la visionneuse que vous souhaitez.
   * Sélectionner **[!UICONTROL Affichage de la grille]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis sous l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, sous la colonne Actions du tableau, sélectionnez **[!UICONTROL Copier l’URL]**.

   * Sélectionner **[!UICONTROL Mode Liste]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis, à droite de l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, sous la colonne Actions du tableau, sélectionnez **[!UICONTROL Copier l’URL]**.

   * Sélectionner **[!UICONTROL Affichage de la grille]**, **[!UICONTROL Mode Liste]**, ou **[!UICONTROL Affichage des détails]**. Dans la même barre d’outils, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, sous la colonne Actions du tableau, sélectionnez **[!UICONTROL Copier l’URL]**.

## Ajout des URL de la visionneuse de zoom à une page web {#adding-zoom-viewer-urls-to-your-web-page}

En règle générale, les visiteurs effectuent un zoom sur les images d’un site web en sélectionnant d’abord une icône Zoom (souvent l’icône affiche l’image d’une loupe). La sélection de cette icône lance une page Web dynamique (ASP ou JSP) qui affiche l’image dans une fenêtre contextuelle. C’est dans cette fenêtre contextuelle que les visiteurs effectuent un zoom sur l’image.

Pour plus d’informations et d’exemples de code, voir la section [Incorporer la visionneuse de zoom de base HTML5 dans le guide de référence des visionneuses d’Adobes](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2).

## Copie de la copie incorporée d’une visionneuse de zoom {#copying-the-embed-copy-of-a-zoom-viewer}

La fonction Code incorporé permet de vérifier le code de la visionneuse de zoom sélectionnée. Vous pouvez également copier le code dans le Presse-papiers afin de le coller dans vos pages web pour le déploiement de la visionneuse. Vous ne pouvez pas modifier le code dans la boîte de dialogue Code incorporé.

**Pour copier le code incorporé d’une visionneuse de zoom :**

1. Dans le panneau Bibliothèque de ressources sur le côté gauche, accédez au dossier de ressources qui contient la visionneuse de zoom dont vous souhaitez copier le code intégré.
1. Au-dessus de panneau de navigation des fichiers, sur le côté droit de la barre d’outils, exécutez l’une des opérations suivantes :

   * Sélectionner **[!UICONTROL Affichage de la grille]**. Dans le panneau de navigation des fichiers, cliquez deux fois sur un fichier pour l’ouvrir dans le mode Affichage des détails. Dans le panneau URL et code intégré à droite, sélectionnez **[!UICONTROL Code incorporé]** à droite de la visionneuse que vous souhaitez.
   * Sélectionner **[!UICONTROL Affichage de la grille]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis sous l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, sous la colonne Actions du tableau, sélectionnez **[!UICONTROL Code incorporé]**.

   * Sélectionner **[!UICONTROL Mode Liste]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis, à droite de l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, sous la colonne Actions du tableau, sélectionnez **[!UICONTROL Code incorporé]**.

   * Sélectionner **[!UICONTROL Affichage de la grille]**, **[!UICONTROL Mode Liste]**, ou **[!UICONTROL Affichage des détails]**. Dans la même barre d’outils, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, sous la colonne Actions du tableau, sélectionnez **[!UICONTROL Code incorporé]**.

1. Dans la boîte de dialogue Code incorporé, sélectionnez **[!UICONTROL Copier dans le Presse-papiers]**.

   Vous ne pouvez pas modifier le code dans la boîte de dialogue Code incorporé.

1. Sélectionner **[!UICONTROL Fermer]**.
