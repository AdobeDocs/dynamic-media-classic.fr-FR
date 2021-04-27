---
title: Configuration personnelle
description: Tous les utilisateurs peuvent modifier les paramètres de l’écran Configuration personnelle de Dynamic Media Classic.
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
feature: Dynamic Media Classic
role: Administrator,Business Practitioner
exl-id: a019f973-7647-466f-8af3-5312e9225e89
translation-type: tm+mt
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 28%

---

# Configuration personnelle {#personal-setup}

Tous les utilisateurs peuvent modifier les paramètres de l’écran Configuration personnelle. Pour ouvrir l’écran Configuration personnelle, cliquez sur Configuration > Configuration personnelle.

>[!NOTE]
>
>L’écran Configuration personnelle liste le rôle utilisateur que vous avez dans Dynamic Media Classic : Administrateur de société, Administrateur ou Utilisateur.

Les paramètres de l’écran Configuration personnelle contrôlent le comportement par défaut du panneau de navigation, le mode de réception des e-mails et la configuration des mots de passe. Pensez à cliquer sur Enregistrer après avoir modifié ces paramètres.

## Informations sur mon compte

Identifie le nom de compte, le nom, le nom d’utilisateur (adresse électronique) et le rôle utilisateur attribué.

## Bureau

* **Effacer le cache**  d&#39;image : supprime tous les fichiers d&#39;image mis en cache par Dynamic Media Adobe de votre ordinateur.
* **Effacer le cache**  des ressources : supprime tous les fichiers de ressources mis en cache par Dynamic Media Adobe de votre ordinateur.

Outre l’effacement du cache d’images et de ressources à l’aide de l’application de bureau, vous pouvez effacer manuellement le cache directement à partir du système de fichiers. En fonction de votre système d’exploitation, accédez aux options suivantes :

* macOS : `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Creative Suite Extension

**Pour installer l&#39;extension Creative Suite d&#39;Adobe Dynamic Media :**

1. Dans Dynamic Media Classic, sur la barre d’outils, cliquez sur **[!UICONTROL Configuration]** > **[!UICONTROL Configuration personnelle]**, sous Creative Suite Extension, cliquez sur **[!UICONTROL Télécharger maintenant]** pour télécharger le fichier `s7csxs.zxp`.
1. Cliquez sur les liens **[!UICONTROL Installation]** et **[!UICONTROL Configuration système requise]** pour plus d&#39;informations sur l&#39;extension.

<!--    A readme file is included at the root of the unzipped file to provide you with additional information about the extension.

1. Depending on your installed operating system, do one of the following: -->

<!-- #### Windows

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, click CC-2014.</li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64.</li><li>Click libraries > flame, and then copy `aflame.dll` to Adobe Illustrator's executable folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead. <br/><ul><li>Return to the same libraries folder, click flamingo, and then copy `aflamingo.dll` to the same Adobe Illustrator executable folder that you used in the previous step. </li><li>Return to the win32 or win64 folder that you selected in step 2, and then copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, click CC. </li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, click 6.0. </li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64. </li><li>Copy AdobeS7FXGFileFormat.aip to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|

#### Mac

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, click CC-2014 > mac64.</li><li>Click libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator’s package contents folder, right-click on the Adobe illustrator CC 2014 icon and click Show Package Contents from context menu).</li><li>Return to the same libraries folder, click `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, click CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, click 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator. -->

## Navigateur

