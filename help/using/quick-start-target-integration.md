---
title: 'Démarrage rapide : intégration d’Adobe Target Standard/Premium'
description: Cette section présente Adobe Target Standard/Premium et fournit un tutoriel de démarrage rapide pour vous aider à maîtriser rapidement les techniques d’intégration d’Adobe Target Standard/Premium dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# Démarrage rapide : intégration d’Adobe Target Standard/Premium{#quick-start-target-integration}

Adobe Target Standard/Premium remet le contrôle directement entre les mains des spécialistes marketing. Cela permet d’exécuter rapidement et en continu plusieurs tests A/B et multivariés, et de mesurer l’efficacité. Il peut également accroître la pertinence du contenu en ligne par le biais de la segmentation, du ciblage et d’Automated Personalization.

Adobe Dynamic Media Classic vous permet de créer des offres et des ensembles d’offres pour les campagnes Adobe Target Standard/Premium. Par exemple, vous pouvez créer un ensemble d’offres avec trois variantes de la même ressource de médias riches. Vous pouvez ensuite utiliser Adobe Target Standard ou Premium pour déterminer la ressource qui offre le meilleur effet élévateur de conversion. Vous pouvez créer des offres et des ensembles d’offres à partir d’un modèle de base ou d’images individuelles. Une fois le jeu d’offres envoyé ou enregistré dans Adobe Target Standard/Premium, où les offres sont associées à des mbox et à des expériences, Adobe Target Standard/Premium peut exécuter des campagnes. Ces campagnes déterminent quelle variation d’un site web est susceptible d’être la plus performante pour les clics publicitaires et la conversion.

Pour une plus grande personnalisation du contenu dynamique d’Adobe Dynamic Media Classic, utilisez les offres Adobe Target Standard/Premium d’HTML. Pour plus d’informations[ consultez la documentation du produit ](https://experienceleague.adobe.com/en/docs/target)Adobe Target Standard/Premium .

>[!NOTE]
>
>Un compte Adobe Target Standard/Premium valide est requis pour utiliser Adobe Target Standard/Premium avec Adobe Dynamic Media Classic.

Ce démarrage rapide est conçu pour vous permettre de vous familiariser rapidement avec les ensembles d’offres d’Adobe Target Standard/Premium HTML. Suivez les étapes 1 à 3. Après chaque étape, il existe une référence croisée à un en-tête de rubrique dans laquelle vous pouvez trouver plus d’informations.

## &#x200B;1. Saisissez l’URL d’Adobe Target Standard/Premium sur la page Paramètres généraux de l’application.

Adobe Dynamic Media Classic a besoin de votre URL Adobe Target Standard/Premium pour s’intégrer à Adobe Target Standard/Premium. Copiez la partie de l’URL d’Adobe Target Standard/Premium allant jusqu’au `.com` inclus et saisissez-la sur la page Adobe Dynamic Media Classic **[!UICONTROL Paramètres généraux de l’application]**, dans le groupe **[!UICONTROL Serveurs]**, **[!UICONTROL Nom du serveur Test&amp;Target]**. Voir [Intégration d’Adobe Dynamic Media Classic à Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

## &#x200B;2. Création de l&#39;ensemble d&#39;offres

Utilisez un modèle paramétré ou des images pour créer un ensemble d&#39;offres. Vous pouvez créer des ensembles d’offres HTML sur la page Ensemble d’offres Test&amp;Target . Pour ouvrir cette page, sélectionnez votre modèle ou vos images, puis, sur la barre de navigation globale, accédez à **[!UICONTROL Créer]** > **[!UICONTROL Test&amp;Target Offer Set]**.

Pour créer une offre avec un modèle, sélectionnez **[!UICONTROL Ajouter et prévisualiser]**. Sur la page Ajouter et prévisualiser , modifiez les valeurs des paramètres.

Pour créer une offre avec des images, faites glisser les images dans la page Jeu d’offres Test&amp;Target. Sélectionnez **[!UICONTROL Aperçu]** et choisissez un paramètre d’image prédéfini pour une image ou toutes les images du jeu d’offres.

Enregistrez le jeu d&#39;offres après l&#39;avoir créé.

Voir [Création d’un ensemble d’offres](creating-offer-set.md#creating_an_offer_set).

## &#x200B;3. Envoyez le jeu d’offres à Adobe Target Standard/Premium

Sur la page Jeu d’offres Test&amp;Target, sélectionnez **[!UICONTROL Intégrer les offres]** et saisissez vos informations de connexion dans la boîte de dialogue Connexion Test&amp;Target. Voir [ Envoi des ensembles d’offres vers Adobe Target Standard/Premium ](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
