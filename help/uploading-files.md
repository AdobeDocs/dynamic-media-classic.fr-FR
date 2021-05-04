---
title: Téléchargement de fichiers
description: Découvrez comment télécharger des fichiers.
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
feature: Dynamic Media Classic,Gestion des ressources
role: Business Practitioner
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
translation-type: tm+mt
source-git-commit: 1beb30b9eda4487dcd549034906079dee0b3149a
workflow-type: tm+mt
source-wordcount: '3833'
ht-degree: 36%

---

# Téléchargement de fichiers{#uploading-files}

Avant de télécharger des fichiers vers Dynamic Media Classic, assurez-vous que leur nom est correct et que la structure de dossiers est configurée et organisée comme vous le souhaitez. Vous pouvez télécharger des fichiers à partir d’un site FTP fourni par Dynamic Media Classic ou directement depuis votre ordinateur ou votre réseau. Options des offres Dynamic Media Classic pour l’optimisation des fichiers au cours du téléchargement. Si vous avez installé l’application de bureau Adobe Dynamic Media Classic, vous pouvez télécharger des fichiers et des dossiers en les faisant glisser directement depuis votre bureau. (voir [Paramètres généraux de l’application](application-setup.md#general_settings)).

## Préparation du téléchargement des fichiers et dossiers {#preparing-your-assets-and-folders-for-uploading}

Avant de télécharger des fichiers vers Dynamic Media Classic, assurez-vous qu’ils sont au bon format et à la bonne taille. Vous devez également respecter les règles Dynamic Media Classic pour nommer les fichiers. La définition d’une organisation et d’une structure de dossiers pour les fichiers garantit une facilité de localisation et d’utilisation de ces derniers.

### Formats de fichiers pris en charge  {#supported-asset-file-formats}

Ce tableau liste les formats de fichier pris en charge par Dynamic Media Classic. Pour plus d’informations sur les fichiers Camera Raw pris en charge, voir [https://www.adobe.com/go/learn_s7_cameraraw_en](https://www.adobe.com/go/learn_s7_cameraraw_en).

| Formats de fichiers | Description |
|--- |--- |
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
| Création d’images Dynamic Media Classic | VNC, VNT, VNW |
| SVG | SVG, SVGX |
| TAR | TAR |
| Vidéo | 3GP, AVI, M2P, M2T, M2TS, M2V, M4V, MOV, MP4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF |
| XML | XML |
| ZIP | ZIP |

La fonction de transfert au format TAR et ZIP offre une case à cocher permettant d’indiquer si vous souhaitez décompresser les fichiers.

### Formats d’image non pris en charge dans Dynamic Media {#unsupported-image-formats-dynamic-media}

La liste suivante décrit les sous-types de formats de fichier image pixellisée *qui ne sont pas* pris en charge dans Dynamic Media.

Voir aussi [Détecter les formats de fichier non pris en charge pour Dynamic Media](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html).

* Fichiers PNG dont la taille de bloc IDAT est supérieure à 100 Mo.
* Fichiers PSB.
* Les fichiers PSD avec un espace colorimétrique autre que CMJN, RVB, Niveaux de gris ou Bitmap ne sont pas pris en charge. Les espaces colorimétriques DuoTone, Lab et Indexé ne sont pas pris en charge.
* Fichiers PSD ayant une profondeur de bits supérieure à 16.
* Fichiers TIFF contenant des données à virgule flottante.
* Fichiers TIFF dotés d’un espace colorimétrique Lab.

### Types de ressource {#asset-types}

Pour obtenir des résultats optimaux avec le programme Dynamic Media Classic, veillez à utiliser les formats et tailles de fichier recommandés. Ce tableau répertorie les types de fichiers, dont certains avec les formats et tailles recommandés pour les fichiers couramment utilisés.

| Type de fichier | Description/Recommandations |
|--- |--- |
| Audio | Les formats de fichiers audio entrants incluent AAC, HE-AAC, AC3, WAV, WMA, AIFF et MP3. Vous pouvez transcoder du contenu audio aux formats suivants : MP3, AAC et HE-AAC. |
| Images (pour le dimensionnement des images, le zoom, les visionneuses d’images, les visionneuses à 360°) | Les images doivent mesurer au moins 2 000 pixels à la taille la plus longue ; la taille d’image standard varie de 1 500 à 2 500 pixels pour la taille la plus longue. Les formats d’image sans perte, notamment TIFF et PNG, sont recommandés. Avec une image JPEG, utilisez les paramètres de qualité les plus élevés. Les fichiers GIF animés sont gérés comme d’autres contenus statiques. |
| Catalogues électroniques | Utilisez des fichiers PDF haute résolution créés dans Adobe® Acrobat® ou dans une application Creative Suite avec un enregistrement « bon à tirer ». Les fichiers PDF incluent l’ensemble des polices, images, masques et éléments graphiques référencés nécessaires, au format de page unique, de planche en double page ou de plusieurs pages. Organisez les pages en nommant les fichiers selon un ordre alphanumérique. Placez tous les fichiers PDF du catalogue électronique dans un dossier unique en vue de faciliter le téléchargement. Vous pouvez sélectionner des options de recadrage lors du téléchargement afin de supprimer la zone de rognage des fichiers PDF, notamment les traits de coupe, les repères de montage ou les gammes de couleurs. La plupart des fichiers PDF « bon à tirer » sont caractérisés par l’espace colorimétrique CMJN ; il est donc important d’obtenir le profil colorimétrique ICC CMJN utilisé avec vos fichiers PDF. |
| Modèles | Image superposée ou disposition pouvant inclure du texte, des images et des calques. Les calques d’image, les chaînes de texte et les attributs, comme la couleur et la taille, peuvent être paramétrés de manière à pouvoir personnaliser les données variables. Pour les modèles, les exigences sont les mêmes que pour les autres images. Préparez vos images dans Photoshop ou un autre éditeur d’images. Enregistrez chaque image sous forme de fichier transparent aplati au format TIFF ou PNG. Assurez-vous que la résolution de l’image est adaptée à l’utilisation qui en sera faite. Les images pour impression sont de 300 ppp. |
| Vidéos | Dynamic Media Classic prend en charge les fichiers vidéo enregistrés aux formats OGV et MP4. Vous pouvez transcoder des fichiers vers le format MP4 lors du téléchargement. Voir [Formats de fichiers pris en charge](#supported-static-file-formats). |
| Polices | Polices TrueType, Type1 (Windows® uniquement), OpenType® et PhotoFonts téléchargées |
| Images | Images et fichiers d’images superposées. |
| Visionneuses d’images et séries d’échantillons | Ensemble d’images associées pouvant être affichées dans une visionneuse. |
| Profils ICC | Profil de couleur pouvant être utilisé pour convertir une image téléchargée depuis son espace colorimétrique source dans un autre espace colorimétrique. |
| Vignettes | Images créées avec le programme de création d’images et les fichiers associés. |
| Fichiers de contenu | Fichiers de contenu Adobe InDesign, Illustrator ou Photoshop. |
| Fichiers FXG | Format de fichiers graphiques à résolution indépendante permettant de créer des modèles personnalisables en vue d’une sortie pour impression, Web, courrier électronique, ordinateur et appareils mobiles. |
| Fichiers SVG | Fichiers Scalable Vector Graphic dont le rendu peut être effectué par des serveurs Image Server. |
| Fichiers XML | Fichiers qui définissent les règles de prétraitement utilisées pour modifier les parties chemin (path) et interrogation (query) des requêtes. |
| Fichiers de feuille de style en cascade | Téléchargez des habillages CSS pour personnaliser des visionneuses HTML5. |
| Fichiers JavaScript™ | Les fichiers JavaScript™ sont utilisés pour l’instrumentation de la visionneuse afin de contenir les informations de compte. Adobe Security recommande ce type d’actif uniquement pour les comptes clients dont un domaine distinct est utilisé pour la diffusion (afin d’éviter les scripts intersites). |

>[!NOTE]
>
>Lorsque vous téléchargez des fichiers d’image et des fichiers PDF vers Dynamic Media Classic, le système convertit ces fichiers source en fichiers P-TIFF (Pyramid TIFF). Ces fichiers P-TIFF sont les fichiers publiés ultérieurement sur les serveurs Dynamic Media Image Server. Dynamic Media Classic utilise le format de fichier Pyramid Tiff, car il contient divers rapports de zoom qui permettent un zoom rapide lors de l’affichage avec une visionneuse de zoom Dynamic Media Classic.

### Formats de fichier statique pris en charge {#supported-static-file-formats}

Dynamic Media Classic prend en charge plusieurs formats de fichier statiques. Le contenu statique est tout fichier publié &quot;en l’état&quot;, tel que CSS, PDF, SVG et XML.

Les types de fichier suivants peuvent être publiés :

* GIF animé
* Fichiers audio
* CSS
* JavaScript™ (lorsque la société est configurée avec son propre domaine)
* Vidéo originale
* PDF (lorsque le fichier PDF est marqué pour publication après le téléchargement, afin d’éviter la diffusion de tous les fichiers PDF pour le flux de travail existant de catalogue électronique/PDF)
* Vidéo PrX
* SVG
* XML
* ZIP

Dynamic Media Classic ne permet pas de générer une URL de prévisualisation de contenu statique.

### Exigences relatives aux noms de fichiers {#filename-requirements}

Etant donné que l’extension est ôtée du nom du fichier durant le processus de téléchargement, le système ne permet pas que des fichiers présentent le même nom racine. Dans le système Dynamic Media Classic, le nom de fichier sans l’extension devient l’ID de fichier du fichier. C’est la raison pour laquelle deux fichiers ne peuvent pas avoir le même nom.

Veillez à ce que tous les utilisateurs de votre entreprise se familiarisent avec les règles de dénomination de fichiers suivantes :

* Les ID de fichier présentant exactement le même nom ne sont pas autorisés dans le système.
* Les noms d’ID de ressource respectent la casse.
* Il est recommandé de s’assurer que les ID de fichier ne contiennent pas d’espace (par exemple, veste noire.tif et veste bleue.jpg). Dynamic Media Classic ASCII code les espaces vides dans les noms de fichier lorsqu’il utilise des noms de fichier pour créer des chaînes URL. Ces codes ASCII sont difficiles à lire, ce qui rend également plus difficile la lecture de ces chaînes.
* Les caractères spécifiques aux langues sont autorisés dans les noms de fichier, à l’exception des caractères suivants :

   \; / ? : @ &amp; = + $, * &quot; &lt; > | &#39; { } %

   Si un nom de fichier contient un ou plusieurs de ces caractères, ceux-ci sont supprimés du nom du fichier au moment du téléchargement.

En règle générale, un nom de fichier peut être identique à son numéro d’article, à son SKU de produit ou à un autre nom, comme dans l’exemple suivant :

| Article | Nom de fichier | ID de fichier |
|--- |--- |--- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Organisation et structure des dossiers  {#folder-organization-and-structure}

Organisez et structurez les dossiers et les sous-dossiers de votre contenu dans Dynamic Media Classic avant de télécharger votre contenu sur le système. Cette procédure présente deux principaux avantages :

* Lorsque vous téléchargez votre contenu vers Dynamic Media Classic via FTP, vous pouvez indiquer au système de répliquer la structure de dossiers pendant le téléchargement. Ainsi, votre contenu est organisé dans les mêmes dossiers et sous-dossiers dans Dynamic Media Classic que sur votre ordinateur ou votre réseau. (Pour répliquer la structure de dossiers dans Dynamic Media Classic, sélectionnez l’option Inclure les sous-dossiers lorsque vous téléchargez des fichiers par FTP.)
* La réorganisation des dossiers au sein du système, une fois les fichiers téléchargés, s’avère beaucoup plus difficile que le démarrage avec une structure de dossiers soigneusement étudiée.

L’approche et la structure de nommage de dossiers que vous choisissez pour stocker votre contenu dans Dynamic Media Classic dépendent des besoins de votre entreprise. Voici quelques exemples de structure de dossiers :

**Basé**  sur le SKU : les dossiers sont nommés en fonction des SKU ou des numéros d’article. Par exemple, des dossiers distincts sont créés pour les séries de numéros 0-, 20-, 30-.

**Basé sur**  la marque : pour les fabricants qui possèdent plusieurs marques et les détaillants qui commercialisent d&#39;autres marques d&#39;autres sociétés, séparez les fichiers en dossiers de produits nommés pour différentes marques.

**Basé sur**  un projet : les dossiers sont organisés en fonction de la date de déploiement/de dépôt ou du nom du projet. Les clients qui produisent principalement des catalogues électroniques favorisent cette approche.

**Miroir de la hiérarchie**  des dossiers du site Web : cette structure de dossiers reflète la structure des dossiers du site Web, avec les dossiers nommés, par exemple, pour les catégories de produits.

## A propos du transfert de fichiers {#uploading-your-files}

Vous pouvez télécharger des fichiers à partir du bureau ou des dossiers complets par FTP (File Transfer Protocol). Si vous souhaitez télécharger plus de 100 Mo de fichiers ou des dossiers et sous-dossiers entiers, sélectionnez l’onglet **VIA FTP**.

Dynamic Media Classic vous envoie un message électronique vous confirmant à quel moment votre tâche de téléchargement commence et se termine et vous avertissant de tout problème.

Pendant (ou immédiatement après) une tâche de téléchargement volumineuse, certains nouveaux éléments peuvent afficher le message &quot;Image non encore optimisée&quot;. Ce message s’affiche, car les fichiers ne sont pas encore entièrement traités et ajoutés à Dynamic Media Classic. Vous pouvez optimiser ces fichiers ultérieurement Voir [Optimiser les fichiers](application-setup.md#optimize_files).

### Téléchargement de fichiers à l’aide de l’onglet De bureau {#upload-files-using-sps-desktop-application}

L’application de bureau Dynamic Media Classic vous permet de télécharger des fichiers et des dossiers en les faisant glisser.

1. Dans l’application de bureau Dynamic Media Classic, sur la barre de navigation globale, cliquez sur **[!UICONTROL Télécharger]**.
1. Sur la page Télécharger, cliquez sur l’onglet **[!UICONTROL De Bureau]**.
1. Sur le côté gauche de la page de téléchargement, dans la zone **[!UICONTROL Sélectionner les fichiers à télécharger]**, cliquez sur **[!UICONTROL Parcourir]** pour sélectionner les fichiers ou les dossiers à télécharger, puis cliquez sur **[!UICONTROL Ouvrir]**.
1. Sur le côté droit de la page de téléchargement, dans la zone **Choisir la destination du dossier**, accédez au dossier de destination dans lequel vous souhaitez ajouter les fichiers ou dossiers téléchargés.
1. (Facultatif) Près du bas de la page Télécharger, dans le champ **[!UICONTROL Nom de la tâche]**, indiquez le nouveau nom de la tâche de téléchargement. Vous pouvez également simplement utiliser le nom généré par le système par défaut fourni par Dynamic Media Classic. La tâche en question, ainsi que les autres tâches de téléchargement et de publication, sont enregistrées sur la page Tâches, sur laquelle vous pouvez vérifier l’état des tâches (voir [Vérification de fichiers de tâche](checking-job-files.md#checking_job_files)).
1. (Facultatif) Près du bas de la page de téléchargement, sélectionnez **[!UICONTROL Publier après le téléchargement]** si vous souhaitez publier automatiquement les fichiers que vous téléchargez.
Lorsque vous publiez des fichiers, ils sont envoyés aux serveurs connectés. Les URL de ces fichiers peuvent alors être utilisées sur des sites Web et des applications externes. Cette même option est également disponible dans la boîte de dialogue Options tâche.
1. (Facultatif) Près du bas de la page de téléchargement, sélectionnez **[!UICONTROL Remplacer dans n’importe quel dossier, même nom de fichier de base, indépendamment de l’extension]** si vous souhaitez que les fichiers que vous téléchargez remplacent les fichiers existants portant le même nom. Cette même option est également disponible dans la boîte de dialogue Options tâche.
Le nom de cette option peut être différent, selon les paramètres définis dans **Configuration de l’application > Paramètres généraux > Télécharger vers l’application > Ecraser les images**.
1. Près du coin inférieur droit de la page de téléchargement, cliquez sur **[!UICONTROL Options tâche]**, puis spécifiez les options de votre choix.

   Voir [Options de téléchargement](uploading-files.md#upload_options).

1. Dans la boîte de dialogue Télécharger les options de la tâche, cliquez sur **[!UICONTROL Enregistrer]**.
1. Dans le coin inférieur droit de la page de téléchargement, cliquez sur **[!UICONTROL Envoyer le téléchargement]**.
Pour afficher la progression du transfert, cliquez sur **[!UICONTROL Tâches]** dans la barre de navigation globale. Vous pouvez continuer à travailler dans Dynamic Media Classic et revenir à la page Tâches à tout moment pour consulter une tâche en cours. Pour annuler une tâche de téléchargement en cours, cliquez sur **[!UICONTROL Annuler]** en regard de la durée.

### Téléchargement de fichiers à l’aide de l’onglet FTP VIA {#upload-files-using-via-ftp}

1. Connectez-vous au site FTP Dynamic Media Classic spécifique à votre région. Utilisez le nom d’utilisateur et le mot de passe FTP qui vous ont été envoyés par votre administrateur.
1. Dans Dynamic Media Classic, sur la barre de navigation globale, cliquez sur **[!UICONTROL Télécharger]**.
1. Sur la page Télécharger, cliquez sur l’onglet **[!UICONTROL VIA FTP]**.
1. Sur le côté gauche de la page de téléchargement, dans la zone **[!UICONTROL Choisir le dossier FTP pour le téléchargement]**, sélectionnez un dossier FTP à partir duquel télécharger les fichiers.
1. Sur le côté droit de la page de téléchargement, dans la zone **[!UICONTROL Choisir le dossier Dynamic Media d&#39;Adobe Destination]**, sélectionnez un dossier de destination dans Dynamic Media Classic.
1. (Facultatif) Près du bas de la page Télécharger, dans le champ **[!UICONTROL Nom de la tâche]**, indiquez le nouveau nom de la tâche de téléchargement. Vous pouvez également simplement utiliser le nom généré par le système par défaut fourni par Dynamic Media Classic. La tâche en question, ainsi que les autres tâches de téléchargement et de publication, sont enregistrées sur la page Tâches, sur laquelle vous pouvez vérifier l’état des tâches (voir [Vérification de fichiers de tâche](checking-job-files.md#checking_job_files)).
1. (Facultatif) Près du bas de la page de téléchargement, sélectionnez **[!UICONTROL Publier après le téléchargement]** si vous souhaitez publier automatiquement les fichiers que vous téléchargez.
Lorsque vous publiez des fichiers, ils sont envoyés aux serveurs connectés. Les URL de ces fichiers peuvent alors être utilisées sur des sites Web et des applications externes. Cette même option est également disponible dans la boîte de dialogue Options tâche.
1. (Facultatif) Près du bas de la page de téléchargement, sélectionnez **[!UICONTROL Remplacer dans n’importe quel dossier, même nom de fichier de base, indépendamment de l’extension]** si vous souhaitez que les fichiers que vous téléchargez remplacent les fichiers existants portant le même nom. Cette même option est également disponible dans la boîte de dialogue Options tâche.
Le nom de cette option peut être différent, selon les paramètres définis dans **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres généraux]** > **[!UICONTROL Télécharger vers l’application]** > **[!UICONTROL Remplacer les images]**.
1. Facultatif ; disponible uniquement si vous avez cliqué sur l’onglet **[!UICONTROL VIA FTP]**. Près du bas de la page de téléchargement, sélectionnez **[!UICONTROL Décompresser les fichiers ZIP ou Tar lors du téléchargement]** si vous souhaitez extraire automatiquement tous les fichiers de votre fichier ZIP ou TAR téléchargé. Cette même option est également disponible dans la boîte de dialogue Options tâche.
1. Près du coin inférieur droit de la page de téléchargement, cliquez sur **[!UICONTROL Options tâche]**, puis spécifiez les options de votre choix.

   Voir [Options de téléchargement](uploading-files.md#upload_options).

1. Dans la boîte de dialogue Télécharger les options de la tâche, cliquez sur **[!UICONTROL Enregistrer]**.
1. Dans le coin inférieur droit de la page de téléchargement, cliquez sur **[!UICONTROL Envoyer le téléchargement]**.

   Pour afficher la progression du transfert, dans la barre de navigation globale, cliquez sur **[!UICONTROL Tâches]**. La page Tâches présente la progression du téléchargement. Vous pouvez continuer à travailler dans Dynamic Media Classic et revenir à la page Tâches à tout moment pour consulter une tâche en cours.

Pour annuler une tâche de téléchargement en cours, cliquez sur **[!UICONTROL Annuler]** en regard de la durée.

## Boîte de dialogue Télécharger les options de la tâche {#upload-options}

Lors du téléchargement de fichiers, vous pouvez choisir l’une des options suivantes dans la boîte de dialogue Télécharger les options de la tâche :

* **TÂCHE**  - Cliquez sur  **** TÂCHE pour choisir les options qui affectent l’ensemble de la tâche de téléchargement.

   Vous pouvez également choisir les options *default* pour télécharger des tâches à l’aide de la boîte de dialogue **[!UICONTROL Options de téléchargement par défaut]** dans Paramètres généraux. Cliquez sur **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres généraux]** > **[!UICONTROL Options de téléchargement par défaut]**, puis définissez les options par défaut.

   * **Lorsque**  : cette option est disponible uniquement si vous avez sélectionné l&#39; **[!UICONTROL onglet]** VIA FTP.
      * **Une fois**  : spécifiez une tâche de téléchargement qui s’exécute une fois. Les options sont les suivantes :
         * **Maintenant**  : exécute la tâche de téléchargement immédiatement après avoir cliqué sur  **** Enregistrer dans la boîte de dialogue Télécharger les options de la tâche, puis sur  **[!UICONTROL Envoyer]** le téléchargement sur la page Télécharger.
         * **Planifier pour plus tard**  : sélectionnez l&#39;année, le mois, le jour et l&#39;heure (par incréments de 15 minutes) que vous souhaitez que la tâche de téléchargement s&#39;exécute.
      * **Récurrent**  : spécifiez une tâche de téléchargement qui s’exécute tous les jours, toutes les semaines ou tous les mois. Vous pouvez également personnaliser la tâche de téléchargement selon vos propres spécifications.
         * **Quotidiennement**  : définissez l&#39;heure à laquelle vous souhaitez que la tâche s&#39;exécute chaque jour. Si vous souhaitez que la tâche s’exécute uniquement du lundi au vendredi, sélectionnez **[!UICONTROL Jours de semaine uniquement]**.
         * **Hebdomadaire**  : choisissez un jour et une heure de la semaine spécifiques pour lesquels vous souhaitez exécuter la tâche.
         * **Mensuellement**  : choisissez un jour spécifique du mois ou du jour de la semaine, y compris l&#39;heure de début, que vous souhaitez que la tâche s&#39;exécute.
         * **Personnalisé**  : personnalisez un intervalle de temps de téléchargement ou de publication selon vos propres spécifications. (voir [Création d’un intervalle de téléchargement ou de publication personnalisé](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval)).
   * **Publier après le téléchargement**  : cette option est disponible si vous avez sélectionné l’ **[!UICONTROL onglet FROM]** DESKTOPou  **[!UICONTROL VIA]** FTPtab. Sélectionnez cette option pour publier automatiquement les fichiers que vous téléchargez. Lorsque vous publiez des fichiers, ils sont envoyés aux serveurs connectés. Les URL de ces fichiers peuvent alors être utilisées sur des sites Web et des applications externes. Cette option est également disponible sur la page de téléchargement.

   * **Ecraser dans n’importe quel dossier, même nom de fichier de base, quelle que soit l’extension**  - Disponible si vous avez sélectionné l’ **[!UICONTROL onglet FROM]** DESKTOP ou  **[!UICONTROL VIA]** FTP. Permet de remplacer des fichiers existants portant le même nom que les fichiers que vous téléchargez. Cette option est également disponible sur la page de téléchargement. Le nom de cette option peut être différent, selon les paramètres définis dans **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]** > **[!UICONTROL Paramètres généraux]** > **[!UICONTROL Télécharger vers l’application]** > **[!UICONTROL Remplacer les images]**.

   * **Décompresser les fichiers Zip ou Tar au téléchargement**  - Disponible si vous avez sélectionné l&#39; **[!UICONTROL onglet FROM]** DESKTOP ou  **[!UICONTROL VIA]** FTP.
Sélectionnez cette option si vous souhaitez extraire automatiquement tous les fichiers de votre fichier ZIP ou TAR téléchargé. Cette même option est également disponible dans la boîte de dialogue Options tâche.

   * **Inclure les sous-dossiers**  - Disponible uniquement si vous avez sélectionné l&#39; **[!UICONTROL onglet]** VIA FTP.
Permet de télécharger les sous-dossiers du dossier que vous avez l’intention de télécharger. Les noms du dossier et de ses sous-dossiers que vous téléchargez sont automatiquement saisis dans Dynamic Media Classic.

   * **Traiter les fichiers**  de métadonnées - Disponible uniquement si vous avez sélectionné l&#39;onglet  **[!UICONTROL VIA]** FTP. Sélectionnez cette option si vous souhaitez télécharger un fichier XML ou délimité par des tabulations pour ajouter des métadonnées à plusieurs fichiers. Voir [Importer des métadonnées (via FTP)](viewing-adding-exporting-metadata.md#import-metadata).


* **OPTIONS**  de recadrage : pour supprimer automatiquement les pixels représentant des espaces blancs d’une image, ouvrez le  **** menu Recadrage, cliquez sur le bouton  **[!UICONTROL Manuel]**, puis saisissez les mesures en pixels dans les champs de texte Haut, Droite, Bas et Gauche pour recadrer les pixels des côtés. Vous pouvez également cliquer sur **[!UICONTROL Rogner]** dans le menu Recadrer et choisir les options suivantes :

   * **Rogner selon**  : choisissez si vous souhaitez recadrer en fonction de la couleur ou de la transparence :
      * **Couleur**  : choisissez l&#39;option Couleur. Sélectionnez ensuite le menu Coin, puis choisissez l’angle de l’image présentant la couleur qui correspond le mieux à l’espace blanc à rogner.
Rognage en fonction de la couleur : Indiquez 0 pour rogner les pixels uniquement s’ils correspondent exactement à la couleur sélectionnée dans l’angle de l’image. Les valeurs qui se rapprochent de 1 admettent un plus grand écart des couleurs.
      * **Transparence**  - Sélectionnez l&#39;option  **** Transparence.
Rognage en fonction de la transparence : Indiquez 0 pour rogner les pixels uniquement s’ils sont transparents ; les valeurs plus proches de 1 permettent une plus grande transparence.
      * **Tolérance**  : faites glisser le curseur pour définir une tolérance comprise entre 0 et 1.

* **OPTIONS**  d&#39;PROFIL COLOR - Choisissez une conversion de couleur lorsque vous créez des fichiers optimisés utilisés pour la diffusion dynamique Dynamic Media Classic :

   * **Conservation**  des couleurs par défaut : conserve les couleurs de l&#39;image source chaque fois que les images contiennent des informations sur l&#39;espace colorimétrique ; il n’existe aucune conversion de couleur. Pour la plupart des images aujourd’hui, un profil colorimétrique approprié est déjà inclus. Toutefois, si une image source CMJN ne contient pas de profil colorimétrique intégré, les couleurs sont converties dans l’espace colorimétrique sRVB (rouge vert bleu standard). sRVB est l’espace colorimétrique recommandé pour l’affichage d’images sur les pages Web.
   * **Conserver l&#39;espace**  colorimétrique d&#39;origine - Conserve les couleurs d&#39;origine sans conversion de couleur au moment de l&#39;assimilation dans Dynamic Media Classic. Pour les images sans profil de couleur incorporé, toute conversion de couleur requise pour traiter les demandes d’image est effectuée à l’aide des profils de couleur par défaut configurés dans les paramètres de publication. Ces profils de couleur ne s’alignent pas toujours avec la couleur des fichiers créés avec cette option. Par conséquent, vous avez intérêt à utiliser l’option de conservation des couleurs par défaut.
   * **Personnalisé de > à**  - Ouvre les menus afin que vous puissiez choisir un espace  **[!UICONTROL Convertir]** le formulaire et  **[!UICONTROL Convertir l&#39;espace]** de couleur. Cette option avancée remplace toutes les informations de couleur incorporées dans le fichier source. Sélectionnez cette option uniquement lorsque toutes les images que vous envoyez contiennent des données de profil de couleur incorrectes ou manquantes.

* **OPTIONS**  DE MODIFICATION D&#39;IMAGE - Vous pouvez conserver les  &lt;> masques d&#39;écrêtage dans les images et choisir un profil de couleur.
(voir [Options d’édition d’images au téléchargement](image-editing-options-upload.md#image-editing-options-at-upload)).

* **OPTIONS**  de PostScript® : vous pouvez pixelliser des fichiers de PostScript®, recadrer des fichiers, conserver des arrière-plans transparents, choisir une résolution et choisir un espace colorimétrique.
(voir [Utilisation de fichiers PostScript et Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)).

* **OPTIONS**  Photoshop : vous pouvez créer des modèles à partir de fichiers Photoshop® Adobe®, conserver des calques, indiquer comment les calques sont nommés, extraire du texte et indiquer comment les images sont ancrées dans les modèles.
(voir [Options de téléchargement des fichiers PSD](psd-files.md#psd_upload_options)).

* **OPTIONS**  PDF : vous pouvez pixelliser les fichiers, extraire des mots de recherche et des liens, générer automatiquement un catalogue électronique, définir la résolution et choisir un espace colorimétrique.
(voir [Options de téléchargement des fichiers PDF](pdfs.md#pdf_upload_options)).

* **OPTIONS**  ILLUSTRATOR - Vous pouvez pixelliser des fichiers Adobe Illustrator®, conserver des arrière-plans transparents, choisir une résolution et choisir un espace colorimétrique.
(voir [Utilisation de fichiers PostScript et Illustrator](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)).

* **OPTIONS**  EVIDEO - Vous pouvez transcoder un fichier vidéo en choisissant un paramètre vidéo prédéfini.
Voir [Utilisation des paramètres prédéfinis de codage vidéo](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **MÉTADONNÉES**  SUPPLÉMENTAIRES - Entrez les mots-clés qui décrivent les fichiers que vous prévoyez de télécharger. Séparez les mots clés-par des virgules. Les mots-clés facilitent les recherches portant sur les fichiers Voir [Recherche avancée](searching-assets.md#conducting_an_advanced_search).

* **PARAMÈTRES PRÉDÉFINIS**  DE VISIONNEUSES PAR LOTS - Si vous souhaitez créer une visionneuse d’images, une visionneuse à 360° multi-axe ou une série d’échantillons à partir des fichiers téléchargés, cliquez sur la colonne Principale du paramètre prédéfini à utiliser. Rien ne vous empêche de sélectionner plusieurs paramètres prédéfinis. Vous créez les paramètres prédéfinis sur la page Configuration de l’application/Paramètres prédéfinis d’ensemble par lot (voir [Paramètres prédéfinis d’ensemble par lot](application-setup.md#batch_set_presets)).

* **AVANCÉ**  - Voir  [Suivre un téléchargement avec une autre tâche](uploading-files.md#follow-an-upload-with-another-job).

## Enchaînement d’une tâche de téléchargement et d’une autre tâche {#follow-an-upload-with-another-job}

Lorsque vous téléchargez des éléments à l’aide du protocole FTP, vous pouvez planifier une tâche ultérieure pour qu’elle commence une fois le transfert terminé. Si d’autres tâches doivent commencer, la tâche planifiée ici est mise en file d’attente après elles.

La nouvelle tâche envoie une notification à l’adresse spécifiée par vos soins de manière à déclencher ce code à cet emplacement. Cette tâche de publication consécutive reprend le nom de la tâche de téléchargement, mais ajoute *Pub_* devant le nom.

**Enchaînement d’une tâche de téléchargement et d’une autre tâche:**

1. Cliquez sur **[!UICONTROL Télécharger]**, puis sur l&#39;onglet **[!UICONTROL VIA FTP]**.
1. Dans le coin inférieur droit de la page de téléchargement, cliquez sur **[!UICONTROL Options tâche]**.
1. Dans la boîte de dialogue Télécharger les options de la tâche, développez la section **[!UICONTROL AVANCÉE]**.
1. Sélectionnez l’une des options suivantes dans la liste déroulante **[!UICONTROL Suivre le téléchargement avec une autre tâche]** :

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
   >Les tâches planifiées régulièrement peuvent parfois entraîner la publication d’aucun fichier.

>[!MORELIKETHIS]
>
>* [Utilisation de dossiers de fichiers](asset-folders.md#working_with_asset_folders)
>* [Gestion de tâches de téléchargement et de publication périodiques](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Utilisation d’une tâche de téléchargement ou de publication comme déclencheur](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)

