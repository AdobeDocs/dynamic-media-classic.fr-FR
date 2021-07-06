---
title: Application de bureau Adobe Dynamic Media Classic - Maintenant disponible
description: En savoir plus sur l’application de bureau Dynamic Media Classic.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
source-git-commit: 9ff171590c65f55cef8c9e5a2b4e77ddbbfa6895
workflow-type: tm+mt
source-wordcount: '1850'
ht-degree: 1%

---

# Maintenant disponible : Application de bureau Adobe Dynamic Media Classic {#dynamic-media-classic-desktop-app}

Les utilisateurs de Dynamic Media Classic ont désormais accès à une nouvelle expérience de l’appli de bureau qui ne repose plus sur la technologie de Flash d’Adobe dans le navigateur.

Cette nouvelle application est désormais disponible pour Windows® et macOS.

>[!IMPORTANT]
>
>Adobe vous recommande d’installer la nouvelle appli de bureau Dynamic Media Classic Adobe d’ici le 1er octobre 2020. Cela vous assurera une transition en douceur avant que le Flash Player Adobe ne soit abandonné le 31 décembre 2020. Après cette date, vous ne pourrez plus vous connecter à la version navigateur de l’interface utilisateur d’Adobe Dynamic Media Classic, appelée Dynamic Media Classic dans le produit.

Consultez la FAQ sur la [Nouvelle connexion Dynamic Media Classic désormais disponible.](/help/new-ui-2020.md)

## Configuration requise pour l’appli de bureau Dynamic Media Classic Adobe {#system-requirements-dmc-app}

L’appli de bureau Dynamic Media Classic Adobe est compatible avec les systèmes d’exploitation suivants :

* macOS 10.10 ou version ultérieure.
* Windows® 7 ou version ultérieure.

>[!NOTE]
>
>La notification de mise à niveau dans l’application de bureau Dynamic Media Classic n’est pas générée pour les versions *mineures*. Les clients qui bénéficient de correctifs dans une version mineure peuvent effectuer une mise à niveau.

## Correctifs de la version mineure (20.21.2) {#minor-release}

* Limite connue dans 20.21.1 de la liste déroulante Serveur étant vide.
* Dans **[!UICONTROL Télécharger les options de tâche]**, la valeur par défaut de dénomination des calques sous **[!UICONTROL Options Photoshop]** est désormais **[!UICONTROL Photoshop et nom de couche]**. Les calques du fichier PSD sont téléchargés comme images distinctes.
   * La valeur par défaut précédente de **[!UICONTROL Nom de calque]**, désignait les images en fonction de leur nom de calque ou de leur numéro de calque dans le fichier PSD. Le numéro de calque a été utilisé si les noms de calque dans le fichier PSD étaient des noms de calque Photoshop par défaut.
   * La nouvelle valeur par défaut **[!UICONTROL Photoshop et Nom de calque]**, nomme les images après le fichier PSD suivi du nom du calque ou du numéro de calque. Le numéro de calque est utilisé si le nom des calques dans le fichier PSD est un nom de calque Photoshop par défaut.
   * Étant donné que les images de calque dans Dynamic Media Classic portent désormais des noms uniques, aucune mise à jour du fichier PSD ou des modèles existants ne sera effectuée (ce qui est le cas des noms de calque partagés dans les fichiers PSD d’origine).
* Miniatures des ressources endommagées.

## Correctifs de la dernière version (20.21.1) {#latest-fixes-desktop-app}

* Problèmes de connexion en raison d’un délai d’expiration, qui entraînent le message suivant : *Cet utilisateur peut être affecté au groupe ou aux groupes sans autorisation. Contactez votre administrateur.*
* Les paramètres prédéfinis de la visionneuse sont dupliqués à chaque tentative de mot de passe incorrect.
* L’application de bureau ne répond plus en raison de la présence de nombreuses ressources dans le dossier racine. (Corrigé sous Windows®; fonctionne comme vous le souhaitez sur macOS.)

## Correctifs de la version précédente (20.20.2) {#previous-version-fixes-desktop-app}

* Le nombre de fichiers que vous pouvez charger via l’interface utilisateur de l’appli de bureau n’est pas limité pour macOS et Windows®.
* Il n’est pas nécessaire de se déconnecter de l’appli de bureau pour basculer entre les entreprises.
* Ctrl+V pour l’opération de collage fonctionne désormais sous Windows®.
* À l’avenir, lorsqu’une nouvelle version de l’appli de bureau sera publiée, les utilisateurs seront avertis dans l’appli de bureau elle-même.

