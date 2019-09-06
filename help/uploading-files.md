---
title: Téléchargement de fichiers
seo-title: Téléchargement de fichiers
description: 'null'
seo-description: Découvrez comment télécharger des fichiers.
uuid: b 3025 f 84-4 f 28-4276-bc 9 c-f 0 c 0 c 2 a 26 e 12
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: b 2 bc 3 bf 9-e 313-481 a -8670-c 3 bedde 21 b 1 a
translation-type: tm+mt
source-git-commit: 684950586bf9b1df897ac46b52d84a21f4cb4120

---


# Téléchargement de fichiers{#uploading-files}

Avant de télécharger des fichiers dans Scene7 Publishing System, assurez-vous que leur nom est correct et que la structure des dossiers est configurée et organisée selon vos souhaits. Vous pouvez télécharger des fichiers à partir d'un site FTP fourni par Dynamic Media Classic ou directement depuis votre ordinateur ou votre réseau. Dynamic Media Classic propose des options d'optimisation des fichiers au moment de leur téléchargement. Si vous avez installé l’application de bureau Scene7 Publishing System, vous pouvez télécharger des fichiers et des dossiers en les faisant glisser directement depuis votre bureau (voir [Paramètres généraux de l’application](application-setup.md#general_settings)).

## Préparation du téléchargement des fichiers et dossiers {#preparing-your-assets-and-folders-for-uploading}

Avant de télécharger des fichiers vers Scene7 Publishing System, vérifiez que leur format et leur taille sont corrects. Vous devez également respecter les règles Dynamic Media Classic pour nommer les fichiers. La définition d’une organisation et d’une structure de dossiers pour les fichiers garantit une facilité de localisation et d’utilisation de ces derniers.

### Formats de fichiers pris en charge {#supported-asset-file-formats}

Ce tableau dresse la liste des formats de fichiers pris en charge par le système de publication Scene7 For information on supported Camera Raw files, see [www.adobe.com/go/learn_s7_cameraraw_en](https://www.adobe.com/go/learn_s7_cameraraw_en).

| Formats de fichiers | Description |
|--- |--- |
| Audio | AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3 |
| Feuille de style en cascade | CSS |
| Profils colorimétriques | ICC, ICM |
| Polices | AFM, OTF, PFB, PFM, PhotoFont, TTC, TTF |
| FXG | FXG |
| Illustrator | AI, FXG |
| Images | BMP, FPX, GIF, JPEG, JPG, PNG, PICT (Windows uniquement), TIF, TIFF |
| InDesign | INDD, INDT |
| MS Office | DOC, PPT, RTF, XLS |
| PDF | PDF |
| Photoshop | PSD, FXG et Camera Raw |
| Postscript | EPS, PS |
| Dynamic Media Classic Image Authoring | VNC, VNT, VNW |
| SVG | SVG, SVGX |
| TAR | TAR |
| Vidéo | 3GP, AVI, M2P, M2T, M2TS, M2V, M4V, MOV, MP4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF |
| XML | XML |
| ZIP | ZIP |

La fonction de transfert au format TAR et ZIP offre une case à cocher permettant d’indiquer si vous souhaitez décompresser les fichiers.

### Types de ressource {#asset-types}

Pour obtenir des résultats optimaux avec la plate-forme Dynamic Media Classic, veillez à utiliser les formats et tailles recommandés. Ce tableau répertorie les types de fichiers, dont certains avec les formats et tailles recommandés pour les fichiers couramment utilisés.

| Type de fichier | Description/Recommandations |
|--- |--- |
| Audio | Les formats de fichiers audio entrants incluent AAC, HE-AAC, AC3, WAV, WMA, AIFF et MP3. Vous pouvez transcoder du contenu audio aux formats suivants : MP3, AAC et HE-AAC. |
| Images (pour le dimensionnement des images, le zoom, les visionneuses d’images, les visionneuses à 360°) | Les images doivent présenter au moins 2 000 pixels pour la dimension la plus longue ; la taille d’une image type est comprise entre 1 500 et 2 500 pixels pour la dimension la plus longue. Les formats d’image sans perte, notamment TIFF et PNG, sont recommandés. Avec une image JPEG, utilisez les paramètres de qualité les plus élevés. Les fichiers GIF animés sont traités comme un autre contenu statique. |
| Catalogues électroniques | Utilisez des fichiers PDF haute résolution créés dans Adobe® Acrobat® ou dans une application Creative Suite avec un enregistrement « bon à tirer ». Les fichiers PDF incluent l’ensemble des polices, images, masques et éléments graphiques référencés nécessaires, au format de page unique, de planche en double page ou de plusieurs pages. Organisez les pages en nommant les fichiers selon un ordre alphanumérique. Placez tous les fichiers PDF du catalogue électronique dans un dossier unique en vue de faciliter le téléchargement. Vous pouvez sélectionner des options de recadrage lors du téléchargement afin de supprimer la zone de rognage des fichiers PDF, notamment les traits de coupe, les repères de montage ou les gammes de couleurs. La plupart des fichiers PDF « bon à tirer » sont caractérisés par l’espace colorimétrique CMJN ; il est donc important d’obtenir le profil colorimétrique ICC CMJN utilisé avec vos fichiers PDF. |
| Modèles | Image superposée ou disposition pouvant inclure du texte, des images et des calques. Les calques d’image, les chaînes de texte et les attributs, comme la couleur et la taille, peuvent être paramétrés de manière à pouvoir personnaliser les données variables. Pour les modèles, les exigences sont les mêmes que pour les autres images. Préparez vos images dans Photoshop ou un autre éditeur d’images. Enregistrez chaque image sous forme de fichier transparent aplati au format TIFF ou PNG. Assurez-vous que la résolution de l’image est adaptée à l’utilisation qui en sera faite. Pour l’impression, elle doit être de 300 ppp. |
| Vidéos | Dynamic Media Classic prend en charge les fichiers vidéo enregistrés au format OGV et MP 4. Vous pouvez transcoder des fichiers au format MP 4 au moment du téléchargement. Voir [Formats de fichiers pris en charge](#supported-static-file-formats). |
| Polices | Polices TrueType, Type1 (Windows uniquement), OpenType et PhotoFonts téléchargées |
| Images | Images et fichiers d’images superposées. |
| Visionneuses d’images et séries d’échantillons | Ensemble d’images associées pouvant être affichées dans une visionneuse. |
| Profils ICC | Profil de couleur pouvant être utilisé pour convertir une image téléchargée depuis son espace colorimétrique source dans un autre espace colorimétrique. |
| Vignettes | Images créées avec le programme Image Authoring, ainsi que les fichiers associés. |
| Fichiers de contenu | Fichiers de contenu Adobe InDesign, Illustrator ou Photoshop. |
| Fichiers FXG | Format de fichiers graphiques à résolution indépendante permettant de créer des modèles personnalisables en vue d’une sortie pour impression, Web, courrier électronique, ordinateur et appareils mobiles. |
| Fichiers SVG | Fichiers Scalable Vector Graphic dont le rendu peut être effectué par des serveurs Image Server. |
| Fichiers XML | Fichiers qui définissent les règles de prétraitement utilisées pour modifier les parties chemin (path) et interrogation (query) des requêtes. |
| Fichiers de feuille de style en cascade | Téléchargez des habillages CSS pour personnaliser des visionneuses HTML5. |
| Fichiers JavaScript | Les fichiers Javascript sont utilisés à des fins d’instrumentalisation de la visionneuse pour conserver des informations sur le compte. Adobe Security recommande cette opération uniquement pour les comptes client qui utilisent un domaine distinct pour l’envoi (afin d’éviter d’utiliser un même script sur plusieurs sites). |

>[!NOTE]
>
>lorsque vous téléchargez des fichiers d’images et des fichiers PDF vers SPS, le système convertit ces fichiers sources en fichiers P-TIFF (Pyramid TIFF). Ces fichiers P-TIFF sont les fichiers publiés ultérieurement sur les serveurs d'images dynamiques de médias. Dynamic Media Classic utilise le format de fichier Pyramid TIFF, car il contient divers ratios de zoom permettant un zoom rapide lors de l'affichage avec une visionneuse de zoom classique Media Classic.

### Formats de fichier statique pris en charge {#supported-static-file-formats}

Dynamic Media Classic prend en charge plusieurs formats de fichier statique. Le contenu statique est tout fichier publié « en l'état », tel que CSS, PDF, SVG, XML, etc.

Les types de fichier suivants peuvent être publiés :

* GIF animé
* Fichiers audio
* CSS
* JavaScript (lorsque l’entreprise est configurée avec son propre domaine)
* Vidéo originale
* PDF (lorsque le fichier PDF est spécifiquement marqué pour publication après le téléchargement, afin d’éviter la diffusion de tous les fichiers PDF pour les flux de travaux de catalogue électronique/PDF existants)
* Vidéo PrX
* SVG
* XML
* ZIP

Dynamic Media Classic ne permet pas de générer une URL d'aperçu du contenu statique.

### Exigences relatives aux noms de fichiers {#filename-requirements}

Etant donné que l’extension est ôtée du nom du fichier durant le processus de téléchargement, le système ne permet pas que des fichiers présentent le même nom racine. Dans le système Dynamic Media Classic, le nom du fichier de ressource, moins l'extension du fichier, devient l'ID de fichier du fichier. C’est la raison pour laquelle deux fichiers ne peuvent pas avoir le même nom.

Veillez à ce que tous les utilisateurs de votre entreprise se familiarisent avec les règles de dénomination de fichiers suivantes :

* Les ID de fichier présentant exactement le même nom ne sont pas autorisés dans le système.
* Les ID de fichier sont sensibles à la casse.
* Il est recommandé de s’assurer que les ID de fichier ne contiennent pas d’espace (par exemple, veste noire.tif et veste bleue.jpg). Dynamic Media Classic code les espaces blancs dans les noms de ressources lorsqu'ils utilisent les noms de fichier pour créer des chaînes URL. Ces codes ASCII sont difficiles à lire, ce qui rend également plus difficile la lecture de ces chaînes.
* Les caractères spécifiques aux langues sont autorisés dans les noms de fichier, à l’exception des caractères suivants :

   \ ; / ? : @ &amp; = + $ , * " &lt; &gt; | ' { } %

   Si un nom de fichier contient un ou plusieurs de ces caractères, ceux-ci sont supprimés du nom du fichier au moment du téléchargement.

Dans la plupart des cas, le nom de fichier correspond au numéro d’article, à l’UGS (unité de gestion des stocks) ou à un autre nom, comme ci-dessous :

| Article | Nom de fichier | ID de fichier |
|--- |--- |--- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Organisation et structure des dossiers {#folder-organization-and-structure}

Organisez et structurez les dossiers et sous-dossiers dans Scene7 Publishing System avant de télécharger votre contenu. Cette procédure présente deux principaux avantages :

* Au moment du téléchargement de votre contenu vers SPS via FTP, vous pouvez indiquer au système de répliquer votre structure de dossiers. Ainsi, votre contenu est organisé dans les mêmes dossiers et sous-dossiers, à la fois dans SPS et sur votre ordinateur ou votre réseau (pour répliquer la structure de dossiers dans SPS, sélectionnez l’option Inclure les sous-dossiers au moment du téléchargement des fichiers via FTP).
* La réorganisation des dossiers au sein du système, une fois les fichiers téléchargés, s’avère beaucoup plus difficile que le démarrage avec une structure de dossiers soigneusement étudiée.

La technique de nommage des dossiers et la structure que vous choisissez pour stocker votre contenu dans Scene7 Publishing System dépendent des besoins de votre entreprise. Voici quelques exemples de structure de dossiers :

**Les dossiers** basés sur SKU sont nommés selon des SKU ou des numéros d'article. Par exemple, des dossiers distincts sont créés pour les séries de numéros 0-, 20-, 30-.

**Pour** les fabricants qui utilisent plusieurs marques et des détaillants qui commercialisent d'autres marques d'autres sociétés, séparez les fichiers en dossiers de produit nommés de différentes marques.

**Les** dossiers basés sur un projet sont organisés selon la date de déploiement/la date de débogage ou le nom du projet. Les clients qui produisent principalement des catalogues électroniques favorisent cette approche.

**Miroir de la hiérarchie des dossiers du site Web** Cette structure de dossiers reflète la structure de dossiers du site Web, avec les dossiers nommés, par exemple, pour les catégories de produits.

## A propos du téléchargement de fichiers {#uploading-your-files}

Vous pouvez télécharger des fichiers à partir du bureau ou des dossiers complets par FTP (File Transfer Protocol). If you want to upload more than 100 MB of files or upload entire folders and subfolders, select the **VIA FTP** tab.

Si vous avez installé l'application de bureau Scene 7 Publishing System, vous pouvez directement faire glisser des fichiers et des dossiers depuis votre bureau vers le dossier de téléchargement.

Scene7 Publishing System vous envoie un message électronique vous confirmant la date et l’heure de début et de fin de votre tâche de téléchargement, et vous avertissant de problèmes éventuels.

Pendant (ou juste après) une tâche de téléchargement volumineuse, le message « Image non optimisée » risque de s’afficher pour certains nouveaux objets. Ce message s'affiche car les fichiers ne sont pas encore entièrement traités et ajoutés à SPS. Vous pouvez optimiser ces fichiers ultérieurement (voir [Optimisation des fichiers](application-setup.md#optimize_files)).

### Téléchargement de fichiers à l'aide de l'onglet DU BUREAU {#upload-files-using-sps-desktop-application}

L’application de bureau Scene7 Publishing System vous permet de télécharger des fichiers et des dossiers en les faisant glisser.

1. Dans l’application de bureau Scene7 Publishing System, sur la barre de navigation globale, cliquez sur **Télécharger**.
1. On the Upload page, click the **FROM DESKTOP** tab.
1. Sur la partie gauche de la page de téléchargement, dans la zone **Sélectionner les fichiers pour le téléchargement** , cliquez **sur Parcourir pour** sélectionner les fichiers ou les dossiers à télécharger, puis cliquez **sur Ouvrir**.
1. Dans la partie droite de la page Télécharger, dans la **zone Choisir le dossier de destination** , accédez à un dossier de destination où les fichiers ou dossiers téléchargés doivent être ajoutés.
1. (Facultatif) Dans le champ Nom **de la tâche, près du bas de la page de téléchargement, indiquez** le nouveau nom de la tâche de téléchargement. Vous pouvez également utiliser le nom généré par le système par défaut fourni par SPS. La tâche en question, ainsi que les autres tâches de téléchargement et de publication, sont enregistrées sur la page Tâches, sur laquelle vous pouvez vérifier l’état des tâches (voir [Vérification de fichiers de tâche](checking-job-files.md#checking_job_files)).
1. (Facultatif) Près du bas de la page Télécharger, sélectionnez **Publier après le téléchargement** si vous souhaitez publier automatiquement les fichiers que vous téléchargez.
Lorsque vous publiez des fichiers, ils sont envoyés aux serveurs connectés. Les URL de ces fichiers peuvent alors être utilisées sur des sites Web et des applications externes. Notez que cette même option est également disponible dans la boîte de dialogue Options tâche.
1. (Facultatif) Près du bas de la page Télécharger, sélectionnez **Remplacer dans n'importe quel dossier, même nom de fichier de base, quelle que soit l'extension** , si vous souhaitez que les fichiers que vous téléchargez remplacent les fichiers existants portant le même nom. Notez que cette même option est également disponible dans la boîte de dialogue Options tâche.
The name of this option could be different, depending on the settings in **Application Setup &gt; General Settings &gt; Upload to Application &gt; Overwrite Images**.
1. Near the lower-right corner of the Upload page, click **Job Options**, then specify the options you want.

   Voir [Options de téléchargement](uploading-files.md#upload_options).

1. Dans la boîte de dialogue Télécharger les options de la tâche, cliquez sur **Enregistrer**.
1. Dans le coin inférieur droit de la page de téléchargement, cliquez **sur Envoyer le téléchargement**.
Pour afficher la progression du transfert, cliquez sur **Tâches** dans la barre de navigation globale. Vous pouvez poursuivre votre travail dans Scene7 Publishing System et revenir à la page Tâches à n’importe quel moment pour consulter une tâche en cours. Pour annuler une tâche de téléchargement en cours, cliquez sur **Annuler** en regard de la durée.

### Téléchargement de fichiers à l'aide de l'onglet VIA FTP {#upload-files-using-via-ftp}

1. Connectez-vous au site FTP Dynamic Media Classic spécifique à votre région particulière. Utilisez le nom d’utilisateur et le mot de passe FTP qui vous ont été envoyés par votre administrateur.
1. Dans Dynamic Media Classic, sur la barre de navigation globale, cliquez **sur Télécharger**.
1. On the Upload page, click the **VIA FTP** tab.
1. Sur le côté gauche de la page de téléchargement, dans la zone **Choisir un dossier FTP pour le téléchargement** , choisissez un dossier FTP à partir duquel télécharger les fichiers.
1. Sur la droite de la page de téléchargement, dans la **zone Choisir le dossier de destination** SPS, choisissez un dossier de destination dans Scene 7 Publishing System.
1. (Facultatif) Dans le champ Nom **de la tâche, près du bas de la page de téléchargement, indiquez** le nouveau nom de la tâche de téléchargement. Vous pouvez également utiliser le nom généré par le système par défaut fourni par SPS. La tâche en question, ainsi que les autres tâches de téléchargement et de publication, sont enregistrées sur la page Tâches, sur laquelle vous pouvez vérifier l’état des tâches (voir [Vérification de fichiers de tâche](checking-job-files.md#checking_job_files)).
1. (Facultatif) Près du bas de la page Télécharger, sélectionnez **Publier après le téléchargement** si vous souhaitez publier automatiquement les fichiers que vous téléchargez.
Lorsque vous publiez des fichiers, ils sont envoyés aux serveurs connectés. Les URL de ces fichiers peuvent alors être utilisées sur des sites Web et des applications externes. Notez que cette même option est également disponible dans la boîte de dialogue Options tâche.
1. (Facultatif) Près du bas de la page Télécharger, sélectionnez **Remplacer dans n'importe quel dossier, même nom de fichier de base, quelle que soit l'extension** , si vous souhaitez que les fichiers que vous téléchargez remplacent les fichiers existants portant le même nom. Notez que cette même option est également disponible dans la boîte de dialogue Options tâche.
The name of this option could be different, depending on the settings in **Application Setup &gt; General Settings &gt; Upload to Application &gt; Overwrite Images**.
1. (Facultatif ; disponible uniquement si vous avez cliqué sur l'onglet **VIA FTP** ) Près du bas de la page de téléchargement, sélectionnez **Décompresser les fichiers zip ou tar au chargement** si vous souhaitez extraire automatiquement tous les fichiers de votre fichier ZIP ou TAR téléchargé. Notez que cette même option est également disponible dans la boîte de dialogue Options tâche.
1. Near the lower-right corner of the Upload page, click **Job Options**, then specify the options you want.

   Voir [Options de téléchargement](uploading-files.md#upload_options).

1. Dans la boîte de dialogue Télécharger les options de la tâche, cliquez sur **Enregistrer**.
1. Dans le coin inférieur droit de la page de téléchargement, cliquez **sur Envoyer le téléchargement**.

   Pour afficher la progression du transfert, dans la barre de navigation globale, cliquez sur **Tâches**. La page Tâches présente la progression du téléchargement. Vous pouvez poursuivre votre travail dans Scene7 Publishing System et revenir à la page Tâches à n’importe quel moment pour consulter une tâche en cours.

Pour annuler une tâche de téléchargement en cours, cliquez sur **Annuler** en regard de la durée.

## Boîte de dialogue Télécharger les options de la tâche {#upload-options}

Lors du téléchargement de fichiers, vous pouvez choisir parmi les options suivantes dans la boîte de dialogue Télécharger les options de la tâche :

* **JOB** — Cliquez **sur TÂCHE** pour sélectionner les options qui affectent la tâche de téléchargement entière.

   Vous pouvez également choisir les options *par défaut* pour télécharger les tâches à l'aide de **la boîte de dialogue Options** de téléchargement par défaut dans Paramètres généraux. Cliquez sur **Configuration &gt; Configuration de l'application &gt; Paramètres généraux &gt; Options de transfert par défaut**, puis définissez les options par défaut de votre choix.

   * **Quand** — L'option **Lorsque** n'est disponible que si vous avez sélectionné l'onglet **VIA FTP** .
      * **Unique** — Spécifiez une tâche de téléchargement qui s'exécute une fois. Les options sont les suivantes :
         * **Maintenant** — Exécute la tâche de téléchargement juste après avoir cliqué **sur Enregistrer** dans la boîte de dialogue Télécharger les options de la tâche, puis cliquez **sur Envoyer le transfert** sur la page Télécharger.
         * **Planifier pour plus tard** — Sélectionnez l'année, le mois, le jour et l'heure (par incréments de 15 minutes) que la tâche de transfert doit exécuter.
      * **Récurrent** — Spécifiez une tâche de téléchargement qui s'exécute quotidiennement, hebdomadaire ou mensuel. Ou personnalisez la tâche de transfert selon vos propres spécifications.
         * **Quotidiennement** — Définissez la durée d'exécution de la tâche chaque jour. Si vous souhaitez que la tâche s'exécute uniquement du lundi au vendredi, sélectionnez **Jours de semaine uniquement**.
         * **Hebdomadaire** — Choisissez un jour précis de la semaine et de l'heure à laquelle la tâche doit être exécutée.
         * **Mensuel** — Choisissez un jour spécifique du mois ou du jour de la semaine, y compris l'heure de début, que vous souhaitez exécuter.
         * **Personnalisé** — Personnalisez un intervalle de travail de téléchargement ou de publication selon vos propres spécifications. (voir [Création d’un intervalle de téléchargement ou de publication personnalisé](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval)).
   * **Publier après le téléchargement** — Disponible si vous avez sélectionné l'onglet **FROM DESKTOP** ou **l'onglet VIA FTP** . Sélectionnez cette option pour publier automatiquement les fichiers que vous téléchargez. Lorsque vous publiez des fichiers, ils sont envoyés aux serveurs connectés. Les URL de ces fichiers peuvent alors être utilisées sur des sites Web et des applications externes. Cette option est également disponible sur la page de téléchargement.

   * **Ecraser dans un dossier, même nom de fichier de base quelle que soit l'extension** : Disponible si vous avez sélectionné l'onglet **FROM DESKTOP** ou **l'onglet VIA FTP** . Permet de remplacer des fichiers existants portant le même nom que les fichiers que vous téléchargez. Cette option est également disponible sur la page de téléchargement. The name of this option could be different, depending on the settings in **Application Setup &gt; General Settings &gt; Upload to Application &gt; Overwrite Images**.

   * **Décompresser les fichiers zip ou tar au chargement** — Disponible si vous avez sélectionné l'onglet **FROM DESKTOP** ou **l'onglet VIA FTP** .
Sélectionnez cette option si vous souhaitez extraire automatiquement tous les fichiers du fichier ZIP ou TAR téléchargé. Notez que cette même option est également disponible dans la boîte de dialogue Options tâche.

   * **Inclure des sous-dossiers** : Disponible uniquement si vous avez sélectionné l'onglet **VIA FTP** .
Permet de télécharger les sous-dossiers du dossier que vous avez l’intention de télécharger. Les noms du dossier et des sous-dossiers associés que vous téléchargez sont automatiquement saisis dans SPS.

   * **Traiter les fichiers** de métadonnées— Disponible uniquement si vous avez sélectionné l'onglet **VIA FTP** . Sélectionnez cette option si vous souhaitez télécharger un fichier XML ou délimité par des tabulations pour ajouter des métadonnées à plusieurs fichiers. Voir [Importer des métadonnées (via FTP)](viewing-adding-exporting-metadata.md#import-metadata).


* **OPTIONS DE RECADRAGE** — Pour supprimer automatiquement les pixels d'espace blanc d'une image, ouvrez le menu Recadrer, choisissez Manuel, puis entrez les mesures en pixels dans les champs Haut, Droite, Bas et Gauche pour recadrer à partir des côtés. Vous pouvez également choisir Rogner dans le menu Recadrer et choisir les options suivantes :

   * **Rogner selon** — Choisissez de recadrer selon la couleur ou la transparence :

      * **Couleur** — Choisissez l'option Couleur. Sélectionnez ensuite le menu Coin, puis choisissez l’angle de l’image présentant la couleur qui correspond le mieux à l’espace blanc à rogner.

         Rognage en fonction de la couleur : Indiquez 0 pour rogner les pixels seulement s'ils correspondent exactement à la couleur sélectionnée dans l'angle de l'image. Les valeurs qui se rapprochent de 1 admettent un plus grand écart des couleurs.

      * **Transparence** — Choisissez l'option Transparence.

         Rognage selon la transparence : Indiquez 0 pour rogner les pixels uniquement s'ils sont entièrement transparents ; les valeurs plus proches de 1 permettent une plus grande transparence.

      * **Tolérance** — Faites glisser le curseur pour définir une valeur de tolérance comprise entre 0 et 1.

* **OPTIONS DE PROFIL COLORIMÉTRIQUE** — Choisissez une conversion de couleurs lorsque vous créez des fichiers optimisés utilisés pour la diffusion dynamique Dynamic Media Classic :

   * **Conservation des couleurs par défaut** — Conserve les couleurs de l'image source chaque fois que les images contiennent des informations d'espace colorimétrique ; il n'y a aucune conversion de couleur. Pour la plupart des images aujourd’hui, un profil colorimétrique approprié est déjà inclus. Toutefois, si une image source CMJN ne contient pas de profil colorimétrique intégré, les couleurs sont converties dans l’espace colorimétrique sRVB (rouge vert bleu standard). sRVB est l’espace colorimétrique recommandé pour l’affichage d’images sur les pages Web.

   * **Conserver l'espace** colorimétrique original— Conserve les couleurs d'origine sans conversion de couleurs au moment de l'assimilation dans Scene 7 Publishing System. Pour les images sans profil incorporé, toute conversion des couleurs nécessaire aux demandes de traitement de l’image sont effectuées à l’aide des profils colorimétriques par défaut configurés dans les paramètres de publication. Ces profils colorimétriques peuvent ne pas correspondre aux couleurs des fichiers créés avec cette option. Par conséquent, vous avez intérêt à utiliser l’option de conservation des couleurs par défaut.

   * **Personnalisé De &gt; Vers** — Ouvre les menus qui vous permettent de choisir un espace colorimétrique Convertir en et Convertir en espace colorimétrique. Cette option avancée remplace toutes les informations de couleur incorporées dans le fichier source. Sélectionnez cette option uniquement lorsque toutes les images que vous envoyez contiennent des données de profil colorimétrique incorrectes ou manquantes.

* **OPTIONS D'ÉDITION D'IMAGES** — Vous pouvez conserver l'écrêtage &lt; &gt; masques dans les images, puis choisir un profil de couleurs.
(voir [Options d’édition d’images au téléchargement](image-editing-options-upload.md#image-editing-options-at-upload)).

* **OPTIONS** POSTSCRIPT— Vous pouvez pixelliser des fichiers postscript®, recadrer des fichiers, conserver des arrière-plans transparents, choisir une résolution et choisir un espace colorimétrique
(voir [Utilisation de fichiers PostScript et Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)).

* **OPTIONS** PHOTOSHOP— Vous pouvez créer des modèles à partir de fichiers Adobe® Photoshop®, conserver les calques, définir leur nom, extraire du texte et définir le mode d'ancrage des images dans les modèles.
(voir [Options de téléchargement des fichiers PSD](psd-files.md#psd_upload_options)).

* **OPTIONS** PDF— Vous pouvez pixelliser les fichiers, extraire des mots de recherche et des liens, générer automatiquement un catalogue électronique, définir la résolution et choisir un espace colorimétrique.
(voir [Options de téléchargement des fichiers PDF](pdfs.md#pdf_upload_options)).

* **OPTIONS** ILLUSTRATOR— Vous pouvez pixelliser des fichiers Adobe Illustrator®, conserver les arrière-plans transparents, choisir une résolution et choisir un espace colorimétrique
(voir [Utilisation de fichiers PostScript et Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)).

* **OPTIONS** EVIDEO— Vous pouvez transcoder un fichier vidéo en choisissant un paramètre vidéo prédéfini.
Voir [Utilisation des paramètres prédéfinis de codage vidéo](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **MÉTADONNÉES** SUPPLÉMENTAIRES— Saisissez des mots-clés décrivant les fichiers que vous téléchargez. Séparez les mots clés-par des virgules. Les mots-clés facilitent les recherches portant sur les fichiers Voir [Recherche avancée](searching-assets.md#conducting_an_advanced_search).

* **PARAMÈTRES PRÉDÉFINIS** D'ENSEMBLE PAR LOT— Si vous souhaitez créer une visionneuse d'images, une visionneuse à 360 ° multi-axe ou une série d'échantillons à partir des fichiers téléchargés, cliquez sur la colonne Actif pour le paramètre prédéfini à utiliser. Rien ne vous empêche de sélectionner plusieurs paramètres prédéfinis. Vous créez les paramètres prédéfinis sur la page Configuration de l’application/Paramètres prédéfinis d’ensemble par lot (voir [Paramètres prédéfinis d’ensemble par lot](application-setup.md#batch_set_presets)).

* **ADVANCED** — Voir [Suivi d'un téléchargement avec une autre tâche](uploading-files.md#follow-an-upload-with-another-job).

## Enchaînement d’une tâche de téléchargement et d’une autre tâche {#follow-an-upload-with-another-job}

Lorsque vous téléchargez des éléments à partir d’un site FTP, vous pouvez planifier une autre tâche de sorte qu’elle commence sitôt le téléchargement terminé. (Si le début d’autres tâches est planifié à ce moment-là, la tâche planifiée ici sera mise en file d’attente derrière elles.)

La nouvelle tâche envoie une notification à l’adresse spécifiée par vos soins de manière à déclencher ce code à cet emplacement. Cette tâche de publication consécutive reprend le nom de la tâche de téléchargement, mais ajoute *Pub_* devant le nom.

**Enchaînement d’une tâche de téléchargement et d’une autre tâche**

1. Click **Upload**, then click the **VIA FTP** tab.
1. In the lower-right corner of the Upload page, click **Job Options**.
1. Dans la boîte de dialogue Télécharger les options de la tâche, développez la section **AVANCÉ** .
1. Dans la liste **déroulante Suivre le téléchargement, choisissez l'une des** options suivantes :

   * Aucun
   * Requête HTTP
   * Publication sur hébergeur d’images
   * Publication de rendu d’image
   * Publication de vidéo

1. Spécifiez l’adresse HTTP.
1. Indiquez si vous souhaitez exécuter uniquement si des fichiers ont été téléchargés.
1. Indiquez si vous souhaitez exécuter cette requête chaque fois que cette tâche se termine ou uniquement lorsque les fichiers ont été publiés.

   >[!NOTE]
   >
   >les tâches régulièrement planifiées peuvent n’entraîner aucune publication de fichiers.

>[!MORELIKETHIS]
>
>* [Utilisation de dossiers de fichiers](asset-folders.md#working_with_asset_folders)
>* [Gestion de tâches de téléchargement et de publication périodiques](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Utilisation d’une tâche de téléchargement ou de publication comme déclencheur](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)
