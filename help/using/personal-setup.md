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
>L’écran Configuration personnelle répertorie le rôle utilisateur que vous avez dans Adobe Dynamic Media Classic : Administrateur d’entreprise, Administrateur ou Utilisateur.

Les paramètres de configuration personnelle contrôlent le comportement par défaut du panneau Parcourir, la manière dont vous recevez des e-mails et des paramètres de mot de passe. N’oubliez pas de sélectionner **[!UICONTROL Enregistrer]** après avoir modifié ces paramètres.

## Informations sur mon compte

Identifie le nom de compte, le nom, le nom d’utilisateur (adresse électronique) et le rôle utilisateur attribué.

## Bureau

* **Effacer le cache d’images**: supprime de votre ordinateur tous les fichiers image mis en cache par Adobe Dynamic Media.
* **Effacer le cache des ressources**: supprime tous les fichiers de ressources mis en cache par Adobe Dynamic Media de votre ordinateur.

Outre l’effacement de l’image et du cache des ressources à l’aide de l’appli de bureau, vous pouvez effacer manuellement le cache directement à partir du système de fichiers. Selon votre système d’exploitation, accédez aux éléments suivants :

* MACOS : `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows® : `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Creative Suite Extension

**Pour installer l’extension Adobe Dynamic Media Creative Suite :**

1. Dans Adobe Dynamic Media Classic, dans la barre d’outils, accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration personnelle]**, sous Extension du Creative Suite, sélectionnez **[!UICONTROL Télécharger maintenant]** pour télécharger le `s7csxs.zxp` fichier .
1. Sélectionnez la variable **[!UICONTROL Installation]** et **[!UICONTROL Configuration requise]** liens pour plus d’informations sur l’extension.

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

* **[!UICONTROL Taille de la miniature]**: détermine la taille par défaut des images miniatures en mode Grille dans le panneau Parcourir.
* **[!UICONTROL Mode Bibliothèque de ressources par défaut]**: détermine si les ressources de la bibliothèque de ressources pour les ensembles de versions apparaissent sous la forme de miniatures ou par nom. Si vous travaillez avec un grand nombre de fichiers dans la bibliothèque, vous pouvez les afficher par nom. Par exemple, si vous créez un catalogue électronique volumineux avec de nombreux fichiers PDF, vous pouvez afficher les fichiers par nom pour que la liste soit plus courte.
* **[!UICONTROL Ordre de tri de la navigation par défaut]**: détermine l’ordre d’affichage des ressources par défaut dans le panneau Parcourir. Choisissez un critère de tri dans le menu, et optez pour un ordre croissant ou décroissant.
* **[!UICONTROL Emplacement de navigation par défaut]**: permet de définir l’emplacement de navigation sur la valeur par défaut, le dernier dossier parcouru ou sur un emplacement spécifique que vous accédez à et identifiez. Vous pouvez également définir l’emplacement de navigation pour trier les fichiers et les dossiers dans l’ordre ascendant ou descendant.
* **[!UICONTROL Mode Parcourir par défaut]**: détermine si le mode Affichage de la grille ou Affichage de la liste est le mode par défaut qui s’affiche lorsque vous ouvrez le panneau Parcourir pour la première fois.
* **[!UICONTROL Affichage de l’écran de démarrage]**: détermine si vous voyez des écrans de démarrage, y compris l’écran de bienvenue.
* **[!UICONTROL Afficher les info-bulles]**: détermine si les info-bulles s’affichent lorsque vous placez le pointeur sur les boutons, les menus et les liens de navigation. Les info-bulles décrivent les éléments de l’interface utilisateur à l’écran.
* **[!UICONTROL Arrière-plan du tableau de bord]**: affiche un calque de damier derrière les images, ce qui vous permet de voir facilement les zones transparentes d’une image comportant un canal alpha.
* **[!UICONTROL Afficher la taille du fichier]**: affiche la taille de fichier d’une ressource en cours de navigation.
* **[!UICONTROL Inclure les champs définis par les utilisateurs dans la recherche]**: pour améliorer les performances système de la plupart des recherches de métadonnées que vous exécutez, désélectionnez (par défaut).

  Si l’inclusion de champs définis par les utilisateurs est bénéfique pour la plupart de vos recherches de métadonnées, activez-la en sélectionnant cette option. Vous pouvez également utiliser la fonction de recherche avancée afin d’offrir une expérience de recherche plus ciblée et plus rapide que l’inclusion de champs définis par l’utilisateur.

  Voir [Recherche avancée](searching-assets.md#conducting_an_advanced_search).

  Voir aussi [Champs définis par l’utilisateur](application-setup.md#user_defined_fields).

* **[!UICONTROL Type de recherche de base]**: vous pouvez effectuer une sélection parmi deux options : **[!UICONTROL Contient]** recherche la valeur spécifiée dans la chaîne complète ; **[!UICONTROL StartsWith]** recherche à partir du début de la chaîne et renvoie les résultats plus rapidement que **[!UICONTROL Contient]**. L’une des options remplace la valeur par défaut définie dans **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres généraux de l’application]** par l’administrateur.
* **[!UICONTROL Afficher les commentaires de commande]**: sélectionnez cette option pour activer l’affichage des requêtes de commande sur le serveur. Désélectionnez cette option pour la désactiver.
* **[!UICONTROL Afficher la boîte de dialogue pendant l’exportation]**: sélectionnez cette option pour afficher une boîte de dialogue contextuelle lors d’une exportation. Si vous désélectionnez (désactivez) cette option, vous pouvez toujours accéder à la page Tâches pour récupérer les résultats de votre exportation.

## E-mail

* **[!UICONTROL Options de messagerie]**: choisissez la manière dont Adobe Dynamic Media Classic doit vous informer par e-mail lorsque les tâches de téléchargement et de publication sont terminées. Vous pouvez recevoir des avis de fin de travaux uniquement si des avertissements ou des erreurs se sont produits.
* **[!UICONTROL Portée de l’email]**: détermine si vous recevez tous les e-mails de tâche pour votre entreprise ou uniquement les e-mails concernant les tâches de téléchargement et de publication que vous lancez.
* **[!UICONTROL Types d’email]**: détermine si vous êtes informé lorsque les tâches de chargement et de publication sont terminées.

## Langue

* **[!UICONTROL Langue préférée]**: détermine la langue que vous souhaitez utiliser pour l’interface.

## Mot de passe

* **[!UICONTROL Mot de passe actuel]**: saisissez le mot de passe de votre mot de passe actuel.
* **[!UICONTROL Nouveau mot de passe]**: saisissez un nouveau mot de passe valide. Votre mot de passe doit répondre aux exigences suivantes :
   * Elle doit comporter entre 8 et 25 caractères.
   * Contient au moins une lettre minuscule.
   * Contient au moins une lettre majuscule.
   * Contient au moins un nombre.
   * contenir au moins l’un des caractères spéciaux suivants : `# $ &: _ : { }`
* **[!UICONTROL Renommer le mot de passe]**: saisissez à nouveau le nouveau mot de passe pour confirmer que vous le saisissez correctement.
* **[!UICONTROL Expiration du mot de passe]**: détermine si votre mot de passe expire après 72 jours en tant que mesure de sécurité. Si vous avez sélectionné Oui, vous êtes invité à créer un mot de passe au bout de 72 jours.
