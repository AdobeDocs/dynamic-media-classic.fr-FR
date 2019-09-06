---
title: Profils ICC
seo-title: Profils ICC
description: 'null'
seo-description: Découvrez les profils ICC.
uuid: 708 ff 2 ad -9 a 47-4 e 3 e-b 643-5 b 19648 f 726 b
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/support_ files
discoiquuid: 44 f 1 b 4 c 4-6 d 7 f -4 e 0 f -84 ce -11 d 26745 e 0 f 0
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# Profils ICC{#icc-profiles}

Un profil ICC (International Color Consortium) est un fichier qui décrit le mode de conversion approprié des fichiers d’images entre deux espaces colorimétriques. Les profils ICC permettent d’obtenir les couleurs appropriées pour vos images. Ainsi, pour afficher correctement les images destinées à l’impression sur un écran d’ordinateur, vous pouvez utiliser un profil ICC. Ce profil convertit l’image dans un espace colorimétrique différent et s’assure que les couleurs s’affichent correctement à l’écran.

Dans Scene7 Publishing System, vous pouvez choisir un profil ICC pour convertir les images dans un espace colorimétrique différent lorsque vous téléchargez les images. Tous les profils ICC Photoshop standard sont disponibles par défaut sur SPS. Pour afficher le nom des profils colorimétriques sur l’écran de téléchargement, sélectionnez le menu Profil de couleurs. Ensuite, choisissez la commande Personnaliser de &gt; à, puis sélectionnez un nom de profil ICC dans les menus Convertir à partir de et Convertir en (voir [Options d’édition d’images au téléchargement](image-editing-options-upload.md#image-editing-options-at-upload)).

Vous pouvez télécharger d’autres profils ICC que les profils par défaut sur le système SPS et les rendre accessibles pour la conversion d’espace de couleurs. Passez en mode Affichage des détails dans le panneau de navigation pour examiner la classe de profil, le type d’espace de couleurs et le type PCS d’un profil ICC.

## Téléchargement de profils ICC {#uploading-icc-profiles}

Téléchargez les profils ICC en procédant de la même façon que pour télécharger les fichiers. Vous pouvez stocker les profils ICC dans n’importe quel dossier SPS (voir [Téléchargement de fichiers](uploading-files.md#uploading_your_files)).

## Examen d’un profil ICC {#examining-an-icc-profile}

Pour examiner un profil ICC, sélectionnez-le dans le panneau de navigation, puis affichez-le en mode Affichage des détails. La vue de détails fournit les informations suivantes sur les profils ICC :

**Classe** de profil ICC (International Color Consortium) définit chaque classe pour couvrir un type d'application. Par exemple, les profils d’entrée s’appliquent aux périphériques tels que les appareils photo numériques et les numériseurs, tandis que les profils de sortie s’appliquent aux imprimantes.

**Type d'espace colorimétrique** Ce nombre correspond à l'espace colorimétrique d'entrée du profil, tel que défini par ICC. Le type d’espace colorimétrique définit le nombre de composantes de l’espace colorimétrique et l’interprétation de ces composantes. Par exemple, RVB est un espace colorimétrique avec trois composantes : le rouge, le vert et le bleu. Le type d’espace colorimétrique ne définit pas les caractéristiques chromatiques particulières de l’espace (par exemple, la chromaticité des couleurs primaires).

**Type PCS** Ce type PCS est l'espace colorimétrique de sortie du profil, son espace de connexion de profil. Par exemple, un profil colorimétrique peut convertir l’espace RVB en espace PCS, qui peut ensuite le convertir en espace CMJN.

Pour un profil d’entrée, d’affichage ou de sortie pratique pour baliser les couleurs ou les images, le type PCS est XYZ ou Lab. Interprétez ce profil comme l’espace colorimétrique spécifique correspondant défini dans la spécification ICC.
