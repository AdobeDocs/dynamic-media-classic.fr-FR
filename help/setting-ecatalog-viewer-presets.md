---
title: Configuration des paramètres prédéfinis de la visionneuse de catalogue électronique
seo-title: Configuration des paramètres prédéfinis de la visionneuse de catalogue électronique
description: 'null'
seo-description: Découvrez comment configurer des paramètres prédéfinis de visionneuse de catalogue électronique.
uuid: aca 66 bc 5-8491-4 d 81-9 a 06-1 d 3531860 a 14
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 6 c 123 f 85-3 bc 4-4392-a 7 fb -55618127 c 65 e
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Configuration des paramètres prédéfinis de la visionneuse de catalogue électronique{#setting-up-ecatalog-viewer-presets}

Les paramètres prédéfinis de la visionneuse de catalogue électronique déterminent le style, le comportement et l’aspect des visionneuses de catalogue électronique. Dynamic Media Classic fournit des paramètres prédéfinis de visionneuse de catalogue électronique. Vous pouvez également créer vos propres paramètres prédéfinis de visionneuse de catalogue électronique si vous êtes administrateur.

Pour créer un paramètre prédéfini, vous pouvez commencer à partir de zéro ou commencer par un paramètre prédéfini fourni par Media Classic Classic, puis l'enregistrer sous un nouveau nom. Vous pouvez créer vos paramètres prédéfinis de visionneuse de catalogue électronique pour présenter un support imprimé dans les couleurs de votre société et définir le ton.

De nombreux paramètres prédéfinis sont disponibles pour la visionneuse de catalogue électronique ; ils portent notamment sur la navigation, l’exécution de zoom, la recherche, ainsi que sur les habillages. L’aspect des commandes et de la visionneuse elle-même est fonction des paramètres prédéfinis de visionneuse de catalogue électronique actuellement sélectionnés.

Pour créer un paramètre prédéfini de visionneuse de catalogue électronique (vous devez être un administrateur), procédez comme suit :

1. Cliquez sur **Configuration** &gt; **Paramètres prédéfinis de la visionneuse**.
1. Dans l’écran Paramètres prédéfinis de la visionneuse, créez un paramètre prédéfini de visionneuse de catalogues électroniques en partant de zéro ou d’un paramètre prédéfini existant :

   **Création d'un paramètre prédéfini de visionneuse de catalogue électronique** Cliquez sur Ajouter. In the Add Viewer Preset dialog box, choose a platform, choose eCatalog Viewer, then click **Add**.

   **Modification d'un paramètre prédéfini de visionneuse de catalogue électronique** Sélectionnez un paramètre prédéfini de visionneuse de catalogue électronique, puis cliquez sur Modifier. Click **Save As** after you finish creating the preset.

1. Dans l’écran Configurer la visionneuse, saisissez le nom à attribuer à votre paramètre prédéfini de visionneuse de catalogue électronique.
1. Dans l’écran Configurer la visionneuse, définissez les options de votre choix.

   Cliquez sur l’icône d’informations  adjacente pour pouvoir voir sa description.

   L’écran de prévisualisation affiche la visionneuse à mesure que vous actualisez et modifiez les paramètres.

1. (Facultatif) Disponible parmi les paramètres du panneau d’informations, l’option URL du serveur d’informations peut inclure les jetons spéciaux suivants, remplacés par la visionneuse :

   | Jeton | Remplacé par | Remarques |
   |--- |--- |--- |
   | `$1$` | valeur rollover_key | The item identifier from the `<area>` element of the map. |
   | `$2$` | frame | Numéro de séquence de l’image actuellement affichée dans la visionneuse d’images |
   | `$3$` | imageroot | Premier élément de chemin du premier objet indiqué dans la commande d’image (en principe, l’identifiant de catalogue d’images de l’entrée de catalogue indiquant la visionneuse d’images) |

1. (Facultatif) Dans la zone Modèle de réponse du panneau d'informations, saisissez le texte qui doit s'afficher si Dynamic Media Classic rencontre une erreur lors de la récupération d'informations pour une zone cliquable. Par exemple, si le système reçoit un nom d’entreprise et un nom de catalogue électronique, mais pas d’identificateur de survol, ce message est affiché à l’intention de l’utilisateur.

>[!NOTE]
>
>pour utiliser ce modèle de réponse à la place du modèle défini dans le catalogue électronique, ajoutez « fmt=1 » à la fin de l’URL du serveur d’informations. Par exemple: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Cliquez sur **Enregistrer**.
1. Cliquez sur Par défaut si vous souhaitez utiliser le paramètre prédéfini de visionneuse de catalogue électronique que vous avez créé pour afficher des catalogues électroniques sur votre page Web.

To delete an eCatalog Viewer Preset, select it on the Viewer Presets screen and click **Delete**.

>[!MORELIKETHIS]
>
>* [Paramètres prédéfinis de la visionneuse](application-setup.md#viewer_presets)

