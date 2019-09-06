---
title: Promotion de visionneuses d'offres sur Adobe Target Classic
seo-title: Promotion de visionneuses d'offres sur Adobe Target Classic
description: 'null'
seo-description: Découvrez comment envoyer des visionneuses d'offres à Adobe Target Classic.
uuid: 8 c 895 a 7 c -21 b 4-4 d 85-8 b 0 b-a 3 d 2 a 420 bf 2 e
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/target_ classic_ integration
discoiquuid: 39 a 05654-4 f 66-4 f 1 e-aec 5-ebe 6 d 174353 f
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Promotion de visionneuses d'offres sur Adobe Target Classic{#pushing-offer-sets-to-adobe-target-classic}

Après avoir créé ou modifié une visionneuse d'offres, envoyez-la à Target Classic en procédant comme suit :

1. Sur l'écran Visionneuse d'offres Target Classic, cliquez sur le bouton Promouvoir des offres.
1. Entrez vos informations de connexion.
1. Cliquez sur le bouton Connexion.

Lors du transfert vers Target Classic, le préfixe S 7_ est automatiquement joint au début des noms d'offre. Ce préfixe est joint pour vous assurer que vous trouvez facilement les offres Dynamic Media Classic dans la liste des offres Target Classic. Par exemple, l’offre apparaît sous la forme suivante : S7_&lt;nom de la visionneuse d’offre&gt;_&lt;nom de l’offre&gt;.

SPS encourage les offres de widgets Target Classic. Vous pouvez utiliser les offres Widget pour héberger votre propre contenu d'offre en dehors de Target Classic. Les offres de widgets sont similaires à une offre standard hébergée en dehors de Target Classic. Elles permettent à Target Classic de déployer le contenu des offres stocké sur votre serveur, ce qui permet une utilisation plus dynamique et élaborée. Les offres Widget récupèrent le contenu d'une URL, en mettant en cache et en utilisant ce contenu pendant environ deux heures. Les offres de widgets fournissent des fonctionnalités de génération de contenu dynamique que d'autres offres ne proposent pas en dehors de Target Classic. If the mbox serving the offer contains mbox parameters such as `mboxProductID` and `mbox.offerId`, the `productId=[PRODUCT_ID]`and `offerID=[OFFERID]` URL parameters are appended to the requested URL. Ces paramètres peuvent être utilisés par un service disponible à l'URL de l'offre Widget pour renvoyer du contenu en dehors de Target Classic qui utilise les informations de produit ou de commande provenant de vos mbox. L'offre de widgets est également accessible via l'API pour créer par programmation des offres en dehors de Target Classic.
