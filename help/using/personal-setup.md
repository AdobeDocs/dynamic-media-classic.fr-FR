---
title: Configuration personnelle
description: Tous les utilisateurs peuvent modifier les paramètres de l’écran Configuration personnelle d’Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin,User
exl-id: a019f973-7647-466f-8af3-5312e9225e89
topic: Administration, Collaboration
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 19%

---

# Configuration personnelle {#personal-setup}

Tous les utilisateurs peuvent modifier les paramètres de l’écran Configuration personnelle. Pour ouvrir l’écran Configuration personnelle, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration personnelle]**.

>[!NOTE]
>
>L’écran Configuration personnelle répertorie les rôles utilisateur que vous avez dans Adobe Dynamic Media Classic : Administrateur de l’entreprise, Administrateur ou Utilisateur.

Les paramètres de configuration personnelle contrôlent le comportement par défaut du panneau de navigation, la manière dont vous recevez le courrier électronique et les paramètres de mot de passe. N’oubliez pas de sélectionner **[!UICONTROL Enregistrer]** après avoir modifié ces paramètres.

## Informations sur mon compte

Identifie le nom de compte, le nom, le nom d’utilisateur (adresse électronique) et le rôle utilisateur attribué.

## Bureau

* **Effacer le cache d’image** : supprime tous les fichiers image Adobe mis en cache Dynamic Media de votre ordinateur.
* **Effacer le cache de ressources** : supprime tous les fichiers de ressources du cache Dynamic Media Adobe de votre ordinateur.

Outre l’effacement de l’image et du cache de ressources à l’aide de l’application de bureau , vous pouvez effacer manuellement le cache directement à partir du système de fichiers. En fonction de votre système d’exploitation, accédez aux éléments suivants :

* MACOS : `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows® : `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Creative Suite Extension

**Pour installer l’extension Adobe Dynamic Media Creative Suite, procédez comme suit**

1. Dans Adobe Dynamic Media Classic, sur la barre d’outils, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration personnelle]**, sous Extension Creative Suite, sélectionnez **[!UICONTROL Télécharger maintenant]** pour télécharger le fichier `s7csxs.zxp`.
1. Sélectionnez les liens **[!UICONTROL Installation]** et **[!UICONTROL Configuration requise]** pour plus d’informations sur l’extension.

<!--    A readme file is included at the root of the unzipped file to provide you with additional information about the extension.

1. Depending on your installed operating system, do one of the following: -->

<!-- #### Windows

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014.</li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li>Select libraries > flame, and then copy `aflame.dll` to Adobe Illustrator's executable folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead. <br/><ul><li>Return to the same libraries folder, select flamingo, and then copy `aflamingo.dll` to the same Adobe Illustrator executable folder that you used in the previous step. </li><li>Return to the win32 or win64 folder that you selected in step 2, and then copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64. </li><li>Copy AdobeS7FXGFileFormat.aip to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|

#### Mac

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014 > mac64.</li><li>Select libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator's package contents folder, right-select on the Adobe illustrator CC 2014 icon and select Show Package Contents from context menu).</li><li>Return to the same libraries folder, select `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator. -->

## Navigateur

