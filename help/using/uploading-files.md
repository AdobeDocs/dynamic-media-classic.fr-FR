---
title: Téléchargement de fichiers
description: Découvrez comment télécharger des fichiers dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
topic: Content Management
level: Intermediate
source-git-commit: 1cd516119da23f5ef4c0195273025ddd4b3fa789
workflow-type: tm+mt
source-wordcount: '3858'
ht-degree: 25%

---

# Téléchargement de fichiers{#uploading-files}

Avant de charger des fichiers de ressources vers Adobe Dynamic Media Classic, assurez-vous qu’ils sont correctement nommés. Assurez-vous également que la structure de dossiers est configurée et organisée comme vous le souhaitez. Vous pouvez télécharger des fichiers à partir d’un site FTP fourni par Adobe Dynamic Media Classic ou directement depuis votre ordinateur ou votre réseau. Adobe Dynamic Media Classic propose des options pour optimiser les fichiers au fur et à mesure de leur chargement. Si vous avez installé l’application de bureau Adobe Dynamic Media Classic, vous pouvez charger des fichiers et des dossiers en les faisant glisser directement depuis votre bureau. (voir [Paramètres généraux de l’application](application-setup.md#general_settings)).

## Préparation du chargement de vos ressources et dossiers {#preparing-your-assets-and-folders-for-uploading}

Avant de charger des ressources vers Adobe Dynamic Media Classic, assurez-vous qu’elles sont au format et à la taille appropriés. Vous devez également respecter les règles d’Adobe Dynamic Media Classic pour nommer les ressources. La définition d’une organisation et d’une structure de dossiers pour les fichiers garantit une facilité de localisation et d’utilisation de ces derniers.

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

### Formats d’image non pris en charge par Dynamic Media {#unsupported-image-formats-dynamic-media}

La liste suivante décrit les sous-types de formats de fichiers d’images pixellisées qui ne sont *pas* pris en charge dans Dynamic Media.

* Fichiers PNG dont la taille du bloc IDAT est supérieure à 100 Mo.
* Fichiers PSB.
* Les fichiers PSD dont l’espace colorimétrique est différent de CMJN, RGB, Niveaux de gris ou Bitmap ne sont pas pris en charge. Les espaces colorimétriques DuoTone, Lab et Indexed ne sont pas pris en charge.
* Fichiers PSD dont la profondeur est supérieure à 16.
* Fichiers TIFF contenant des données à virgule flottante.
* Fichiers TIFF avec espace colorimétrique Lab.

### Types de ressource {#asset-types}

Pour obtenir des résultats optimaux avec le programme Adobe Dynamic Media Classic, veillez à utiliser les formats et tailles de fichiers recommandés. Ce tableau répertorie les types de fichiers, dont certains avec les formats et tailles recommandés pour les fichiers couramment utilisés.

| Type de fichier | Description/Recommandations |
| --- | --- |
| Audio | Les formats de fichiers audio entrants incluent AAC, HE-AAC, AC3, WAV, WMA, AIFF et MP3. Vous pouvez transcoder du contenu audio aux formats suivants : MP3, AAC et HE-AAC. |
| Images (pour le dimensionnement des images, le zoom, les visionneuses d’images, les visionneuses à 360°) | Les images doivent faire au moins 2 000 pixels pour la plus grande taille. Les tailles d’image standard vont de 1 500 à 2 500 pixels pour la plus grande taille. Les formats d’image sans perte, notamment TIFF et PNG, sont recommandés. Avec une image JPEG, utilisez les paramètres de qualité les plus élevés. Les fichiers GIF animés sont gérés comme tout autre contenu statique. |
| Catalogues électroniques | Utilisez des fichiers PDF haute résolution créés dans Adobe Acrobat ou une application Adobe Creative Suite enregistrée en tant que « Prêt pour l’impression ». Les fichiers PDF comprennent toutes les polices, images et masques nécessaires. De plus, incluez tous les éléments graphiques référencés nécessaires, que ce soit sous la forme de pages simples, de pages doubles ou d’un format de plusieurs pages. Organisez les pages en nommant les fichiers selon un ordre alphanumérique. Placez tous les fichiers PDF du catalogue électronique dans un dossier unique en vue de faciliter le téléchargement. Vous pouvez sélectionner des options de recadrage lors du téléchargement afin de supprimer la zone de rognage des fichiers PDF, notamment les traits de coupe, les repères de montage ou les gammes de couleurs. La plupart des fichiers PDF « bon à tirer » sont caractérisés par l’espace colorimétrique CMJN ; il est donc important d’obtenir le profil colorimétrique ICC CMJN utilisé avec vos fichiers PDF. |
| Modèles | Image superposée ou disposition pouvant inclure du texte, des images et des calques. Les calques d’image, les chaînes de texte et les attributs, comme la couleur et la taille, peuvent être paramétrés de manière à pouvoir personnaliser les données variables. Pour les modèles, les exigences sont les mêmes que pour les autres images. Préparez vos images dans Photoshop ou un autre éditeur d’images. Enregistrez chaque image sous forme de fichier transparent aplati au format TIFF ou PNG. Assurez-vous que la résolution de l’image est adaptée à l’utilisation qui en sera faite. Les images à imprimer sont de 300 ppp. |
| Vidéos | Adobe Dynamic Media Classic prend en charge les fichiers vidéo enregistrés aux formats OGV et MP4. Vous pouvez transcoder les fichiers au format MP4 lors du chargement. Voir [Formats de fichiers pris en charge](#supported-static-file-formats). |
| Polices | a téléchargé TrueType, `Type1` (Windows® uniquement), OpenType® fonts et PhotoFonts. |
| Images | Images et fichiers d’images superposées. |
| Visionneuses d’images et séries d’échantillons | Ensemble d’images associées pouvant être affichées dans une visionneuse. |
| Profils ICC | Profil colorimétrique que vous pouvez utiliser pour convertir une image chargée depuis son espace colorimétrique source dans un autre espace colorimétrique. |
| Vignettes | Images créées avec le programme de création d’images et les fichiers associés. |
| Fichiers de contenu | Fichiers de contenu Adobe InDesign, Illustrator ou Photoshop. |
| Fichiers FXG | Format de fichiers graphiques à résolution indépendante permettant de créer des modèles personnalisables en vue d’une sortie pour impression, Web, courrier électronique, ordinateur et appareils mobiles. |
| Fichiers SVG | Fichiers Scalable Vector Graphic dont le rendu peut être effectué par des serveurs Image Server. |
| Fichiers XML | Fichiers qui définissent les règles de prétraitement utilisées pour modifier les parties chemin (path) et interrogation (query) des requêtes. |
| Fichiers de feuille de style en cascade | Chargez les habillages CSS pour la personnalisation des visionneuses HTML5. |
| Fichiers JavaScript | Les fichiers JavaScript sont utilisés pour l’instrumentation de la visionneuse afin de contenir les informations de compte. La sécurité Adobe recommande ce type de ressource uniquement pour les comptes clients qui disposent d’un domaine distinct utilisé pour la diffusion (afin d’éviter le cross-site scripting). |

>[!NOTE]
>
>Lorsque vous téléchargez des fichiers image et PDF vers Adobe Dynamic Media Classic, le système convertit ces fichiers sources en fichiers P-TIFF (Pyramid TIFF). Ces fichiers P-TIFF sont les fichiers qui sont publiés ultérieurement sur les serveurs d’images Dynamic Media. Adobe Dynamic Media Classic utilise le format de fichier Pyramid Tiff, car il contient différents rapports de zoom qui permettent un zoom rapide lors de l’affichage avec une visionneuse de zoom Adobe Dynamic Media Classic.

### Formats de fichier statique pris en charge {#supported-static-file-formats}

Adobe Dynamic Media Classic prend en charge plusieurs formats de fichiers statiques. Le contenu statique désigne toute ressource publiée « en l’état », telle que CSS, PDF, SVG et XML.

Les types de fichier suivants peuvent être publiés :

* GIF animé
* Fichiers audio
* CSS
* JavaScript (lorsque l’entreprise est configurée avec son propre domaine)
* Principal vidéo
* PDF (lorsque PDF est marqué pour publication après le chargement, afin d’éviter la diffusion de tous les PDF pour le workflow de catalogue électronique/PDF existant)
* Vidéo PrX
* SVG
* XML
* ZIP

Adobe Dynamic Media Classic ne fournit pas la possibilité de générer une URL d’aperçu de contenu statique.

### Exigences relatives aux noms de fichiers {#filename-requirements}

Etant donné que l’extension est ôtée du nom du fichier durant le processus de téléchargement, le système ne permet pas que des fichiers présentent le même nom racine. Dans le système Adobe Dynamic Media Classic, le nom de fichier de la ressource moins l’extension de nom de fichier devient l’identifiant de la ressource. C’est la raison pour laquelle deux fichiers ne peuvent pas avoir le même nom.

Assurez-vous que tous les utilisateurs de votre entreprise comprennent ces règles pour nommer les fichiers :

* Les identifiants de ressources portant le même nom ne sont pas autorisés dans le système.
* Les noms des ID de ressources sont sensibles à la casse.
* Il est recommandé de s’assurer que les ID de fichier ne contiennent pas d’espace (par exemple, veste noire.tif et veste bleue.jpg). Adobe Dynamic Media Classic ASCII code les espaces vides dans les noms de ressources lorsqu’il utilise les noms de ressources pour construire des chaînes d’URL. Ces codes ASCII sont difficiles à lire, ce qui rend également plus difficile la lecture de ces chaînes.
* Les caractères spécifiques aux langues sont autorisés dans les noms de fichier, à l’exception des caractères suivants :

  `\ ; / ? : @ & = + $ , &#42; " &lt; > | ' { } %`

  Si un nom de fichier contient un ou plusieurs de ces caractères, ceux-ci sont supprimés du nom du fichier au moment du téléchargement.

En règle générale, un nom de fichier de ressource peut être identique à son numéro d’article, à son SKU de produit ou à tout autre nom, comme dans l’exemple suivant :

| Article | Nom de fichier | ID de fichier |
| --- | --- | --- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Organisation et structure des dossiers {#folder-organization-and-structure}

Organisez et structurez les dossiers et les sous-dossiers pour votre contenu dans Adobe Dynamic Media Classic avant de charger votre contenu dans le système. Cette procédure présente deux principaux avantages :

* Lorsque vous chargez votre contenu vers Adobe Dynamic Media Classic par FTP, vous pouvez demander au système de répliquer la structure de vos dossiers pendant le chargement. Ainsi, votre contenu est organisé dans les mêmes dossiers et sous-dossiers dans Adobe Dynamic Media Classic que sur votre ordinateur ou réseau. (Pour répliquer la structure de vos dossiers dans Adobe Dynamic Media Classic, sélectionnez l’option Inclure les sous-dossiers lorsque vous chargez des ressources par FTP.)
* La réorganisation des dossiers au sein du système, une fois les fichiers téléchargés, s’avère beaucoup plus difficile que le démarrage avec une structure de dossiers soigneusement étudiée.

L’approche et la structure de dénomination des dossiers que vous choisissez pour stocker votre contenu dans Adobe Dynamic Media Classic dépendent des besoins de votre entreprise. Voici quelques exemples de structure de dossiers :

**Basé sur les SKU** : les dossiers sont nommés en fonction des SKU ou des numéros d’élément. Par exemple, des dossiers distincts sont créés pour toutes les séries de numéros 0, 20 et 30.

**Basé sur les marques** : pour les fabricants disposant de plusieurs lignes de marque et les revendeurs qui commercialisent d’autres marques d’autres sociétés, séparez les fichiers dans des dossiers de produits nommés en fonction de différentes marques.

**Basé sur un projet** : les dossiers sont organisés en fonction de la date de déploiement/dépôt ou du nom du projet. Les clients qui produisent principalement des catalogues électroniques favorisent cette approche.

**Miroir de la hiérarchie des dossiers du site Web** : cette structure de dossiers reflète la structure de dossiers du site Web, avec les dossiers nommés, par exemple, pour les catégories de produits.

## À propos du chargement de fichiers {#uploading-your-files}

Vous pouvez charger des fichiers individuels à partir du bureau ou charger des dossiers par FTP. Si vous souhaitez charger plus de 100 Mo de fichiers ou charger des dossiers et sous-dossiers entiers, sélectionnez l’onglet **VIA FTP**.

Adobe Dynamic Media Classic vous envoie un e-mail pour confirmer le début et la fin de la tâche de chargement et vous informer de tout problème.

Pendant (ou immédiatement après) une tâche de chargement volumineuse, certains nouveaux éléments peuvent afficher le message « Image non encore optimisée ». Ce message s’affiche, car les fichiers ne sont pas encore entièrement traités et ajoutés à Adobe Dynamic Media Classic. Vous pouvez optimiser ces fichiers ultérieurement Voir [Optimisation des fichiers](application-setup.md#optimize_files).

### Chargez des fichiers à l’aide de l’onglet Depuis le bureau . {#upload-files-using-sps-desktop-application}

L’application Adobe Dynamic Media Classic Desktop vous permet de télécharger des fichiers et des dossiers en les faisant glisser.

1. Dans l’application de bureau Adobe Dynamic Media Classic, sur la barre de navigation générale, sélectionnez **[!UICONTROL Charger]**.
1. Sur la page Charger, sélectionnez l’onglet **[!UICONTROL À partir du bureau]**.
1. Sur le côté gauche de la page Charger, dans la zone **[!UICONTROL Sélectionner les fichiers à charger]**, sélectionnez **[!UICONTROL Parcourir]** pour sélectionner les fichiers ou les dossiers à charger, puis sélectionnez **[!UICONTROL Ouvrir]**.
1. Sur le côté droit de la page Charger, dans la zone choisie **Destination du dossier**, accédez à un dossier de destination où vous souhaitez ajouter les fichiers ou dossiers chargés.
1. (Facultatif) Près du bas de la page Charger, dans le champ de texte Nom de la tâche, saisissez le nouveau nom de la tâche de chargement. Vous pouvez également simplement utiliser le nom par défaut, généré par le système, fourni par Adobe Dynamic Media Classic. Les tâches de chargement et de publication sont enregistrées sur la page Tâches, où vous pouvez vérifier leur statut. (voir [Vérification de fichiers de tâche](checking-job-files.md#checking_job_files)).
1. (Facultatif) Près du bas de la page Charger, sélectionnez **[!UICONTROL Publier après le chargement]** afin de publier automatiquement les ressources que vous chargez.
Lorsque vous publiez des fichiers, ils sont envoyés aux serveurs connectés. Les URL de ces fichiers peuvent alors être utilisées sur des sites Web et des applications externes. Cette même option est également disponible dans la boîte de dialogue Options de tâche.
1. (Facultatif) Près du bas de la page Charger, sélectionnez **[!UICONTROL Remplacer dans n’importe quel dossier, même nom de ressource de base, indépendamment de l’extension]** si vous souhaitez que les fichiers chargés remplacent des fichiers existants portant les mêmes noms. Cette même option est également disponible dans la boîte de dialogue Options de tâche.
Le nom de cette option peut être différent en fonction des paramètres dans **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres généraux]** > **[!UICONTROL Télécharger dans l’application]** > **[!UICONTROL Remplacer les images]**.
1. Dans le coin inférieur droit de la page Charger, sélectionnez **[!UICONTROL Options de la tâche]** puis spécifiez les options de votre choix.

   Voir [Options de téléchargement](uploading-files.md#upload_options).

1. Dans la boîte de dialogue Charger les options de la tâche, sélectionnez **[!UICONTROL Enregistrer]**.
1. Dans le coin inférieur droit de la page Charger, sélectionnez **[!UICONTROL Lancer le chargement]**.
Pour afficher la progression du chargement, sélectionnez **[!UICONTROL Tâches]** dans la barre de navigation générale. Vous pouvez continuer à travailler dans Adobe Dynamic Media Classic. Revenez à tout moment à la page Tâches pour consulter une tâche en cours. Pour annuler une tâche de téléchargement en cours, cliquez sur **[!UICONTROL Annuler]** en regard de la durée.

### Télécharger des fichiers à l’aide de l’onglet VIA FTP {#upload-files-using-via-ftp}

1. Connectez-vous au site FTP d’Adobe Dynamic Media Classic spécifique à votre région. Utilisez le nom d’utilisateur et le mot de passe FTP qui vous ont été envoyés par votre administrateur.
1. Dans Adobe Dynamic Media Classic, sur la barre de navigation générale, sélectionnez **[!UICONTROL Charger]**.
1. Sur la page Charger , sélectionnez l’onglet **[!UICONTROL VIA FTP]** .
1. Sur le côté gauche de la page Charger, dans la zone **[!UICONTROL Choisir le dossier FTP pour le chargement]**, choisissez un dossier FTP à partir duquel charger les fichiers.
1. Sur le côté droit de la page Charger, dans la zone **[!UICONTROL Destination du dossier Dynamic Media Adobe]** choisie, choisissez un dossier de destination dans Adobe Dynamic Media Classic.
1. (Facultatif) Près du bas de la page Charger, dans le champ de texte Nom de la tâche, saisissez le nouveau nom de la tâche de chargement. Vous pouvez également simplement utiliser le nom par défaut, généré par le système, fourni par Adobe Dynamic Media Classic. Les tâches de chargement et de publication sont enregistrées sur la page Tâches, où vous pouvez vérifier leur statut.
(voir [Vérification de fichiers de tâche](checking-job-files.md#checking_job_files)).
1. (Facultatif) Près du bas de la page Charger, sélectionnez **[!UICONTROL Publier après le chargement]** afin de publier automatiquement les ressources que vous chargez.
Lorsque vous publiez des fichiers, ils sont envoyés aux serveurs connectés. Les URL de ces fichiers peuvent alors être utilisées sur des sites Web et des applications externes. Cette même option est également disponible dans la boîte de dialogue Options de tâche.
1. (Facultatif) Près du bas de la page Charger, sélectionnez **[!UICONTROL Remplacer dans n’importe quel dossier, même nom de ressource de base, indépendamment de l’extension]** si vous souhaitez que les fichiers chargés remplacent des fichiers existants portant les mêmes noms. Cette même option est également disponible dans la boîte de dialogue Options de tâche.
Le nom de cette option peut être différent en fonction des paramètres dans **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres généraux]** > **[!UICONTROL Télécharger dans l’application]** > **[!UICONTROL Remplacer les images]**.
1. Facultatif ; disponible uniquement si vous avez sélectionné l’onglet **[!UICONTROL VIA FTP]**. Près du bas de la page Charger, sélectionnez **[!UICONTROL Décompresser les fichiers ZIP ou Tar au chargement]** afin de pouvoir extraire automatiquement tous les fichiers de votre fichier ZIP ou TAR chargé. Cette même option est également disponible dans la boîte de dialogue Options de tâche.
1. Dans le coin inférieur droit de la page Charger, sélectionnez **[!UICONTROL Options de la tâche]** puis spécifiez les options de votre choix.

   Voir [Options de téléchargement](uploading-files.md#upload_options).

1. Dans la boîte de dialogue Charger les options de la tâche, sélectionnez **[!UICONTROL Enregistrer]**.
1. Dans le coin inférieur droit de la page Charger, sélectionnez **[!UICONTROL Lancer le chargement]**.

   Pour afficher la progression du chargement, sur la barre de navigation générale, sélectionnez **[!UICONTROL Tâches]**. La page Tâches présente la progression du téléchargement. Vous pouvez continuer à travailler dans Adobe Dynamic Media Classic. Revenez à tout moment à la page Tâches pour consulter une tâche en cours.

Pour annuler une tâche de téléchargement en cours, cliquez sur **[!UICONTROL Annuler]** en regard de la durée.

## Boîte de dialogue Charger les options de la tâche {#upload-options}

Lors du chargement de fichiers, vous pouvez choisir l’une des options suivantes dans la boîte de dialogue Charger les options de la tâche :

* **TÂCHE** : sélectionnez **[!UICONTROL TÂCHE]** pour choisir les options qui affectent l’ensemble de la tâche de chargement.

  Vous pouvez également choisir les options *par défaut* pour les tâches de chargement à l’aide de la boîte de dialogue **[!UICONTROL Options de chargement par défaut]** dans Paramètres généraux. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres généraux]** > **[!UICONTROL Options de chargement par défaut]**, puis définissez les options par défaut de votre choix.

   * **[!UICONTROL Quand]** : cette option est disponible uniquement si vous avez sélectionné l’onglet **[!UICONTROL VIA FTP]**.
      * **[!UICONTROL Une fois]** : spécifiez une tâche de chargement qui s’exécute une fois. Les options incluent les suivantes :
         * **[!UICONTROL Maintenant]** : exécute la tâche de chargement immédiatement après avoir sélectionné **[!UICONTROL Enregistrer]** dans la boîte de dialogue Options de la tâche de chargement, puis sélectionnez **[!UICONTROL Soumettre le chargement]** sur la page Charger.
         * **[!UICONTROL Planifier pour plus tard]** : sélectionnez l’année, le mois, le jour et l’heure (par incréments de 15 minutes) auxquels vous souhaitez que la tâche de chargement s’exécute.
      * **[!UICONTROL Récurrent]** : spécifiez une tâche de chargement qui s’exécute tous les jours, toutes les semaines ou tous les mois. Vous pouvez également personnaliser la tâche de chargement en fonction de vos propres spécifications.
         * **[!UICONTROL Quotidien]** : définissez l’heure à laquelle vous souhaitez que la tâche s’exécute tous les jours. Si vous souhaitez que le traitement s’exécute uniquement du lundi au vendredi, sélectionnez **[!UICONTROL Jours de la semaine uniquement]**.
         * **[!UICONTROL Hebdomadaire]** : sélectionnez le jour et l’heure de la semaine où vous souhaitez que la tâche s’exécute.
         * **[!UICONTROL Mensuel]** : sélectionnez un jour spécifique du mois ou de la semaine, y compris l’heure de début, pour l’exécution de la tâche.
         * **[!UICONTROL Personnalisé]** : personnalisez un intervalle de temps de tâche de chargement ou de publication selon vos propres spécifications. Voir [ Création d’un intervalle personnalisé de chargement ou de publication](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).

   * **[!UICONTROL Publier après le chargement]** : disponible si vous avez sélectionné l’onglet **[!UICONTROL À PARTIR DE L’ORDINATEUR DE BUREAU]** ou l’onglet **[!UICONTROL VIA FTP]**. Sélectionnez cette option pour publier automatiquement les ressources que vous chargez. Lorsque vous publiez des fichiers, ils sont envoyés aux serveurs connectés. Les URL de ces fichiers peuvent alors être utilisées sur des sites Web et des applications externes. Cette option est également disponible sur la page de téléchargement.

   * **[!UICONTROL Remplacer dans un dossier, même nom de ressource de base, quelle que soit l’extension]** : disponible si vous avez sélectionné l’onglet **[!UICONTROL À PARTIR DE L’ORDINATEUR DE BUREAU]** ou l’onglet **[!UICONTROL VIA FTP]**. Permet de remplacer des fichiers existants portant le même nom que les fichiers que vous téléchargez. Cette option est également disponible sur la page de téléchargement. Le nom de cette option peut être différent en fonction des paramètres dans **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres généraux]** > **[!UICONTROL Télécharger dans l’application]** > **[!UICONTROL Remplacer les images]**.

   * **[!UICONTROL Décompresser les fichiers Zip ou Tar lors du chargement]** : disponible si vous avez sélectionné l’onglet **[!UICONTROL À PARTIR DE L’ORDINATEUR DE BUREAU]** ou l’onglet **[!UICONTROL VIA FTP]**.
Sélectionnez cette option pour extraire automatiquement tous les fichiers de votre fichier ZIP ou TAR chargé. Cette même option est également disponible dans la boîte de dialogue Options de tâche.

   * **[!UICONTROL Inclure les sous-dossiers]** : disponible uniquement si vous avez sélectionné l’onglet **[!UICONTROL VIA FTP]**.
Permet de télécharger les sous-dossiers du dossier que vous avez l’intention de télécharger. Les noms du dossier et des sous-dossiers chargés sont saisis automatiquement dans Adobe Dynamic Media Classic.

   * **[!UICONTROL Traiter les fichiers de métadonnées]** : disponible uniquement si vous avez sélectionné l’onglet **[!UICONTROL VIA FTP]**. Sélectionnez cette option si vous souhaitez charger un fichier XML ou délimité par des tabulations pour ajouter des métadonnées à plusieurs ressources.
Voir [Importer des métadonnées (via FTP)](viewing-adding-exporting-metadata.md#import-metadata).

* **Options de recadrage** : recadrez automatiquement les pixels d’espace blanc d’une image. Ouvrez le menu **[!UICONTROL Recadrage]**, sélectionnez **[!UICONTROL Manuel]** et saisissez les mesures en pixels dans les champs de texte Haut, Droite, Bas et Gauche pour recadrer sur les côtés. Vous pouvez également sélectionner **[!UICONTROL Rogner]** dans le menu Recadrer et choisir les options suivantes :

   * **[!UICONTROL Rogner en fonction de]** : choisissez de recadrer en fonction de la couleur ou de la transparence :
      * **[!UICONTROL Couleur]** : sélectionnez l’option Couleur. Sélectionnez ensuite le menu Coin et choisissez l’angle de l’image présentant la couleur qui correspond le mieux à l’espace blanc à rogner.
Rognage en fonction de la couleur : spécifiez 0 pour rogner les pixels uniquement s’ils correspondent exactement à la couleur que vous avez sélectionnée dans le coin de l’image. Les valeurs qui se rapprochent de 1 admettent un plus grand écart des couleurs.
      * **[!UICONTROL Transparence]** : sélectionnez l’option **[!UICONTROL Transparence]**.
Rognage en fonction de la transparence : spécifiez 0 pour rogner les pixels uniquement s’ils sont transparents ; les nombres plus proches de 1 permettent une plus grande transparence.
      * **[!UICONTROL Tolérance]** : faites glisser le curseur pour définir une tolérance comprise entre 0 et 1.

* **Options de profil colorimétrique** : sélectionnez une conversion de couleurs lors de la création de fichiers optimisés utilisés pour la diffusion dynamique d’Adobe Dynamic Media Classic :

   * **[!UICONTROL Conservation des couleurs par défaut]** : conserve les couleurs de l’image source chaque fois que les images contiennent des informations sur l’espace colorimétrique ; il n’y a pas de conversion des couleurs. Pour la plupart des images aujourd’hui, un profil colorimétrique approprié est déjà inclus. Toutefois, si une image source CMJN ne contient pas de profil colorimétrique intégré, les couleurs sont converties dans l’espace colorimétrique sRVB (rouge vert bleu standard). sRGB est l’espace colorimétrique recommandé pour afficher les images sur les pages web.
   * **[!UICONTROL Conserver l’espace colorimétrique d’origine]** : permet de conserver les couleurs d’origine sans conversion de couleurs au point d’ingestion dans Adobe Dynamic Media Classic. Pour les images sans profil colorimétrique incorporé, toute conversion de couleur requise pour traiter les demandes d’image est effectuée à l’aide des profils colorimétriques par défaut configurés dans les paramètres de publication. Ces profils de couleurs ne s’alignent pas toujours sur les couleurs des fichiers créés avec cette option. Par conséquent, vous avez intérêt à utiliser l’option de conservation des couleurs par défaut.
   * **[!UICONTROL Personnaliser à partir de]** > **[!UICONTROL Vers]** : ouvre les menus afin que vous puissiez choisir un espace colorimétrique **[!UICONTROL Convertir à partir de]** et **[!UICONTROL Convertir en]**. Cette option avancée remplace toutes les informations de couleur incorporées dans le fichier source. Sélectionnez cette option uniquement lorsque toutes les images que vous envoyez contiennent des données de profil de couleurs incorrectes ou manquantes.

* **Options d’édition de l’image** : vous pouvez conserver les masques &lt;> d’écrêtage dans les images et choisir un profil de couleurs.
Voir [Options de réglage d’image au moment du chargement](image-editing-options-upload.md#image-editing-options-at-upload).

* **Options PostScript®** : pixellisez des fichiers PostScript®, recadrez des fichiers, conservez les arrière-plans transparents, choisissez une résolution et choisissez un espace colorimétrique.
Voir [ Utilisation de fichiers PostScript et Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Options Photoshop** : vous pouvez créer des modèles à partir de fichiers Adobe® Photoshop®, conserver les calques, spécifier le mode de dénomination des calques, extraire du texte et spécifier le mode d’ancrage des images dans les modèles.
(voir [Options de téléchargement des fichiers PSD](psd-files.md#psd_upload_options)).

* **Options PDF** : pixellisez les fichiers, extrayez des mots de recherche et des liens, générez automatiquement un catalogue électronique, définissez la résolution et choisissez un espace colorimétrique.
(voir [Options de téléchargement des fichiers PDF](pdfs.md#pdf_upload_options)).

* **Options Illustrator** : pixellisez les fichiers Adobe Illustrator®, conservez les arrière-plans transparents, choisissez une résolution et choisissez un espace colorimétrique.
Voir [ Utilisation de fichiers PostScript et Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Options EVIDEO** : vous pouvez transcoder un fichier vidéo en choisissant un paramètre vidéo prédéfini.
Voir [ Utilisation de paramètres prédéfinis de codage vidéo](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **Plus de métadonnées** : entrez des mots-clés qui décrivent les fichiers que vous avez l’intention de télécharger. Séparez les mots clés-par des virgules. Les mots-clés facilitent la recherche de ressources.
Voir [Réalisation d’une recherche avancée](searching-assets.md#conducting_an_advanced_search).
Consultez également la vidéo de formation [Charger des mots-clés](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/548_upload-keywords_converted%20renamed_Done-AVS) .

* **Paramètres prédéfinis de lot** : pour créer une visionneuse d’images, à 360° ou une visionneuse d’échantillons à partir des fichiers chargés, sélectionnez la colonne **[!UICONTROL Actif]** du paramètre prédéfini à utiliser. Rien ne vous empêche de sélectionner plusieurs paramètres prédéfinis. Vous pouvez créer les paramètres prédéfinis dans la page Configuration de l’application/Paramètres prédéfinis d’ensemble par lot .
(voir [Paramètres prédéfinis d’ensemble par lot](application-setup.md#batch_set_presets)).

* **Avancé** : consultez la section [Suivre un chargement avec une autre tâche](uploading-files.md#follow-an-upload-with-another-job).

## Enchaînement d’une tâche de téléchargement et d’une autre tâche {#follow-an-upload-with-another-job}

Lorsque vous chargez des éléments via FTP, vous pouvez planifier une tâche ultérieure pour qu’elle commence une fois le chargement terminé. Si d’autres tâches sont planifiées pour commencer, les tâches que vous planifiez ici sont placées en file d’attente après elles.

Le nouveau traitement envoie une notification à l’adresse que vous spécifiez afin que le code de cet emplacement puisse être déclenché. Cette tâche de publication consécutive reprend le nom de la tâche de téléchargement, mais ajoute *Pub_* devant le nom.

**Pour suivre un chargement avec une autre tâche :**

1. Sélectionnez **[!UICONTROL Charger]**, puis sélectionnez l’onglet **[!UICONTROL VIA FTP]**.
1. Dans le coin inférieur droit de la page Charger, sélectionnez **[!UICONTROL Options de tâche]**.
1. Dans la boîte de dialogue Charger les options de la tâche, développez la section **[!UICONTROL AVANCÉ]**.
1. Sélectionnez l’une des options suivantes dans la liste déroulante **[!UICONTROL Suivre le chargement avec une autre tâche]** :

   * Aucun
   * Requête HTTP
   * Publication sur hébergeur d’images
   * Publication de rendu d’image
   * Publication de vidéo

1. Spécifiez l’adresse HTTP.
1. Indiquez si vous souhaitez exécuter uniquement si les fichiers ont été chargés.
1. Indiquez si vous souhaitez exécuter cette requête chaque fois que cette tâche se termine ou uniquement lorsque les fichiers ont été publiés.

   >[!NOTE]
   >
   >Les tâches planifiées régulièrement peuvent parfois entraîner l’absence de publication de fichiers.

>[!MORELIKETHIS]
>
>* [Utilisation des dossiers de ressources](asset-folders.md#working_with_asset_folders)
>* [Gérer les tâches récurrentes de chargement et de publication](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Utiliser une tâche de chargement ou de publication comme déclencheur](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)