* **Taille**  des miniatures : détermine la taille par défaut des miniatures dans la vue de la grille du panneau de navigation.
* **Vue**  de bibliothèque de fichiers par défaut : détermine si les fichiers de la bibliothèque de fichiers pour les visionneuses de génération apparaissent sous forme de miniatures ou par nom. Si vous travaillez avec un grand nombre de fichiers dans la bibliothèque, vous pouvez les afficher par nom. Par exemple, si vous créez un catalogue électronique volumineux avec de nombreux fichiers PDF, vous pouvez afficher les fichiers par nom pour que la liste soit plus courte.
* **Ordre**  de tri par défaut de la navigation : détermine l’ordre dans lequel les fichiers apparaissent par défaut dans le panneau de navigation. Choisissez un critère de tri dans le menu, et optez pour un ordre croissant ou décroissant.
* **Emplacement**  de navigation par défaut : permet de définir l&#39;emplacement de navigation sur la valeur par défaut, le dernier dossier parcouru ou un emplacement spécifique que vous accédez et identifiez. Vous pouvez également définir l’emplacement de navigation pour trier les fichiers et les dossiers dans l’ordre ascendant ou descendant.
* **Vue**  de navigation par défaut : détermine si la vue de grille ou la vue de Liste est la vue par défaut qui s’affiche lorsque vous ouvrez le panneau de navigation pour la première fois.
* **Affichage**  de l’écran de démarrage : détermine si vous voyez des écrans de démarrage, y compris l’écran de démarrage de l’accueil.
* **Afficher les info-bulles**  - Détermine si les info-bulles s&#39;affichent lorsque vous déplacez le pointeur sur des boutons, des menus et des liens de navigation. Les info-bulles décrivent les éléments de l’interface utilisateur à l’écran.
* **Arrière-plan**  du damier - Affiche un damier derrière les images, ce qui vous permet de voir facilement les zones transparentes d&#39;une image qui comporte un canal alpha.
* **Afficher la taille**  du fichier : affiche la taille du fichier lorsque vous naviguez sur le site.
* **Inclure les champs définis par les utilisateurs dans la recherche**  - Pour améliorer les performances du système pour la plupart des recherches de métadonnées que vous exécutez, désélectionnez (par défaut).

   Si l’inclusion de champs définis par les utilisateurs est bénéfique pour la plupart de vos recherches de métadonnées, activez-la en sélectionnant cette option. Vous pouvez également utiliser Recherche avancée afin d’effectuer des recherches mieux orientées et plus rapides qu’avec l’inclusion de tous les champs définis par les utilisateurs.

   Voir [Recherche avancée](searching-assets.md#conducting_an_advanced_search).

   Voir aussi [Champs définis par l’utilisateur](application-setup.md#user_defined_fields).

* **Type**  de recherche de base : vous pouvez choisir entre deux options :  **** Containsrecherche la valeur spécifiée dans la chaîne complète ;  **** CommenceRetire les recherches depuis le début de la chaîne et renvoie les résultats plus rapidement que  **[!UICONTROL Contient]**. L’une des options remplace la valeur par défaut définie dans **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres généraux de l’application]** par l’administrateur.
* **Afficher les commentaires**  des commandes : sélectionnez cette option pour activer l&#39;affichage des requêtes de commandes sur le serveur ; désélectionnez cette option pour désactiver.
* **Afficher la boîte de dialogue pendant l&#39;exportation**  - Sélectionnez cette option pour afficher une boîte de dialogue contextuelle pendant l&#39;exportation. Si vous désélectionnez (désactivez) cette option, vous pouvez toujours accéder à la page Tâches pour récupérer les résultats de votre exportation.

## E-mail

* **Options**  de messagerie - Choisissez comment vous souhaitez que Dynamic Media Classic vous informe par e-mail lorsque les tâches de téléchargement et de publication sont terminées. Vous pouvez recevoir des avis de fin de travaux uniquement si des avertissements ou des erreurs se sont produits.
* **Portée**  du courrier électronique - Détermine si vous recevez tous les e-mails de tâche pour votre société ou uniquement des e-mails sur les tâches de téléchargement et de publication que vous lancez.
* **Types**  de courrier électronique - Détermine si vous êtes informé de la fin des tâches de téléchargement et de publication.

## Langue

* **Langue**  préférée : détermine la langue que vous souhaitez utiliser pour l&#39;interface.

## Mot de passe

* **Mot de passe**  actuel - Entrez le mot de passe de votre mot de passe actuel.
* **Nouveau mot de passe**  - Entrez un nouveau mot de passe valide. Votre mot de passe doit répondre aux exigences suivantes :
   * Comporter entre 8 et 25 caractères.
   * Contenir au moins une lettre minuscule.
   * Contenir au moins une lettre majuscule.
   * Contient au moins un nombre.
   * Contenir au moins l’un des caractères spéciaux suivants : `# $ & - _ : { }`
* **Renommez le mot de passe**  : entrez à nouveau le nouveau mot de passe pour confirmer que vous l&#39;avez saisi correctement.
* **Expiration**  du mot de passe : détermine si votre mot de passe expire après 72 jours à titre de mesure de sécurité. Si vous sélectionnez Oui, vous serez invité à créer un nouveau mot de passe passé ce délai.
