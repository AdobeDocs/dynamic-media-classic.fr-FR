---
title: Application de bureau Adobe Classic - Maintenant disponible
seo-title: Application de bureau Adobe Classic - Maintenant disponible
description: 'null'
seo-description: En savoir plus sur l’application de bureau Dynamic Media Classic.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
translation-type: tm+mt
source-git-commit: f2b8c8a5bdac38a48157c6eaa80cd09692ee2259
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---


# Maintenant disponible : Application de bureau Adobe Classic {#dynamic-media-classic-desktop-app}

Les utilisateurs de Dynamic Media Classic ont désormais accès à une nouvelle application de bureau qui ne repose plus sur la technologie Adobe Flash dans le navigateur.

Cette nouvelle application est désormais disponible pour Windows et macOS.

>[!IMPORTANT]
>
>Nous vous recommandons d’installer la nouvelle application de bureau Adobe Classic d’ici le 1er octobre 2020. Ainsi, vous aurez une transition fluide avant que Adobe Flash Player ne soit abandonné le 31 décembre 2020. A cette date, vous ne pourrez plus vous connecter à la version navigateur de l’interface utilisateur Adobe Classic, appelée Scene7 Publishing System dans le produit.

Reportez-vous à la FAQ relative à l’expérience de connexion à [Dynamic Media Classic, désormais disponible.](/help/new-ui-2020.md)

## Configuration requise pour l’application de bureau Adobe Classic {#system-requirements-dmc-app}

L’application de bureau Adobe Classic est compatible avec les systèmes d’exploitation suivants :
* macOS X 10.10 ou version ultérieure.
* Windows 7 ou version ultérieure.

## Téléchargement et installation de l’application de bureau Adobe Classic {#installation-dmc-app}

1. Désinstallez toutes les anciennes versions d’application de bureau Dynamic Media Classic sur votre système.

1. Téléchargez le dernier programme d’installation de l’application de bureau Adobe Classic.

   * [macOS (.dmg) - Télécharger.](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.dmg)
   * [Windows (.exe) - Télécharger.](lhttp://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.exe)

1. Effectuez l’une des opérations suivantes en fonction du programme d’installation que vous avez téléchargé.

   * **Pour macOS** - Dans la boîte de dialogue **[!UICONTROL glisser-déposer pour installer]** , faites glisser l’outil **[!UICONTROL Adobe Classic]** et déposez-le sur **[!UICONTROL Applications]**.

      ![Effectuer un glisser-déposer d’installation sur macOS](/help/assets/dragondrop-install1.png)

   * Dans le dossier **[!UICONTROL Applications]** , appuyez sur l’icône Adobe Classic.
   * Dans la boîte de dialogue, appuyez sur **[!UICONTROL Ouvrir]** pour ouvrir l’application de bureau Adobe Classic.

      ![Ouvrir l’application téléchargée](/help/assets/open-dmclassicapp1.png)

   * **Pour Windows** - Exécutez le fichier binaire du programme d’installation et suivez les instructions à l’écran pour installer l’application de bureau.

1. Lorsque vous ouvrez l’application, la nouvelle page de connexion Adobe Classic s’affiche :

   ![Connexion Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Utilisez les mêmes informations d’identification que celles de votre navigateur pour vous connecter à Adobe Classic.

   Pour que le **[!UICONTROL serveur]** puisse utiliser, voir le mappage suivant pour l’environnement de production :

   | URL du navigateur | Nom du serveur d’applications de bureau |
   |---|---|
   | https://s7sps1.scene7.com/ | Production de NA (Amérique du Nord) |
   | https://s7sps3.scene7.com/ | Production EMEA (Europe, Moyen-Orient et Afrique) |
   | https://s7sps5.scene7.com/ | Production d&#39;APAC (Asie-Pacifique) |

1. Après avoir publié l’interface utilisateur de connexion, vous remarquerez l’expérience familière de l’interface utilisateur du navigateur. Vous pouvez désormais transmettre votre activité quotidienne comme d’habitude dans l’interface utilisateur de l’application de bureau.

## Limites connues dans Dynamic Media Classic

**_S’applique uniquement à Windows : le nombre de fichiers pouvant être téléchargés via l’interface utilisateur de l’application de bureau est-il limité ?_**<br> Oui, un maximum de 150 fichiers peuvent être téléchargés à la fois via l’interface utilisateur de l’application de bureau.

**_Application pour Windows et macOS - Comment puis-je passer d’une société à l’autre ?_**<br> Pour passer d’une société à l’autre, procédez comme suit :
* Dans l’application Dynamic Media Classic, sélectionnez la nouvelle société dans la liste déroulante société.
* Lorsque la fenêtre contextuelle s’affiche, appuyez sur **[!UICONTROL OK]** pour vous déconnecter et fermer l’application.

   ![Redémarrez l’application pour utiliser la nouvelle société.](/help/assets/dmclassic-new-company1.png)
* Redémarrez Dynamic Media Classic, puis connectez-vous comme d’habitude pour utiliser la nouvelle société.

## Conseils et astuces

**_Je ne peux pas voir le panneau Panier sur le landing page de Dynamic Media Classic._**<br> Dans Dynamic Media Classic, appuyez sur **[!UICONTROL Configuration > Configuration]** personnelle. Dans la section Navigateur, assurez-vous que l’option **[!UICONTROL Afficher les fonctionnalités]** MediaPortal est sélectionnée (cochée). Appuyez sur **[!UICONTROL Enregistrer > Fermer]**.

**_L’état de publication (indicateur vert) d’une ressource n’est pas reflété correctement._**<br> Dans l’interface utilisateur du navigateur, une nouvelle connexion à l’interface utilisateur était nécessaire pour afficher l’état de publication correct des ressources. Dans l’application de bureau, nous avons introduit une icône **[!UICONTROL Actualiser]** sur la barre d’outils, à droite du bouton **[!UICONTROL Sélectionner aucun]** . Appuyez sur l’icône **[!UICONTROL Actualiser]** pour afficher le dernier état de toutes les ressources d’une page donnée. Aucune nouvelle connexion n’est requise, comme dans l’interface utilisateur du navigateur.

![Icône Actualiser](/help/assets/refresh-icon1.png)*Icône Actualiser*

**_Je ne vois pas les paramètres prédéfinis d’ensemble par lot fonctionner dans l’application de bureau._**<br> Appuyez sur **[!UICONTROL Télécharger > Options tâche > Paramètres prédéfinis]** d’ensemble par lot. Assurez-vous que le paramètre prédéfini **[!UICONTROL d’ensemble]** par lot approprié est activé. Cliquez sur **[!UICONTROL Enregistrer et envoyer le transfert]**.
