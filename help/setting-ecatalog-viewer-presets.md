---
title: Configuration des paramètres prédéfinis de la visionneuse de catalogue électronique
description: Découvrez comment configurer les paramètres prédéfinis de la visionneuse de catalogue électronique.
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
feature: Dynamic Media Classic, Visionneuses, Paramètres prédéfinis de la visionneuse, Catalogue électronique
role: Business Practitioner
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
translation-type: tm+mt
source-git-commit: 6f3801a71dd2a5f162acacf7d8199dbf8c3520f7
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 42%

---

# Configuration des paramètres prédéfinis de la visionneuse de catalogue électronique{#setting-up-ecatalog-viewer-presets}

Les paramètres prédéfinis de la visionneuse de catalogue électronique déterminent le style, le comportement et l’aspect des visionneuses de catalogue électronique. Dynamic Media Classic fournit des paramètres prédéfinis de visionneuse de catalogue électronique et vous pouvez créer vos propres paramètres prédéfinis de visionneuse de catalogue électronique si vous êtes administrateur.

Pour créer un paramètre prédéfini, vous pouvez le début de zéro ou de début à l’aide d’un paramètre prédéfini de visionneuse de catalogue électronique fourni par Dynamic Media Classic et l’enregistrer sous un nouveau nom. Vous pouvez créer vos paramètres prédéfinis de visionneuse de catalogue électronique pour présenter un support imprimé dans les couleurs de votre société et définir le ton.

De nombreux paramètres prédéfinis sont disponibles pour la visionneuse de catalogue électronique ; ils portent notamment sur la navigation, l’exécution de zoom, la recherche, ainsi que sur les habillages. L’aspect de ces commandes et l’apparence de la visionneuse dépendent des paramètres prédéfinis de visionneuse de catalogue électronique que vous avez choisis.

Pour créer un paramètre prédéfini de visionneuse de catalogue électronique (vous devez être un administrateur), procédez comme suit :

1. Sur la barre de navigation globale, cliquez sur **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres prédéfinis de la visionneuse]**.
1. Dans l’écran Paramètres prédéfinis de la visionneuse, créez un paramètre prédéfini de visionneuse de catalogues électroniques en partant de zéro ou d’un paramètre prédéfini existant :

   * **Création d’un paramètre prédéfini**  de visionneuse de catalogue électronique - Cliquez sur  **[!UICONTROL Ajouter]**. Dans la boîte de dialogue Ajouter un paramètre prédéfini de visionneuse, choisissez une plate-forme, choisissez Visionneuse de catalogue électronique, puis cliquez sur **[!UICONTROL Ajouter]**.

   * **Modification d’un paramètre prédéfini**  de visionneuse de catalogue électronique - Sélectionnez un paramètre prédéfini de visionneuse de catalogue électronique, puis cliquez sur Modifier. Cliquez sur **[!UICONTROL Enregistrer sous]** après avoir créé le paramètre prédéfini.

1. Dans l’écran Configurer la visionneuse, saisissez le nom à attribuer à votre paramètre prédéfini de visionneuse de catalogue électronique.
1. Dans l’écran Configurer la visionneuse, définissez les options de votre choix.

   Cliquez sur l&#39;icône **[!UICONTROL Info-bulle]** en regard de l&#39;option si vous souhaitez lire sa description.

   La page Prévisualisation affiche la visionneuse à mesure que vous mettez à jour et modifiez les paramètres.

1. (Facultatif) Dans **[!UICONTROL Paramètres du panneau d’informations]**, l’URL **[!UICONTROL du serveur d’informations]** peut inclure les jetons spéciaux suivants, que le lecteur remplace :

   | Jeton | Remplacé par | Remarques |
   |--- |--- |--- |
   | `$1$` | valeur rollover_key | Identificateur d&#39;élément de l&#39;élément `<area>` de la carte. |
   | `$2$` | frame | Numéro de séquence de l’image actuellement affichée dans la visionneuse d’images |
   | `$3$` | imageroot | Premier élément de chemin du premier objet indiqué dans la commande d’image (en principe, l’identifiant de catalogue d’images de l’entrée de catalogue indiquant la visionneuse d’images) |

1. (Facultatif) Dans la zone **[!UICONTROL Paramètres du panneau d’informations]**, dans la zone **[!UICONTROL Modèle de réponse]**, saisissez le texte à afficher si Dynamic Media Classic rencontre une erreur lors de la récupération d’informations pour une zone cliquable. Par exemple, si le système reçoit un nom d’entreprise et un nom de catalogue électronique, mais pas d’identificateur de survol, ce message est affiché à l’intention de l’utilisateur.

>[!NOTE]
>
>Pour utiliser ce modèle de réponse à la place du modèle défini dans le catalogue électronique lui-même, ajoutez `fmt=1` à la fin de l’URL du serveur d’informations. Par exemple: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Cliquez sur **Enregistrer**.
1. Cliquez sur Par défaut si vous souhaitez utiliser le paramètre prédéfini de visionneuse de catalogue électronique que vous avez créé pour afficher des catalogues électroniques sur votre page Web.

Pour supprimer un paramètre prédéfini de visionneuse de catalogue électronique, sélectionnez-le dans l’écran Paramètres prédéfinis de la visionneuse, puis cliquez sur **[!UICONTROL Supprimer]**.

>[!MORELIKETHIS]
>
>* [Paramètres prédéfinis de la visionneuse](application-setup.md#viewer_presets)

