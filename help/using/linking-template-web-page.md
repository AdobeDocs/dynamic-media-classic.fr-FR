---
title: Associer un modèle à une page Web
description: Découvrez comment lier un modèle à une page web dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
topic: Administration, Content Management, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 17%

---

# Associer un modèle à une page Web{#linking-a-template-to-a-web-page}

Vos sites Web et applications accèdent au contenu du serveur d’images Dynamic Media au moyen de chaînes URL. Après avoir publié un modèle, Adobe Dynamic Media Classic active une chaîne URL qui référence le modèle sur les serveurs d’images Dynamic Media. Vous pouvez coller cette URL dans un navigateur Web à des fins de test.

Pour placer des chaînes URL dans vos pages et applications Web, copiez-les depuis Adobe Dynamic Media Classic. Pour obtenir une chaîne d’URL de modèle générée avec un paramètre d’image prédéfini, accédez à l’écran Aperçu ou au panneau Parcourir (en mode Affichage des détails). Ensuite, sélectionnez un paramètre d’image prédéfini, puis cliquez sur le bouton Copier l’URL.

>[!NOTE]
>
>l’URL n’est activée qu’une fois le fichier publié.

## Obtention d’une URL de modèle {#obtaining-a-template-url}

Vous pouvez obtenir une chaîne URL de modèle générée par un paramètre d’image prédéfini depuis l’écran Prévisualisation du modèle. Une fois l’URL copiée, elle est stockée dans le Presse-papiers ; vous pouvez ainsi la coller si nécessaire. Pour obtenir une chaîne d’URL de modèle générée avec un paramètre d’image prédéfini à partir de la page d’aperçu du modèle, procédez comme suit :

1. Sélectionnez le bouton de survol **[!UICONTROL Aperçu]** du modèle ou accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Aperçu]**.
1. À l’aide des menus du paramètre prédéfini, choisissez le paramètre d’image prédéfini avec lequel vous souhaitez diffuser l’image du modèle. La page Aperçu vous montre à quoi ressemble le modèle lorsqu’il est diffusé à partir du serveur.
1. Sélectionnez **[!UICONTROL Copier l’URL]** pour pouvoir copier l’URL dans le Presse-papiers.

## Ajouter des URL de modèle à votre page Web {#adding-template-urls-to-your-web-page}

Pour ajouter un modèle à votre page Web, consultez votre équipe de développement de page Web afin de modifier la balise `<IMG>` dans le code de page Web de votre HTML. Utilisez la chaîne URL Adobe Dynamic Media Classic pour envoyer une requête aux serveurs d’images Dynamic Media. Le moteur de commerce ou le code de page Web dynamique insère l’image du modèle à la taille et avec la spécification de formatage définie par le paramètre d’image prédéfini que vous choisissez pour votre modèle.

>[!MORELIKETHIS]
>
>* [Ajouter des images dynamiques à votre page web](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
