---
title: Liaison d’un catalogue électronique à une page web
description: Découvrez comment lier un catalogue électronique à une page web dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: aee72576-1e3e-401c-953d-cc2be27f7dfd
topic: Integrations, Development
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 23%

---

# Liaison d’un catalogue électronique à une page web{#linking-an-ecatalog-to-a-web-page}

Vos sites web et applications accèdent au contenu du serveur d’images Dynamic Media, y compris les catalogues électroniques, par le biais de chaînes URL ou de code incorporé. Ces chaînes URL sont activées au cours du processus de publication. Pour placer la chaîne URL ou le code incorporé de votre catalogue électronique dans vos pages Web et applications, vous devez le copier à partir d’Adobe Dynamic Media Classic.

>[!NOTE]
>
>l’URL n’est activée qu’une fois le fichier publié.

## Copie d’une URL de catalogue électronique {#copying-an-ecatalog-url}

1. Dans le panneau Exploration des ressources, dans la liste déroulante Afficher, sélectionnez **[!UICONTROL Catalogue]**.
1. dans le panneau Bibliothèque de ressources sur le côté gauche, accédez au dossier de ressources contenant le catalogue électronique dont vous souhaitez copier le code intégré.
1. Au-dessus de panneau de navigation des fichiers, sur le côté droit de la barre d’outils, exécutez l’une des opérations suivantes :

   * Sélectionnez **[!UICONTROL Vue Grille]**. Dans le panneau de navigation des fichiers, cliquez deux fois sur un fichier pour l’ouvrir dans le mode Affichage des détails. Dans le panneau URL et code intégré à droite, sélectionnez **[!UICONTROL Copier l’URL]** à droite de la visionneuse souhaitée.
   * Sélectionnez **[!UICONTROL Vue Grille]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis, sous l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Sur la page Liste des visionneuses, dans la colonne Actions du tableau, sélectionnez **[!UICONTROL Copier l’URL]**.

   * Sélectionnez **[!UICONTROL Vue Liste]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis à droite de l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste de visionneuses]**.

     Sur la page Liste des visionneuses, dans la colonne Actions du tableau, sélectionnez **[!UICONTROL Copier l’URL]**.

   * Sélectionnez **[!UICONTROL Vue Grille]**, **[!UICONTROL Vue Liste]** ou **[!UICONTROL Vue Détail]**. Dans la même barre d’outils, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Sur la page Liste des visionneuses, dans la colonne Actions du tableau, sélectionnez **Copier l’URL**.

## Ajout d’URL de catalogue électronique à une page web {#adding-ecatalog-urls-to-your-web-page}

La méthode la plus courante pour déployer un catalogue électronique consiste à placer un lien sous la forme d’une page de garde de miniature de catalogue électronique sur votre page web. Consultez votre équipe informatique pour vous assurer que le catalogue électronique s’ouvre dans une fenêtre contextuelle nette et centrée. Demandez-lui de masquer dans le navigateur la barre d’outils et la barre d’adresse.

Pour plus d’informations et d’exemples de code, consultez la section [&#x200B; Incorporer la visionneuse de catalogue électronique HTML5 dans le guide de référence des visionneuses Adobe](https://experienceleague.adobe.com/fr/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/ecatalog/c-html5-20-ecatalog-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2).

## Copie du code intégré d’une visionneuse de catalogue électronique {#copying-the-embed-code-of-an-ecatalog-viewer}

L’utilisation de la fonction Code incorporé permet de vérifier le code de la visionneuse du catalogue électronique sélectionné. Vous pouvez également copier le code dans le presse-papiers afin de le coller dans vos pages web pour le déploiement de la visionneuse. Vous ne pouvez pas modifier le code dans la boîte de dialogue Code incorporé.

**Pour copier le code intégré d’une visionneuse de catalogue électronique, procédez comme suit**

1. Dans le panneau Exploration des ressources, dans la liste déroulante Afficher, sélectionnez **[!UICONTROL Catalogue]**.
1. dans le panneau Bibliothèque de ressources sur le côté gauche, accédez au dossier de ressources contenant le catalogue électronique dont vous souhaitez copier le code intégré.
1. Au-dessus de panneau de navigation des fichiers, sur le côté droit de la barre d’outils, exécutez l’une des opérations suivantes :

   * Sélectionnez **[!UICONTROL Vue Grille]**. Dans le panneau de navigation des fichiers, cliquez deux fois sur un fichier pour l’ouvrir dans le mode Affichage des détails. Dans le panneau URL à droite, sélectionnez **[!UICONTROL Code intégré]**.
   * Sélectionnez **[!UICONTROL Vue Grille]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis, sous l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, dans la colonne Actions du tableau, sélectionnez **[!UICONTROL Code incorporé]**.

   * Sélectionnez **[!UICONTROL Vue Liste]**. Dans le panneau de navigation des ressources, sélectionnez une seule ressource, puis à droite de l’image miniature, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste de visionneuses]**.

     Dans la page Liste des visionneuses, dans la colonne Actions du tableau, sélectionnez **[!UICONTROL Code incorporé]**.

   * Sélectionnez **[!UICONTROL Vue Grille]**, **[!UICONTROL Vue Liste]** ou **[!UICONTROL Vue Détail]**. Dans la même barre d’outils, accédez à **[!UICONTROL Aperçu]** > **[!UICONTROL Liste des visionneuses]**.

     Dans la page Liste des visionneuses, dans la colonne Actions du tableau, sélectionnez **[!UICONTROL Code incorporé]**.

1. Dans la boîte de dialogue Code incorporé, sélectionnez **[!UICONTROL Copier dans le presse-papiers]**.

   Vous ne pouvez pas modifier le code dans la boîte de dialogue Code incorporé.

1. Sélectionnez **[!UICONTROL Fermer]**.
