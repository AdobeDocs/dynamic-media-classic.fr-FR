---
title: Pousser les jeux d’offres vers Adobe Target Standard/Premium
seo-title: Pousser les jeux d’offres vers Adobe Target Standard/Premium
description: 'null'
seo-description: Découvrez comment pousser les jeux d’offres vers Adobe Target Standard/Premium.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 5%

---


# Pousser les jeux d’offres vers Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Après avoir créé ou modifié un jeu d’offres, poussez-le vers Target Standard/Premium en procédant comme suit :

1. In the Test&amp;Target Offer Set screen, click **[!UICONTROL Push Offers]**.
1. Entrez votre code client et vos informations de connexion.
1. Cliquez sur **[!UICONTROL Connexion]**.

Lors du transfert vers Target Standard/Premium, le préfixe S7_ est automatiquement attaché au début des noms d’offre. Ce préfixe est joint afin de vous assurer que vous pouvez facilement trouver les offres Dynamic Media Classic dans la liste offre Test&amp;Cible. Par exemple, l’offre apparaît sous la forme suivante : S7_&lt;nom de la visionneuse d’offre>_&lt;nom de l’offre>.

Dynamic Media Classic envoie les offres de widgets Target Standard/Premium. Vous pouvez utiliser des offres de widgets pour héberger votre propre contenu d’offre en dehors de Target Standard/Premium. Les offres de widgets sont similaires à une offre standard hébergée en dehors de Target Standard/Premium. Elles permettent à Target Standard/Premium de déployer le contenu d’offre stocké sur votre serveur, ce qui permet une utilisation plus dynamique et sophistiquée. Les offres de widgets récupèrent le contenu d’une URL, en le mettant en cache et en le diffusant pendant environ deux heures. Les offres de widgets offrent certaines fonctionnalités de génération de contenu dynamique que d’autres offres en dehors de Target Standard/Premium ne proposent pas. If the mbox serving the offer contains mbox parameters such as `mboxProductID` and `mbox.offerId`, the `productId=[PRODUCT_ID]`and `offerID=[OFFERID]` URL parameters are appended to the requested URL. Ces paramètres peuvent être utilisés par un service disponible à l’adresse URL de l’offre de widgets pour renvoyer du contenu en dehors de Target Standard/Premium qui utilise les informations de produit ou de commande provenant de vos mbox. L’offre de widgets est également accessible via l’API pour créer par programmation des offres en dehors de Target Standard/Premium.
