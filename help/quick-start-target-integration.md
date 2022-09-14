---
title: "Démarrage rapide : Intégration d’Adobe Target Standard/Premium"
description: Présentation et démarrage rapide d’Adobe Target Standard/Premium pour vous aider à maîtriser rapidement les techniques d’intégration d’Adobe Target Standard/Premium dans Adobe Dynamic Media Classic.
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 7%

---

# Démarrage rapide : Intégration d’Adobe Target Standard/Premium{#quick-start-target-integration}

Adobe Target Standard/Premium offre un contrôle direct entre les mains des marketeurs pour exécuter rapidement et continuellement plusieurs tests A/B et multivariés, mesurer l’efficacité et accroître la pertinence du contenu en ligne par le biais de la segmentation, du ciblage et d’Automated Personalization.

Adobe Dynamic Media Classic vous permet de créer des offres et des ensembles d’offres pour les campagnes Adobe Target Standard/Premium. Par exemple, vous pouvez créer un ensemble d’offres avec trois variantes d’une même ressource de média enrichi. Vous pouvez ensuite demander à Adobe Target Standard/Premium de déterminer quelle ressource offre un meilleur effet élévateur de conversion. Vous pouvez créer des offres et des visionneuses d’offres à partir d’un modèle de base ou d’images individuelles. Une fois que la visionneuse d’offres a été envoyée ou enregistrée dans Adobe Target Standard/Premium, où les offres sont associées à des mbox et à des expériences, Adobe Target Standard/Premium peut exécuter des campagnes. Ces campagnes déterminent la variante d’un site web qui sera la plus performante pour les clics publicitaires et les conversions.

Pour une plus grande personnalisation du contenu Adobe Dynamic Media Classic dynamique, utilisez les offres de HTML Adobe Target Standard/Premium . Voir [Documentation du produit Adobe Target Standard/Premium](https://experienceleague.adobe.com/docs/target.html) pour plus d’informations.

>[!NOTE]
>
>Un compte Adobe Target Standard/Premium valide est requis pour utiliser Adobe Target Standard/Premium avec Adobe Dynamic Media Classic.

Ce didacticiel de mise en route est conçu pour vous aider à maîtriser rapidement les opérations liées aux ensembles d’offres de HTML Adobe Target Standard/Premium. Suivez les étapes 1 à 3. Après chaque étape, il existe une référence croisée à un en-tête de rubrique où vous trouverez plus d’informations.

## 1. Saisissez votre URL Adobe Target Standard/Premium dans la page Paramètres généraux de l’application.

Adobe Dynamic Media Classic a besoin de votre URL Adobe Target Standard/Premium pour s’intégrer à Adobe Target Standard/Premium. Copiez la partie de votre URL Adobe Target Standard/Premium jusqu’à et incluez `.com`, puis saisissez-la dans Adobe Dynamic Media Classic. **[!UICONTROL Paramètres généraux de l’application]** , dans la **[!UICONTROL Serveurs]** groupe, **[!UICONTROL Nom du serveur Test&amp;Target]** Champ de texte. Voir [Intégration d’Adobe Dynamic Media Classic à Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

## 2. Créez la visionneuse d’offres

Utilisez un modèle paramétré ou des images pour créer une visionneuse d’offres. Vous créez des ensembles d’offres de HTML sur la page Jeu d’offres Test&amp;Target. Pour ouvrir cette page, sélectionnez votre modèle ou vos images, puis, sur la barre de navigation globale, accédez à **[!UICONTROL Build]** > **[!UICONTROL Jeu d’offres Test&amp;Target]**.

Pour créer une offre avec un modèle, sélectionnez **[!UICONTROL Ajouter et prévisualiser]**. Sur la page Ajouter et prévisualiser , modifiez les valeurs des paramètres.

Pour créer une offre avec des images, faites glisser les images sur la page de la visionneuse d’offres Test&amp;Target. Sélectionner **[!UICONTROL Aperçu]** et choisissez un paramètre d’image prédéfini pour une image ou toutes les images de la visionneuse d’offres.

Enregistrez la visionneuse d’offres après l’avoir créée.

Voir [Créer un ensemble d’offres](creating-offer-set.md#creating_an_offer_set).

## 3. Envoyez la visionneuse d’offres à Adobe Target Standard/Premium.

Sur la page du jeu d’offres Test&amp;Target, sélectionnez **[!UICONTROL Offres push]**, puis saisissez vos informations de connexion dans la boîte de dialogue Connexion à Test&amp;Target . Voir [Jeux d’offres push vers Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
