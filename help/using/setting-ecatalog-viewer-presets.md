---
title: Configuration des paramètres prédéfinis de la visionneuse de catalogue électronique
description: Découvrez comment configurer les paramètres prédéfinis de la visionneuse de catalogue électronique dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T19:57:04.669Z'
TQID: 'https://experienceleague.adobe.com/Ej7QeFT62FLz2hWS2w-ll2H9m2pkHXlMSJJDJTsgERg'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
source-git-commit: dbe8354bb3a9240d20af51249b4b61e2544120bd
workflow-type: tm+mt
source-wordcount: 464
ht-degree: 12%

---

# Configurer les paramètres prédéfinis de la visionneuse de catalogue électronique{#setting-up-ecatalog-viewer-presets}

Les paramètres prédéfinis de la visionneuse de catalogue électronique déterminent le style, le comportement et l’aspect des visionneuses de catalogue électronique. Adobe Dynamic Media Classic inclut des paramètres prédéfinis de visionneuse de catalogue électronique et vous pouvez créer des paramètres prédéfinis personnalisés si vous disposez d’un accès administrateur.

Pour créer un paramètre prédéfini, vous pouvez créer un nouveau paramètre prédéfini ou commencer par un paramètre prédéfini de la visionneuse de catalogue électronique fourni par Adobe Dynamic Media Classic et l’enregistrer sous un nouveau nom. Pour présenter le matériel imprimé dans les couleurs de votre entreprise et définir le style, vous pouvez créer vos propres paramètres prédéfinis de visionneuse de catalogue électronique.

Les paramètres prédéfinis de la visionneuse de catalogue électronique offrent de nombreux paramètres pour la navigation sur les pages, le zoom, la recherche et la sélection de « thèmes ». L’aspect de ces commandes et l’apparence de la visionneuse dépendent de votre choix de paramètres prédéfinis de la visionneuse de catalogue électronique.

**Pour configurer un paramètre prédéfini de la visionneuse de catalogue électronique (vous devez disposer d’un accès administrateur) :**

1. Sur la barre de navigation générale, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Paramètres prédéfinis de la visionneuse]**.
1. Dans l’écran Paramètres prédéfinis de la visionneuse, créez un paramètre prédéfini de visionneuse de catalogue électronique en créant un nouveau paramètre prédéfini ou en commençant par un paramètre prédéfini de visionneuse de catalogue électronique existant :

   * **Créer un paramètre prédéfini de la visionneuse de catalogue électronique** : sélectionnez **[!UICONTROL Ajouter]**. Dans la boîte de dialogue Ajouter un paramètre prédéfini de visionneuse, choisissez une plateforme, une visionneuse de catalogue électronique, puis sélectionnez **[!UICONTROL Ajouter]**.

   * **Modification d’un paramètre prédéfini de la visionneuse de catalogue électronique** : sélectionnez un paramètre prédéfini de la visionneuse de catalogue électronique, puis sélectionnez **[!UICONTROL Modifier]**. Sélectionnez **[!UICONTROL Enregistrer sous]** une fois la création du paramètre prédéfini terminée.

1. Sur la page `Configure Viewer`, saisissez un nom pour le paramètre prédéfini de la visionneuse de catalogue électronique.
1. Définissez les options de votre choix dans la page `Configure Viewer`.

   Sélectionnez l’icône **[!UICONTROL Info-bulle]** en regard de l’option si vous souhaitez lire sa description.

   La page Aperçu affiche la visionneuse lorsque vous mettez à jour et modifiez des paramètres.

1. (Facultatif) Dans la section **[!UICONTROL Paramètres du panneau Informations]**, l’option **[!UICONTROL URL du serveur d’informations]** peut inclure les jetons spéciaux suivants que la visionneuse remplace.

   | Jeton | Remplacé par | Remarques |
   | --- | --- | --- |
   | `$1$` | valeur rollover_key | Identifiant d’élément de l’élément `<area>` du mappage. |
   | `$2$` | frame | Numéro de séquence de l’image actuellement affichée dans la visionneuse d’images |
   | `$3$` | racine de l’image | Premier élément de chemin du premier objet indiqué dans la commande d’image (en principe, l’identifiant de catalogue d’images de l’entrée de catalogue indiquant la visionneuse d’images) |

1. (Facultatif) Dans la zone **[!UICONTROL Paramètres du panneau Informations]**, dans le champ **[!UICONTROL Modèle de réponse]**, saisissez le texte à afficher si Adobe Dynamic Media Classic rencontre une erreur lors de la récupération des informations d’une zone cliquable. Par exemple, si le système reçoit un nom de société et de catalogue électronique, mais pas d’identifiant de substitution, ce message s’affiche.

>[!NOTE]
>
>Pour utiliser ce modèle de réponse au lieu du modèle défini dans le catalogue électronique lui-même, ajoutez `fmt=1` à la fin de l’URL du serveur d’informations. Par exemple : `https://.../$3$/$4$/$1$/?FMT=1`.

1. Sélectionnez **[!UICONTROL Enregistrer]**.
1. Sélectionnez **[!UICONTROL Par défaut]** afin que le paramètre prédéfini de la visionneuse de catalogue électronique que vous avez créé soit utilisé pour afficher les catalogues électroniques sur votre page web.

Pour supprimer un paramètre prédéfini de la visionneuse de catalogue électronique, sélectionnez-le dans l’écran Paramètres prédéfinis de la visionneuse et sélectionnez **[!UICONTROL Supprimer]**.

>[!MORELIKETHIS]
>
>* [Paramètres prédéfinis de la visionneuse](application-setup.md#viewer_presets)
