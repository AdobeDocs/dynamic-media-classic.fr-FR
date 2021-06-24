---
title: Pousser des ensembles d’offres vers Adobe Target Standard/Premium
description: Découvrez comment envoyer des visionneuses d’offres vers Adobe Target Standard/Premium.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Pousser des ensembles d’offres vers Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Une fois que vous avez créé ou modifié un jeu d’offres, poussez-le vers Adobe Target Standard/Premium en procédant comme suit :

1. Dans l’écran Visionneuse d’offres Test&amp;Target, cliquez sur **[!UICONTROL Offres push]**.
1. Saisissez votre code client et vos informations de connexion.
1. Cliquez sur **[!UICONTROL Connexion]**.

Lors du transfert vers Adobe Target Standard/Premium, le préfixe `S7_` est automatiquement associé au début des noms d’offres. Ce préfixe est joint afin de vous assurer que vous pouvez facilement trouver les offres Dynamic Media Classic dans la liste d’offres Test&amp;Target. Par exemple, l’offre s’affiche sous la forme `S7_<name of offer set>_<offer name>`.

Dynamic Media Classic transmet les offres de widget Adobe Target Standard/Premium. Vous pouvez utiliser les offres de widgets pour héberger votre propre contenu d’offre en dehors d’Adobe Target Standard/Premium. Les offres de widgets sont similaires à une offre standard hébergée en dehors d’Adobe Target Standard/Premium. Ils permettent à Adobe Target Standard/Premium de déployer le contenu des offres stocké sur votre serveur, ce qui permet une utilisation plus dynamique et sophistiquée. Les offres de widgets récupèrent le contenu d’une URL, en le mettant en cache et en le diffusant pendant environ deux heures. Les offres de widgets fournissent des fonctionnalités de génération de contenu dynamique qui ne sont pas disponibles dans les autres offres en dehors d’Adobe Target Standard/Premium. Si la mbox qui diffuse l’offre contient des paramètres de mbox tels que `mboxProductID` et `mbox.offerId`, les paramètres d’URL `productId=[PRODUCT_ID]`et `offerID=[OFFERID]` sont ajoutés à l’URL demandée. Ces paramètres peuvent être utilisés par un service disponible à l’adresse URL de l’offre de widgets pour renvoyer du contenu en dehors d’Adobe Target Standard/Premium qui utilise les informations de produit ou de commande de vos mbox. L’offre de widgets est également accessible par le biais de l’API pour créer par programmation des offres en dehors d’Adobe Target Standard/Premium.
