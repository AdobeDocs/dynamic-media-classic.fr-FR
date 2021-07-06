---
title: Profils ICC
description: Découvrez les profils ICC.
uuid: 708ff2ad-9a47-4e3e-b643-5b19648f726b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 44f1b4c4-6d7f-4e0f-84ce-11d26745e0f0
feature: Dynamic Media Classic
role: User
exl-id: 989f2761-f5d0-4ece-b2a6-f7b4577aa8a2
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 71%

---

# Profils ICC{#icc-profiles}

Un profil ICC (International Color Consortium) est un fichier qui décrit le mode de conversion approprié des fichiers d’images entre deux espaces colorimétriques. Les profils ICC permettent d’obtenir les couleurs appropriées pour vos images. Ainsi, pour afficher correctement les images destinées à l’impression sur un écran d’ordinateur, vous pouvez utiliser un profil ICC. Ce profil convertit l’image dans un espace colorimétrique différent et s’assure que les couleurs s’affichent correctement à l’écran.

Dans Dynamic Media Classic, vous pouvez choisir un profil ICC pour convertir les images dans un autre espace colorimétrique lorsque vous chargez les images. Tous les profils ICC Photoshop standard sont disponibles par défaut sur Dynamic Media Classic. Pour afficher le nom des profils colorimétriques sur l’écran de téléchargement, sélectionnez le menu Profil de couleurs. Ensuite, choisissez la commande Personnaliser de > à, puis sélectionnez un nom de profil ICC dans les menus Convertir à partir de et Convertir en 

(voir [Options d’édition d’images au téléchargement](image-editing-options-upload.md#image-editing-options-at-upload)).

Outre l’utilisation des profils ICC par défaut, vous pouvez charger d’autres profils ICC dans Dynamic Media Classic et les rendre disponibles pour la conversion de l’espace colorimétrique. Passez en mode Affichage des détails dans le panneau de navigation pour examiner la classe de profil, le type d’espace de couleurs et le type PCS d’un profil ICC.

## Téléchargement de profils ICC {#uploading-icc-profiles}

Téléchargez les profils ICC en procédant de la même façon que pour télécharger les fichiers. Vous pouvez stocker des profils ICC dans n’importe quel dossier Dynamic Media Classic.

(voir [Téléchargement de fichiers](uploading-files.md#uploading_your_files)).

## Examen d’un profil ICC {#examining-an-icc-profile}

Pour examiner un profil ICC, sélectionnez-le dans le panneau de navigation, puis affichez-le en mode Affichage des détails. La vue de détails fournit les informations suivantes sur les profils ICC :

* **Classe de profil**  : l’ICC (International Color Consortium) définit chaque classe pour couvrir un type d’application. Par exemple, les profils d’entrée s’appliquent aux périphériques tels que les appareils photo numériques et les numériseurs, tandis que les profils de sortie s’appliquent aux imprimantes.

* **Type d’espace colorimétrique**  : ce nombre est l’espace colorimétrique &quot;d’entrée&quot; du profil, tel que défini par l’ICC. Le type d’espace colorimétrique définit le nombre de composantes de l’espace colorimétrique et l’interprétation de ces composantes. Par exemple, RVB est un espace colorimétrique avec trois composantes : le rouge, le vert et le bleu. Le type d’espace colorimétrique ne définit pas les caractéristiques chromatiques particulières de l’espace (par exemple, la chromaticité des couleurs primaires).

* **Type PCS**  : ce type PCS est l’espace colorimétrique &quot;de sortie&quot; du profil, son espace de connexion au profil. Par exemple, un profil colorimétrique peut convertir l’espace RVB en espace PCS, qui peut ensuite le convertir en espace CMJN.

Pour un profil d’entrée, d’affichage ou de sortie pratique pour baliser les couleurs ou les images, le type PCS est XYZ ou Lab. Interprétez ce profil comme l’espace colorimétrique spécifique correspondant défini dans la spécification ICC.
