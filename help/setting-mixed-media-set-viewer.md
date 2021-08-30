---
title: Configuration d’un paramètre prédéfini de visionneuse de médias mixtes
description: Découvrez comment configurer un paramètre prédéfini de visionneuse de médias mixtes dans Adobe Dynamic Media Classic.
uuid: d5bf1840-e453-445d-bebc-84889b29f3c8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
discoiquuid: 8029aad8-d696-4d7c-99e2-3b08edb68181
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: d41b30e7-994a-43f3-8698-7dbfc36305ae
source-git-commit: e47c22508230adbb1ece323be0c1413a3f27ad89
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Configuration d’un paramètre prédéfini de visionneuse de médias mixtes{#setting-up-a-mixed-media-set-viewer-preset}

Les paramètres prédéfinis de visionneuse de supports variés définissent le style, le comportement et l’aspect de votre visionneuse principale. Lorsque vous configurez un paramètre prédéfini, vous pouvez indiquer les autres visionneuses qui doivent apparaître dans la visionneuse de supports variés. Par exemple, si vous avez inclus une visionneuse d’images dans la visionneuse de supports variés, spécifiez un paramètre prédéfini de visionneuse d’images pour la visionneuse de supports variés.

Vous pouvez choisir d’inclure tout ou partie des fonctionnalités de la communauté dans la visionneuse de supports variés. La fonctionnalité Incorporation ajoute un lien vers la visionneuse qui permet aux utilisateurs de copier le code requis pour afficher la visionneuse sur une page externe (par exemple, un blog, un site Web ou un site de réseau social). La fonctionnalité Lien fournit l’URL vers la visionneuse permettant aux utilisateurs de revenir à la visionneuse. La fonctionnalité Visite fournit un lien vers le site Web de votre choix.

1. Dans la barre de navigation globale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres prédéfinis de la visionneuse]**.
1. Sur la page Paramètres visionneuse, effectuez l’une des opérations suivantes :

   * Pour créer un paramètre prédéfini, sélectionnez **[!UICONTROL Ajouter]**. Dans la boîte de dialogue Ajouter un paramètre prédéfini de visionneuse, choisissez une plateforme, sélectionnez **[!UICONTROL Visionneuse de médias mixtes]**, puis sélectionnez **[!UICONTROL Ajouter]**.
   * Pour modifier un paramètre prédéfini de visionneuse de médias mixtes, sélectionnez-le, puis sélectionnez **[!UICONTROL Modifier]**.

1. Sur la page Visionneuse de configuration, saisissez un nom dans la zone Nom du paramètre prédéfini de la visionneuse de médias mixtes.
1. Spécifiez **[!UICONTROL Onglets]** ou **[!UICONTROL Aucun onglet]**. L’option Onglet sépare les éléments par type, par exemple, les vidéos, les échantillons et les images à 360°. Lorsque vous ne spécifiez aucun onglet, tous les éléments s’affichent sur une ligne sous la fenêtre Aperçu.
1. Dans la zone **[!UICONTROL Name]**, saisissez le nom de la visionneuse à ajouter.

   Par exemple, si vous ajoutez une série d’échantillons à votre visionneuse de médias mixtes, saisissez `Swatch Set A`.

1. Dans le menu Visionneuse, choisissez le type de fichier que vous souhaitez afficher, par exemple les séries d’échantillons.
1. Dans le menu Paramètre prédéfini, choisissez un paramètre pour le type de fichier choisi.

   Par exemple, si vous ajoutez une série d’échantillons, choisissez **[!UICONTROL SwatchSet1-Colors]**.

1. Sélectionnez **[!UICONTROL Ajouter]**.

   Le nouveau paramètre prédéfini de visionneuse apparaît dans la liste.

1. Répétez les étapes 6 à 9 pour tous les paramètres prédéfinis que vous souhaitez ajouter.
1. Pour modifier la liste des paramètres prédéfinis, effectuez l’une des opérations suivantes :

   * Pour supprimer un paramètre prédéfini de la liste, sélectionnez-le, puis sélectionnez **[!UICONTROL Supprimer]**.
   * Pour réorganiser les paramètres prédéfinis dans la liste, sélectionnez un paramètre prédéfini, puis cliquez sur la flèche bleue **[!UICONTROL Haut]** ou **[!UICONTROL Bas]**.

1. Pour ajouter des fonctionnalités de la communauté (Incorporation, Lien et Visite) à la visionneuse, spécifiez les options pour chacun des éléments suivants :

   * **Email**  : sélectionnez  **** Onpour activer un bouton Email dans la visionneuse. Lorsque les utilisateurs cliquent sur le bouton Courrier électronique lors de l’affichage de la visionneuse, un courrier électronique contenant le lien vers la visionneuse s’ouvre.

   * **Incorporer**  : sélectionnez  **[!UICONTROL En ligne]**. Dans la zone Etiquette de bouton d’intégration, tapez le nom de bouton d’intégration que vous souhaitez afficher dans la visionneuse. Si vous le souhaitez, sélectionnez **[!UICONTROL Parcourir]** pour localiser et sélectionner un habillage personnalisé pour le bouton.

   * **Lien**  : sélectionnez  **[!UICONTROL En direct]**. Dans la zone Libellé du bouton de lien , saisissez le nom que vous souhaitez afficher dans la visionneuse pour le bouton Lien . Si vous le souhaitez, sélectionnez **[!UICONTROL Parcourir]** pour localiser et sélectionner un habillage personnalisé pour le bouton.

   * **Visite**  : sélectionnez  **[!UICONTROL En ligne]**. Dans la zone Libellé du bouton de visite , saisissez le nom que vous souhaitez afficher dans la visionneuse pour le bouton Visite . Dans la boîte de dialogue URL de visite, tapez l’URL du site Web auquel vous souhaitez accéder d’un clic par le biais du lien.

1. Spécifiez les autres options voulues. Pour afficher la description d’une option, cliquez sur l’icône d’info-bulle en regard de l’option.

   La page Aperçu affiche la visionneuse au fur et à mesure que vous mettez à jour et modifiez les paramètres.

1. Sélectionnez **[!UICONTROL Enregistrer]**.

>[!MORELIKETHIS]
>
>* [Création et modification de paramètres prédéfinis de visionneuse](application-setup.md#adding_and_editing_viewer_presets)

