---
title: Liaison d’un modèle à une page Web
description: Découvrez comment lier un modèle à une page Web.
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
feature: Dynamic Media Classic
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 68%

---


# Liaison d’un modèle à une page Web{#linking-a-template-to-a-web-page}

Vos sites Web et applications accèdent au contenu du serveur Dynamic Media Image Server au moyen de chaînes URL. Après avoir publié un modèle, Dynamic Media Classic active une chaîne URL qui référence le modèle sur les serveurs Dynamic Media Image Server. Vous pouvez coller cette URL dans un navigateur Web afin de la tester.

Pour placer des chaînes URL dans vos pages Web et applications, copiez-les à partir de Dynamic Media Classic. Pour obtenir une chaîne URL générée avec un paramètre d’image prédéfini, affichez l’écran de prévisualisation ou le panneau de navigation (vue de détails). Ensuite, sélectionnez un paramètre d’image prédéfini, puis cliquez sur le bouton Copier l’URL.

>[!NOTE]
>
>l’URL n’est activée qu’une fois le fichier publié.

## Obtention d’une URL de modèle  {#obtaining-a-template-url}

Vous pouvez obtenir une chaîne URL de modèle générée par un paramètre d’image prédéfini depuis l’écran Prévisualisation du modèle. Une fois l’URL copiée, elle est stockée dans le Presse-papiers ; vous pouvez ainsi la coller si nécessaire. Pour obtenir, à partir de l’écran Prévisualisation du modèle, une chaîne URL de modèle générée avec un paramètre d’image prédéfini, procédez comme suit :

1. Cliquez sur le bouton de prévisualisation en survol du modèle ou choisissez la commande Fichier > Prévisualiser. L’écran de prévisualisation s’ouvre. 
1. A l’aide des menus du paramètre prédéfini, choisissez le paramètre d’image prédéfini avec lequel vous souhaitez diffuser l’image de modèle. L’écran de prévisualisation affiche le modèle tel qu’il apparaîtra lors de sa diffusion à partir du serveur.
1. Cliquez sur le bouton Copier l’URL pour copier l’URL dans le Presse-papiers.

## Ajout d’URL de modèle à une page Web  {#adding-template-urls-to-your-web-page}

Pour ajouter un modèle à votre page Web, consultez votre équipe de développement de page Web afin de modifier la balise `<IMG>` dans votre code de page Web HTML à l’aide de la chaîne URL Dynamic Media Classic pour envoyer une requête aux serveurs Dynamic Media Image Server. Le moteur de commerce électronique ou le code de page Web dynamique insère l’image de modèle en respectant la taille et les paramètres de formatage définis dans le paramètre d’image prédéfini que vous avez choisi pour le modèle.

>[!MORELIKETHIS]
>
>* [Ajout d’images dynamiques à une page Web](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

