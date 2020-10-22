---
title: Application de bureau Adobe Dynamic Media Classic - Maintenant disponible
seo-title: Application de bureau Adobe Dynamic Media Classic - Maintenant disponible
description: 'null'
seo-description: En savoir plus sur l’application de bureau Dynamic Media Classic.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
translation-type: tm+mt
source-git-commit: bc79edcdb378fab906df851971acd33f8af18105
workflow-type: tm+mt
source-wordcount: '1422'
ht-degree: 0%

---


# Maintenant disponible : Application de bureau Adobe Dynamic Media Classic {#dynamic-media-classic-desktop-app}

Les utilisateurs de Dynamic Media Classic ont désormais accès à une nouvelle application de bureau qui ne repose plus sur la technologie de Flash d’Adobe dans le navigateur.

Cette nouvelle application est désormais disponible pour Windows et macOS.

>[!IMPORTANT]
>
>Nous vous recommandons d’installer la nouvelle application de bureau Adobe Dynamic Media Classic d’ici le 1er octobre 2020. Ainsi, vous aurez une transition en douceur avant que le Flash Player Adobe ne soit abandonné le 31 décembre 2020. A cette date, vous ne pourrez plus vous connecter à la version de navigateur de l’interface utilisateur Adobe Dynamic Media Classic, appelée Contenu multimédia dynamique classique dans le produit.

Reportez-vous à la FAQ pour l’expérience de connexion à [New Dynamic Media Classic, désormais disponible.](/help/new-ui-2020.md)

## Configuration requise pour l’application de bureau Adobe Dynamic Media Classic {#system-requirements-dmc-app}

L’application de bureau Adobe Dynamic Media Classic est compatible avec les systèmes d’exploitation suivants :
* macOS X 10.10 ou version ultérieure.
* Windows 7 ou version ultérieure.

## Correctifs de la dernière version 20.20.2 {#latest-fixes-desktop-app}

* Le nombre de fichiers que vous pouvez télécharger via l’interface utilisateur de l’application de bureau n’est pas limité pour macOS et Windows.
* Il n’est pas nécessaire de se déconnecter de l’application de bureau pour basculer entre les sociétés.
* Ctrl+V pour l’opération de collage fonctionne désormais sous Windows.
* À l’avenir, lorsqu’une nouvelle version de l’application de bureau sera publiée, les utilisateurs seront avertis au sein de l’application de bureau elle-même.

## Téléchargez et installez la dernière application de bureau Adobe Dynamic Media Classic sur macOS ou Windows. {#installation-dmc-app}

Voir aussi:

