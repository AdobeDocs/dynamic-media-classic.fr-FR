---
title: Application de bureau Adobe Dynamic Media Classic - Maintenant disponible
description: En savoir plus sur l’application de bureau Dynamic Media Classic.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Administrator,Business Practitioner
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
translation-type: tm+mt
source-git-commit: 8427c3ea6ca3083fd0868286e634a5569c62f7ab
workflow-type: tm+mt
source-wordcount: '1845'
ht-degree: 1%

---

# Maintenant disponible : Adobe de l’application de bureau Dynamic Media Classic {#dynamic-media-classic-desktop-app}

Les utilisateurs de Dynamic Media Classic ont désormais accès à une nouvelle expérience d’application de bureau qui ne repose plus sur la technologie de Flash d’Adobe dans le navigateur.

Cette nouvelle application est désormais disponible pour Windows® et macOS.

>[!IMPORTANT]
>
>Adobe vous recommande d’installer la nouvelle application de bureau Adobe Dynamic Media Classic d’ici le 1er octobre 2020. Ainsi, vous aurez une transition en douceur avant que le Flash Player Adobe ne soit abandonné le 31 décembre 2020. Après cette date, vous ne pouvez plus vous connecter à la version navigateur de l’interface utilisateur d’Adobe Dynamic Media Classic, appelée Dynamic Media Classic dans le produit.

Consultez la FAQ pour l&#39;[expérience de connexion à la nouvelle version de Dynamic Media Classic désormais disponible.](/help/new-ui-2020.md)

## Configuration système requise pour l’application de bureau Dynamic Media Classic {#system-requirements-dmc-app} Adobe

L’application de bureau Adobe Dynamic Media Classic est compatible avec les systèmes d’exploitation suivants :

* macOS 10.10 ou version ultérieure.
* Windows® 7 ou version ultérieure.

>[!NOTE]
>
>La notification de mise à niveau dans l’application de bureau Dynamic Media Classic n’est pas générée pour les versions *mineures*. Les clients qui bénéficient de correctifs dans une version mineure peuvent effectuer une mise à niveau.

## Correctifs de la version mineure (20.21.2) {#minor-release}

* Limite connue dans la version 20.21.1 de la liste déroulante Serveur vide.
* Dans **[!UICONTROL Télécharger les options de la tâche]**, la valeur par défaut de nommage de calque sous **[!UICONTROL Options Photoshop]**, est désormais **[!UICONTROL Nom de la couche]**. Les calques du fichier PSD sont téléchargés comme images distinctes.
   * La valeur par défaut précédente de **[!UICONTROL Nom de calque]** désignait les images en fonction de leur nom de calque ou de leur numéro de calque dans le fichier PSD. Le numéro de calque a été utilisé si les noms de calque du fichier PSD étaient des noms de calque Photoshop par défaut.
   * La nouvelle valeur par défaut **[!UICONTROL Photoshop and Layer Name]** désigne les images situées après le fichier PSD suivi du nom du calque ou du numéro de calque. Le numéro de calque est utilisé si le nom des calques dans le fichier PSD est un nom de calque Photoshop par défaut.
   * Étant donné que les images de calque dans Dynamic Media Classic ont désormais des noms uniques, aucune mise à jour du fichier PSD ou des modèles existants n’est effectuée (les noms de calque partagés dans les fichiers PSD d’origine).
* Miniatures endommagées des ressources.

## Correctifs de la dernière version (20.21.1) {#latest-fixes-desktop-app}

* Problèmes de connexion dus au dépassement de délai, qui se traduisent par le message suivant : *Cet utilisateur peut être affecté au groupe ou aux groupes sans autorisation. Contactez votre administrateur.*
* Les paramètres prédéfinis de la visionneuse sont dupliqués à chaque tentative de mot de passe incorrecte.
* L’application de bureau ne répond plus en raison de nombreux fichiers contenus dans le dossier racine. (Correction sous Windows® ; fonctionne comme vous le souhaitez sur macOS.)

## Correctifs de la version précédente (20.20.2) {#previous-version-fixes-desktop-app}

* Le nombre de fichiers que vous pouvez télécharger via l’interface utilisateur de l’application de bureau n’est pas limité pour macOS et Windows®.
* Il n’est pas nécessaire de se déconnecter de l’application de bureau pour basculer entre les sociétés.
* Ctrl+V pour l’opération de collage fonctionne désormais sous Windows®.
* À l’avenir, lorsqu’une nouvelle version de l’application de bureau sera publiée, les utilisateurs seront avertis au sein de l’application de bureau elle-même.

