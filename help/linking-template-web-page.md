---
title: Liaison d’un modèle à une page Web
description: Découvrez comment lier un modèle à une page web dans Adobe Dynamic Media Classic.
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 40%

---

# Liaison d’un modèle à une page Web{#linking-a-template-to-a-web-page}

Vos sites web et applications accèdent au contenu du serveur d’images Dynamic Media au moyen de chaînes URL. Une fois que vous avez publié un modèle, Adobe Dynamic Media Classic active une chaîne URL qui référence le modèle sur les serveurs d’images Dynamic Media. Vous pouvez coller cette URL dans un navigateur Web afin de la tester.

Pour placer des chaînes URL dans vos pages et applications web, copiez-les depuis Adobe Dynamic Media Classic. Pour obtenir une chaîne URL de modèle générée avec un paramètre d’image prédéfini, accédez à l’écran Aperçu ou au panneau de navigation (dans la vue Détails). Ensuite, sélectionnez un paramètre d’image prédéfini, puis cliquez sur le bouton Copier l’URL.

>[!NOTE]
>
>l’URL n’est activée qu’une fois le fichier publié.

## Obtention d’une URL de modèle {#obtaining-a-template-url}

Vous pouvez obtenir une chaîne URL de modèle générée par un paramètre d’image prédéfini depuis l’écran Prévisualisation du modèle. Une fois l’URL copiée, elle est stockée dans le Presse-papiers ; vous pouvez ainsi la coller si nécessaire. Pour obtenir une chaîne d’URL de modèle générée avec un paramètre d’image prédéfini à partir de la page d’aperçu du modèle, procédez comme suit :

1. Sélectionnez le bouton de survol **[!UICONTROL Aperçu]** du modèle ou accédez à **[!UICONTROL Fichier]** > **[!UICONTROL Aperçu]**.
1. A l’aide des menus du paramètre prédéfini, choisissez le paramètre d’image prédéfini avec lequel vous souhaitez diffuser l’image de modèle. La page Aperçu vous montre à quoi ressemble le modèle lorsqu’il est diffusé à partir du serveur.
1. Sélectionnez **[!UICONTROL Copier l’URL]** pour pouvoir copier l’URL dans le Presse-papiers.

## Ajout d’URL de modèles  à votre page Web {#adding-template-urls-to-your-web-page}

Pour ajouter un modèle à votre page web, consultez votre équipe de développement de page web afin de modifier la balise `<IMG>` dans le code de votre page web HTML. Utilisez la chaîne URL Dynamic Media Classic Adobe pour envoyer une demande aux serveurs d’images Dynamic Media. Le moteur de commerce électronique ou le code de page Web dynamique insère l’image de modèle en respectant la taille et les paramètres de formatage définis dans le paramètre d’image prédéfini que vous avez choisi pour le modèle.

>[!MORELIKETHIS]
>
>* [Ajout d’images dynamiques à une page web](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

