---
title: Intégrer les ensembles d’offres à Adobe Target Standard/Premium
description: Découvrez comment envoyer des ensembles d’offres vers Adobe Target Standard/Premium à partir d’Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
topic: Integrations, Development
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# Intégrer les ensembles d’offres à Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Après avoir créé ou modifié un ensemble d’offres, poussez-le vers Adobe Target Standard/Premium en procédant comme suit :

1. Dans l’écran Test&amp;Target Offer Set, sélectionnez **[!UICONTROL Intégrer les offres]**.
1. Saisissez votre code client et vos informations de connexion.
1. Sélectionnez **[!UICONTROL Connexion]**.

Lors du transfert vers Adobe Target Standard/Premium, le préfixe `S7_` est automatiquement ajouté au début des noms d’offres. Ce préfixe est joint pour vous assurer que vous pouvez facilement trouver des offres Adobe Dynamic Media Classic dans la liste des offres de Test&amp;Target. Par exemple, l’offre s’affiche sous la forme `S7_<name of offer set>_<offer name>`.

Adobe Dynamic Media Classic intègre les offres de widgets d’Adobe Target Standard/Premium. Vous pouvez utiliser les offres de widget pour héberger votre propre contenu proposé sur Adobe Target Standard/Premium. Les offres de widgets sont similaires à une offre standard hébergée par Adobe Target Standard/Premium. Ils permettent à Adobe Target Standard/Premium de déployer le contenu de l’offre stocké sur votre serveur, pour une utilisation plus sophistiquée et plus dynamique. Les offres de widget peuvent récupérer le contenu d’une URL, en mettant en cache et en diffusant ce contenu pendant environ deux heures. Les offres de widget fournissent certaines fonctionnalités de génération de contenu dynamique que d’autres offres en dehors d’Adobe Target Standard/Premium ne fournissent pas. Si la mbox qui diffuse l’offre contient des paramètres de mbox tels que `mboxProductID` et `mbox.offerId`, les paramètres d’URL `productId=[PRODUCT_ID]` et `offerID=[OFFERID]` sont ajoutés à l’URL demandée. Ces paramètres sont utilisés par un service disponible dans l’URL de l’offre de widgets pour renvoyer du contenu en dehors d’Adobe Target Standard/Premium qui utilise des informations sur les produits ou les commandes à partir de vos mbox. L’offre Widget est également accessible via l’API afin que vous puissiez créer des offres par programmation en dehors d’Adobe Target Standard/Premium.
