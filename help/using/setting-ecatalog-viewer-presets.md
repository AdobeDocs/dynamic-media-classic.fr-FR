---
title: Configuration des paramètres prédéfinis de la visionneuse de catalogue électronique
description: Découvrez comment configurer des paramètres prédéfinis de visionneuse de catalogue électronique dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
topic: Integrations, Development
level: Experienced
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 25%

---

# Configuration des paramètres prédéfinis de la visionneuse de catalogue électronique{#setting-up-ecatalog-viewer-presets}

Les paramètres prédéfinis de la visionneuse de catalogue électronique déterminent le style, le comportement et l’aspect des visionneuses de catalogue électronique. Adobe Dynamic Media Classic fournit des paramètres prédéfinis de visionneuse de catalogue électronique. Vous pouvez également créer vos propres paramètres prédéfinis de visionneuse de catalogue électronique si vous êtes administrateur.

Pour créer un paramètre prédéfini, vous pouvez partir de zéro ou commencer avec un paramètre prédéfini de visionneuse de catalogue électronique fourni par Adobe Dynamic Media Classic et l’enregistrer sous un nouveau nom. Vous pouvez créer vos paramètres prédéfinis de visionneuse de catalogue électronique pour présenter un support imprimé dans les couleurs de votre société et définir le ton.

Les paramètres prédéfinis de la visionneuse de catalogue électronique offrent de nombreux paramètres pour passer d’une page à l’autre, effectuer un zoom, effectuer une recherche et choisir &quot;habillages&quot;. L’aspect de ces commandes et l’affichage de la visionneuse dépendent de votre choix de paramètres prédéfinis de visionneuse de catalogue électronique.

Pour créer un paramètre prédéfini de visionneuse de catalogue électronique (vous devez être administrateur), procédez comme suit :

1. Sur la barre de navigation globale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres prédéfinis de la visionneuse]**.
1. Dans l’écran Paramètres prédéfinis de la visionneuse, créez un paramètre prédéfini de visionneuse de catalogues électroniques en partant de zéro ou d’un paramètre prédéfini existant :

   * **Créer un paramètre prédéfini de visionneuse de catalogue électronique** : sélectionnez **[!UICONTROL Ajouter]**. Dans la boîte de dialogue Ajouter un paramètre prédéfini de visionneuse, choisissez une plate-forme, choisissez Visionneuse de catalogue électronique, puis sélectionnez **[!UICONTROL Ajouter]**.

   * **Modifier un paramètre prédéfini de visionneuse de catalogue électronique** : sélectionnez un paramètre prédéfini de visionneuse de catalogue électronique, puis sélectionnez **[!UICONTROL Modifier]**. Sélectionnez **[!UICONTROL Enregistrer sous]** une fois le paramètre prédéfini créé.

1. Sur la page `Configure Viewer`, saisissez un nom pour votre paramètre prédéfini de visionneuse de catalogue électronique.
1. Sur la page `Configure Viewer`, définissez les options de votre choix.

   sélectionnez l’icône **[!UICONTROL Conseil d’informations]** en regard de l’option si vous souhaitez lire sa description.

   La page Aperçu affiche la visionneuse au fur et à mesure que vous mettez à jour et modifiez les paramètres.

1. (Facultatif) Dans les **[!UICONTROL paramètres du panneau d’informations]**, l’option **[!UICONTROL URL du serveur d’informations]** peut inclure les jetons spéciaux suivants, que la visionneuse remplace :

   | Jeton | Remplacé par | Remarques |
   | --- | --- | --- |
   | `$1$` | valeur rollover_key | Identifiant de l’élément de l’élément `<area>` de la carte. |
   | `$2$` | frame | Numéro de séquence de l’image actuellement affichée dans la visionneuse d’images |
   | `$3$` | racine de l’image | Premier élément de chemin du premier objet indiqué dans la commande d’image (en principe, l’identifiant de catalogue d’images de l’entrée de catalogue indiquant la visionneuse d’images) |

1. (Facultatif) Dans la zone **[!UICONTROL Paramètres du panneau d’informations]**, dans la zone **[!UICONTROL Modèle de réponse]**, saisissez le texte à afficher si Adobe Dynamic Media Classic rencontre une erreur lors de la récupération des informations d’une zone cliquable. Par exemple, si le système reçoit un nom d’entreprise et un nom de catalogue électronique, mais pas d’identificateur de survol, ce message est affiché à l’intention de l’utilisateur.

>[!NOTE]
>
>Pour utiliser ce modèle de réponse au lieu du modèle défini dans le catalogue électronique, ajoutez `fmt=1` à la fin de l’URL du serveur d’informations. Par exemple : `https://.../$3$/$4$/$1$/?FMT=1`.

1. Sélectionnez **[!UICONTROL Enregistrer]**.
1. Sélectionnez **[!UICONTROL Par défaut]** afin que le paramètre prédéfini de visionneuse de catalogue électronique que vous avez créé soit celui qui est utilisé pour afficher les catalogues électroniques sur votre page Web.

Pour supprimer un paramètre prédéfini de visionneuse de catalogue électronique, sélectionnez-le dans l’écran Paramètres prédéfinis de la visionneuse et sélectionnez **[!UICONTROL Supprimer]**.

>[!MORELIKETHIS]
>
>* [Paramètres prédéfinis de la visionneuse](application-setup.md#viewer_presets)
