---
title: Limites de Dynamic Media
description: 'Découvrez les bonnes pratiques et les limites appliquées lorsque vous créez une visionneuse d’images ou à 360° ou chargez un PDF. Découvrez également les combinaisons de navigateur web et de système d’exploitation non prises en charge pour les visionneuses Dynamic Media. '
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Asset Management,Viewers,Image Sets,Spin Sets,eCatalog
role: User
exl-id: ee30a2c1-2b26-41bd-8758-e7337a3727bb
source-git-commit: ec840640b1131a56c1261f22b7638e53dac1bce8
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 2%

---

# Limites de Dynamic Media

Les sections suivantes décrivent les limites dans Dynamic Media.

Cette rubrique comprend les sections suivantes :

* [Bonnes pratiques et limites appliquées par Dynamic Media sur les types de ressources](#best-practice-enforced-limits)
* [Combinaisons de navigateur web et de système d’exploitation non prises en charge pour les visionneuses Dynamic Media](#unsupported-browser-os)

## Bonnes pratiques et limites appliquées par Dynamic Media sur les types de ressources {#best-practice-enforced-limits}

Lorsque vous créez une visionneuse à 360° ou une visionneuse d’images, ou que vous chargez des PDF pour l’extraction de page, Adobe recommande les bonnes pratiques suivantes et applique les limites suivantes :

| Ressource - Type de limite | Pratique recommandée | Limite imposée | Modification de la limite le 31 décembre 2022 |
| --- | --- | --- | --- |
| **Image** - Nombre de recadrages intelligents par image | 5 | 100 | 20 |
| **Tous les ensembles** - Nombre de ressources en double par ensemble | Aucun doublon | 20 | Non applicable |
| **Tous les ensembles** - Nombre maximal de ressources par ensemble | 5 à 10 images par visionneuse | 1 000 | Non applicable |
| **Visionneuse à 360°** - Nombre maximal de lignes/colonnes par jeu 2D | 12 à 18 images par visionneuse | 1 000 | Non applicable |
| **PDF** - Nombre maximal de pages qu’un PDF doit prendre en compte pour l’extraction |  | 5000 (pour les nouveaux chargements) | 100 (pour tous les PDF) |

<!-- See also [Dynamic Media limitations](/help/assets/limitations.md). -->

## Combinaisons de navigateur web et de système d’exploitation non prises en charge pour les visionneuses Dynamic Media {#unsupported-browser-os}

<!-- CQDOC-19433 -->

Les visionneuses Dynamic Media Adobe ne prennent pas en charge les combinaisons de navigateur web et de système d’exploitation suivantes.

* Internet Explorer 11 + Windows 7
* Internet Explorer 11 + Windows 8.1
* Internet Explorer 11 + Windows Phone 8.1
* Mise à jour d’Internet Explorer 11 + Windows Phone 8.1
* Safari 6 + iOS 6.0.1
* Safari 7 + iOS 7.1
* Mavericks Safari 7 + OS X 10.9
* Safari 8 + iOS 8.4
* Safari 8 + OS X 10.10 Yosemite

## Fin de la prise en charge de TLS 1.0 et 1.1 {#tls}

<!-- CQDOC-19433 -->

À compter du 30 septembre 2022, les visionneuses Dynamic Media Adobe ne prendront plus en charge les éléments suivants :

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

