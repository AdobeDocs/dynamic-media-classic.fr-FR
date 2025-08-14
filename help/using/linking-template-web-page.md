---
title: Liaison d’un modèle à une page web
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

# Liaison d’un modèle à une page web{#linking-a-template-to-a-web-page}

Vos sites web et applications accèdent au contenu du serveur d’images Dynamic Media par le biais de chaînes URL. Après la publication d’un modèle, Adobe Dynamic Media Classic active une chaîne d’URL qui référence le modèle sur les serveurs d’images Dynamic Media. Vous pouvez coller cette URL dans un navigateur Web à des fins de test.

Pour placer des chaînes URL dans vos pages Web et applications, copiez-les depuis Adobe Dynamic Media Classic. Pour obtenir une chaîne d’URL de modèle générée avec un paramètre d’image prédéfini, accédez à l’écran de prévisualisation ou au panneau de navigation (dans la vue détaillée). Ensuite, sélectionnez un paramètre d’image prédéfini, puis cliquez sur le bouton Copier l’URL.

>[!NOTE]
>
>l’URL n’est activée qu’une fois le fichier publié.

## Obtention d’une URL de modèle {#obtaining-a-template-url}

Vous pouvez obtenir une chaîne URL de modèle générée par un paramètre d’image prédéfini depuis l’écran Prévisualisation du modèle. Une fois l’URL copiée, elle est stockée dans le Presse-papiers ; vous pouvez ainsi la coller si nécessaire. Pour obtenir une chaîne d’URL de modèle générée avec un paramètre d’image prédéfini à partir de la page d’aperçu du modèle, procédez comme suit :

1. Sélectionnez le bouton de survol du modèle **[!UICONTROL Aperçu]** ou accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Aperçu]**.
1. À l’aide des menus Paramètre prédéfini , sélectionnez le Paramètre d’image prédéfini avec lequel vous souhaitez diffuser l’image de modèle. La page Aperçu vous indique à quoi ressemble le modèle lorsqu’il est diffusé à partir du serveur.
1. Sélectionnez **[!UICONTROL Copier l’URL]** afin de copier l’URL dans le Presse-papiers.

## Ajouter des URL de modèle à votre page web {#adding-template-urls-to-your-web-page}

Pour ajouter un modèle à votre page web, contactez votre équipe de développement de pages web afin de modifier la balise `<IMG>` dans le code de votre page web HTML. Utilisez la chaîne d’URL Adobe Dynamic Media Classic pour adresser une requête aux serveurs d’images Dynamic Media. Le moteur de commerce ou le code de page web dynamique insère l’image de modèle à la taille et avec la spécification de mise en forme définie par le paramètre d’image prédéfini que vous choisissez pour votre modèle.

>[!MORELIKETHIS]
>
>* [Ajouter des images dynamiques à votre page web](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
