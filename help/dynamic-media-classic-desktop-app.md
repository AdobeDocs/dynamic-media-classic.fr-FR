---
title: Application de bureau Adobe Dynamic Media Classic - Maintenant disponible
description: En savoir plus sur l’application de bureau Adobe Dynamic Media Classic.
contentOwner: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
source-git-commit: f0c02d40a1a84e52b25d1c4558958af970859a07
workflow-type: tm+mt
source-wordcount: '2025'
ht-degree: 1%

---

# Maintenant disponible : Application de bureau Adobe Dynamic Media Classic {#dynamic-media-classic-desktop-app}

Les utilisateurs d’Adobe Dynamic Media Classic ont désormais accès à une nouvelle expérience de l’appli de bureau qui ne repose plus sur la technologie de Flash d’Adobe dans le navigateur.

Cette nouvelle application est désormais disponible pour Windows® et macOS.

>[!IMPORTANT]
>
>Adobe vous recommande d’installer la nouvelle appli de bureau Adobe Dynamic Media Classic d’ici au 1er octobre 2020. Cela vous assurera une transition en douceur avant que le Flash Player Adobe ne soit abandonné le 31 décembre 2020. Après cette date, vous ne pourrez plus vous connecter à la version de navigateur de l’interface utilisateur d’Adobe Dynamic Media Classic, appelée Adobe Dynamic Media Classic dans le produit.

Consultez la FAQ pour [Nouvelle expérience de connexion à Adobe Dynamic Media Classic désormais disponible.](/help/new-ui-2020.md)

## Configuration requise pour l’appli de bureau Adobe Dynamic Media Classic {#system-requirements-dmc-app}

L’appli de bureau Adobe Dynamic Media Classic est compatible avec les systèmes d’exploitation suivants :

* macOS 10.10 ou version ultérieure.

   >[!NOTE]
   >
   >L’appli de bureau Dynamic Media Classic voit sa fonctionnalité dégradée lorsqu’elle est utilisée avec macOS Monterey. Par conséquent, Adobe travaille à la publication d’une nouvelle version de l’appli de bureau dans les semaines à venir.

* Windows® 7 ou version ultérieure.

La notification de mise à niveau dans l’application de bureau Adobe Dynamic Media Classic n’est pas générée pour *mineur* versions. Les clients qui bénéficient de correctifs dans une version mineure peuvent effectuer une mise à niveau.

## Correctifs de la dernière version (20.22.1) {#release-jan2022}

* Modification des images **[!UICONTROL Enregistrer]** Les boutons n’étaient pas fonctionnels.
* Dans les éditeurs de visionneuse, la variable **[!UICONTROL Fermer]**, **[!UICONTROL Enregistrer]**, et **[!UICONTROL Enregistrer sous]** les boutons deviennent désactivés après avoir fait défiler les ressources dans la **[!UICONTROL Ajouter des ressources]** du panneau.
* **[!UICONTROL Play]** ne fonctionnait pas dans la vue Détails de la vidéo.
* Impossible de saisir `d` et `e` in **[!UICONTROL Nom d’utilisateur]** et **[!UICONTROL Mot de passe]** lors de l’exécution de macOS Monterey.
* Déplacement des API d’analyse restantes vers la version 2.0.

## Correctifs de la version 20.21.3 {#release-sept2021}