* [Téléchargement et installation silencieuse de la dernière application de bureau Adobe Dynamic Media Classic sous Mac](#install-silent-mac-dmc-app)
* [Téléchargement et installation silencieuse de la dernière application de bureau Adobe Dynamic Media Classic sous Windows](#install-silent-windows-dmc-app)

1. Désinstallez toutes les anciennes versions d’application de bureau de Dynamic Media Classic sur votre système.

1. Téléchargez le dernier programme d’installation de l’application de bureau Adobe Dynamic Media Classic.

   >[!NOTE]
   >
   >L&#39;utilisateur qui a déjà installé la version GA doit la *désinstaller* de son système Windows local avant d&#39;installer la dernière version. Ou, les utilisateurs peuvent simplement *remplacer* la version GA installée sur leur système macOS local par la dernière version. Les nouveaux utilisateurs doivent installer directement la dernière version 20.20.2.

   La dernière version est la version 20.20.2 disponible à l’adresse suivante :

   * [macOS (.DMG) - Télécharger.](http://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
   * [Windows (.EXE) - Télécharger.](http://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe)

   La version GA (General Availability) de la version 20.20.1 était disponible à l&#39;adresse suivante :

   * [macOS (.DMG) - Télécharger.](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.dmg)
   * [Windows (.EXE) - Télécharger.](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.exe)




1. Effectuez l’une des opérations suivantes en fonction du programme d’installation que vous avez téléchargé.

   * **Pour macOS** - Dans la boîte de dialogue **[!UICONTROL glisser-déposer pour installer]** , faites glisser **[!UICONTROL Adobe Dynamic Media Classic]** et déposez-le sur **[!UICONTROL Applications]**.

      ![Effectuer un glisser-déposer d’installation sur macOS](/help/assets/dragondrop-install1.png)

   * Dans le dossier **[!UICONTROL Applications]** , appuyez sur l’icône Adobe Dynamic Media Classic.
   * Dans la boîte de dialogue, appuyez sur **[!UICONTROL Ouvrir]** pour ouvrir l’application de bureau Adobe Dynamic Media Classic.

      ![Ouvrir l’application téléchargée](/help/assets/open-dmclassicapp1.png)

   * **Pour Windows** - Exécutez le fichier binaire du programme d’installation et suivez les instructions à l’écran pour installer l’application de bureau.

1. Lorsque vous ouvrez l’application, la nouvelle page de connexion à Contenu multimédia dynamique classique Adobe s’affiche :

   ![Connexion à Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Utilisez les mêmes informations d’identification que celles de votre navigateur pour vous connecter à Adobe Dynamic Media Classic.

   Pour que le **[!UICONTROL serveur]** puisse utiliser, voir le mappage suivant pour l’environnement de production :

   | URL du navigateur | Nom du serveur d’applications de bureau |
   |---|---|
   | https://s7sps1.scene7.com/ | Production de NA (Amérique du Nord) |
   | https://s7sps3.scene7.com/ | Production EMEA (Europe, Moyen-Orient et Afrique) |
   | https://s7sps5.scene7.com/ | Production d&#39;APAC (Asie-Pacifique) |

1. Après avoir publié l’interface utilisateur de connexion, vous remarquerez l’expérience familière de l’interface utilisateur du navigateur. Vous pouvez désormais transmettre votre activité quotidienne comme d’habitude dans l’interface utilisateur de l’application de bureau.

## Téléchargement et installation *silencieuse* de la dernière application de bureau Adobe Dynamic Media Classic sur macOS {#install-silent-mac-dmc-app}

Voir aussi:

* [Téléchargez et installez la dernière application de bureau Adobe Dynamic Media Classic sous Mac ou Windows.](#installation-dmc-app)
* [Téléchargement et installation silencieuse de la dernière application de bureau Adobe Dynamic Media Classic sous Windows](#install-silent-windows-dmc-app)

Pour télécharger et *silencieusement* installer la dernière version de l’application de bureau Adobe Dynamic Media Classic sur macOS :

1. Désinstallez toutes les anciennes versions d’application de bureau de Dynamic Media Classic sur votre système.

1. Téléchargez le dernier programme d’installation de l’application de bureau Adobe Dynamic Media Classic pour macOS.

   * [macOS (.DMG) - Télécharger.](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.2.dmg)

1. Montez l&#39;image de disque (.DMG) téléchargée à un emplacement de point de montage à l&#39;aide de la commande suivante :

   `hdiutil attach adobe-dynamic-media-classic-20.20.2.dmg -mountpoint <mount_point_path>`

1. Copiez le fichier .APP dans **[!UICONTROL Applications]** à l’aide de la commande suivante :

   `rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
Unmount DMG - hdiutil detach <mount_point_path>`

1. Lorsque vous ouvrez l’application, la nouvelle page de connexion à Contenu multimédia dynamique classique Adobe s’affiche :

   ![Connexion à Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Utilisez les mêmes informations d’identification que celles de votre navigateur pour vous connecter à Adobe Dynamic Media Classic.

   Pour que le **[!UICONTROL serveur]** puisse utiliser, voir le mappage suivant pour l’environnement de production :

   | URL du navigateur | Nom du serveur d’applications de bureau |
   |---|---|
   | https://s7sps1.scene7.com/ | Production de NA (Amérique du Nord) |
   | https://s7sps3.scene7.com/ | Production EMEA (Europe, Moyen-Orient et Afrique) |
   | https://s7sps5.scene7.com/ | Production d&#39;APAC (Asie-Pacifique) |

## Téléchargement et installation *silencieuse* de la dernière application de bureau Adobe Dynamic Media Classic sous Windows {#install-silent-windows-dmc-app}

La commande que vous utilisez est destinée à une installation silencieuse MSI de base. Cependant, le programme d’installation de l’application de bureau Dynamic Media Classic est un programme d’installation MSI InstallScript créé à l’aide d’InstallShield. Lorsque vous exécutez le programme d’installation en mode d’enregistrement, toute interaction utilisateur est enregistrée dans un fichier de réponse. Ce fichier de réponse est ensuite utilisé pour une installation silencieuse, comme décrit dans [Exécution d’installations en mode silencieux.](https://docs.flexera.com/installshield19helplib/helplibrary/SilentInstall.htm)

Voir aussi:

* [Téléchargez et installez la dernière application de bureau Adobe Dynamic Media Classic sous Mac ou Windows.](#installation-dmc-app)
* [Téléchargement et installation silencieuse de la dernière application de bureau Adobe Dynamic Media Classic sur macOS](#install-silent-mac-dmc-app)

Pour télécharger et *silencieusement* installer la dernière version de l’application de bureau Adobe Dynamic Media Classic sous Windows :

1. Désinstallez toutes les anciennes versions d’application de bureau de Dynamic Media Classic sur votre système.

1. Téléchargez le dernier programme d’installation de l’application de bureau Adobe Dynamic Media Classic.

   * [Windows (.EXE) - Télécharger.](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.2.exe)

1. Exécutez le programme d’installation en mode enregistrement à l’aide de la commande suivante :

   `adobe-dynamic-media-classic-20.20.2.exe /r /f1"C:\Setup.iss"`

1. Dans la fenêtre du programme d’installation de l’interface utilisateur graphique, suivez les étapes d’installation pour que les interactions/entrées, telles que l’emplacement d’installation, soient enregistrées dans `Setup.iss` un fichier.

1. Copiez le `Setup.iss` fichier créé et collez-le `adobe-dynamic-media-classic-20.20.2.exe` sur un autre ordinateur.

1. Exécutez la commande suivante pour une installation silencieuse :

   `adobe-dynamic-media-classic-20.20.2.exe /s /f1"C:\Setup.iss"`

   Vous trouverez des informations détaillées sur les paramètres de ligne de commande dans [Setup.exe et Update.exe Command-Line Parameters.](https://docs.flexera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. Lorsque vous ouvrez l’application, la nouvelle page de connexion à Contenu multimédia dynamique classique Adobe s’affiche :

   ![Connexion à Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Utilisez les mêmes informations d’identification que celles de votre navigateur pour vous connecter à Adobe Dynamic Media Classic.

   Pour que le **[!UICONTROL serveur]** puisse utiliser, voir le mappage suivant pour l’environnement de production :

   | URL du navigateur | Nom du serveur d’applications de bureau |
   |---|---|
   | https://s7sps1.scene7.com/ | Production de NA (Amérique du Nord) |
   | https://s7sps3.scene7.com/ | Production EMEA (Europe, Moyen-Orient et Afrique) |
   | https://s7sps5.scene7.com/ | Production d&#39;APAC (Asie-Pacifique) |


## Présentation vidéo de l’utilisation de l’application de bureau Dynamic Media Classic

Regardez une présentation [vidéo sur l’utilisation de l’application](https://docs.adobe.com/content/help/en/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html) de bureau Dynamic Media Classic (durée : 2 minutes 36 secondes).

## Limites connues de Dynamic Media Classic 20.20.1 (fixées dans la version 20.20.2)

**_S’applique uniquement à Windows : le nombre de fichiers pouvant être téléchargés via l’interface utilisateur de l’application de bureau est-il limité ?_**<br>Oui, un maximum de 150 fichiers peuvent être téléchargés à la fois via l’interface utilisateur de l’application de bureau.

**_Application pour Windows et macOS - Comment puis-je passer d’une société à l’autre ?_**<br>Pour passer d’une société à l’autre, procédez comme suit :
* Dans l’application Contenu multimédia dynamique classique, sélectionnez la nouvelle société dans la liste déroulante société.
* Lorsque la fenêtre contextuelle s’affiche, appuyez sur **[!UICONTROL OK]** pour vous déconnecter et fermer l’application.

   ![Redémarrez l’application pour utiliser la nouvelle société.](/help/assets/dmclassic-new-company1.png)
* Redémarrez Dynamic Media Classic, puis connectez-vous comme d’habitude pour utiliser la nouvelle société.

## Conseils et astuces

**_Je ne parviens pas à afficher le panneau Panier sur le landing page de Contenu multimédia dynamique Classic._**<br>Dans Dynamic Media Classic, appuyez sur**[!UICONTROL Configuration > Configuration ]**personnelle. Dans la section Navigateur, assurez-vous que l’option**[!UICONTROL Afficher les fonctionnalités ]**MediaPortal est sélectionnée (cochée). Appuyez sur**[!UICONTROL Enregistrer > Fermer ]**.

**_L’état de publication (indicateur vert) d’une ressource n’est pas reflété correctement._**<br>Dans l’interface utilisateur du navigateur, une nouvelle connexion à l’interface utilisateur était nécessaire pour afficher l’état de publication correct des ressources. Dans l’application de bureau, nous avons introduit une icône**[!UICONTROL Actualiser ]**sur la barre d’outils, à droite du bouton**[!UICONTROL Sélectionner aucun ]**. Appuyez sur l’icône**[!UICONTROL Actualiser ]**pour afficher le dernier état de toutes les ressources d’une page donnée. Aucune nouvelle connexion n’est requise, comme dans l’interface utilisateur du navigateur.

![Icône Actualiser](/help/assets/refresh-icon1.png)*Icône Actualiser*

**_Je ne vois pas les paramètres prédéfinis d’ensemble par lot fonctionner dans l’application de bureau._**<br>Appuyez sur**[!UICONTROL Télécharger > Options tâche > Paramètres prédéfinis ]**d’ensemble par lot. Assurez-vous que le paramètre prédéfini**[!UICONTROL d’ensemble ]**par lot approprié est activé. Cliquez sur**[!UICONTROL Enregistrer et envoyer le transfert ]**.
