---
title: Jeux d’offres push vers Adobe Target Standard/Premium
description: Découvrez comment envoyer des visionneuses d’offres vers Adobe Target Standard/Premium à partir d’Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
topic: Integrations, Development
level: Experienced
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Jeux d’offres push vers Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Une fois que vous avez créé ou modifié un jeu d’offres, poussez-le vers Adobe Target Standard/Premium en procédant comme suit :

1. Dans l’écran Visionneuse d’offres Test&amp;Target, sélectionnez **[!UICONTROL Offres push]**.
1. Saisissez votre code client et vos informations de connexion.
1. Sélectionner **[!UICONTROL Connexion]**.

Pendant le transfert vers Adobe Target Standard/Premium, le préfixe `S7_` est jointe automatiquement au début des noms des offres. Ce préfixe est joint afin de vous assurer que vous pouvez facilement trouver les offres Adobe Dynamic Media Classic dans la liste d’offres Test&amp;Target. Par exemple, l’offre s’affiche comme suit : `S7_<name of offer set>_<offer name>`.

Adobe Dynamic Media Classic transmet les offres du widget Adobe Target Standard/Premium. Vous pouvez utiliser les offres de widgets pour héberger votre propre contenu proposé en dehors d’Adobe Target Standard/Premium. Les offres de widgets sont similaires à une offre standard hébergée en dehors d’Adobe Target Standard/Premium. Ils permettent à Adobe Target Standard/Premium de déployer le contenu des offres stocké sur votre serveur, ce qui permet une utilisation plus dynamique et sophistiquée. Les offres de widgets peuvent récupérer le contenu d’une URL, en le mettant en cache et en le diffusant pendant environ deux heures. Les offres de widgets fournissent des fonctionnalités de génération de contenu dynamique qui ne sont pas disponibles dans les autres offres en dehors d’Adobe Target Standard/Premium. Si la mbox qui diffuse l’offre contient des paramètres de mbox tels que `mboxProductID` et `mbox.offerId`, la variable `productId=[PRODUCT_ID]`et `offerID=[OFFERID]` Les paramètres d’URL sont ajoutés à l’URL demandée. Ces paramètres peuvent être utilisés par un service disponible à l’adresse URL de l’offre de widgets pour renvoyer du contenu en dehors d’Adobe Target Standard/Premium qui utilise les informations de produit ou de commande de vos mbox. L’offre de widgets est également accessible par le biais de l’API pour créer par programmation des offres en dehors d’Adobe Target Standard/Premium.
