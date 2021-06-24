---
title: '"Démarrage rapide : Intégration d’Adobe Target Standard/Premium"'
description: Présentation et démarrage rapide d’Adobe Target Standard/Premium pour vous aider à maîtriser rapidement les techniques d’intégration d’Adobe Target Standard/Premium.
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 12%

---

# Démarrage rapide : Intégration d’Adobe Target Standard/Premium{#quick-start-target-integration}

Adobe Target Standard/Premium offre un contrôle direct aux marketeurs pour qu’ils exécutent rapidement et continuellement plusieurs tests A/B et multivariés, mesurent l’efficacité et augmentent la pertinence du contenu en ligne par le biais de la segmentation, du ciblage et de la personnalisation automatisée.

Dynamic Media Classic vous permet de créer des offres et des ensembles d’offres pour les campagnes Adobe Target Standard/Premium. Par exemple, vous pouvez créer un ensemble d’offres avec trois variantes d’une même ressource de média enrichi. Vous pouvez ensuite demander à Adobe Target Standard/Premium de déterminer quelle ressource offre un meilleur effet élévateur de conversion. Vous pouvez créer des offres et des visionneuses d’offres à partir d’un modèle de base ou d’images individuelles. Une fois que la visionneuse d’offres a été envoyée ou enregistrée dans Adobe Target Standard/Premium, où les offres sont associées à des mbox et à des expériences, Adobe Target Standard/Premium peut exécuter des campagnes. Ces campagnes déterminent la variante d’un site web qui sera la plus performante pour les clics publicitaires et les conversions.

Pour une plus grande personnalisation du contenu dynamique de Dynamic Media Classic, utilisez les offres HTML Adobe Target Standard/Premium . Pour plus d’informations, consultez la [documentation du produit Adobe Target Standard/Premium](https://experienceleague.adobe.com/docs/target.html) .

>[!NOTE]
>
>Un compte Adobe Target Standard/Premium valide est requis pour utiliser Adobe Target Standard/Premium avec Dynamic Media Classic.

Ce didacticiel de mise en route est conçu pour vous aider à maîtriser rapidement les opérations liées aux ensembles d’offres HTML Adobe Target Standard/Premium. Suivez les étapes 1 à 3. Chaque étape se termine par un renvoi à une rubrique contenant de plus amples informations.

## 1. Saisissez votre URL Adobe Target Standard/Premium dans la page Paramètres généraux de l’application.

Dynamic Media Classic a besoin de votre URL Adobe Target Standard/Premium pour s’intégrer à Adobe Target Standard/Premium. Copiez la partie de votre URL Adobe Target Standard/Premium jusqu’à `.com` et indiquez-la dans la page **[!UICONTROL Paramètres généraux de l’application de Dynamic Media Classic]**, dans le groupe **[!UICONTROL Servers]**, **[!UICONTROL Nom du serveur Test&amp;Target]**. Voir [Intégration de Dynamic Media Classic à Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

## 2. Créez la visionneuse d’offres

Utilisez un modèle paramétré ou des images pour créer une visionneuse d’offres. Vous créez des ensembles d’offres HTML sur la page du jeu d’offres Test&amp;Target. Pour ouvrir cette page, sélectionnez votre modèle ou vos images, puis, sur la barre de navigation globale, cliquez sur **[!UICONTROL Créer]** > **[!UICONTROL Visionneuse d’offres Test&amp;Target]**.

Pour créer une offre avec un modèle, cliquez sur **[!UICONTROL Ajouter et prévisualiser]**. Sur la page Ajouter et prévisualiser , modifiez les valeurs des paramètres.

Pour créer une offre avec des images, faites glisser les images sur la page de la visionneuse d’offres Test&amp;Target. Cliquez sur **[!UICONTROL Aperçu]** et choisissez un paramètre d’image prédéfini pour une image ou toutes les images de la visionneuse d’offres.

Enregistrez la visionneuse d’offres après l’avoir créée.

Voir [Création d’une visionneuse d’offres](creating-offer-set.md#creating_an_offer_set).

## 3. Envoyez la visionneuse d’offres à Adobe Target Standard/Premium.

Sur la page Jeu d’offres Test&amp;Target, cliquez sur **[!UICONTROL Envoyer les offres]**, puis saisissez vos informations de connexion dans la boîte de dialogue Connexion à Test&amp;Target. Voir [Pousser des ensembles d’offres vers Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
