---
title: Liaison d’un modèle à une page Web
seo-title: Liaison d’un modèle à une page Web
description: 'null'
seo-description: Découvrez comment lier un modèle à une page Web.
uuid: f 111 ef 06-4 afc -454 c -86 ce -5 d 640236 d 40 b
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/template_ basics
discoiquuid: 989 dba 07-448 a -45 b 1-b 157-af 50 abb 5359 a
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Liaison d’un modèle à une page Web{#linking-a-template-to-a-web-page}

Vos sites Web et applications accèdent au contenu du serveur Dynamic Media Image Server au moyen de chaînes URL. Après avoir publié un modèle, Dynamic Media Classic active une chaîne URL qui référence le modèle sur les serveurs d'images de médias dynamiques. Vous pouvez coller cette URL dans un navigateur Web afin de la tester.

Pour placer les chaînes URL dans vos pages Web et applications, copiez-les à partir de Scene7 Publishing System. Pour obtenir une chaîne URL générée avec un paramètre d’image prédéfini, affichez l’écran de prévisualisation ou le panneau de navigation (vue de détails). Ensuite, sélectionnez un paramètre d’image prédéfini, puis cliquez sur le bouton Copier l’URL.

>[!NOTE]
>
>l’URL n’est activée qu’une fois le fichier publié.

## Obtention d’une URL de modèle {#obtaining-a-template-url}

Vous pouvez obtenir une chaîne URL de modèle générée par un paramètre d’image prédéfini depuis l’écran Prévisualisation du modèle. Une fois l’URL copiée, elle est stockée dans le Presse-papiers ; vous pouvez ainsi la coller si nécessaire. Pour obtenir, à partir de l’écran Prévisualisation du modèle, une chaîne URL de modèle générée avec un paramètre d’image prédéfini, procédez comme suit :

1. Cliquez sur le bouton de prévisualisation en survol du modèle ou choisissez la commande Fichier &gt; Prévisualiser. L’écran de prévisualisation s’ouvre. 
1. A l’aide des menus du paramètre prédéfini, choisissez le paramètre d’image prédéfini avec lequel vous souhaitez diffuser l’image de modèle. L’écran de prévisualisation affiche le modèle tel qu’il apparaîtra lors de sa diffusion à partir du serveur.
1. Cliquez sur le bouton Copier l’URL pour copier l’URL dans le Presse-papiers.

## Ajout d’URL de modèle à une page Web {#adding-template-urls-to-your-web-page}

To add a template to your web page, consult with your web page development team to modify the `<IMG>` tag in your HTML web page code using the Dynamic Media Classic URL string to make a request to Dynamic Media Image Servers. Le moteur de commerce électronique ou le code de page Web dynamique insère l’image de modèle en respectant la taille et les paramètres de formatage définis dans le paramètre d’image prédéfini que vous avez choisi pour le modèle.

>[!MORELIKETHIS]
>
>* [Ajout d’images dynamiques à une page Web](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