## Téléchargez et installez la dernière application de bureau Dynamic Media Classic Adobe sous macOS ou Windows® {#installation-dmc-app}

Voir aussi:

* [Télécharger et installer en mode silencieux la dernière application de bureau Dynamic Media Classic Adobe sous Mac](#install-silent-mac-dmc-app)
* [Téléchargez et installez en mode silencieux la dernière application de bureau Adobe Dynamic Media Classic sous Windows®](#install-silent-windows-dmc-app)

1. Désinstallez toutes les anciennes versions de l’appli de bureau Dynamic Media Classic de votre système.

1. Téléchargez la dernière version du programme d’installation de l’appli de bureau Dynamic Media Classic Adobe.

   * La dernière version (20.21.2) est disponible à l’adresse suivante :

      * [macOS (.DMG) - Téléchargement](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
      * [Windows® (.EXE) - Téléchargement](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe)
   * La version précédente (20.21.1) est disponible à l’adresse suivante :

      * [macOS (.DMG) - Téléchargement](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.dmg)
      * [Windows® (.EXE) - Téléchargement](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.exe)


<!--         * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. Effectuez l’une des opérations suivantes en fonction du programme d’installation que vous avez téléchargé.

   * **Pour macOS**  - Dans la boîte de dialogue  **[!UICONTROL Faire glisser et déposer vers l’]** installation, faites glisser  **[!UICONTROL Adobe Dynamic Media]** Classic et déposez-le sur  **[!UICONTROL Applications]**.

      ![Installation par glisser-déposer sur macOS](/help/assets/dragondrop-install1.png)

   * Dans le dossier **[!UICONTROL Applications]** , appuyez sur l’icône Adobe Dynamic Media Classic .
   * Dans la boîte de dialogue, appuyez sur **[!UICONTROL Ouvrir]** pour ouvrir l’appli de bureau Dynamic Media Classic Adobe.

      ![Ouvrir l’application téléchargée](/help/assets/open-dmclassicapp1.png)

   * **Pour Windows**  : exécutez le fichier binaire du programme d’installation et suivez les instructions à l’écran pour installer l’appli de bureau .

1. Lorsque vous ouvrez l’application, la nouvelle page de connexion Dynamic Media Classic Adobe s’affiche :

   ![Connexion à Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Pour vous connecter à l’appli de bureau Dynamic Media Classic Adobe, utilisez les mêmes informations d’identification que celles que vous utilisiez pour vous connecter à Dynamic Media Classic dans le navigateur.

   Pour que **[!UICONTROL Serveur]** soit utilisé, voir le mappage suivant pour l’environnement de production :

   | URL du navigateur | Nom du serveur d’applications de bureau |
   |---|---|
   | https://s7sps1.scene7.com/ | Production NA (Amérique du Nord) |
   | https://s7sps3.scene7.com/ | Production EMEA (Europe, Moyen-Orient et Afrique) |
   | https://s7sps5.scene7.com/ | Production APAC (Asie-Pacifique) |

1. Après vous être connecté, notez l’expérience familière de l’interface utilisateur du navigateur. Vous pouvez continuer votre activité Dynamic Media Classic au quotidien comme vous le faites habituellement sur l’appli de bureau .

## Téléchargez et *silencieux* installez la dernière application de bureau Dynamic Media Classic Adobe sous macOS. {#install-silent-mac-dmc-app}

Voir aussi:

* [Téléchargez et installez la dernière application de bureau Dynamic Media Classic Adobe sous Mac ou Windows®](#installation-dmc-app)
* [Téléchargez et installez en mode silencieux la dernière application de bureau Adobe Dynamic Media Classic sous Windows®](#install-silent-windows-dmc-app)

Pour télécharger et *silencieux* installer la dernière version de l’appli de bureau Dynamic Media Classic Adobe sous macOS :

1. Désinstallez toutes les anciennes versions de l’appli de bureau Dynamic Media Classic de votre système.

1. Téléchargez la dernière version du programme d’installation de l’appli de bureau Dynamic Media Classic Adobe pour macOS.

   * [macOS (.DMG) - Téléchargement](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)

1. Montez l’image de disque (.DMG) téléchargée vers un emplacement de point de montage à l’aide de la commande suivante :

   `hdiutil attach adobe-dynamic-media-classic-20.21.2.dmg -mountpoint <mount_point_path>`

1. Copiez le fichier .APP dans **[!UICONTROL Applications]** à l’aide de la commande suivante :

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG - hdiutil detach <mount_point_path>
   ```

1. Lorsque vous ouvrez l’application, la nouvelle page de connexion Dynamic Media Classic Adobe s’affiche :

   ![Connexion à Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Pour vous connecter à l’appli de bureau Dynamic Media Classic Adobe, utilisez les mêmes informations d’identification que celles que vous utilisiez pour vous connecter à Dynamic Media Classic dans le navigateur.

   Pour que **[!UICONTROL Serveur]** soit utilisé, voir le mappage suivant pour l’environnement de production :

   | URL du navigateur | Nom du serveur d’applications de bureau |
   |---|---|
   | https://s7sps1.scene7.com/ | Production NA (Amérique du Nord) |
   | https://s7sps3.scene7.com/ | Production EMEA (Europe, Moyen-Orient et Afrique) |
   | https://s7sps5.scene7.com/ | Production APAC (Asie-Pacifique) |

## Téléchargez et *silencieux* installez la dernière application de bureau Dynamic Media Classic Adobe sous Windows® {#install-silent-windows-dmc-app}

La commande que vous utilisez est pour une installation silencieuse MSI de base. Cependant, le programme d’installation de l’appli de bureau Dynamic Media Classic est un programme d’installation MSI InstallScript créé à l’aide de InstallShield. Lorsque vous exécutez le programme d’installation en mode d’enregistrement, toute interaction utilisateur est enregistrée dans un fichier de réponse. Ce fichier de réponse est ensuite utilisé pour une installation silencieuse, comme décrit dans [Exécution des installations en mode silencieux.](https://docs.revenera.com/installshield19helplib/helplibrary/SilentInstall.htm)

Voir aussi:

* [Téléchargez et installez la dernière application de bureau Dynamic Media Classic Adobe sous Mac ou Windows®](#installation-dmc-app)
* [Télécharger et installer en mode silencieux la dernière application de bureau Adobe Dynamic Media Classic sous macOS](#install-silent-mac-dmc-app)

Pour télécharger et *silencieux* installer la dernière version de l’appli de bureau Dynamic Media Classic Adobe sous Windows® :

1. Désinstallez toutes les anciennes versions de l’appli de bureau Dynamic Media Classic de votre système.

1. Téléchargez la dernière version du programme d’installation de l’appli de bureau Dynamic Media Classic Adobe.

   * [Windows® (.EXE) - Téléchargement](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe)

1. Exécutez le programme d’installation en mode d’enregistrement à l’aide de la commande suivante :

   `adobe-dynamic-media-classic-20.21.2.exe /r /f1"C:\Setup.iss"`

1. Dans la fenêtre du programme d’installation de l’interface utilisateur graphique, suivez les étapes à suivre pour que les interactions/entrées, comme l’emplacement d’installation, soient enregistrées dans le fichier `Setup.iss`.

1. Copiez le fichier `Setup.iss` créé et `adobe-dynamic-media-classic-20.21.2.exe` sur un autre ordinateur.

1. Exécutez la commande suivante pour une installation silencieuse :

   `adobe-dynamic-media-classic-20.21.2.exe /s /f1"C:\Setup.iss"`

   Vous trouverez des informations détaillées sur les paramètres de ligne de commande à l’adresse [Setup.exe et Update.exe Paramètres de ligne de commande.](https://docs.revenera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. Lorsque vous ouvrez l’application, la nouvelle page de connexion Dynamic Media Classic Adobe s’affiche :

   ![Connexion à Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Pour vous connecter à l’appli de bureau Dynamic Media Classic Adobe, utilisez les mêmes informations d’identification que celles que vous utilisiez pour vous connecter à Dynamic Media Classic dans le navigateur.

   Pour que **[!UICONTROL Serveur]** soit utilisé, voir le mappage suivant pour l’environnement de production :

   | URL du navigateur | Nom du serveur d’applications de bureau |
   |---|---|
   | https://s7sps1.scene7.com/ | Production NA (Amérique du Nord) |
   | https://s7sps3.scene7.com/ | Production EMEA (Europe, Moyen-Orient et Afrique) |
   | https://s7sps5.scene7.com/ | Production APAC (Asie-Pacifique) |


## Présentation vidéo de l’utilisation de l’application de bureau Dynamic Media Classic {#dmc-app-video-walk-through}

Regardez une [présentation vidéo sur l’utilisation de l’application de bureau Dynamic Media Classic](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media) (Longueur : 2 minutes 36 secondes).

## Effacement du cache des images et du cache des ressources sur votre ordinateur à l’aide de l’appli de bureau {#clear-cache}

1. Dans l’appli de bureau Dynamic Media Classic, près du coin supérieur droit, appuyez sur **[!UICONTROL Configuration]** > **[!UICONTROL Configuration personnelle]**.
1. Sur la page **[!UICONTROL Configuration personnelle]**, sous l’en-tête **[!UICONTROL Bureau]**, effectuez l’une des opérations suivantes :
   * Pour supprimer tous les fichiers image mis en cache par Adobe Dynamic Media de votre ordinateur, appuyez sur **[!UICONTROL Effacer le cache d’image]**, puis appuyez sur **[!UICONTROL OK]**.
   * Pour supprimer tous les fichiers de ressources mis en cache par Adobe Dynamic Media de votre ordinateur, appuyez sur **[!UICONTROL Effacer le cache de ressources]**, puis appuyez sur **[!UICONTROL OK]**.
1. Dans le coin inférieur droit de la page, appuyez sur **[!UICONTROL Fermer]**.

### Effacement manuel du cache d’image et du cache de ressources

Outre l’effacement de l’image et du cache des ressources à l’aide de l’appli de bureau, vous pouvez effacer manuellement le cache directement à partir du système de fichiers.

1. Selon votre système d’exploitation, accédez aux éléments suivants :

   * macOS : `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Limites connues dans Dynamic Media Classic 20.21.1

* La liste déroulante **[!UICONTROL Serveur]** est vide après la mise à jour vers l’appli de bureau Dynamic Media Classic 20.21.1 - Scénario : Vous installez et vous connectez à Dynamic Media Classic 20.20.1 ou 20.20.2, puis fermez l’application. Ensuite, vous effectuez la mise à jour vers Dynamic Media Classic 20.21.1. Lorsque vous tentez de vous connecter, la liste déroulante **[!UICONTROL Serveur]** de la boîte de dialogue **[!UICONTROL Se connecter à votre compte]** est vide. Pour contourner ce problème, vous devez [effacer manuellement le cache](#clear-cache) (voir les étapes ci-dessus).

## Limites connues dans Dynamic Media Classic 20.20.1 (corrigées dans 20.20.2)

**_S’applique uniquement à Windows® : y a-t-il une limitation du nombre de fichiers pouvant être chargés via l’interface utilisateur de l’appli de bureau ?_**<br>Oui, vous pouvez charger un maximum de 150 fichiers à la fois au moyen de l’interface utilisateur de l’appli de bureau.

**_S’applique à Windows® et macOS - Comment changer d’entreprise ?_**<br>Pour passer d’une entreprise à l’autre, procédez comme suit :

* Dans l’application Dynamic Media Classic, sélectionnez la nouvelle société dans la liste déroulante Société .
* Lorsque la fenêtre contextuelle s’affiche, appuyez sur **[!UICONTROL OK]** pour vous déconnecter et fermer l’application.

   ![Pour utiliser la nouvelle entreprise, redémarrez l’application.](/help/assets/dmclassic-new-company1.png)

* Redémarrez Dynamic Media Classic, puis connectez-vous comme d’habitude pour travailler avec la nouvelle société.

## Conseils et astuces

**_Je ne parviens pas à voir le panneau Panier multimédia sur la page d’entrée de Dynamic Media Classic._**<br>Dans Dynamic Media Classic, appuyez sur**[!UICONTROL Configuration > Configuration personnelle ]**. Dans la section Navigateur , assurez-vous que l’option**[!UICONTROL Afficher les fonctionnalités MediaPortal ]**est sélectionnée (cochée). Appuyez sur**[!UICONTROL Enregistrer > Fermer ]**.

**_L’état de publication (indicateur vert) d’une ressource n’est pas correctement reflété._**<br>Dans l’interface utilisateur du navigateur, une nouvelle connexion à l’interface utilisateur était nécessaire pour afficher l’état de publication correct des ressources. Dans l’appli de bureau, Adobe a introduit une icône**[!UICONTROL Actualiser ]**dans la barre d’outils, à droite du bouton**[!UICONTROL Sélectionner Aucun ]**. Appuyez sur l’icône**[!UICONTROL Actualiser ]**pour afficher le dernier état de toutes les ressources sur la page donnée. Aucune nouvelle connexion n’est requise, comme avec l’interface utilisateur du navigateur.

![Icône Actualiser ](/help/assets/refresh-icon1.png)
*Icône Actualiser*

**_Je ne vois pas les paramètres prédéfinis d’ensemble par lot fonctionner dans l’appli de bureau ._**<br>Appuyez sur**[!UICONTROL Upload > Job Options > Batch Set Presets ]**(Télécharger > Options de tâche > Paramètres prédéfinis d’ensemble par lot). Vérifiez que le**[!UICONTROL paramètre prédéfini d’ensemble par lot ]**approprié est activé. Cliquez sur**[!UICONTROL Enregistrer et envoyer le chargement ]**.
