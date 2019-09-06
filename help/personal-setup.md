---
title: Configuration personnelle
seo-title: Configuration personnelle
description: 'null'
seo-description: Tous les utilisateurs peuvent modifier les paramètres de l'écran Configuration personnelle de Dynamic Media Classic.
uuid: 29 cb 825 a-f 158-4 a 1 e -9 d 5 f -7636 ee 411 b 6 e
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/setup
discoiquuid: 6314 e 7 b 7-5 bde -4 fe 2-8674-e 4 fc 525 d 4 d 1 c
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Configuration personnelle {#personal-setup}

Tous les utilisateurs peuvent modifier les paramètres de l’écran Configuration personnelle. Pour ouvrir l’écran Configuration personnelle, cliquez sur Configuration &gt; Configuration personnelle.

>[!NOTE]
>
>l’écran Configuration personnelle répertorie vos rôles utilisateurs dans Scene7 Publishing System : Administrateur d’entreprise, Administrateur ou Utilisateur.

Les paramètres de l’écran Configuration personnelle contrôlent le comportement par défaut du panneau de navigation, le mode de réception des e-mails et la configuration des mots de passe. Pensez à cliquer sur Enregistrer après avoir modifié ces paramètres.

## Informations sur mon compte

Identifie le nom de compte, le nom, le nom d’utilisateur (adresse électronique) et le rôle utilisateur attribué.

### Version de bureau

Cliquez sur Installer maintenant pour installer la version de bureau de Scene7 Publishing System sur le disque dur local. Sinon, cliquez sur Réinstaller maintenant pour réinstaller la version de bureau.

### Module externe d’Illustator pour l’impression en ligne

Sous Windows 7 ou 8, vous devez disposer de droits d’administrateur et être connecté en tant qu’administrateur sous Windows pour installer le module externe d’Adobe Illustrator pour l’impression en ligne. Une fois le module externe installé, il est disponible dans Adobe Illustrator.

Le module externe est pris en charge pour les versions suivantes d’Adobe Illustrator :

* Adobe Illustrator 18 dans Adobe Creative Cloud 2014.
* Adobe Illustrator 17 dans Adobe Creative Cloud.
* Adobe Illustrator 16 dans Adobe Creative Suite 6.

Les plates-formes prises en charge d’Adobe Illustrator sont les suivantes :

* Appel Mac OS X 10.7 ou version ultérieure.
* Windows 8, 32 et 64 bits.
* Windows 7, 32 et 64 bits.
* Windows XP, 32 et 64 bits (pour Adobe Illustrator 16 dans Adobe Creative Suite 6 uniquement).

Voir aussi [Module de publication à l’aide de modèles prédéfinis](quick-start-template-publishing.md).

## Pour installer le module externe sur votre disque dur local

1. Sur la page Configuration personnelle dans Scene7 Publishing System, sous le module externe d’Illustrator pour l’impression en ligne, cliquez sur **Télécharger maintenant** pour télécharger le fichier **Module externe d’Illustrator pour Web-to-Print.zip**.
1. Décompressez le fichier ZIP dans un dossier temporaire.

   Un fichier Lisez-moi relatif est inclus dans la racine du fichier décompressé pour fournir des informations supplémentaires sur le module externe.

1. Selon votre système d’exploitation, effectuez l’une des opérations suivantes :

### Windows

| Si vous exécutez | Instructions : |
|--- |--- |
| Adobe Illustrator 18 dans Adobe Creative Cloud 2014 | <ul><li>A partir de la racine du dossier décompressé, cliquez sur CC-2014.</li><li>Selon la version de bits d’Adobe Illustrator utilisée, cliquez sur win32 ou sur win64.</li><li>Cliquez sur Bibliothèques &gt; flamme, puis copiez `aflame.dll` dans le dossier exécutable d’Adobe Illustrator. Par exemple, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Remarque**: Cet exemple de chemin concerne l'emplacement 64 bits ; l'emplacement 32 bits peut se trouver sous Program Files (x 86). <br/><ul><li>Revenez au même dossier Bibliothèques, cliquez sur flamingo, puis copiez `aflamingo.dll` dans le même dossier exécutable d’Adobe Illustrator utilisé à l’étape précédente. </li><li>Revenez au dossier win32 ou win64 sélectionné à l’étape 2, puis copiez `AdobeS7FXGFileFormat.aip` dans le dossier Modules externes d’Adobe Illustrator. Par exemple, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Remarque**: Cet exemple de chemin concerne l'emplacement 64 bits ; l'emplacement 32 bits peut se trouver sous Program Files (x 86). |
| Adobe Illustrator 17 dans Adobe Creative Cloud | <ul><li>A partir de la racine du dossier décompressé, cliquez sur CC. </li><li>Selon la version de bits d’Adobe Illustrator utilisée, cliquez sur win32 ou sur win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. Par exemple, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Remarque**: Cet exemple de chemin concerne l'emplacement 64 bits ; l'emplacement 32 bits peut se trouver sous Program Files (x 86). |
| Adobe Illustrator 16 dans Adobe Creative Suite 6 | <ul><li>A partir de la racine du dossier décompressé, cliquez sur 6.0. </li><li>Selon la version de bits d’Adobe Illustrator utilisée, cliquez sur win32 ou sur win64. </li><li>Copiez AdobeS7FXGFileFormat.aip dans le dossier des modules externes d’Adobe Illustrator. Par exemple, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Remarque**: Cet exemple de chemin concerne l'emplacement 64 bits ; l'emplacement 32 bits peut se trouver sous Program Files (x 86). |

### Mac

| Si vous exécutez | Instructions : |
|--- |--- |
| Adobe Illustrator 18 dans Adobe Creative Cloud 2014 | <ul><li>A partir de la racine du dossier décompressé, cliquez sur  CC-2014 &gt; mac64.</li><li>Cliquez sur Bibliothèques &gt; flame, puis copiez le dossier `aflame.framework` dans le dossier de contenu de package d’Adobe Illustrator. Par exemple, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (Pour ouvrir le dossier du contenu du pack d'Adobe Illustrator, cliquez avec le bouton droit de la souris sur l'icône Adobe illustrator CC 2014 et cliquez sur Afficher le contenu du progiciel dans le menu contextuel).</li><li>Revenez au même dossier bibliothèques, cliquez sur `flamingo`, puis copiez le dossier `aflamingo.framework` dans le même dossier de contenu du package d’Adobe Illustrator utilisé à l’étape précédente.</li><li>Revenez au dossier mac64 sélectionné à l’étape 1, puis copiez le dossier `AdobeS7FXGFileFormat.aip` dans le dossier du module externe d’Adobe Illustrator. Par exemple, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/> |
| Adobe Illustrator 17 dans Adobe Creative Cloud | <ul><li>A partir de la racine du dossier décompressé, cliquez sur CC &gt; mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. Par exemple, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/> |
| Adobe Illustrator 16 dans Adobe Creative Suite 6 | <ul><li>A partir de la racine du dossier décompressé, cliquez sur 6.0 &gt; mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. Par exemple, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul> |

Le module externe est désormais disponible pour être utilisé dans Adobe Illustrator.

### Navigateur

* **Taille des miniatures**
   * Définit la taille par défaut des images miniatures dans le panneau de navigation en mode Affichage de la grille.
* **Affichage par défaut de la bibliothèque de fichiers**
   * Détermine si les fichiers de la bibliothèque destinés à la création des visionneuses apparaissent sous la forme de miniatures ou par nom. Si vous travaillez avec un grand nombre de fichiers dans la bibliothèque, vous pouvez les afficher par nom. Par exemple, si vous créez un catalogue électronique volumineux avec de nombreux fichiers PDF, vous pouvez afficher les fichiers par nom pour que la liste soit plus courte.
* **Ordre de tri par défaut de la navigation**
   * Détermine l’ordre d’affichage par défaut des fichiers dans le panneau de navigation. Choisissez un critère de tri dans le menu, et optez pour un ordre croissant ou décroissant.
* **Emplacement de navigation par défaut**
   * Vous permet de définir comme emplacement de navigation le dossier par défaut, le dossier dans lequel vous avez navigué en dernier ou un emplacement spécifique dans lequel vous avez navigué et que vous avez identifié. Vous pouvez également définir l’emplacement de navigation pour trier les fichiers et les dossiers dans l’ordre ascendant ou descendant.
* **Affichage de la navigation par défaut**
   * Définit le mode d’affichage par défaut du panneau de navigation à sa première ouverture : Affichage de la grille ou Affichage par liste.
* **Affichage de l’écran de lancement**
   * Permet d’activer ou non l’affichage des écrans de lancement, notamment l’écran de bienvenue.
* **Afficher les info-bulles**
   * Permet d’activer ou non l’affichage des info-bulles lorsque le pointeur survole des boutons, des menus et des liens de navigation. Les info-bulles décrivent les objets à l’écran.
* **Damier de fond**
   * Affiche un damier derrière les images qui vous permet de voir facilement les zones transparentes d’une image qui contient une couche alpha.
* **Afficher la taille du fichier**
   * Affiche la taille d’un fichier au cours de la navigation.
* **Confirmer avant de quitter SPS**
   * Affiche une fenêtre de confirmation avant que vous quittiez Scene7 Publishing System.
* **Inclure les champs définis par les utilisateurs dans la recherche**
   * Option désélectionnée (par défaut) pour améliorer les performances du système pour la plupart des recherches de métadonnées que vous exécutez.

Si l’inclusion de champs définis par les utilisateurs est bénéfique pour la plupart de vos recherches de métadonnées, activez-la en sélectionnant cette option. Vous pouvez également utiliser Recherche avancée afin d’effectuer des recherches mieux orientées et plus rapides qu’avec l’inclusion de tous les champs définis par les utilisateurs.

Voir [Recherche avancée](searching-assets.md#conducting_an_advanced_search).

Voir aussi [Champs définis par l’utilisateur](application-setup.md#user_defined_fields).

* **Recherche de base**
   * Choisissez un type de recherche par défaut, Contient ou Commence par.
* **Afficher les fonctionnalités MediaPortal**
   * Sélectionnez cette option pour accéder aux fonctionnalités du portail multimédia, telle que le panier.
* **Afficher les commentaires sur les commandes**
   * Affiche les demandes de commandes envoyées au serveur.
* **Afficher la boîte de dialogue pendant l’exportation**
   * Affiche une boîte de dialogue lorsque vous effectuez une exportation. Si vous désélectionnez cette option, vous pouvez toujours accéder à la page Tâches pour récupérer les résultats de votre exportation.

## E-mail

* **Options de messagerie**
   * Choisissez comment vous souhaitez que Dynamic Media Classic vous informe par e-mail lorsque des tâches de téléchargement et de publication sont terminées. Vous pouvez recevoir des avis de fin de travaux uniquement si des avertissements ou des erreurs se sont produits.
* **Destinataires des e-mails**
   * Indique si vous recevez tous les e-mails des tâches de votre société ou uniquement les e-mails sur les tâches de téléchargement et de publication que vous avez lancées.
* **Types d’e-mails**
   * Détermine si vous êtes informé de la fin des tâches de téléchargement et de publication.
* **Langue**
* **Langue souhaitée**
   * Détermine la langue de l’interface.
* **Mot de passe**
* **Nouveau mot de passe**
   * Saisissez un nouveau mot de passe valide. Votre mot de passe doit respecter les exigences suivantes :
      * Comporter entre 8 et 25 caractères
      * Contenir au moins une lettre minuscule
      * Contenir au moins une lettre majuscule
      * Contenir au moins un nombre
      * Contient au moins l'un des caractères spéciaux suivants : # $ &amp;-_ : {}

* **Confirmer le mot de passe**
   * Entrez une seconde fois le nouveau mot de passe pour vous assurer de le saisir correctement.
* **Expiration du mot de passe**
   * Indique si votre mot de passe expire à l’issue d’un délai de 72 jours par mesure de sécurité. Si vous sélectionnez Oui, vous serez invité à créer un nouveau mot de passe passé ce délai.