* Vignettes endommagées pour les ressources affichées après une période d’inactivité sur l’appli de bureau.
* L’appli de bureau cesse de répondre, généralement après les opérations Set .
* Activation automatique de l’obscurcissement et du mode de verrouillage des demandes sous **[!UICONTROL Test de la diffusion d’images]**.

   Voir [Test du service Secure Testing](/help/testing-assets-making-them-public.md#testing-the-secure-testing-service).

* Mise à jour du mécanisme d’authentification avec Adobe Analytics. Convient aux nouvelles intégrations ou si certaines variables Analytics doivent être mises à jour dans l’appli de bureau Dynamic Media Classic.

   Voir [Connexion à Adobe Analytics](/help/log-analytics.md) pour les étapes mises à jour.

## Correctifs de la version 20.21.2 {#minor-release}

* Limites connues en 20.21.1 : la valeur **[!UICONTROL Serveur]** La liste déroulante de l’écran de connexion était vide.
* Dans **[!UICONTROL Télécharger les options de la tâche]**, valeur par défaut du nommage de calque sous **[!UICONTROL Options Photoshop]**, est maintenant **[!UICONTROL Photoshop et nom de calque]**. Les calques du fichier PSD sont téléchargés comme images distinctes.
   * La valeur par défaut précédente de **[!UICONTROL Nom du calque]**, nommé les images en fonction de leur nom de calque ou de leur numéro de calque dans le fichier de PSD. Le numéro de calque a été utilisé si les noms de calque dans le fichier de PSD étaient des noms de calque Photoshop par défaut.
   * La nouvelle valeur par défaut de **[!UICONTROL Photoshop et nom de calque]**, nomme les images après le fichier de PSD suivi du nom du calque ou du numéro du calque. Le numéro de calque est utilisé si le nom des calques dans le fichier PSD est un nom de calque Photoshop par défaut.
   * Étant donné que les images de calque dans Adobe Dynamic Media Classic portent désormais des noms uniques, aucune mise à jour du PSD ou des modèles existants ne sera effectuée (ce qui est le cas des noms de calque partagés dans les fichiers de PSD d’origine).
* Miniatures des ressources endommagées.

## Correctifs de la version 20.21.1 {#latest-fixes-desktop-app}

* Problèmes de connexion en raison d’un délai d’expiration, qui entraînent le message suivant : *Cet utilisateur peut être affecté au ou aux groupes sans autorisation. Contactez votre administrateur.*
* Les paramètres prédéfinis de la visionneuse sont dupliqués à chaque tentative de mot de passe incorrect.
* L’application de bureau ne répond plus en raison de la présence de nombreuses ressources dans le dossier racine. (Corrigé sous Windows®; en fonction de vos besoins sur macOS.)

## Correctifs de la version 20.20.2 {#previous-version-fixes-desktop-app}

* Le nombre de fichiers que vous pouvez charger via l’interface utilisateur de l’appli de bureau n’est pas limité pour macOS et Windows®.
* Il n’est pas nécessaire de se déconnecter de l’appli de bureau pour basculer entre les entreprises.
* Ctrl+V pour l’opération de collage fonctionne désormais sous Windows®.
* À l’avenir, lorsqu’une nouvelle version de l’appli de bureau sera publiée, les utilisateurs seront avertis dans l’appli de bureau elle-même.

## Téléchargez et installez la dernière appli de bureau Adobe Dynamic Media Classic sur macOS ou Windows® {#installation-dmc-app}

Voir aussi:

* [Télécharger et installer en mode silencieux la dernière application de bureau Adobe Dynamic Media Classic sur Mac](#install-silent-mac-dmc-app)
* [Téléchargez et installez en mode silencieux la dernière application de bureau Adobe Dynamic Media Classic sous Windows®](#install-silent-windows-dmc-app)

1. Désinstallez toutes les anciennes versions de l’appli de bureau Adobe Dynamic Media Classic de votre système.

1. Téléchargez la dernière version du programme d’installation de l’appli de bureau Adobe Dynamic Media Classic.

   * La dernière version (20.22.1) est disponible à l’adresse suivante :

      * [macOS (.DMG) - Téléchargement](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [Windows (.EXE) - Téléchargement](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)
   * La version précédente (20.21.3) est disponible à l’adresse suivante :

      * [macOS (.DMG) - Téléchargement](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg)
      * [Windows® (.EXE) - Téléchargement](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)


<!--    * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) -->

<!--    * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. Effectuez l’une des opérations suivantes en fonction du programme d’installation que vous avez téléchargé.

   * **macOS** - Dans le **[!UICONTROL Effectuez un glisser-déposer pour installer]** boîte de dialogue, faites glisser **[!UICONTROL Adobe Dynamic Media Classic]** et déposez-le sur **[!UICONTROL Applications]**.

      ![Installation par glisser-déposer sur macOS](/help/assets/dragondrop-install1.png)

   * Dans le **[!UICONTROL Applications]** , appuyez sur l’icône Adobe Dynamic Media Classic .
   * Dans la boîte de dialogue, appuyez sur **[!UICONTROL Ouvrir]** pour ouvrir l’appli de bureau Adobe Dynamic Media Classic.

      ![Ouvrir l’application téléchargée](/help/assets/open-dmclassicapp1.png)

   * **Windows** - Exécutez le fichier binaire du programme d’installation et suivez les instructions à l’écran pour installer l’appli de bureau .

1. Lorsque vous ouvrez l’application, la nouvelle page de connexion à Adobe Dynamic Media Classic s’affiche :

   ![Connexion Adobe Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Pour vous connecter à l’appli de bureau Adobe Dynamic Media Classic, utilisez les mêmes informations d’identification que celles que vous utilisiez pour vous connecter à Adobe Dynamic Media Classic dans le navigateur.

   Pour le **[!UICONTROL Serveur]** pour l’utiliser, voir le mappage suivant pour l’environnement de production :

   | Serveur | URL du navigateur |
   | --- | --- |
   | Production NA (Amérique du Nord) | https://s7sps1.scene7.com/ |
   | Production EMEA (Europe, Moyen-Orient et Afrique) | https://s7sps3.scene7.com/ |
   | Production APAC (Asie-Pacifique) | https://s7sps5.scene7.com/ |

1. Après vous être connecté, notez l’expérience familière de l’interface utilisateur du navigateur. Vous pouvez continuer votre activité Adobe Dynamic Media Classic quotidienne comme vous le faites habituellement sur l’appli de bureau .

## Téléchargement et *silence* installation de la dernière appli de bureau Adobe Dynamic Media Classic sur macOS {#install-silent-mac-dmc-app}

Voir aussi:

* [Téléchargez et installez la dernière appli de bureau Adobe Dynamic Media Classic sur Mac ou Windows®](#installation-dmc-app)
* [Téléchargez et installez en mode silencieux la dernière application de bureau Adobe Dynamic Media Classic sous Windows®](#install-silent-windows-dmc-app)

Pour télécharger et *silence* installez la dernière version de l’appli de bureau Adobe Dynamic Media Classic sur macOS :

1. Désinstallez toutes les anciennes versions de l’appli de bureau Adobe Dynamic Media Classic de votre système.

1. Téléchargez la dernière version du programme d’installation de l’appli de bureau Adobe Dynamic Media Classic pour macOS.

   * [macOS (.DMG) - Téléchargement](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)

1. Montez l’image de disque (.DMG) téléchargée vers un emplacement de point de montage à l’aide de la commande suivante :

   `hdiutil attach adobe-dynamic-media-classic-20.22.1.dmg -mountpoint <mount_point_path>`

1. Copiez le fichier .APP dans **[!UICONTROL Applications]** à l’aide de la commande suivante :

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG - hdiutil detach <mount_point_path>
   ```

1. Lorsque vous ouvrez l’application, la nouvelle page de connexion à Adobe Dynamic Media Classic s’affiche :

   ![Connexion Adobe Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Pour vous connecter à l’appli de bureau Adobe Dynamic Media Classic, utilisez les mêmes informations d’identification que celles que vous utilisiez pour vous connecter à Adobe Dynamic Media Classic dans le navigateur.

   Pour le **[!UICONTROL Serveur]** pour l’utiliser, voir le mappage suivant pour l’environnement de production :

   | Serveur | URL du navigateur |
   | --- | --- |
   | Production NA (Amérique du Nord) | https://s7sps1.scene7.com/ |
   | Production EMEA (Europe, Moyen-Orient et Afrique) | https://s7sps3.scene7.com/ |
   | Production APAC (Asie-Pacifique) | https://s7sps5.scene7.com/ |

## Téléchargement et *silence* installation de la dernière appli de bureau Adobe Dynamic Media Classic sous Windows® {#install-silent-windows-dmc-app}

La commande que vous utilisez est pour une installation silencieuse MSI de base. Cependant, le programme d’installation de l’appli de bureau Adobe Dynamic Media Classic est un programme d’installation MSI InstallScript créé à l’aide de InstallShield. Lorsque vous exécutez le programme d’installation en mode d’enregistrement, toute interaction utilisateur est enregistrée dans un fichier de réponse. Ce fichier de réponse est ensuite utilisé pour une installation silencieuse, comme décrit dans la section [Exécution des installations en mode silencieux.](https://docs.revenera.com/installshield19helplib/helplibrary/SilentInstall.htm)

Voir aussi:

* [Téléchargez et installez la dernière appli de bureau Adobe Dynamic Media Classic sur Mac ou Windows®](#installation-dmc-app)
* [Télécharger et installer en mode silencieux la dernière application de bureau Adobe Dynamic Media Classic sur macOS](#install-silent-mac-dmc-app)

Pour télécharger et *silence* installez la dernière version de l’appli de bureau Adobe Dynamic Media Classic sous Windows® :

1. Désinstallez toutes les anciennes versions de l’appli de bureau Adobe Dynamic Media Classic de votre système.

1. Téléchargez la dernière version du programme d’installation de l’appli de bureau Adobe Dynamic Media Classic.

   * [Windows® (.EXE) - Téléchargement](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. Exécutez le programme d’installation en mode d’enregistrement à l’aide de la commande suivante :

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. Dans la fenêtre du programme d’installation de l’interface utilisateur graphique, suivez les étapes à suivre pour que les interactions/entrées, comme l’emplacement d’installation, soient enregistrées dans `Setup.iss` fichier .

1. Copiez le créé `Setup.iss` et `adobe-dynamic-media-classic-20.22.1.exe` sur un autre ordinateur.

1. Exécutez la commande suivante pour une installation silencieuse :

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   Vous trouverez des informations détaillées sur les paramètres de ligne de commande à l’adresse [Paramètres de ligne de commande Setup.exe et Update.exe.](https://docs.revenera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. Lorsque vous ouvrez l’application, la nouvelle page de connexion à Adobe Dynamic Media Classic s’affiche :

   ![Connexion Adobe Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Pour vous connecter à l’appli de bureau Adobe Dynamic Media Classic, utilisez les mêmes informations d’identification que celles que vous utilisiez pour vous connecter à Adobe Dynamic Media Classic dans le navigateur.

   Pour le **[!UICONTROL Serveur]** pour l’utiliser, voir le mappage suivant pour l’environnement de production :

   | Serveur | URL du navigateur |
   | --- | --- |
   | Production NA (Amérique du Nord) | https://s7sps1.scene7.com/ |
   | Production EMEA (Europe, Moyen-Orient et Afrique) | https://s7sps3.scene7.com/ |
   | Production APAC (Asie-Pacifique) | https://s7sps5.scene7.com/ |

## Présentation vidéo lors de l’utilisation de l’application de bureau Adobe Dynamic Media Classic {#dmc-app-video-walk-through}

Regardez une [Présentation vidéo sur l’utilisation de l’application de bureau Adobe Dynamic Media Classic](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media) (Longueur : 2 minutes 36 secondes).

## Effacement du cache des images et du cache des ressources sur votre ordinateur à l’aide de l’appli de bureau {#clear-cache}

1. Dans l’appli de bureau Adobe Dynamic Media Classic, près du coin supérieur droit, appuyez sur **[!UICONTROL Configuration]** > **[!UICONTROL Configuration personnelle]**.
1. Sur le **[!UICONTROL Configuration personnelle]** , sous **[!UICONTROL Bureau]** , effectuez l’une des opérations suivantes :
   * Pour supprimer tous les fichiers image Dynamic Media mis en cache d’Adobe de votre ordinateur, appuyez sur **[!UICONTROL Effacer le cache d’images]**, puis appuyez sur **[!UICONTROL OK]**.
   * Pour supprimer tous les fichiers de ressources en cache Dynamic Media Adobe de votre ordinateur, appuyez sur **[!UICONTROL Effacer le cache des ressources]**, puis appuyez sur **[!UICONTROL OK]**.
1. Dans le coin inférieur droit de la page, appuyez sur **[!UICONTROL Fermer]**.

### Effacement manuel du cache d’image et du cache de ressources

Outre l’effacement de l’image et du cache des ressources à l’aide de l’appli de bureau, vous pouvez effacer manuellement le cache directement à partir du système de fichiers.

1. Selon votre système d’exploitation, accédez aux éléments suivants :

   * macOS : `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Limites connues dans Adobe Dynamic Media Classic 20.21.1

* Le **[!UICONTROL Serveur]** La liste déroulante est vide après la mise à jour vers l’appli de bureau Adobe Dynamic Media Classic 20.21.1 - Scénario : Vous installez et vous connectez à Adobe Dynamic Media Classic 20.20.1 ou 20.20.2, puis fermez l’application. Ensuite, vous effectuez la mise à jour vers Adobe Dynamic Media Classic 20.21.1. Lorsque vous tentez de vous connecter, la variable **[!UICONTROL Serveur]** Liste déroulante dans la **[!UICONTROL Connexion à votre compte]** est vide. Pour contourner ce problème, vous devez : [effacer manuellement le cache](#clear-cache) (voir les étapes ci-dessus).

## Limites connues dans Adobe Dynamic Media Classic 20.20.1 (corrigées dans 20.20.2)

**_S’applique uniquement à Windows® : y a-t-il une limitation du nombre de fichiers pouvant être chargés via l’interface utilisateur de l’appli de bureau ?_**<br>Oui, vous pouvez charger un maximum de 150 fichiers à la fois au moyen de l’interface utilisateur de l’appli de bureau.

**_S’applique à Windows® et macOS. Comment puis-je passer d’une entreprise à l’autre ?_**<br>Pour passer d’une entreprise à l’autre, procédez comme suit :

* Dans l’application Adobe Dynamic Media Classic, sélectionnez la nouvelle société dans la liste déroulante Société .
* Lorsque la fenêtre contextuelle s’affiche, appuyez sur **[!UICONTROL OK]** pour vous déconnecter et fermer l’application.

   ![Pour utiliser la nouvelle entreprise, redémarrez l’application.](/help/assets/dmclassic-new-company1.png)

* Redémarrez Adobe Dynamic Media Classic, puis connectez-vous comme d’habitude pour travailler avec la nouvelle société.

## Conseils et astuces

**_Je ne parviens pas à voir le panneau Panier multimédia sur la page d’entrée d’Adobe Dynamic Media Classic._**<br>Dans Adobe Dynamic Media Classic, appuyez sur**[!UICONTROL Configuration > Configuration personnelle ]**. Dans la section Navigateur , assurez-vous que**[!UICONTROL Afficher les fonctionnalités MediaPortal ]**est sélectionné (coché). Appuyer**[!UICONTROL Enregistrer > Fermer ]**.

**_L’état de publication (indicateur vert) d’une ressource n’est pas correctement reflété._**<br>Dans l’interface utilisateur du navigateur, une nouvelle connexion à l’interface utilisateur était nécessaire pour afficher l’état de publication correct des ressources. Dans l’appli de bureau, Adobe a introduit une**[!UICONTROL Actualiser ]**dans la barre d’outils, à droite de la**[!UICONTROL Sélectionner Aucun ]**bouton . Appuyez sur le bouton**[!UICONTROL Actualiser ]**pour afficher l’état le plus récent de toutes les ressources sur la page donnée. Aucune nouvelle connexion n’est requise, comme avec l’interface utilisateur du navigateur.

![Icône Actualiser](/help/assets/refresh-icon1.png)
*Icône Actualiser*

**_Je ne vois pas les paramètres prédéfinis d’ensemble par lot fonctionner dans l’appli de bureau ._**<br>Appuyer**[!UICONTROL Télécharger > Options de tâche > Paramètres prédéfinis d’ensemble par lot ]**. Assurez-vous que la variable**[!UICONTROL Paramètre prédéfini d’ensemble par lot ]**est activée. Cliquez sur**[!UICONTROL Enregistrement et envoi du chargement ]**.