* **[!UICONTROL Taille des miniatures]** : détermine la taille par défaut des images miniatures en mode Grille dans le panneau Parcourir.
* **[!UICONTROL Affichage de la bibliothèque de ressources par défaut]** : détermine si les ressources de la bibliothèque de ressources pour les jeux de versions s’affichent sous forme de miniatures ou par nom. Si vous travaillez avec un grand nombre de fichiers dans la bibliothèque, vous pouvez les afficher par nom. Par exemple, si vous créez un catalogue électronique volumineux avec de nombreux fichiers PDF, vous pouvez afficher les fichiers par nom pour que la liste soit plus courte.
* **[!UICONTROL Ordre de tri de navigation par défaut]** : détermine l’ordre dans lequel les ressources s’affichent par défaut dans le panneau de navigation. Choisissez un critère de tri dans le menu, et optez pour un ordre croissant ou décroissant.
* **[!UICONTROL Emplacement de navigation par défaut]** : permet de définir l’emplacement de navigation par défaut, le dernier dossier parcouru ou un emplacement spécifique auquel vous accédez et que vous identifiez. Vous pouvez également définir l’emplacement de navigation pour trier les fichiers et les dossiers dans l’ordre ascendant ou descendant.
* **[!UICONTROL Vue de navigation par défaut]** : détermine si la vue Grille ou Liste est la vue par défaut affichée lorsque vous ouvrez le panneau de navigation pour la première fois.
* **[!UICONTROL Affichage de l’écran de démarrage]** : détermine si des écrans de démarrage s’affichent, y compris l’écran de démarrage de bienvenue.
* **[!UICONTROL Afficher les info-bulles]** : détermine si des info-bulles s’affichent lorsque vous déplacez le pointeur sur des boutons, des menus et des liens de navigation. Les info-bulles décrivent les éléments de l’interface utilisateur à l’écran.
* **[!UICONTROL Arrière-plan en damier]** : affiche un calque en damier derrière les images, ce qui vous permet de voir facilement les zones transparentes d’une image dotée d’une couche alpha.
* **[!UICONTROL Afficher la taille de fichier]** : affiche la taille de fichier d’une ressource lorsque vous naviguez.
* **[!UICONTROL Inclure les FDU dans la recherche]** : pour améliorer les performances du système pour la plupart des recherches de métadonnées que vous exécutez, désélectionnez cette option (par défaut).

  Si l’inclusion de champs définis par les utilisateurs est bénéfique pour la plupart de vos recherches de métadonnées, activez-la en sélectionnant cette option. Vous pouvez également utiliser la recherche avancée pour obtenir une expérience de recherche plus ciblée et plus rapide qu’en incluant des champs définis par l’utilisateur.

  Voir [Recherche avancée](searching-assets.md#conducting_an_advanced_search).

  Voir aussi [Champs définis par l’utilisateur](application-setup.md#user_defined_fields).

* **[!UICONTROL Type de recherche de base]** : vous pouvez choisir parmi deux options : **[!UICONTROL Contient]** recherche la valeur spécifiée dans toute la chaîne ; **[!UICONTROL CommencePar]** recherche au début de la chaîne et renvoie des résultats plus rapidement que **[!UICONTROL Contient]**. L’une ou l’autre des options remplace la valeur par défaut définie dans **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres généraux de l’application]** par l’administrateur.
* **[!UICONTROL Afficher le retour d’informations sur la commande]** : sélectionnez cette option pour activer l’affichage des requêtes de commande au serveur ; désélectionnez-la pour le désactiver.
* **[!UICONTROL Afficher la boîte de dialogue lors de l’exportation]** : sélectionnez cette option pour afficher une boîte de dialogue pop-up lors d’une exportation. Si vous désélectionnez (désactivez) cette option, vous pouvez toujours accéder à la page Tâches pour récupérer les résultats de votre exportation.

## E-mail

* **[!UICONTROL Options de messagerie électronique]** : choisissez la manière dont vous souhaitez qu’Adobe Dynamic Media Classic vous informe par courrier électronique lorsque les tâches de chargement et de publication sont terminées. Vous pouvez recevoir des avis de fin de travaux uniquement si des avertissements ou des erreurs se sont produits.
* **[!UICONTROL Portée de l’e-mail]** : détermine si vous recevez tous les e-mails relatifs aux tâches de votre entreprise ou uniquement ceux relatifs aux tâches de chargement et de publication que vous lancez.
* **[!UICONTROL Types d’e-mail]** : détermine si vous êtes informé lorsque les tâches de chargement et de publication sont terminées.

## Langue

* **[!UICONTROL Langue préférée]** : détermine la langue que vous souhaitez utiliser pour l’interface.

## Mot de passe

* **[!UICONTROL Mot de passe actuel]** : saisissez le mot de passe de votre mot de passe actuel.
* **[!UICONTROL Nouveau mot de passe]** : saisissez un nouveau mot de passe valide. Votre mot de passe doit répondre aux exigences suivantes :
   * Il doit comporter entre 8 et 25 caractères.
   * Contiennent au moins une lettre minuscule.
   * Contiennent au moins une lettre majuscule.
   * Contiennent au moins un chiffre.
   * contiennent au moins l’un des caractères spéciaux suivants : `# $ &: _ : { }` ;
* **[!UICONTROL Confirmer la saisie du mot de passe]** : saisissez à nouveau le nouveau mot de passe pour confirmer que vous le saisissez correctement.
* **[!UICONTROL Expiration du mot de passe]** : détermine si votre mot de passe expire après 72 jours par mesure de sécurité. Si vous avez sélectionné Oui, vous êtes invité à créer un mot de passe après 72 jours.
