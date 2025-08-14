---
title: Adobe Dynamic Media Classic Desktop
description: En savoir plus sur l’application de bureau Adobe Dynamic Media Classic désormais disponible.
contentOwner: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
topic: Administration
level: Intermediate
source-git-commit: afc347201b13c3b91ec5e1bd3ac5304442772f8d
workflow-type: tm+mt
source-wordcount: '1994'
ht-degree: 0%

---

# Disponible maintenant : appli de bureau Adobe Dynamic Media Classic {#dynamic-media-classic-desktop-app}

Les utilisateurs d’Adobe Dynamic Media Classic ont désormais accès à une nouvelle expérience d’application de bureau qui ne repose plus sur la technologie Adobe Flash dans le navigateur.

Cette nouvelle application est désormais disponible pour Windows® et macOS.

>[!IMPORTANT]
>
>Adobe vous recommande d’installer la nouvelle application de bureau Adobe Dynamic Media Classic d’ici le 1er octobre 2020. Vous aurez ainsi une transition en douceur avant l’abandon d’Adobe Flash Player le 31 décembre 2020. Passée cette date, vous ne pouvez pas vous connecter à la version du navigateur de l’interface utilisateur d’Adobe Dynamic Media Classic, étiquetée comme Adobe Dynamic Media Classic dans le produit .

Voir la FAQ pour la [Nouvelle connexion à Adobe Dynamic Media Classic maintenant disponible.](/help/using/new-ui-2020.md)

## Configuration requise pour l’application de bureau Adobe Dynamic Media Classic {#system-requirements-dmc-app}

L’application de bureau Adobe Dynamic Media Classic est compatible avec les systèmes d’exploitation suivants :

* macOS 10.10 ou version ultérieure.
* Windows® 7 ou version ultérieure.

Consultez la configuration requise complète dans [Configuration requise pour l’application de bureau Adobe Dynamic Media Classic](/help/using/system-requirements.md).

La notification de mise à niveau dans l’application de bureau Adobe Dynamic Media Classic n’est pas générée pour les versions *mineures*. Les clients qui bénéficient de correctifs dans une version mineure peuvent effectuer une mise à niveau.

## Correction de la dernière version (20.22.2) de macOS uniquement {#release-feb2022}

* macOS Monterey : la page de chargement de fichier est figée lors des chargements suivants. <!-- https://jira.corp.adobe.com/browse/ASSETS-7948 -->

## Correctifs de la dernière version (20.22.1) {#release-jan2022}

* Lors de la modification d’une image, les boutons **[!UICONTROL Enregistrer]** ne fonctionnaient pas.
* Dans les éditeurs de visionneuse, les boutons **[!UICONTROL Fermer]**, **[!UICONTROL Enregistrer]** et **[!UICONTROL Enregistrer sous]** sont désactivés après le défilement des ressources dans le panneau **[!UICONTROL Ajouter Assets]**.
* Le bouton **[!UICONTROL Lecture]** dans la vue Détails de la vidéo ne fonctionnait pas.
* Impossible de saisir `d` et `e` dans les champs **[!UICONTROL Nom d’utilisateur]** et **[!UICONTROL Mot de passe]** lors de l’exécution de macOS Monterey.
* Déplacement des API Analytics restantes vers la version 2.0.

## Correctifs de la version 20.21.3 {#release-sept2021}

