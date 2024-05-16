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
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 41%

---

# Profils ICC{#icc-profiles}

Un profil ICC (International Color Consortium) est un fichier qui décrit comment convertir correctement des fichiers image d’un espace colorimétrique à un autre. Les profils ICC permettent d’obtenir les couleurs appropriées pour vos images. Par exemple, pour afficher correctement les images destinées à l’impression sur un écran d’ordinateur, vous pouvez choisir un profil ICC. Ce profil convertit l’image dans un espace colorimétrique différent et s’assure que les couleurs s’affichent correctement à l’écran.

Dans Adobe Dynamic Media Classic, vous pouvez choisir un profil ICC pour convertir les images dans un autre espace colorimétrique lorsque vous chargez les images. Tous les profils ICC Photoshop standard sont disponibles par défaut sur Adobe Dynamic Media Classic. Pour afficher le nom des profils colorimétriques sur l’écran de téléchargement, sélectionnez le menu Profil de couleurs. Sélectionnez ensuite Personnaliser de > à, puis choisissez un nom de profil ICC dans les menus Converti de et Converti en .

Voir [Options de modification d’image lors du téléchargement](image-editing-options-upload.md#image-editing-options-at-upload).

Outre l’utilisation des profils ICC par défaut, vous pouvez charger d’autres profils ICC dans Adobe Dynamic Media Classic et les rendre disponibles pour la conversion de l’espace colorimétrique. Passez en mode Affichage des détails dans le panneau de navigation pour examiner la classe de profil, le type d’espace colorimétrique et le type PCS d’un profil ICC.

## Chargement de profils ICC {#uploading-icc-profiles}

Téléchargez les profils ICC en procédant de la même façon que pour télécharger les fichiers. Vous pouvez stocker des profils ICC dans n’importe quel dossier Adobe Dynamic Media Classic.

Voir [Chargement des fichiers](uploading-files.md#uploading_your_files).

## Examiner un profil ICC {#examining-an-icc-profile}

Pour examiner un profil ICC, sélectionnez-le dans le panneau de navigation et affichez-le dans la vue Détails. La vue Détails fournit ces informations sur les profils ICC :

* **[!UICONTROL Classe de profil]**: l’ICC (International Color Consortium) définit chaque classe pour couvrir un type d’application. Par exemple, les profils d’entrée s’appliquent aux périphériques tels que les appareils photo numériques et les numériseurs, tandis que les profils de sortie s’appliquent aux imprimantes.

* **[!UICONTROL Type d’espace colorimtrique]**: ce nombre est l’espace colorimétrique &quot;d’entrée&quot; du profil, tel que défini par l’ICC. Le type d’espace colorimétrique définit le nombre de composantes de l’espace colorimétrique et l’interprétation de ces composantes. Par exemple, RVB est un espace colorimétrique avec trois composantes : le rouge, le vert et le bleu. Le type d’espace colorimétrique ne définit pas les caractéristiques chromatiques particulières de l’espace (par exemple, la chromaticité des couleurs primaires).

* **[!UICONTROL Type PCS]**: ce type PCS est l’espace colorimétrique &quot;output&quot; du profil, son espace de connexion au profil. Par exemple, un profil colorimétrique peut convertir l’espace RVB en espace PCS, qui peut ensuite le convertir en espace CMJN.

Pour un profil d’entrée, d’affichage ou de sortie pratique pour baliser les couleurs ou les images, le type PCS est XYZ ou Lab. Interprétez ce profil comme l’espace colorimétrique spécifique correspondant défini dans la spécification ICC.
