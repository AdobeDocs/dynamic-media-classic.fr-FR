---
title: Téléchargement de fichiers
description: Découvrez comment charger des fichiers dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
topic: Content Management
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '3868'
ht-degree: 25%

---

# Téléchargement de fichiers{#uploading-files}

Avant de charger des fichiers de ressources vers Adobe Dynamic Media Classic, assurez-vous que leur nom est correct. Assurez-vous également que votre structure de dossiers est configurée et organisée comme vous le souhaitez. Vous pouvez transférer des fichiers depuis un site FTP fourni par Adobe Dynamic Media Classic ou directement depuis votre ordinateur ou votre réseau. Adobe Dynamic Media Classic propose des options d’optimisation des fichiers lors de leur chargement. Si vous avez installé l’application de bureau Adobe Dynamic Media Classic, vous pouvez charger des fichiers et des dossiers en les faisant glisser directement depuis votre bureau. (voir [Paramètres généraux de l’application](application-setup.md#general_settings)).

## Préparation du chargement des ressources et des dossiers {#preparing-your-assets-and-folders-for-uploading}

Avant de charger des ressources vers Adobe Dynamic Media Classic, assurez-vous qu’elles sont au format et à la taille adéquats. Vous devez également respecter les règles Adobe Dynamic Media Classic pour nommer les ressources. La définition d’une organisation et d’une structure de dossiers pour les fichiers garantit une facilité de localisation et d’utilisation de ces derniers.

### Formats de fichiers pris en charge {#supported-asset-file-formats}

Ce tableau répertorie les formats de fichiers de ressources pris en charge par Adobe Dynamic Media Classic. Pour plus d’informations sur les fichiers Camera Raw pris en charge, voir [https://helpx.adobe.com/camera-raw/using/supported-cameras.html](https://helpx.adobe.com/camera-raw/using/supported-cameras.html).

| Formats de fichiers | Description |
| --- | --- |
| Audio | AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3 |
| Feuille de style en cascade | CSS |
| Profils colorimétriques | ICC, ICM |
| Polices | AFM, OTF, PFB, PFM, PhotoFont, TTC, TTF |
| FXG | FXG |
| Illustrator | AI, FXG |
| Images | BMP, FPX, GIF, JPEG, JPG, PNG, PICT (Windows® uniquement), TIF, TIFF |
| InDesign | INDD, INDT |
| MS® Office | DOC, PPT, RTF, XLS |
| PDF | PDF |
| Photoshop | PSD, FXG et Camera Raw |
| Postscript | EPS, PS |
| Création d’images Adobe Dynamic Media Classic | VNC, VNT, VNW |
| SVG | SVG, SVGX |
| TAR | TAR |
| Vidéo | 3GP, AVI, M2P, M2T, M2TS, M2V, M4V, MOV, MP4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF |
| XML | XML |
| ZIP | ZIP |

La fonction de transfert au format TAR et ZIP offre une case à cocher permettant d’indiquer si vous souhaitez décompresser les fichiers.

### Formats d’image non pris en charge dans Dynamic Media {#unsupported-image-formats-dynamic-media}

La liste suivante décrit les sous-types de formats de fichiers image pixellisés *et non* pris en charge dans Dynamic Media.

Voir aussi [Détecter les formats de fichiers non pris en charge pour Dynamic Media](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html).

* Fichiers PNG dont la taille de bloc IDAT est supérieure à 100 Mo.
* Fichiers PSB.
* Les fichiers de PSD avec un espace colorimétrique autre que CMJN, RGB, Niveaux de gris ou Bitmap ne sont pas pris en charge. Les espaces colorimétriques DuoTone, Lab et indexé ne sont pas pris en charge.
* Fichiers de PSD dont la profondeur est supérieure à 16.
* Fichiers de TIFF contenant des données à virgule flottante.
* Fichiers de TIFF dotés d’un espace colorimétrique Lab.

### Types de ressource {#asset-types}

Pour obtenir des résultats optimaux avec le programme Adobe Dynamic Media Classic, veillez à utiliser les formats et tailles de fichier recommandés. Ce tableau répertorie les types de fichiers, dont certains avec les formats et tailles recommandés pour les fichiers couramment utilisés.

| Type de fichier | Description/Recommandations |
| --- | --- |
| Audio | Les formats de fichiers audio entrants incluent AAC, HE-AAC, AC3, WAV, WMA, AIFF et MP3. Vous pouvez transcoder du contenu audio aux formats suivants : MP3, AAC et HE-AAC. |
| Images (pour le dimensionnement des images, le zoom, les visionneuses d’images, les visionneuses à 360°) | Les images doivent mesurer au moins 2 000 pixels à la taille la plus longue ; les tailles d’image standard sont comprises entre 1 500 et 2 500 pixels à la taille la plus longue. Les formats d’image sans perte, notamment TIFF et PNG, sont recommandés. Avec une image JPEG, utilisez les paramètres de qualité les plus élevés. Les fichiers de GIF animés sont gérés comme tout autre contenu statique. |
| Catalogues électroniques | Utilisez des fichiers PDF haute résolution créés dans Adobe Acrobat ou une application de Creative Suite d’Adobe enregistrée en tant que &quot;presready&quot;. Les PDF comprennent toutes les polices, images et masques nécessaires. Incluez également tous les éléments graphiques référencés nécessaires, sous la forme de pages simples, de planches de deux pages ou dans un format multi-page. Organisez les pages en nommant les fichiers selon un ordre alphanumérique. Placez tous les fichiers PDF du catalogue électronique dans un dossier unique en vue de faciliter le téléchargement. Vous pouvez sélectionner des options de recadrage lors du téléchargement afin de supprimer la zone de rognage des fichiers PDF, notamment les traits de coupe, les repères de montage ou les gammes de couleurs. La plupart des fichiers PDF « bon à tirer » sont caractérisés par l’espace colorimétrique CMJN ; il est donc important d’obtenir le profil colorimétrique ICC CMJN utilisé avec vos fichiers PDF. |
| Modèles | Image superposée ou disposition pouvant inclure du texte, des images et des calques. Les calques d’image, les chaînes de texte et les attributs, comme la couleur et la taille, peuvent être paramétrés de manière à pouvoir personnaliser les données variables. Pour les modèles, les exigences sont les mêmes que pour les autres images. Préparez vos images dans Photoshop ou un autre éditeur d’images. Enregistrez chaque image sous forme de fichier transparent aplati au format TIFF ou PNG. Assurez-vous que la résolution de l’image est adaptée à l’utilisation qui en sera faite. Les images pour impression sont de 300 ppp. |
| Vidéos | Adobe Dynamic Media Classic prend en charge les fichiers vidéo enregistrés aux formats OGV et MP4. Vous pouvez transcoder des fichiers au format MP4 lors du téléchargement. Voir [Formats de fichiers pris en charge](#supported-static-file-formats). |
| Polices | Chargement des polices TrueType, `Type1` (Windows® uniquement), OpenType® et PhotoFonts. |
| Images | Images et fichiers d’images superposées. |
| Visionneuses d’images et séries d’échantillons | Ensemble d’images associées pouvant être affichées dans une visionneuse. |
| Profils ICC | Profil colorimétrique que vous pouvez utiliser pour convertir une image téléchargée depuis son espace colorimétrique source en un autre espace colorimétrique. |
| Vignettes | Images créées avec le programme de création d’images et les fichiers associés. |
| Fichiers de contenu | Fichiers de contenu Adobe InDesign, Illustrator ou Photoshop. |
| Fichiers FXG | Format de fichiers graphiques à résolution indépendante permettant de créer des modèles personnalisables en vue d’une sortie pour impression, Web, courrier électronique, ordinateur et appareils mobiles. |
| Fichiers SVG | Fichiers Scalable Vector Graphic dont le rendu peut être effectué par des serveurs Image Server. |
| Fichiers XML | Fichiers qui définissent les règles de prétraitement utilisées pour modifier les parties chemin (path) et interrogation (query) des requêtes. |
| Fichiers de feuille de style en cascade | Chargez des habillages CSS pour personnaliser les visionneuses HTML5. |
| Fichiers JavaScript | Les fichiers JavaScript sont utilisés pour que l’instrumentation de la visionneuse contienne des informations de compte. Adobe Security recommande ce type de ressource uniquement pour les comptes clients disposant d’un domaine distinct en cours d’utilisation pour la diffusion (afin d’éviter les scripts intersites). |

>[!NOTE]
>
>Lorsque vous chargez des fichiers image et des PDF vers Adobe Dynamic Media Classic, le système convertit ces fichiers source en fichiers de TIFF P (Pyramid TIFF). Ces TIFFs P sont les fichiers qui sont publiés ultérieurement sur les serveurs d’images Dynamic Media. Adobe Dynamic Media Classic utilise le format de fichier Pyramid Tiff , car il contient divers rapports de zoom qui permettent un zoom rapide lors de l’affichage à l’aide d’une visionneuse de zoom Adobe Dynamic Media Classic.

### Formats de fichier statique pris en charge {#supported-static-file-formats}

Adobe Dynamic Media Classic prend en charge plusieurs formats de fichiers statiques. Le contenu statique est toute ressource publiée &quot;en l’état&quot;, telle que CSS, PDF, SVG et XML.

Les types de fichier suivants peuvent être publiés :

* GIF animé
* Fichiers audio
* CSS
* JavaScript (lorsque l’entreprise est configurée avec son propre domaine)
* Vidéo Principal
* PDF (lorsque le PDF est marqué pour publication après le chargement, afin d’éviter la diffusion de tous les PDF pour le processus eCatalog/PDF existant)
* Vidéo PrX
* SVG
* XML
* ZIP

Adobe Dynamic Media Classic ne permet pas de générer une URL d’aperçu de contenu statique.

### Exigences relatives aux noms de fichiers {#filename-requirements}

Etant donné que l’extension est ôtée du nom du fichier durant le processus de téléchargement, le système ne permet pas que des fichiers présentent le même nom racine. Dans le système Adobe Dynamic Media Classic, le nom de fichier de la ressource moins l’extension devient l’identifiant de la ressource. C’est la raison pour laquelle deux fichiers ne peuvent pas avoir le même nom.

Assurez-vous que tous les utilisateurs de votre entreprise comprennent les règles suivantes pour nommer les fichiers :

* Les identifiants de ressources portant le même nom ne sont pas autorisés dans le système.
* Les noms d’ID de ressource sont sensibles à la casse.
* Il est recommandé de s’assurer que les ID de fichier ne contiennent pas d’espace (par exemple, veste noire.tif et veste bleue.jpg). Adobe Dynamic Media Classic code les espaces vides dans les noms de ressources à l’aide de noms de ressources pour créer des chaînes d’URL. Ces codes ASCII sont difficiles à lire, ce qui rend également plus difficile la lecture de ces chaînes.
* Les caractères spécifiques aux langues sont autorisés dans les noms de fichier, à l’exception des caractères suivants :

  `\ ; / ? : @ & = + $ , &#42; " &lt; > | ' { } %`

  Si un nom de fichier contient un ou plusieurs de ces caractères, ceux-ci sont supprimés du nom du fichier au moment du téléchargement.

En règle générale, un nom de fichier de ressource peut être identique à son numéro d’élément, à la référence du produit ou à un autre nom, comme dans l’exemple suivant :

| Article | Nom de fichier | ID de fichier |
| --- | --- | --- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Organisation et structure des dossiers {#folder-organization-and-structure}

Organisez et structurez les dossiers et les sous-dossiers de votre contenu dans Adobe Dynamic Media Classic avant de télécharger votre contenu vers le système. Cette procédure présente deux principaux avantages :

* Lorsque vous transférez votre contenu vers Adobe Dynamic Media Classic par FTP, vous pouvez indiquer au système de répliquer la structure de dossiers lors du transfert. Ainsi, votre contenu est organisé dans les mêmes dossiers et sous-dossiers dans Adobe Dynamic Media Classic que sur votre ordinateur ou votre réseau. (Pour répliquer la structure de dossiers dans Adobe Dynamic Media Classic, sélectionnez l’option Inclure les sous-dossiers lorsque vous chargez des ressources par FTP.)
* La réorganisation des dossiers au sein du système, une fois les fichiers téléchargés, s’avère beaucoup plus difficile que le démarrage avec une structure de dossiers soigneusement étudiée.

L’approche et la structure de nommage de dossiers que vous choisissez pour stocker votre contenu dans Adobe Dynamic Media Classic dépendent des besoins de votre entreprise. Voici quelques exemples de structure de dossiers :

**Basé sur un SKU** : les dossiers sont nommés en fonction des SKU ou des numéros d’éléments. Par exemple, des dossiers distincts sont créés pour toutes les séries 0, 20 et 30.

**Marque basée sur** : pour les fabricants disposant de plusieurs marques et les détaillants qui commercialisent d’autres marques d’autres sociétés, séparez les fichiers en dossiers de produits nommés pour différentes marques.

**Basé sur un projet** : les dossiers sont organisés en fonction de la date de déploiement/de dépôt ou du nom du projet. Les clients qui produisent principalement des catalogues électroniques favorisent cette approche.

**Miroir de la hiérarchie de dossiers du site web** : cette structure de dossiers reflète la structure de dossiers du site web, avec les dossiers nommés, par exemple, pour les catégories de produits.

## A propos du téléchargement de fichiers {#uploading-your-files}

Vous pouvez télécharger des fichiers individuels à partir du bureau ou des dossiers par FTP. Si vous souhaitez télécharger plus de 100 Mo de fichiers ou des dossiers et sous-dossiers entiers, sélectionnez l’onglet **VIA FTP** .

Adobe Dynamic Media Classic vous envoie un e-mail pour confirmer le début et la fin de votre tâche de téléchargement et vous informer des problèmes éventuels.

Au cours (ou immédiatement après) d’une tâche de téléchargement volumineuse, certains nouveaux éléments peuvent afficher le message &quot;Image non encore optimisée&quot;. Ce message s’affiche, car les fichiers ne sont pas encore entièrement traités et ajoutés à Adobe Dynamic Media Classic. Vous pouvez optimiser ces fichiers ultérieurement Voir [Optimisation des fichiers](application-setup.md#optimize_files).

### Chargement de fichiers à l’aide de l’onglet De bureau {#upload-files-using-sps-desktop-application}

L’application de bureau Adobe Dynamic Media Classic vous permet de télécharger des fichiers et des dossiers par glisser-déposer.

1. Dans l’application de bureau Adobe Dynamic Media Classic, dans la barre de navigation globale, sélectionnez **[!UICONTROL Télécharger]**.
1. Sur la page Télécharger , sélectionnez l’onglet **[!UICONTROL Depuis le bureau]** .
1. Sur le côté gauche de la page Télécharger, dans la zone **[!UICONTROL Sélectionner les fichiers à télécharger]**, sélectionnez **[!UICONTROL Parcourir]** pour sélectionner les fichiers ou les dossiers à télécharger, puis sélectionnez **[!UICONTROL Ouvrir]**.
1. Sur le côté droit de la page Télécharger, dans la zone sélectionnée **Destination du dossier**, accédez à un dossier de destination où vous souhaitez que les fichiers ou dossiers chargés soient ajoutés.
1. (Facultatif) Près du bas de la page Télécharger, dans le champ de texte Nom de la tâche , saisissez le nouveau nom de la tâche de téléchargement. Vous pouvez également utiliser le nom généré par le système par défaut fourni par Adobe Dynamic Media Classic. Les tâches de téléchargement et de publication sont enregistrées sur la page Tâches, où vous pouvez vérifier l’état des tâches. (voir [Vérification de fichiers de tâche](checking-job-files.md#checking_job_files)).
1. (Facultatif) Près du bas de la page Télécharger, sélectionnez **[!UICONTROL Publish After Uploading]** afin de pouvoir publier automatiquement les ressources que vous chargez.
Lorsque vous publiez des fichiers, ils sont envoyés aux serveurs connectés. Les URL de ces fichiers peuvent alors être utilisées sur des sites Web et des applications externes. Cette même option est également disponible dans la boîte de dialogue Options de tâche.
1. (Facultatif) Près du bas de la page Télécharger, sélectionnez **[!UICONTROL Écraser dans un dossier, même nom de fichier, extension indépendante]** si vous souhaitez que les fichiers que vous téléchargez remplacent les fichiers existants portant le même nom. Cette même option est également disponible dans la boîte de dialogue Options de tâche.
Le nom de cette option peut être différent, selon les paramètres définis dans **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres généraux]** > **[!UICONTROL Télécharger vers l’application]** > **[!UICONTROL Remplacer les images]**.
1. Près du coin inférieur droit de la page Télécharger, sélectionnez **[!UICONTROL Options de tâche]**, puis spécifiez les options de votre choix.

   Voir [Options de téléchargement](uploading-files.md#upload_options).

1. Dans la boîte de dialogue Télécharger les options de la tâche, sélectionnez **[!UICONTROL Enregistrer]**.
1. Dans le coin inférieur droit de la page Télécharger, sélectionnez **[!UICONTROL Submit Upload]**.
Pour afficher la progression du chargement, sélectionnez **[!UICONTROL Tâches]** dans la barre de navigation globale. Vous pouvez continuer à travailler dans Adobe Dynamic Media Classic. Revenez à tout moment à la page Tâches pour consulter une tâche en cours. Pour annuler une tâche de téléchargement en cours, cliquez sur **[!UICONTROL Annuler]** en regard de la durée.

### Chargement de fichiers à l’aide de l’onglet FTP via {#upload-files-using-via-ftp}

1. Connectez-vous au site FTP Adobe Dynamic Media Classic spécifique à votre région. Utilisez le nom d’utilisateur et le mot de passe FTP qui vous ont été envoyés par votre administrateur.
1. Dans Adobe Dynamic Media Classic, sur la barre de navigation globale, sélectionnez **[!UICONTROL Télécharger]**.
1. Sur la page Télécharger , sélectionnez l’onglet **[!UICONTROL VIA FTP]** .
1. Sur le côté gauche de la page Télécharger, dans la zone **[!UICONTROL Choisir le dossier FTP à télécharger]**, sélectionnez un dossier FTP à partir duquel télécharger les fichiers.
1. Sur le côté droit de la page Télécharger, dans la zone **[!UICONTROL Adobe Dynamic Media Folder Destination]** sélectionnée, sélectionnez un dossier de destination dans Adobe Dynamic Media Classic.
1. (Facultatif) Près du bas de la page Télécharger, dans le champ de texte Nom de la tâche , saisissez le nouveau nom de la tâche de téléchargement. Vous pouvez également utiliser le nom généré par le système par défaut fourni par Adobe Dynamic Media Classic. Les tâches de téléchargement et de publication sont enregistrées sur la page Tâches, où vous pouvez vérifier l’état des tâches.
(voir [Vérification de fichiers de tâche](checking-job-files.md#checking_job_files)).
1. (Facultatif) Près du bas de la page Télécharger, sélectionnez **[!UICONTROL Publish After Upload]** afin de pouvoir publier automatiquement les ressources que vous chargez.
Lorsque vous publiez des fichiers, ils sont envoyés aux serveurs connectés. Les URL de ces fichiers peuvent alors être utilisées sur des sites Web et des applications externes. Cette même option est également disponible dans la boîte de dialogue Options de tâche.
1. (Facultatif) Près du bas de la page Télécharger, sélectionnez **[!UICONTROL Écraser dans un dossier, même nom de fichier, extension indépendante]** si vous souhaitez que les fichiers que vous téléchargez remplacent les fichiers existants portant le même nom. Cette même option est également disponible dans la boîte de dialogue Options de tâche.
Le nom de cette option peut être différent, selon les paramètres définis dans **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres généraux]** > **[!UICONTROL Télécharger vers l’application]** > **[!UICONTROL Remplacer les images]**.
1. Facultatif ; disponible uniquement si vous avez sélectionné l’onglet **[!UICONTROL VIA FTP]**. Près du bas de la page Télécharger, sélectionnez **[!UICONTROL Décompresser les fichiers ZIP ou tar lors du téléchargement]** afin que vous puissiez extraire automatiquement tous les fichiers de votre fichier ZIP ou TAR chargé. Cette même option est également disponible dans la boîte de dialogue Options de tâche.
1. Près du coin inférieur droit de la page Télécharger, sélectionnez **[!UICONTROL Options de tâche]**, puis spécifiez les options de votre choix.

   Voir [Options de téléchargement](uploading-files.md#upload_options).

1. Dans la boîte de dialogue Télécharger les options de la tâche, sélectionnez **[!UICONTROL Enregistrer]**.
1. Dans le coin inférieur droit de la page Télécharger, sélectionnez **[!UICONTROL Submit Upload]**.

   Pour afficher la progression du chargement, dans la barre de navigation globale, sélectionnez **[!UICONTROL Tâches]**. La page Tâches présente la progression du téléchargement. Vous pouvez continuer à travailler dans Adobe Dynamic Media Classic. Revenez à tout moment à la page Tâches pour consulter une tâche en cours.

Pour annuler une tâche de téléchargement en cours, cliquez sur **[!UICONTROL Annuler]** en regard de la durée.

## Boîte de dialogue Télécharger les options de la tâche {#upload-options}

Lors du téléchargement de fichiers, vous pouvez choisir l’une des options suivantes dans la boîte de dialogue Télécharger les options de la tâche :

* **JOB** : sélectionnez **[!UICONTROL JOB]** pour choisir les options qui affectent l’ensemble de la tâche de téléchargement.

  Vous pouvez également choisir les options *default* pour télécharger des tâches à l’aide de la boîte de dialogue **[!UICONTROL Default Upload Options]** dans Paramètres généraux. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres généraux]** > **[!UICONTROL Options de téléchargement par défaut]**, puis définissez les options par défaut de votre choix.

   * **[!UICONTROL When]** : cette option n’est disponible que si vous avez sélectionné l’onglet **[!UICONTROL VIA FTP]**.
      * **[!UICONTROL Unique]** : spécifiez une tâche de téléchargement qui s’exécute une fois. Les options disponibles sont les suivantes :
         * **[!UICONTROL Maintenant]** : exécute la tâche de téléchargement immédiatement après avoir sélectionné **[!UICONTROL Enregistrer]** dans la boîte de dialogue Télécharger les options de la tâche, puis sélectionnez **[!UICONTROL Envoyer le téléchargement]** sur la page de téléchargement.
         * **[!UICONTROL Planifier pour plus tard]** : sélectionnez l’année, le mois, le jour et l’heure (par incréments de 15 minutes) que vous souhaitez que la tâche de téléchargement s’exécute.
      * **[!UICONTROL Récurrent]** : spécifiez une tâche de téléchargement qui s’exécute tous les jours, toutes les semaines ou tous les mois. Vous pouvez également personnaliser la tâche de chargement selon vos propres spécifications.
         * **[!UICONTROL Quotidien]** : définissez l’heure d’exécution de la tâche tous les jours. Si vous souhaitez que la tâche s’exécute uniquement du lundi au vendredi, sélectionnez **[!UICONTROL Jours de semaine uniquement]**.
         * **[!UICONTROL Hebdomadaire]** : choisissez un jour spécifique de la semaine et l’heure d’exécution de la tâche.
         * **[!UICONTROL Mensuel]** : sélectionnez un jour spécifique du mois ou du jour de la semaine, y compris l’heure de début, que vous souhaitez que la tâche s’exécute.
         * **[!UICONTROL Personnalisé]** : personnalisez un intervalle de temps de tâche de téléchargement ou de publication selon vos propres spécifications. Voir [Création d’un intervalle de temps de tâche de téléchargement ou de publication personnalisé](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).

   * **[!UICONTROL Publish After Uploading]** : disponible si vous avez sélectionné l’onglet **[!UICONTROL FROM BUKTOP]** ou l’onglet **[!UICONTROL VIA FTP]**. Sélectionnez cette option pour publier automatiquement les ressources que vous chargez. Lorsque vous publiez des fichiers, ils sont envoyés aux serveurs connectés. Les URL de ces fichiers peuvent alors être utilisées sur des sites Web et des applications externes. Cette option est également disponible sur la page de téléchargement.

   * **[!UICONTROL Écraser dans un dossier, même nom de ressource de base, extension indépendante]** : disponible si vous avez sélectionné l’onglet **[!UICONTROL FROM DESKTOP]** ou l’onglet **[!UICONTROL VIA FTP]**. Permet de remplacer des fichiers existants portant le même nom que les fichiers que vous téléchargez. Cette option est également disponible sur la page de téléchargement. Le nom de cette option peut être différent, selon les paramètres définis dans **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres généraux]** > **[!UICONTROL Télécharger vers l’application]** > **[!UICONTROL Remplacer les images]**.

   * **[!UICONTROL Décompresser les fichiers ZIP ou Tar lors du téléchargement]** : ce paramètre est disponible si vous avez sélectionné l’onglet **[!UICONTROL DEPUIS LE BUREAU]** ou l’onglet **[!UICONTROL VIA FTP]**.
Sélectionnez cette option pour extraire automatiquement tous les fichiers de votre fichier ZIP ou TAR chargé. Cette même option est également disponible dans la boîte de dialogue Options de tâche.

   * **[!UICONTROL Inclure les sous-dossiers]** : disponible uniquement si vous avez sélectionné l’onglet **[!UICONTROL VIA FTP]**.
Permet de télécharger les sous-dossiers du dossier que vous avez l’intention de télécharger. Les noms du dossier et de ses sous-dossiers que vous chargez sont automatiquement renseignés dans Adobe Dynamic Media Classic.

   * **[!UICONTROL Traiter les fichiers de métadonnées]** : disponible uniquement si vous avez sélectionné l’onglet **[!UICONTROL VIA FTP]**. Sélectionnez cette option si vous souhaitez charger un fichier XML ou délimité par des tabulations afin d’ajouter des métadonnées à plusieurs ressources.
Voir [Importer des métadonnées (via FTP)](viewing-adding-exporting-metadata.md#import-metadata).

* **Options de recadrage** : recadrez automatiquement les pixels d’espace blanc d’une image. Ouvrez le menu **[!UICONTROL Recadrer]**, sélectionnez **[!UICONTROL Manuel]** et saisissez des mesures en pixels dans les champs de texte Haut, Droite, Bas et Gauche pour recadrer depuis les côtés. Vous pouvez également sélectionner **[!UICONTROL Rogner]** dans le menu Recadrer et choisir les options suivantes :

   * **[!UICONTROL Rogner en fonction de]** : choisissez si vous souhaitez recadrer en fonction de la couleur ou de la transparence :
      * **[!UICONTROL Color]** : choisissez l’option Color. Sélectionnez ensuite le menu Coin et choisissez l’angle de l’image dont la couleur représente le mieux l’espace blanc que vous souhaitez recadrer.
Rognage en fonction de la couleur : indiquez 0 pour rogner uniquement les pixels qui correspondent exactement à la couleur sélectionnée dans le coin de l’image. Les valeurs qui se rapprochent de 1 admettent un plus grand écart des couleurs.
      * **[!UICONTROL Transparence]** : sélectionnez l’option **[!UICONTROL Transparence]** .
Rognage en fonction de la transparence : indiquez 0 pour rogner les pixels seulement s’ils sont transparents ; les nombres plus proches de 1 permettent une plus grande transparence.
      * **[!UICONTROL Tolérance]** : faites glisser le curseur pour spécifier une tolérance comprise entre 0 et 1.

* **Options de profil colorimétrique** : choisissez une conversion de couleurs lorsque vous créez des fichiers optimisés utilisés pour la diffusion dynamique Adobe Dynamic Media Classic :

   * **[!UICONTROL Conservation des couleurs par défaut]** : conserve les couleurs de l’image source chaque fois que les images contiennent des informations sur l’espace colorimétrique ; il n’y a pas de conversion des couleurs. Pour la plupart des images aujourd’hui, un profil colorimétrique approprié est déjà inclus. Toutefois, si une image source CMJN ne contient pas de profil colorimétrique intégré, les couleurs sont converties dans l’espace colorimétrique sRVB (rouge vert bleu standard). sRVB est l’espace colorimétrique recommandé pour l’affichage des images sur les pages Web.
   * **[!UICONTROL Conserver l’espace colorimétrique d’origine]** : conserve les couleurs d’origine sans conversion des couleurs au moment de l’ingestion dans Adobe Dynamic Media Classic. Pour les images sans profil colorimétrique incorporé, toute conversion de couleur requise pour traiter les demandes de l’image est effectuée à l’aide des profils colorimétriques par défaut configurés dans les paramètres de publication. Ces profils de couleurs ne correspondent pas toujours aux couleurs des fichiers créés avec cette option. Par conséquent, vous avez intérêt à utiliser l’option de conservation des couleurs par défaut.
   * **[!UICONTROL Personnalisé de]** > **[!UICONTROL À]** : ouvre les menus pour vous permettre de choisir un espace colorimétrique **[!UICONTROL Convertir à partir de]** et **[!UICONTROL Convertir en]**. Cette option avancée remplace toutes les informations de couleur incorporées dans le fichier source. Sélectionnez cette option uniquement lorsque toutes les images que vous envoyez contiennent des données de profil colorimétrique incorrectes ou manquantes.

* **Options de modification d’image** : vous pouvez conserver les masques &lt;> d’écrêtage dans les images et choisir un profil colorimétrique.
Voir [Options d’optimisation des images lors du téléchargement](image-editing-options-upload.md#image-editing-options-at-upload).

* **Options PostScript®** : vous pouvez pixelliser des fichiers PostScript®, recadrer des fichiers, conserver des arrière-plans transparents, choisir une résolution et choisir un espace colorimétrique.
Voir [Utilisation de fichiers PostScript et Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Options Photoshop** : vous pouvez créer des modèles à partir de fichiers Adobe® Photoshop®, conserver les calques, spécifier le mode de nommage des calques, extraire du texte et spécifier le mode d’ancrage des images dans les modèles.
(voir [Options de téléchargement des fichiers PSD](psd-files.md#psd_upload_options)).

* **Options de PDF** : vous pouvez pixelliser les fichiers, extraire des mots de recherche et des liens, générer automatiquement un catalogue électronique, définir la résolution et choisir un espace colorimétrique.
(voir [Options de téléchargement des fichiers PDF](pdfs.md#pdf_upload_options)).

* **Options Illustrator** : vous pouvez pixelliser les fichiers Adobe Illustrator®, conserver les arrière-plans transparents, choisir une résolution et choisir un espace colorimétrique.
Voir [Utilisation de fichiers PostScript et Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Options EVIDEO** : vous pouvez transcoder un fichier vidéo en choisissant un paramètre vidéo prédéfini.
Voir [Utilisation des paramètres prédéfinis de codage vidéo](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **Plus de métadonnées** : entrez des mots-clés qui décrivent les fichiers que vous avez l’intention de charger. Séparez les mots clés-par des virgules. Les mots-clés facilitent la recherche de ressources.
Voir [Réaliser une recherche avancée](searching-assets.md#conducting_an_advanced_search).
Voir également la vidéo de formation [Téléchargement de mots-clés](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/548_upload-keywords_converted%20renamed_Done-AVS).

* **Paramètres prédéfinis d’ensemble par lot** : pour créer une visionneuse d’images, une visionneuse à 360° ou une série d’échantillons à partir des fichiers transférés, sélectionnez la colonne **[!UICONTROL Actif]** correspondant au paramètre prédéfini que vous souhaitez utiliser. Rien ne vous empêche de sélectionner plusieurs paramètres prédéfinis. Vous pouvez créer les paramètres prédéfinis sur la page Configuration de l’application/Paramètres prédéfinis d’ensemble par lot .
(voir [Paramètres prédéfinis d’ensemble par lot](application-setup.md#batch_set_presets)).

* **Avancé** : voir [Suivre un téléchargement avec une autre tâche](uploading-files.md#follow-an-upload-with-another-job).

## Enchaînement d’une tâche de téléchargement et d’une autre tâche {#follow-an-upload-with-another-job}

Lorsque vous transférez des éléments par FTP, vous pouvez planifier une tâche ultérieure qui commencera une fois le transfert terminé. Si d’autres tâches sont planifiées pour commencer, les tâches que vous programmez ici sont mises en file d’attente après elles.

La nouvelle tâche envoie une notification à l’adresse que vous spécifiez afin que le code à cet emplacement puisse être déclenché. Cette tâche de publication consécutive reprend le nom de la tâche de téléchargement, mais ajoute *Pub_* devant le nom.

**Pour suivre un téléchargement avec une autre tâche :**

1. Sélectionnez **[!UICONTROL Télécharger]**, puis sélectionnez l’onglet **[!UICONTROL VIA FTP]**.
1. Dans le coin inférieur droit de la page Télécharger, sélectionnez **[!UICONTROL Options de tâche]**.
1. Dans la boîte de dialogue Télécharger les options de la tâche, développez la section **[!UICONTROL AVANCÉ]** .
1. Sélectionnez l’une des options suivantes dans la liste déroulante **[!UICONTROL Suivre le téléchargement avec une autre tâche]** :

   * Aucun
   * Requête HTTP
   * Publication sur hébergeur d’images
   * Publication de rendu d’image
   * Publication de vidéo

1. Spécifiez l’adresse HTTP.
1. Indiquez si vous souhaitez exécuter uniquement si des fichiers ont été chargés.
1. Indiquez si vous souhaitez exécuter cette requête chaque fois que cette tâche se termine ou uniquement lorsque les fichiers ont été publiés.

   >[!NOTE]
   >
   >Les tâches planifiées régulièrement peuvent parfois empêcher la publication de fichiers.

>[!MORELIKETHIS]
>
>* [ Utilisation de dossiers de ressources](asset-folders.md#working_with_asset_folders)
>* [Gérer les tâches de chargement et de publication récurrentes](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Utiliser une tâche de téléchargement ou de publication comme déclencheur](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)
