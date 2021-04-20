---
title: '"Début rapide : Intégration de Target Standard/Premium"'
description: Une introduction et un Début rapide à Adobe Target Standard/Premium pour vous aider à maîtriser rapidement les techniques d’intégration de Target Standard/Premium.
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 19%

---


# Début rapide : Intégration d’Adobe Target Standard/Premium{#quick-start-target-integration}

Adobe Target Standard/Premium permet aux spécialistes du marketing d’exécuter rapidement et continuellement plusieurs tests A/B et multivariés, de mesurer l’efficacité et d’accroître la pertinence du contenu en ligne par le biais de la segmentation, du ciblage et de la personnalisation automatisée.

Dynamic Media Classic vous permet de créer des offres et des jeux d’offres pour les campagnes Target Standard/Premium. Par exemple, vous pouvez créer une visionneuse d’offres avec trois variantes du même fichier de média enrichi. Ensuite, Target Standard/Premium peut déterminer quel fichier offre un meilleur effet élévateur de conversion. Vous pouvez créer des offres et des visionneuses d’offres à partir d’un modèle de base ou d’images individuelles. Une fois que la visionneuse d’offres a été envoyée ou enregistrée dans Adobe Target Standard/Premium, où les offres sont associées à des mbox et à des expériences, Target Standard/Premium peut exécuter des campagnes pour déterminer quelle variation d’un site Web est susceptible de générer les meilleurs résultats pour les clics publicitaires et les conversions.

Pour une meilleure personnalisation du contenu Dynamic Media Classic dynamique, utilisez les offres HTML Target Standard/Premium. Pour plus d’informations, voir la documentation du produit Target Standard/Premium.

>[!NOTE]
>
>Un compte Adobe Target Standard/Premium valide est nécessaire pour utiliser Target Standard/Premium avec Dynamic Media Classic.

**Début rapide**

Ce Début rapide est conçu pour vous aider à maîtriser rapidement les opérations liées aux jeux d’offres HTML Target Standard/Premium. Suivez les étapes 1 à 3. Chaque étape se termine par un renvoi à une rubrique contenant de plus amples informations.

**1. Entrez votre URL Adobe Target Standard/Premium dans l&#39;écran Paramètres généraux de l&#39;application.**

Dynamic Media Classic a besoin de votre URL Target Standard/Premium pour s’intégrer à Target Standard/Premium. Copiez la partie de votre URL Target Standard/Premium jusqu’à *.com* et saisissez-la dans l’écran Paramètres généraux de l’application Dynamic Media Classic. Voir [Intégration de Dynamic Media Classic à Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

**2. Créez la visionneuse d’offres.**

Utilisez un modèle paramétré ou des images pour créer une visionneuse d’offres. Vous pouvez créer des visionneuses d’offres HTML sur l’écran Visionneuse d’offres Test&amp;Target. Pour ouvrir cet écran, sélectionnez votre modèle ou vos images, puis cliquez sur **Créer** > **Visionneuse d’Offres Test&amp;Cible**.

Pour créer une offre avec un modèle, cliquez sur **Ajouter et Prévisualisation**. Dans l’écran Ajouter et Prévisualisation, modifiez les valeurs des paramètres.

Pour créer une offre à partir d’images, faites glisser les images vers l’écran Visionneuse d’offres Test&amp;Target. Cliquez sur **Prévisualisation** pour choisir un paramètre d’image prédéfini pour une image ou toutes les images de la visionneuse d’offres.

Enregistrez la visionneuse d’offres après l’avoir créée.

Voir [Création d’une visionneuse d’offres](creating-offer-set.md#creating_an_offer_set).

**Cookie. Placez le jeu d’offres sur Adobe Target Standard/Premium**.

Dans l’écran Jeu d’Offres Test&amp;Cible, cliquez sur **Envoyer les Offres**, puis saisissez vos informations de connexion dans la boîte de dialogue Connexion à Test&amp;Cible. Voir [Pousser les jeux d’offres vers Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