* Miniatures endommagées pour les ressources affichées après une période d’inactivité sur l’application de bureau.
* L’application Desktop cesse de répondre, généralement après les opérations Set.
* Activation automatique du mode Demander l’obscurcissement et le verrouillage sous **[!UICONTROL Test de la diffusion d’images]**.

  Voir [Service Secure Testing](/help/using/testing-assets-making-them-public.md#testing-the-secure-testing-service).

* Mise à jour du mécanisme d’authentification avec Adobe Analytics. Pertinent pour les nouvelles intégrations ou si certaines variables Analytics doivent être mises à jour à partir de l’application de bureau Dynamic Media Classic.

  Voir [Connexion à Adobe Analytics](/help/using/log-analytics.md) pour connaître les étapes mises à jour.

## Correctifs de la version 20.21.2 {#minor-release}

* Limites connues dans la version 20.21.1 : la liste déroulante **[!UICONTROL Serveur]** de l’écran de connexion était vide.
* Dans **[!UICONTROL Charger les options de la tâche]**, la valeur par défaut du nom du calque sous **[!UICONTROL Options Photoshop]** est désormais **[!UICONTROL Photoshop et Nom du calque]**. Les calques du fichier PSD sont chargés en tant qu’images distinctes.
   * Valeur par défaut antérieure de **[!UICONTROL Nom de calque]**, nommée les images d’après leur nom de calque ou leur numéro de calque dans le fichier PSD. Le numéro de calque était utilisé si les noms de calque dans le fichier PSD étaient des noms de calque Photoshop par défaut.
   * La nouvelle valeur par défaut, **[!UICONTROL Photoshop et Nom de calque]**, nomme les images d’après le fichier PSD suivi du nom ou du numéro du calque. Le numéro de calque est utilisé si les noms de calque figurant dans le fichier PSD sont des noms de calque Photoshop par défaut.
   * Étant donné que les images de calque dans Adobe Dynamic Media Classic portent désormais des noms uniques, aucune mise à jour de PSD ou de modèles existants ne sera effectuée (c’est-à-dire les noms de calque partagés dans les fichiers PSD d’origine).
* Miniatures des ressources endommagées.

## Correctifs de la version 20.21.1 {#latest-fixes-desktop-app}

* Problèmes de connexion dus à la temporisation. Message suivant : *Cet utilisateur peut être affecté au(x) groupe(s) sans autorisation. Contactez votre administrateur.*
* Les paramètres prédéfinis de la visionneuse sont dupliqués à chaque tentative de mot de passe incorrecte.
* L’application de bureau ne répond plus en raison du grand nombre de ressources dans le dossier racine. (Correctif sous Windows® ; fonctionnant comme vous le souhaitez sur macOS.)

## Correctifs de la version 20.20.2 {#previous-version-fixes-desktop-app}

* Aucune limitation sur le nombre de fichiers que vous pouvez charger via l’interface utilisateur de l’appli de bureau pour macOS et Windows®.
* Il n’est pas nécessaire de se déconnecter de l’application de bureau pour basculer entre les sociétés.
* Ctrl+V pour l’opération de collage fonctionne désormais sous Windows®.
* À l’avenir, lorsqu’une nouvelle version de l’application de bureau sera publiée, les utilisateurs seront avertis dans l’application de bureau elle-même.

## Télécharger et installer la dernière application de bureau Adobe Dynamic Media Classic sous macOS ou Windows® {#installation-dmc-app}

Voir également :

* [Télécharger et installer silencieusement la dernière application de bureau Adobe Dynamic Media Classic sur Mac](#install-silent-mac-dmc-app)
* [Télécharger et installer silencieusement la dernière application de bureau Adobe Dynamic Media Classic sous Windows](#install-silent-windows-dmc-app)

1. Désinstallez toutes les anciennes versions de l’application de bureau Adobe Dynamic Media Classic sur votre système.

1. Téléchargez le dernier programme d’installation de l’application de bureau Adobe Dynamic Media Classic.

   * La dernière version est disponible à l’adresse suivante :

      * [macOS (.DMG) : Télécharger](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)
      * [Windows (.EXE) : Télécharger](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

   * La version précédente est disponible à l’adresse suivante :

      * [macOS (.DMG) : Télécharger](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [Windows® (.EXE) : Télécharger](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)

<!--         * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg) -->

<!--    * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows&reg; (.EXE): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) -->

<!--    * [macOS (.DMG): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. Effectuez l’une des opérations suivantes en fonction du programme d’installation que vous avez téléchargé.

   * **macOS** - Dans la boîte de dialogue **[!UICONTROL Glisser-déposer pour installer]**, faites glisser **[!UICONTROL Adobe Dynamic Media Classic]** et déposez-le sur **[!UICONTROL Applications]**.

     ![Installation par glisser-déposer sur macOS](/help/using/assets/dragondrop-install1.png)

   * Dans le dossier **[!UICONTROL Applications]**, appuyez sur l’icône Adobe Dynamic Media Classic.
   * Dans la boîte de dialogue, appuyez sur **[!UICONTROL Ouvrir]** pour ouvrir l’application de bureau Adobe Dynamic Media Classic.

     ![Ouvrir l’application téléchargée](/help/using/assets/open-dmclassicapp1.png)

   * **Windows** - Exécutez le fichier binaire du programme d’installation et suivez les instructions à l’écran pour installer l’application de bureau.

1. Lorsque vous ouvrez l’application, la nouvelle page de connexion d’Adobe Dynamic Media Classic s’affiche :

   ![Connexion à Adobe Dynamic Media Classic](/help/using/assets/dmclassic-login1.png)

1. Pour vous connecter à l’application de bureau Adobe Dynamic Media Classic, utilisez les mêmes informations d’identification que celles que vous avez utilisées pour vous connecter à Adobe Dynamic Media Classic dans le navigateur.

   Pour que le **[!UICONTROL Serveur]** à utiliser, consultez le mappage suivant pour l’environnement de production :

   | Serveur | URL du navigateur |
   | --- | --- |
   | Production de NA (Amérique du Nord) | https://s7sps1.scene7.com/ |
   | EMEA Production (Europe, Moyen-Orient et Afrique) | https://s7sps3.scene7.com/ |
   | Production APAC (Asie-Pacifique) | https://s7sps5.scene7.com/ |

1. Après vous être connecté, remarquez l’expérience familière de l’interface utilisateur du navigateur. Vous pouvez continuer votre activité quotidienne Adobe Dynamic Media Classic comme vous le faites habituellement sur l’application de bureau.

## Télécharger et installer *silencieusement* dernière application de bureau Adobe Dynamic Media Classic sur macOS {#install-silent-mac-dmc-app}

Voir également :

* [Télécharger et installer la dernière application de bureau Adobe Dynamic Media Classic sous Mac ou Windows](#installation-dmc-app)
* [Télécharger et installer silencieusement la dernière application de bureau Adobe Dynamic Media Classic sous Windows](#install-silent-windows-dmc-app)

Pour télécharger et *silencieusement* installez la dernière version de l’application de bureau Adobe Dynamic Media Classic sur macOS :

1. Désinstallez toutes les anciennes versions de l’application de bureau Adobe Dynamic Media Classic sur votre système.

1. Téléchargez le dernier programme d’installation de l’application de bureau Adobe Dynamic Media Classic pour macOS.

   * [macOS (.DMG) : Télécharger](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)

1. Montez l’image disque téléchargée (.DMG) à un emplacement de point de montage à l’aide de la commande suivante :

   `hdiutil attach adobe-dynamic-media-classic-20.22.2.dmg -mountpoint <mount_point_path>`

1. Copiez le fichier .APP dans **[!UICONTROL Applications]** à l’aide de la commande suivante :

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG: hdiutil detach <mount_point_path>
   ```

1. Lorsque vous ouvrez l’application, la nouvelle page de connexion d’Adobe Dynamic Media Classic s’affiche :

   ![Connexion à Adobe Dynamic Media Classic](/help/using/assets/dmclassic-login1.png)

1. Pour vous connecter à l’application de bureau Adobe Dynamic Media Classic, utilisez les mêmes informations d’identification que celles que vous avez utilisées pour vous connecter à Adobe Dynamic Media Classic dans le navigateur.

   Pour que le **[!UICONTROL Serveur]** à utiliser, consultez le mappage suivant pour l’environnement de production :

   | Serveur | URL du navigateur |
   | --- | --- |
   | Production de NA (Amérique du Nord) | https://s7sps1.scene7.com/ |
   | EMEA Production (Europe, Moyen-Orient et Afrique) | https://s7sps3.scene7.com/ |
   | Production APAC (Asie-Pacifique) | https://s7sps5.scene7.com/ |

## Téléchargez et *silencieusement* installez la dernière application de bureau Adobe Dynamic Media Classic sous Windows® {#install-silent-windows-dmc-app}

La commande que vous utilisez est destinée à une installation silencieuse MSI de base. Cependant, le programme d’installation de l’appli de bureau Adobe Dynamic Media Classic est un programme d’installation MSI InstallScript créé à l’aide d’InstallShield. Lorsque vous exécutez le programme d’installation en mode d’enregistrement, toute interaction de l’utilisateur est enregistrée dans un fichier de réponse. Ce fichier de réponse est ensuite utilisé pour une installation silencieuse, comme décrit dans la section [Exécution d’installations en mode silencieux](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/SilentInstall.htm).

Voir également :

* [Télécharger et installer la dernière application de bureau Adobe Dynamic Media Classic sous Mac ou Windows](#installation-dmc-app)

* [Télécharger et installer silencieusement la dernière application de bureau Adobe Dynamic Media Classic sur macOS](#install-silent-mac-dmc-app)

Pour télécharger et *silencieusement* installez la dernière version de l’application de bureau Adobe Dynamic Media Classic sous Windows® :

1. Désinstallez toutes les anciennes versions de l’application de bureau Adobe Dynamic Media Classic sur votre système.

1. Téléchargez le dernier programme d’installation de l’application de bureau Adobe Dynamic Media Classic.

   * [Windows® (.EXE) : Télécharger](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. Exécutez le programme d’installation en mode d’enregistrement à l’aide de la commande suivante :

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. Dans la fenêtre du programme d’installation de l’interface utilisateur graphique, suivez les étapes d’installation afin que les interactions/entrées, comme l’emplacement d’installation, soient enregistrées dans `Setup.iss` fichier .

1. Copiez le fichier `Setup.iss` et le `adobe-dynamic-media-classic-20.22.1.exe` créés sur un autre ordinateur.

1. Exécutez la commande suivante pour une installation en mode silencieux :

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   Vous trouverez des informations détaillées sur les paramètres de ligne de commande aux adresses [Setup.exe et Update.exe](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/IHelpSetup_EXECmdLine.htm?Highlight=Setup.exe%20and%20Update.exe%20Command-Line%20Parameters).

1. Lorsque vous ouvrez l’application, la nouvelle page de connexion d’Adobe Dynamic Media Classic s’affiche :

   ![Connexion à Adobe Dynamic Media Classic](/help/using/assets/dmclassic-login1.png)

1. Pour vous connecter à l’application de bureau Adobe Dynamic Media Classic, utilisez les mêmes informations d’identification que celles que vous avez utilisées pour vous connecter à Adobe Dynamic Media Classic dans le navigateur.

   Pour que le **[!UICONTROL Serveur]** à utiliser, consultez le mappage suivant pour l’environnement de production :

   | Serveur | URL du navigateur |
   | --- | --- |
   | Production de NA (Amérique du Nord) | https://s7sps1.scene7.com/ |
   | EMEA Production (Europe, Moyen-Orient et Afrique) | https://s7sps3.scene7.com/ |
   | Production APAC (Asie-Pacifique) | https://s7sps5.scene7.com/ |

## Présentation vidéo sur l’utilisation de l’application de bureau Adobe Dynamic Media Classic {#dmc-app-video-walk-through}

Regardez une [présentation vidéo sur l’utilisation de l’application de bureau Adobe Dynamic Media Classic](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application#dynamic-media) (durée : 2 minutes 36 secondes).

## Effacement du cache d’images et du cache de ressources sur votre ordinateur à l’aide de l’application de bureau {#clear-cache}

1. Dans l’application de bureau Adobe Dynamic Media Classic, près du coin supérieur droit, appuyez sur **[!UICONTROL Configuration]** > **[!UICONTROL Configuration personnelle]**.
1. Sur la page **[!UICONTROL Configuration personnelle]**, sous l’en-tête **[!UICONTROL Bureau]**, effectuez l’une des opérations suivantes :
   * Pour supprimer tous les fichiers image Adobe Dynamic Media mis en cache sur votre ordinateur, appuyez sur **[!UICONTROL Effacer le cache d’image]** puis sur **[!UICONTROL OK]**.
   * Pour supprimer tous les fichiers de ressources Adobe Dynamic Media mis en cache sur votre ordinateur, appuyez sur **[!UICONTROL Effacer le cache de ressources]** puis sur **[!UICONTROL OK]**.
1. Dans le coin inférieur droit de la page, appuyez sur **[!UICONTROL Fermer]**.

### Effacement manuel du cache d’images et du cache de ressources

Outre l’effacement de l’image et du cache de ressources à l’aide de l’application de bureau , vous pouvez effacer manuellement le cache directement à partir du système de fichiers.

1. En fonction de votre système d’exploitation, accédez aux éléments suivants :

   * MACOS : `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows® : `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Limites connues dans Adobe Dynamic Media Classic 20.21.1

* La liste déroulante **[!UICONTROL Serveur]** est vide après la mise à jour vers l’application de bureau Adobe Dynamic Media Classic 20.21.1 : scénario : vous installez et vous connectez à Adobe Dynamic Media Classic 20.20.1 ou 20.20.2, puis fermez l’application. Vous passez ensuite à la version Adobe Dynamic Media Classic 20.21.1. Lorsque vous tentez de vous connecter, la liste déroulante **[!UICONTROL Serveur]** de la boîte de dialogue **[!UICONTROL Connexion à votre compte]** est vide. Pour contourner ce problème, vous devez [effacer manuellement le cache](#clear-cache) (voir les étapes ci-dessus).

## Limites connues d’Adobe Dynamic Media Classic 20.20.1 (corrigées dans la version 20.20.2)

**_S’applique uniquement à Windows® - Existe-t-il une limitation du nombre de fichiers pouvant être chargés via l’interface utilisateur de l’application de bureau ?_**<br>Oui, un maximum de 150 fichiers peuvent être chargés à la fois à l’aide de l’interface utilisateur de l’appli de bureau.

**_S’applique à Windows® et macOS - Comment changer de société ?_**<br>Pour changer de société, procédez comme suit :

* Dans l’application Adobe Dynamic Media Classic, sélectionnez la nouvelle société dans la liste déroulante.
* Lorsque la fenêtre pop-up s’affiche, appuyez sur **[!UICONTROL OK]** pour vous déconnecter et fermer l’application.

  ![Pour utiliser la nouvelle entreprise, redémarrez l’application](/help/using/assets/dmclassic-new-company1.png)

* Redémarrez Adobe Dynamic Media Classic, puis connectez-vous comme d’habitude pour travailler avec la nouvelle entreprise.

## Conseils et astuces

**_Je ne parviens pas à voir le panneau Panier de médias sur la page de destination d’Adobe Dynamic Media Classic._**<br>Dans Adobe Dynamic Media Classic, appuyez sur&#x200B;**[!UICONTROL Configuration > Configuration personnelle &#x200B;]**. Dans la section Navigateur , assurez-vous que&#x200B;**[!UICONTROL Afficher les fonctionnalités de MediaPortal &#x200B;]**&#x200B;est sélectionné (coché). Appuyez sur&#x200B;**[!UICONTROL Enregistrer > Fermer &#x200B;]**.

**_L’état de publication (indicateur vert) d’une ressource n’est pas correctement reflété._**<br>Dans l’interface utilisateur du navigateur, une nouvelle connexion à l’interface utilisateur était nécessaire pour afficher le statut de publication correct des ressources. Dans l’application de bureau, Adobe a introduit une icône&#x200B;**[!UICONTROL Actualiser &#x200B;]**&#x200B;dans la barre d’outils, à droite du bouton&#x200B;**[!UICONTROL Ne rien sélectionner &#x200B;]**. Appuyez sur l’icône&#x200B;**[!UICONTROL Actualiser &#x200B;]**&#x200B;pour afficher le dernier statut de toutes les ressources sur la page donnée. Aucune nouvelle connexion n’est requise comme avec l’interface utilisateur du navigateur.

![Icône Actualiser](/help/using/assets/refresh-icon1.png)
*Icône Actualiser*

**_Je ne vois pas les paramètres prédéfinis de lot qui fonctionnent dans l’application de bureau._**<br>Appuyez sur&#x200B;**[!UICONTROL Charger > Options de tâche > Paramètres prédéfinis de lot &#x200B;]**. Assurez-vous que le&#x200B;**[!UICONTROL paramètre prédéfini de lot &#x200B;]**&#x200B;approprié est activé. Cliquez sur&#x200B;**[!UICONTROL Enregistrer et soumettre le chargement &#x200B;]**.
