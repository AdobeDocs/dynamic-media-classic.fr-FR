---
title: Création d’un document PDF
seo-title: Création d’un document PDF
description: 'null'
seo-description: Découvrez comment créer un document PDF à l’aide du processus d’impression en ligne dans Dynamic Media Classic.
uuid: 274fb06b-320b-40fa-8b61-c224d8aceaa1
contentOwner: admin
content-type: référence
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template-publishing
discoiquuid: 87e91e8e-10a2-4fba-87c7-aad2bd798146
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Création d’un document PDF {#creating-a-pdf-document}

La dernière étape du processus d’impression en ligne consiste à créer un document PDF personnalisé. Pour ce faire, les utilisateurs doivent d’abord personnaliser le modèle à l’aide de l’application en ligne que vous avez créée, puis créer le fichier PDF final. Ensuite, le fichier PDF final est généralement envoyé à un prestataire de prépresse pour une impression professionnelle. Pour s’assurer que le fichier PDF final est imprimé comme prévu, les développeurs utilisent un fichier joboptions et configurent les polices, les repères d’impression et les couleurs en conséquence.

## Configuration des paramètres prédéfinis d’un document PDF {#setting-up-pdf-presets}

Spécifiez le niveau de compatibilité PDF et les paramètres d’imprimante en créant et en téléchargeant un fichier PDF joboptions sur le serveur Dynamic Media Classic. Vous pouvez par exemple sélectionner l’option de compatibilité PDF/X-4 pour votre sortie PDF (recommandée pour les flux de travail de publication d’impression PDF). Le fichier joboptions peut être créé dans un logiciel de création (comme Adobe Illustrator) ou dans Acrobat. Vérifiez toujours avec votre imprimeur ; il sera en mesure de vous conseiller sur les paramètres appropriés à votre tâche d’impression.

Pour plus d’informations sur la création de fichiers joboptions et sur la création d’un fichier joboptions dans Acrobat, voir l’Aide d’Adobe Acrobat.

Pour créer un fichier joboptions dans Illustrator :

1. Choisissez Edition &gt; Paramètres prédéfinis Adobe PDF.
1. Dans la boîte de dialogue qui apparaît, sélectionnez le paramètre prédéfini à utiliser.

   Les paramètres d’option de tâche suivants sont pris en charge par Dynamic Media Classic :

   | Option de tâche | Description |
   |--- |--- |
   | Généraux | <ul><li>Compatibilité </li><li>Compression de niveau objet</li><li>Incorporer les vignettes</li><li>Optimiser pour l’affichage rapide des pages Web</li></ul> |
   | Images | <ul><li>Sous-échantillonnage</li><li>Résolution</li><li>Seuil</li><li>Compression couleur/niveaux de gris/monochrome</li></ul> |
   | Polices | <ul><li>Incorporer toutes les polices (les polices sont incorporées par défaut)</li><li>Incorporer les polices OpenType</li><li>Jeux partiels de polices lorsque le pourcentage de caractères est inférieur à :</li><li>Liste Toujours incorporer</li><li>Liste Ne jamais incorporer</li></ul> |
   | Couleur | <ul><li>Gestion des couleurs (l’option Référencer les images uniquement est traitée comme l’option Référencer les couleurs)</li><li>Mode de rendu du document</li><li>Seuls les espaces de travail suivants sont pris en charge par la version 4.2.5. Dans la version 4.3, vous pourrez utiliser n’importe quel profil de client téléchargé dans IPS.</li><li>En attendant, vous pouvez spécifier l’espace colorimétrique de destination de l’illustration à convertir au moyen des profils colorimétriques par défaut de la société.</li></ul> |
   | RVB | <ul><li>e-sRGB </li><li>scRGB with encoding range [-4.0, 4.0]</li><li>Lab D50</li><li>PCS XYZ</li><li>Flat XYZ</li><li>Linear ROMM-RGB</li><li>ROMM-RGB</li><li>sYCC 8-bit</li><li>e-sYCC 8-bit</li></ul> |
   | Gris | <ul><li>Gray Gamma 1.8</li><li>Gray Gamma 2.2</li><li>Dot Gain 10%</li><li>Dot Gain 15%</li><li>Dot Gain 20%</li><li>Dot Gain 25%</li><li>Dot Gain 30%</li><li>sGray</li></ul> |
   | Conserver les valeurs CMJN pour les espaces colorimétriques CMJN étalonnés |  |
   | Avancés | Conserver les commentaires OPI (option toujours activée) |
   | Normes | Norme de conformité |

   >[!NOTE]
   >
   >Dynamic Media Classic ignore les paramètres de repères d’impression dans le fichier joboptions. Les repères d’impression sont plutôt configurés à l’aide des commandes URL de Dynamic Media Classic.

1. Cliquez sur Exporter, spécifiez ensuite un nom et un emplacement, puis cliquez sur Enregistrer.
1. Téléchargez le fichier d’options de tâche en tant que fichier vers Scene7 Publishing System.

   Utilisez le fichier avec votre modèle publié en y faisant référence dans l’URL. Par exemple :

   `https://yourpublishserver.scene7.com/is/agm/SiliconPublishing/PetNews?&fmt=pdf,cmyk&joboption=SPSfilenameid`

## Préparation d’un fichier PDF pour l’impression {#preparing-the-pdf-for-print}

Avant de finaliser le fichier PDF pour l’impression, assurez-vous d’avoir respecté à la lettre les instructions figurant dans cette section.

**Images**

Assurez-vous que toutes les images de votre tâche de publication ont été téléchargées sur votre serveur Dynamic Media Classic et publiées.

**Polices**

Assurez-vous que toutes les polices de votre tâche de publication ont été téléchargées sur votre serveur Dynamic Media Classic et publiées. Assurez-vous que vous disposez des droits nécessaires pour autoriser les nouvelles polices si vous voulez autoriser les utilisateurs à modifier les polices.

**Résolution d’image (pixels par pouce)**

La résolution des images bitmap est conservée par le serveur Dynamic Media Classic dans les fichiers PDF générés prêts pour l’impression. Dynamic Media Classic met à niveau la résolution des images si nécessaire. Pour optimiser les résultats, laissez la résolution par défaut (en général 72 ppp) lorsque vous prévisualisez un fichier en ligne. La résolution par défaut appliquée à toutes les images de votre société est définie dans la fenêtre Paramètres de publication/Image Server, à la section Résolution d’impression par défaut. Des résolutions plus élevées (comme 300 ppp) peuvent allonger le traitement et doivent être appliquées uniquement à un fichier PDF prêt pour l’impression. Insérez la commande imageRes= dans l’URL pour remplacer manuellement la résolution par défaut pour les tâches PDF.

**Gestion des couleurs**

Vous pouvez appliquer à votre document et à vos images les modèles de couleurs Gris, CMJN, Ton direct, RVB ou Lab. Il est possible d’étalonner ou non chacun de ces modèles de couleurs au moyen d’un profil de couleur ICC. Pour de meilleurs résultats, incorporez le profil dans le fichier PDF prêt pour l’impression. Le serveur Dynamic Media Classic le fait par défaut. Assurez-vous que tous les profils colorimétriques requis ont été téléchargés sur la plateforme Dynamic Media Classic. Assurez-vous, de préférence, que les options de gestion des couleurs définies dans votre application de conception correspondent à celles définies dans votre serveur Dynamic Media Classic :

* **Paramètres de gestion des couleurs de l’application de création :** dans les paramètres de couleurs de votre application de création (par exemple, Adobe Illustrator), spécifiez les profils de couleurs RVB et CMJN dans la section des espaces de travail.

* **** Paramètres de gestion des couleurs de Dynamic Media Classic : En règle générale, les paramètres de gestion des couleurs de l’application de conception doivent correspondre aux profils de couleurs par défaut de votre serveur Dynamic Media Classic. Ces paramètres sont disponibles dans la fenêtre Configuration de la publication d’Image Server.

## Affichage des repères d’impression {#displaying-printer-marks}

Vous pouvez créer un document PDF pour :

* un document terminé ;
* un document intermédiaire, tel qu’un film ou une plaque, pouvant être envoyé à un imprimeur.

Un document intermédiaire peut comprendre du contenu de production supplémentaire, comme des marges de fond perdu, des repères d’impression et autres. Ce contenu apparaît en général au-delà des bordures de la page finale.

Tous les repères disponibles dans l’écran « Ajouter des repères d’impression » dans Acrobat sont pris en charge. Les repères d’imprimante sont contrôlés avec le paramètre `printerMark`. The syntax is `&printerMark=trim marks, bleed marks, registration marks, color bars, page information, style, line weight, layer embed`.

* trim marks = 0|1
* bleed marks = 0|1
* registration marks = 0|1
* color bars = 0|1
* page information = 0|1
* style = Illustrator | IllustratorJ | QuarkXPress
* line weight = 0.125 | 0.25 | 0.50
* layer embed = 0|1

Lors de la préparation d’un document à imprimer, les repères d’impression peuvent être nécessaires pour aider le service d’impression à aligner les films de séparation pour produire des épreuves, mesurer le film pour l’étalonnage et la densité d’encre corrects, ajuster le film à la taille, etc. Les repères d’impression indiquent les limites des zones du document telles que les zones de rognage et les zones de fond perdu. Le contenu lié à la production peut inclure :

* **Zone** multimédia Limites du support physique sur lequel la page sera imprimée. Le contenu hors de la zone de support peut être supprimé sans affecter la signification du fichier.

* **Zone** de fond perdu Zone dans laquelle le contenu de la page est coupé lors de la sortie dans un environnement de production. La zone de fond perdu peut inclure les zones nécessaires pour prendre en compte les limites physiques du matériel de découpe, pliage et rognage. La valeur par défaut est la zone de recadrage de la page.

* **Zone** de rognage Dimensions souhaitées de la page terminée après rognage. La zone de rognage peut être plus petite que la zone de support, pour pouvoir ajouter le contenu lié à la production (instructions d’impression, traits de coupe et gammes de couleurs). La valeur par défaut est la zone de recadrage de la page.

* **Zone** graphique L’étendue du contenu significatif de la page (y compris l’espace blanc potentiel) tel que prévu par le créateur de la page. La valeur par défaut est la zone de recadrage de la page.

Vous pouvez utiliser les modificateurs illustrés dans ce tableau pour reproduire les repères d’impression disponibles dans Adobe Illustrator, InDesign et Acrobat :

| Modificateur/valeurs | Description |
|--- |--- |
| bleedMargin=haut, gauche, bas, droite | Spécifié dans Acrobat au moyen de l’option Définir des zones de page. Sélectionnez Zone de fond perdu, puis définissez les marges au moyen de l’option Commandes de marge.<br><br>Ces valeurs représentent la distance des bords supérieur, gauche, inférieur et droit par rapport aux bords originaux de l’illustration (zone de support), allant vers l’intérieur. Les valeurs (0 à 1 000) sont exprimées en points.<br><br>Nouvelle hauteur=hauteur d’origine - (haut+bas)<br><br>Nouvelle largeur= largeur d’origine - (gauche+droite) |
| mediaMargin=haut, gauche, bas, droite | Spécifié dans Acrobat au moyen de l’option Définir des zones de page. Modifiez la taille de la page personnalisée au moyen de l’option Modification du format de page.<br><br>Ces valeurs représentent la distance des bords supérieur, gauche, inférieur et droit par rapport aux bords originaux de l’illustration (zone de support), allant vers l’extérieur. Les valeurs (0 à 1 000) sont exprimées en points.<br><br>Nouvelle hauteur=haut+bas+<br><br>hauteur d’origineNouvelle largeur=haut+bas+<br><br>largeur d’origineLes nouvelles valeurs de hauteur et de largeur déterminent le nouveau format de page du PDF généré.<br><br>Lorsqu’une nouvelle zone de support est définie, tous les calculs de marge de rognage et de marge de fond perdu doivent tenir compte de la nouvelle zone de support comme limites de l’illustration. |
| trimMargin=haut, gauche, bas, droite | Spécifié dans Acrobat au moyen de l’option Définir des zones de page. Sélectionnez Zone de rognage, puis définissez les marges au moyen de l’option Commandes de marge.<br><br>Ces valeurs représentent la distance des bords supérieur, gauche, inférieur et droit par rapport aux bords originaux de l’illustration (zone de support), allant vers l’intérieur. Les valeurs (0 à 1 000) sont exprimées en points.<br><br>Nouvelle hauteur=hauteur d’origine - (haut+bas)<br><br>Nouvelle largeur=largeur d’origine - (gauche+droite) |
| printerMark= repères de rognage, repères de fond perdu, repères de montage, gammes de couleurs, informations sur la page, style, épaisseur du trait, calque incorporé | Les valeurs sont les suivantes :<br><br>repères de rognage = 0,1 (la valeur par défaut est 0)<br><br>repères de fond perdu = 0,1 (la valeur par défaut est 0)<br><br>repères de montage = 0,1 (la valeur par défaut est 0)Barres de<br><br>couleurs = 0,1 (la valeur par défaut est 0)Informations de<br><br>page = 0,1 (la valeur par défaut est 0)<br><br>style = Par défaut, Instyle = Par défaut, InDesignJ1, InDesignJ1, InJJ2, InDesignDesignJJ2, InJJ2, Illustrator, Illustrator, Illustrator, Illustrator QuarkXPress (valeur par défaut : Default)<br><br>line weight= 0.125-0.2, les deux valeurs inclusives (valeur par défaut : 0.25)layer embed = 0, 1, avec 1 créant un nouveau calque contenant tous les repères d’impression (valeur par défaut : 1)Selon le style utilisé, les repères et les gammes de couleurs apparaissent différents et correspondent aux styles correspondants utilisés par Acrobat.<br><br><br><br> |

Notez les éléments suivants au sujet des repères d’impression :

* Précisez les marges de fond perdu, de rognage et de support via les appels d’URL lors de la spécification des repères d’impression. Si les repères d’impression sont spécifiés sans avoir précisé ces marges, les repères s’affichent en dehors de la partie visible du fichier PDF créé. En outre, les repères de rognage et les repères de fond perdu se chevaucheront.
* Si la même valeur est spécifiée pour la marge de rognage et la marge de fond perdu, les repères de rognage et les repères de fond perdu se chevauchent lorsque ces deux indicateurs équivalent à 1 dans `&printerMark`.
* Si les formats fmt=swf/image sont spécifiés via les appels d’URL, le document est imprimé sans repère ni marge, car cette fonction est spécifique aux sorties PDF.
* Specifying `&printerMark=`through the URL results in default values being used for all parameters. Specifying `&printerMark=1` results in trim marks being set to 1 and default values for other parameters. Mais, pour que le énième élément (nth) soit défini sur ON, tous les paramètres (n-1) doivent être spécifiés via l’URL.
* Specifying only one value for `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in that value being applied to all the top, bottom, left, and right margins of the original artwork.
* Specifying only the top and left values through `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in the top value being assigned to the bottom value and the left value being equal to the right.
* Not specifying the right value through `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in the left value being assigned to the right.
* Pour un fichier PDF de plusieurs pages, les marges/repères d’impression sont appliqués à toutes les pages (dans Acrobat, les utilisateurs peuvent appliquer ces repères/marges sur des étendues de pages).
* La sortie d’un document PDF avec des repères/marges activés correspond exactement à une sortie Acrobat X sauf autrement spécifié.

Lorsque vous créez un document PDF compatible PDF/X-4 à l’aide du modificateur &amp;joboption dans l’URL, vous devez tenir compte des limites liées aux repères d’impression spécifiés dans le fichier PDF ISO_15930-7-2008.pdf :

* Chacun des objets de page d’un fichier PDF inclut une zone de support. Et chaque objet de page d’un fichier PDF/X-4 conforme doit inclure soit une zone de rognage, soit une zone graphique, mais pas les deux. Par ailleurs, la zone de support peut être héritée.
* Si une zone de fond perdu est incluse, la zone graphique ou la zone de rognage ne doit pas s’étendre au-delà des limites de la zone de fond perdu. Si une zone de recadrage est incluse, ni la zone graphique, ni la zone de rognage, ni la zone de fond perdu ne doit s’étendre au-delà des limites de la zone de recadrage.
* Ni la zone graphique, ni la zone de rognage, ni la zone de fond perdu ne doit s’étendre au-delà des limites de la zone de support.
* Certaines pratiques dans le secteur imposent d’utiliser la zone de fond perdu. Vous devez suivre les pratiques qui conviennent.
* Il est préférable d’utiliser la zone de rognage plutôt que la zone graphique.
* La valeur Rect de toutes les annotations autres que TrapNet et PrinterMark doit se trouver totalement en dehors de la zone de fond perdu (ou des zones de rognage ou graphique en l’absence de zone de fond perdu). La valeur Rect de toutes les annotations PrinterMark doit être totalement en dehors de la zone de rognage ou de la zone graphique. Un lecteur conforme au format PDF/X-4 peut ignorer complètement les annotations hormis les annotations PDF TrapNet.
* Une valeur Rect doit être considérée comme totalement hors des limites de la zone si toutes les coordonnées de cette valeur se trouvent au-delà des limites ou sur les bords et si l’intersection de deux rectangles est au point zéro.
* Si le dictionnaire ViewerPreferences contient les clés ViewArea, ViewClip, PrintArea ou PrintClip, chacune de ces clés contient la valeur MediaBox ou (si une zone de fond perdu est présente dans tous les objets de page du fichier) BleedBox.

