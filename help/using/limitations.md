---
title: Limites de Dynamic Media
description: Découvrez les bonnes pratiques et les limites appliquées lorsque vous créez une visionneuse d’images ou à 360° ou chargez une visionneuse PDF. Découvrez également les combinaisons de navigateur web et de système d’exploitation non prises en charge par Dynamic Media.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Asset Management,Image Sets,Spin Sets,eCatalog
role: User
exl-id: ee30a2c1-2b26-41bd-8758-e7337a3727bb
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T20:02:23.354Z'
TQID: 'https://experienceleague.adobe.com/7dtiaPb7sWkPb5gocOc8xLOnz3U3gJuSdaW2LSkajMk'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 352
ht-degree: 1%

---

# Limites de Dynamic Media

Les sections suivantes décrivent les limites dans Dynamic Media.

Cette rubrique comprend les sections suivantes :

* [Bonnes pratiques et limites appliquées par Dynamic Media sur les types de ressources](#best-practice-enforced-limits)
* [Combinaisons de navigateur web et de système d’exploitation non prises en charge par Dynamic Media](#unsupported-browser-os)

## Bonnes pratiques et limites appliquées par Dynamic Media sur les types de ressources {#best-practice-enforced-limits}

Lorsque vous créez une visionneuse à 360° ou une visionneuse d’images, ou que vous téléchargez des PDF pour l’extraction de page, Adobe recommande les bonnes pratiques suivantes. Adobe applique également les limites suivantes :

| Ressource : type de limite | Pratique recommandée | Limite imposée |
| --- | --- | --- |
| **Image** : nombre de recadrages intelligents par image | 5 | 100 |
| **Tous les ensembles** : nombre de ressources en double par ensemble | Aucun doublon | 20 ‡ |
| **Tous les ensembles** : nombre maximal de ressources par ensemble | 5 à 10 images par ensemble | 1000 |
| **Visionneuse à 360°** : nombre maximal de lignes/colonnes par visionneuse 2D | 12 à 18 images par ensemble | 1000 |
| **&#x200B;**&#x200B;: nombre maximal de pages qu’un PDF doit prendre en compte pour l’extraction |  | 100 (pour tous les PDF) |

‡ Il est recommandé de ne pas avoir de ressources en double dans un ensemble. La limite est de 20 doublons pour une seule ressource. Si vous ajoutez un autre doublon pour cette ressource (dans ce jeu), la requête soit génère une erreur, soit ignore le doublon.

<!-- See also [Dynamic Media limitations](/help/using/assets/limitations.md). -->

## Combinaisons de navigateur web et de système d’exploitation non prises en charge par Dynamic Media {#unsupported-browser-os}

<!-- CQDOC-19433 -->

Adobe Dynamic Media ne prend pas en charge les combinaisons de navigateur web et de système d’exploitation ci-après.

* Internet Explorer 11 + Windows 7
* Internet Explorer 11 + Windows 8.1
* Internet Explorer 11 + Windows Phone 8.1
* Mise à jour d’Internet Explorer 11 + Windows Phone 8.1
* Safari 6 + iOS 6.0.1
* Safari 7 + iOS 7.1
* Safari 7 + OS X 10.9 Mavericks
* Safari 8 + iOS 8.4
* Safari 8 + OS X 10.10 Yosemite

## Fin de la prise en charge de Secure Socket Layer 2.0 et 3.0 et de Transport Layer Security 1.0 et 1.1 {#tls}

<!-- 
CQDOC-19433 (original ticket)
and CQDOC-19792 (removed as per this ticket December 5, 2022) 
-->

À compter du 30 avril 2024, Adobe Dynamic Media ne prendra plus en charge les éléments suivants :

* SSL (Secure Socket Layer) 2.0
* SSL 3.0
* TLS (Transport Layer Security) 1.0 et 1.1
* Les chiffrements faibles suivants dans TLS 1.2 :
   * `TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384`
   * `TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA`
   * `TLS_RSA_WITH_AES_256_GCM_SHA384`
   * `TLS_RSA_WITH_AES_256_CBC_SHA256`
   * `TLS_RSA_WITH_AES_256_CBC_SHA`
   * `TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA256`
   * `TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA`
   * `TLS_RSA_WITH_AES_128_GCM_SHA256`
   * `TLS_RSA_WITH_AES_128_CBC_SHA256`
   * `TLS_RSA_WITH_AES_128_CBC_SHA`
   * `TLS_RSA_WITH_CAMELLIA_256_CBC_SHA`
   * `TLS_RSA_WITH_CAMELLIA_128_CBC_SHA`
   * `TLS_ECDHE_RSA_WITH_3DES_EDE_CBC_SHA`
   * `TLS_RSA_WITH_SDES_EDE_CBC_SHA`