## Téléchargez et installez la dernière application de bureau Dynamic Media Classic Adobe sur macOS ou Windows® {#installation-dmc-app}

Voir aussi:

* [Téléchargement et installation silencieuse de la dernière application de bureau Dynamic Media Classic Adobe sous Mac](#install-silent-mac-dmc-app)
* [Téléchargez et installez en mode silencieux la dernière application de bureau Adobe Dynamic Media Classic sous Windows®.](#install-silent-windows-dmc-app)

1. Désinstallez toutes les anciennes versions d’application de bureau Dynamic Media Classic sur votre système.

1. Téléchargez le dernier programme d’installation de l’application de bureau Adobe Dynamic Media Classic.

   * La dernière version (20.21.2) est disponible à l’adresse suivante :

      * [macOS (.DMG) - Télécharger](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
      * [Windows® (.EXE) - Télécharger](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe)
   * La version précédente (20.21.1) est disponible à l’adresse suivante :

      * [macOS (.DMG) - Télécharger](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.dmg)
      * [Windows® (.EXE) - Télécharger](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.exe)


<!--         * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. Effectuez l’une des opérations suivantes en fonction du programme d’installation que vous avez téléchargé.

   * **Pour macOS**  - Dans la boîte de dialogue  **[!UICONTROL Faire glisser pour]** installer, faites glisser l’ **[!UICONTROL Adobe Dynamic Media]** Classicet et déposez-le sur  **[!UICONTROL Applications]**.

      ![Effectuer un glisser-déposer d’installation sur macOS](/help/assets/dragondrop-install1.png)

   * Dans le dossier **[!UICONTROL Applications]**, appuyez sur l’icône Adobe Dynamic Media Classic.
   * Dans la boîte de dialogue, appuyez sur **[!UICONTROL Ouvrir]** pour ouvrir l’application de bureau Dynamic Media Classic Adobe.

      ![Ouvrir l’application téléchargée](/help/assets/open-dmclassicapp1.png)

   * **Pour Windows**  - Exécutez le fichier binaire du programme d’installation et suivez les instructions à l’écran pour installer l’application de bureau.

1. Lorsque vous ouvrez l’application, la nouvelle page de connexion à l’Adobe Dynamic Media Classic s’affiche :

   ![Connexion Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Pour vous connecter à l’application de bureau Dynamic Media Classic Adobe, utilisez les mêmes informations d’identification que celles utilisées pour vous connecter à Dynamic Media Classic dans le navigateur.

   Pour que le **[!UICONTROL serveur]** puisse être utilisé, consultez le mappage suivant pour l&#39;environnement de production :

   | URL du navigateur | Nom du serveur d’applications de bureau |
   |---|---|
   | https://s7sps1.scene7.com/ | Production de NA (Amérique du Nord) |
   | https://s7sps3.scene7.com/ | Production EMEA (Europe, Moyen-Orient et Afrique) |
   | https://s7sps5.scene7.com/ | Production d&#39;APAC (Asie-Pacifique) |

1. Après la connexion, notez l’expérience d’interface utilisateur du navigateur qui vous est familière. Vous pouvez continuer votre activité quotidienne Dynamic Media Classic comme d’habitude sur l’application de bureau.

## Téléchargez et *silencieuse* installez la dernière application de bureau Dynamic Media Classic Adobe sur macOS {#install-silent-mac-dmc-app}

Voir aussi:

* [Téléchargement et installation de la dernière application de bureau Adobe Dynamic Media Classic sous Mac ou Windows®](#installation-dmc-app)
* [Téléchargez et installez en mode silencieux la dernière application de bureau Adobe Dynamic Media Classic sous Windows®.](#install-silent-windows-dmc-app)

Pour télécharger et *silencieux* installer la dernière version de l’application de bureau Dynamic Media Classic Adobe sur macOS :

1. Désinstallez toutes les anciennes versions d’application de bureau Dynamic Media Classic sur votre système.

1. Téléchargez le dernier programme d’installation pour l’application de bureau Dynamic Media Classic Adobe pour macOS.

   * [macOS (.DMG) - Télécharger](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)

1. Montez l&#39;image de disque (.DMG) téléchargée à un emplacement de point de montage à l&#39;aide de la commande suivante :

   `hdiutil attach adobe-dynamic-media-classic-20.21.2.dmg -mountpoint <mount_point_path>`

1. Copiez le fichier .APP dans **[!UICONTROL Applications]** à l’aide de la commande suivante :

   `rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
Unmount DMG - hdiutil detach <mount_point_path>`

1. Lorsque vous ouvrez l’application, la nouvelle page de connexion à l’Adobe Dynamic Media Classic s’affiche :

   ![Connexion Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Pour vous connecter à l’application de bureau Dynamic Media Classic Adobe, utilisez les mêmes informations d’identification que celles utilisées pour vous connecter à Dynamic Media Classic dans le navigateur.

   Pour que le **[!UICONTROL serveur]** puisse être utilisé, consultez le mappage suivant pour l&#39;environnement de production :

   | URL du navigateur | Nom du serveur d’applications de bureau |
   |---|---|
   | https://s7sps1.scene7.com/ | Production de NA (Amérique du Nord) |
   | https://s7sps3.scene7.com/ | Production EMEA (Europe, Moyen-Orient et Afrique) |
   | https://s7sps5.scene7.com/ | Production d&#39;APAC (Asie-Pacifique) |

## Téléchargez et *silencieuse* installez la dernière application de bureau Dynamic Media Classic Adobe sous Windows® {#install-silent-windows-dmc-app}.

La commande que vous utilisez est destinée à une installation silencieuse MSI de base. Cependant, le programme d’installation de l’application de bureau Dynamic Media Classic est un programme d’installation MSI InstallScript créé à l’aide d’InstallShield. Lorsque vous exécutez le programme d’installation en mode d’enregistrement, toute interaction utilisateur est enregistrée dans un fichier de réponse. Ce fichier de réponse est ensuite utilisé pour une installation silencieuse, comme décrit dans [Exécution d&#39;installations en mode silencieux.](https://docs.revenera.com/installshield19helplib/helplibrary/SilentInstall.htm)

Voir aussi:

* [Téléchargement et installation de la dernière application de bureau Adobe Dynamic Media Classic sous Mac ou Windows®](#installation-dmc-app)
* [Téléchargement et installation silencieuse de la dernière application de bureau Dynamic Media Classic Adobe sur macOS](#install-silent-mac-dmc-app)

Pour télécharger et *silencieux* installer la dernière version de l’application de bureau Dynamic Media Classic Adobe sous Windows® :

1. Désinstallez toutes les anciennes versions d’application de bureau Dynamic Media Classic sur votre système.

1. Téléchargez le dernier programme d’installation de l’application de bureau Adobe Dynamic Media Classic.

   * [Windows® (.EXE) - Télécharger](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe)

1. Exécutez le programme d’installation en mode enregistrement à l’aide de la commande suivante :

   `adobe-dynamic-media-classic-20.21.2.exe /r /f1"C:\Setup.iss"`

1. Dans la fenêtre du programme d’installation de l’interface utilisateur graphique, suivez les étapes pour installer de sorte que les interactions/entrées, telles que l’emplacement d’installation, soient enregistrées dans le fichier `Setup.iss`.

1. Copiez le fichier `Setup.iss` et `adobe-dynamic-media-classic-20.21.2.exe` créé sur un autre ordinateur.

1. Exécutez la commande suivante pour une installation silencieuse :

   `adobe-dynamic-media-classic-20.21.2.exe /s /f1"C:\Setup.iss"`

   Pour plus d&#39;informations sur les paramètres de ligne de commande, consultez les sections [Setup.exe et Paramètres de ligne de commande Update.exe.](https://docs.revenera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. Lorsque vous ouvrez l’application, la nouvelle page de connexion à l’Adobe Dynamic Media Classic s’affiche :

   ![Connexion Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Pour vous connecter à l’application de bureau Dynamic Media Classic Adobe, utilisez les mêmes informations d’identification que celles utilisées pour vous connecter à Dynamic Media Classic dans le navigateur.

   Pour que le **[!UICONTROL serveur]** puisse être utilisé, consultez le mappage suivant pour l&#39;environnement de production :

   | URL du navigateur | Nom du serveur d’applications de bureau |
   |---|---|
   | https://s7sps1.scene7.com/ | Production de NA (Amérique du Nord) |
   | https://s7sps3.scene7.com/ | Production EMEA (Europe, Moyen-Orient et Afrique) |
   | https://s7sps5.scene7.com/ | Production d&#39;APAC (Asie-Pacifique) |


## Présentation vidéo de l’utilisation de l’application de bureau Dynamic Media Classic {#dmc-app-video-walk-through}

Regardez une présentation [vidéo sur l’utilisation de l’application de bureau Dynamic Media Classic](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media) (durée : 2 minutes 36 secondes).

## Effacement du cache d&#39;image et du cache de ressources sur votre ordinateur à l&#39;aide de l&#39;application de bureau {#clear-cache}

1. Dans l’application de bureau Dynamic Media Classic, près du coin supérieur droit, appuyez sur **[!UICONTROL Configuration]** > **[!UICONTROL Configuration personnelle]**.
1. Sur la page **[!UICONTROL Configuration personnelle]**, sous l&#39;en-tête **[!UICONTROL Bureau]**, effectuez l&#39;une des opérations suivantes :
   * Pour supprimer tous les fichiers d’image mis en cache de Dynamic Media Adobe de votre ordinateur, appuyez sur **[!UICONTROL Effacer le cache d’image]**, puis sur **[!UICONTROL OK]**.
   * Pour supprimer tous les fichiers de ressources mis en cache de Dynamic Media Adobe de votre ordinateur, appuyez sur **[!UICONTROL Effacer le cache de ressources]**, puis sur **[!UICONTROL OK]**.
1. Dans le coin inférieur droit de la page, appuyez sur **[!UICONTROL Fermer]**.

### Suppression manuelle du cache d’images et du cache de ressources

Outre l’effacement du cache d’images et de ressources à l’aide de l’application de bureau, vous pouvez effacer manuellement le cache directement à partir du système de fichiers.

1. En fonction de votre système d’exploitation, accédez aux options suivantes :

   * macOS : `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Limite connue dans Dynamic Media Classic 20.21.1

* La liste déroulante **[!UICONTROL Serveur]** est vide après la mise à jour vers l’application de bureau Dynamic Media Classic 20.21.1 - Scénario : Vous installez et vous connectez à Dynamic Media Classic 20.20.1 ou 20.20.2, puis fermez l’application. Ensuite, vous passez à Dynamic Media Classic 20.21.1. Lorsque vous tentez de vous connecter, la liste déroulante **[!UICONTROL Serveur]** de la boîte de dialogue **[!UICONTROL Se connecter à votre compte]** est vide. Pour résoudre ce problème, vous devez [effacer manuellement le cache](#clear-cache) (voir les étapes ci-dessus).

## Limites connues dans Dynamic Media Classic 20.20.1 (fixées dans la version 20.20.2)

**_S’applique uniquement à Windows® : le nombre de fichiers pouvant être téléchargés via l’interface utilisateur de l’application de bureau est-il limité ?_**<br>Oui, un maximum de 150 fichiers peuvent être téléchargés à la fois via l’interface utilisateur de l’application de bureau.

**_Application pour Windows® et macOS - Comment puis-je passer d’une société à l’autre ?_**<br>Pour passer d’une société à l’autre, procédez comme suit :

* Dans l’application Dynamic Media Classic, sélectionnez la nouvelle société dans la liste déroulante société.
* Lorsque la fenêtre contextuelle s’affiche, appuyez sur **[!UICONTROL OK]** pour vous déconnecter et fermer l’application.

   ![Pour utiliser la nouvelle société, redémarrez l’application.](/help/assets/dmclassic-new-company1.png)

* Redémarrez Dynamic Media Classic, puis connectez-vous comme d’habitude pour utiliser la nouvelle société.

## Conseils et astuces

**_Je ne peux pas voir le panneau Panier sur le landing page de Dynamic Media Classic._**<br>Dans Dynamic Media Classic, appuyez sur**[!UICONTROL Configuration > Configuration ]**personnelle. Dans la section Navigateur, vérifiez que**[!UICONTROL Afficher les fonctionnalités MediaPortal ]**est sélectionné (coché). Appuyez sur**[!UICONTROL Enregistrer > Fermer ]**.

**_L’état de publication (indicateur vert) d’une ressource n’est pas reflété correctement._**<br>Dans l’interface utilisateur du navigateur, une nouvelle connexion à l’interface utilisateur était nécessaire pour afficher l’état de publication correct des ressources. Dans l’application de bureau, l’Adobe a introduit une icône**[!UICONTROL Actualiser ]**dans la barre d’outils, à droite du bouton**[!UICONTROL Sélectionner aucun ]**. Appuyez sur l’icône**[!UICONTROL Actualiser ]**pour afficher le dernier état de toutes les ressources sur la page donnée. Aucune nouvelle connexion n’est requise, comme dans l’interface utilisateur du navigateur.

![Actualiser ](/help/assets/refresh-icon1.png)
*l&#39;icôneActualiser l&#39;icône*

**_Je ne vois pas les paramètres prédéfinis d’ensemble par lot fonctionner dans l’application de bureau._**<br>Appuyez sur**[!UICONTROL Télécharger > Options tâche > Paramètres prédéfinis ]**d’ensemble par lot. Vérifiez que le**[!UICONTROL paramètre prédéfini d’ensemble par lot ]**approprié est activé. Cliquez sur**[!UICONTROL Enregistrer et envoyer le transfert ]**.
