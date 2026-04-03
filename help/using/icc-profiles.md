---
title: Profils ICC (International Color Consortium)
description: Découvrez les profils ICC dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
feature: Dynamic Media Classic
role: User
exl-id: 989f2761-f5d0-4ece-b2a6-f7b4577aa8a2
topic: Administration, Content Management
level: Intermediate
source-git-commit: 2893110e9629ef72a0e919b47abc94c916e132e9
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 31%

---

# Profils ICC{#icc-profiles}

Un profil ICC (International Color Consortium) est un fichier qui décrit comment convertir correctement les fichiers image d’un espace colorimétrique à un autre. Les profils ICC permettent d’obtenir les couleurs appropriées pour vos images. Par exemple, pour afficher correctement les images conçues pour être imprimées sur un écran d’ordinateur, vous pouvez choisir un profil ICC. Ce profil convertit l’image dans un espace colorimétrique différent et s’assure que les couleurs s’affichent correctement à l’écran.

Dans Adobe Dynamic Media Classic, vous pouvez choisir un profil ICC pour convertir les images en un espace colorimétrique différent lorsque vous chargez les images. Tous les profils ICC Photoshop standard sont disponibles par défaut sur Adobe Dynamic Media Classic. Pour afficher le nom des profils colorimétriques sur l’écran de téléchargement, sélectionnez le menu Profil de couleurs. Ensuite, choisissez la commande Personnaliser de > à, puis sélectionnez un nom de profil ICC dans les menus Convertir à partir de et Convertir en

Voir [Options de modification d’image lors du chargement](image-editing-options-upload.md#image-editing-options-at-upload).

Outre l’utilisation des profils ICC par défaut, vous pouvez charger d’autres profils ICC vers Adobe Dynamic Media Classic et les rendre disponibles pour la conversion des espaces colorimétriques. Passez à la Vue détaillée dans le panneau de navigation pour examiner la classe de profil, le type d’espace colorimétrique et le type PCS d’un profil ICC.

En résumé, les points clés pour les profils ICC sont les suivants :

* Les profils ICC permettent une conversion correcte des couleurs entre les différents espaces colorimétriques des fichiers image.
* Adobe Dynamic Media Classic intègre tous les profils ICC Photoshop standard pour des conversions d’images robustes.
* Les profils ICC personnalisés offrent une flexibilité accrue pour les besoins de conversion d’espace colorimétrique avancés.
* L’affichage de détails tels que la classe de profil et le type PCS dans l’affichage des détails vous aide à gérer les paramètres ICC.
* Le chargement des profils ICC est simple et garantit l’accès à tous les dossiers dans Dynamic Media Classic.


## Chargement de profils ICC {#uploading-icc-profiles}

Téléchargez les profils ICC en procédant de la même façon que pour télécharger les fichiers. Vous pouvez stocker des profils ICC dans n’importe quel dossier Adobe Dynamic Media Classic.

Voir [Charger vos fichiers](uploading-files.md#uploading_your_files).

## Examiner un profil ICC {#examining-an-icc-profile}

Pour examiner un profil ICC, sélectionnez-le dans le panneau Parcourir et affichez-le dans la vue Détail. L’affichage des détails fournit les informations suivantes sur les profils ICC :

* **[!UICONTROL Classe de profil]** : l’ICC définit chaque classe pour couvrir un type d’application. Par exemple, les profils d’entrée s’appliquent aux appareils, tels que les appareils photo numériques et les scanners. Les profils de sortie s’appliquent aux imprimantes.

* **[!UICONTROL Type d’espace colorimétrique]** : ce nombre correspond à l’espace colorimétrique « d’entrée » du profil, tel que défini par l’ICC. Le type d’espace colorimétrique définit le nombre de composantes de l’espace colorimétrique et l’interprétation de ces composantes. Par exemple, RVB est un espace colorimétrique avec trois composantes : le rouge, le vert et le bleu. Le type d’espace colorimétrique ne définit pas les caractéristiques chromatiques particulières de l’espace (par exemple, la chromaticité des couleurs primaires).

* **[!UICONTROL Type PCS]** : ce type PCS est l’espace colorimétrique de « sortie » du profil, c’est-à-dire son espace de connexion au profil. Par exemple, un profil colorimétrique peut convertir l’espace RVB en espace PCS, qui peut ensuite le convertir en espace CMJN.

Pour un profil d’entrée, d’affichage ou de sortie utile pour le balisage des couleurs ou des images, le type PCS est XYZ ou Lab. Interprétez ce profil comme l’espace colorimétrique spécifique correspondant défini dans la spécification ICC.
