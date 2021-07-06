---
title: Téléchargement des images originales
description: Découvrez comment télécharger des images originales.
uuid: 50bcf2e2-852b-48f1-a7c7-5063a87ce9c1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 8c94bafc-94cc-496f-a394-a945cd7b02cf
feature: Dynamic Media Classic,Gestion des ressources
role: User
exl-id: 410ba80c-7f01-4cd0-9ab3-db9658757ba7
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 19%

---

# Téléchargement des images originales{#uploading-master-images}

Avant de charger des images dans Dynamic Media Classic, assurez-vous qu’elles ont la taille et le format les plus performants. Dynamic Media Classic recommande de télécharger des images de haute qualité avec un nombre de pixels suffisant (de 1 500 à 2 000 pixels en taille longue). Ce dimensionnement permet de créer toute image dynamique requise.

Pour plus d’informations sur le téléchargement d’images, voir [Téléchargement de fichiers](uploading-files.md#uploading_files).

**Préparation des images originales pour leur téléchargement:**

Préparez les fichiers image originaux avant de les télécharger vers Dynamic Media Classic :

* **Taille de l’image**  : créez les images de la plus grande taille que vous prévoyez d’utiliser. La taille d’image standard est comprise entre 1 500 et 2 500 pixels pour la taille la plus longue. Si vous envisagez d’utiliser la fonction Zoom, Dynamic Media Classic vous recommande d’utiliser des images d’au moins 2 000 pixels de la plus grande taille pour un détail de zoom optimal. Dynamic Media Classic peut générer des images de 25 mégapixels chacune. Par exemple, vous pouvez utiliser une image de 5 000 x 5 000 mégapixels ou toute autre combinaison de taille pouvant atteindre 25 mégapixels.

* **Formats**  de fichier : Dynamic Media Classic prend en charge tous les formats de fichier image standard, notamment TIFF, BMP, JPEG, PSD, GIF et EPS. Il est recommandé de privilégier les formats d’image sans perte, à savoir TIFF et PNG. Si vous utilisez une image JPEG, utilisez les paramètres de qualité supérieure.

* **Espace colorimétrique**  : RVB est l’espace colorimétrique pour les présentations d’images web ; Les images CMJN couramment utilisées pour l’impression sont automatiquement converties en RVB lorsque vous les chargez. Il est recommandé de télécharger des images CMJN dotées d’un profil de couleurs ICC incorporé pour la conversion en mode RVB (voir aussi [Profils ICC](/help/icc-profiles.md)).
