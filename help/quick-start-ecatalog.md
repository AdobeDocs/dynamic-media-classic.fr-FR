---
title: '"Démarrage rapide : Catalogues électroniques"'
seo-title: '"Démarrage rapide : Catalogues électroniques"'
description: 'null'
seo-description: Une introduction et un démarrage rapide des catalogues électroniques pour vous aider à maîtriser rapidement les techniques de catalogue électronique.
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: admin
content-type: référence
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
translation-type: tm+mt
source-git-commit: e1b74f30faab334453f941e9075910c8a8565462

---


# Démarrage rapide : Catalogues électroniques{#quick-start-ecatalogs}

Un catalogue électronique est une version en ligne numérique de documents imprimés, tels qu’un catalogue, une brochure, un dépliant, un guide de produits ou un prospectus. Un catalogue électronique s’affiche dans une visionneuse de catalogue électronique sur un site Web. Cette visionneuse simule le processus de lecture de documents imprimés. Selon les paramètres que vous choisissez pour votre catalogue électronique, le lecteur de contenu peut vous permettre d’effectuer les opérations suivantes :

* Recherchez un mot-clé ou des mots-clés dans le catalogue. Les résultats de la recherche s’affichent sous la forme d’une liste de miniatures dans un panneau de recherche situé à gauche du catalogue. Chaque miniature cliquable représente une planche de catalogue dans laquelle le terme de recherche surligné a été trouvé.

* Partagez le catalogue sur les réseaux sociaux ; télécharger le catalogue pour l’afficher hors ligne ; activez l’option Favoris pour marquer les éléments auxquels vous souhaitez revenir rapidement ou pour imprimer le catalogue.
* Accédez au catalogue à l’aide de la table des matières ou de la vue de grille de page ; en avant ou en arrière en cliquant sur le bord central d’une page.
* effectuer un zoom avant, un zoom arrière ou un panoramique pour examiner des articles figurant sur une page ;
* déplacer le pointeur sur une zone de la page (appelée zone cliquable) pour afficher une fenêtre contextuelle contenant des informations sur un article ;
* cliquer sur une zone de la page pour ouvrir une nouvelle page Web contenant d’autres informations sur un article ;
* rédiger un pense-bête et l’associer à une page du catalogue électronique ;
* cliquer sur les icônes d’images interactives pour lancer les pages Web associées ou les panneaux d’informations contextuels ;
* utiliser les interactions de mouvement, y compris le zoom pincé et le feuilletage des pages ;
* effectuer des recherches par mot-clé.

![Catalogue électronique présenté aux utilisateurs. A) Page d’ouverture du catalogue électronique. B)eCatalog turned to page 2.](/help/assets/ec_cat_viewer_popup.png)

En règle générale, pour créer un catalogue électronique, vous utilisez des fichiers PDF haute résolution créés dans Adobe® Acrobat® ou un autre programme d’impression. Néanmoins, rien ne vous empêche d’avoir recours à des fichiers d’images.

Lorsque vous créez un catalogue électronique, vous agencez les pages ou les planches dans l’ordre de votre choix. Vous pouvez également indiquer si vous souhaitez obtenir des pages simples, des planches en double page ou des planches de plusieurs pages. A cela s’ajoute la possibilité de créer des zones cliquables à certains endroits de la page, afin que les utilisateurs puissent ouvrir une nouvelle page de votre site Web d’un simple clic. Vous pouvez gérer le texte de survol qui s’affiche à l’aide des paramètres du panneau d’informations dans l’écran Catalogue électronique. Vous disposez également de plus de 100 options de configuration différentes pour configurer la visionneuse de catalogue électronique à votre convenance. Vous pouvez ainsi adapter les fonctionnalités et l’aspect de votre visionneuse en fonction de votre clientèle.

>[!NOTE]
>
>Si vous êtes un utilisateur du mode AEM Dynamic Media - Scene7 et souhaitez utiliser des catalogues électroniques, vous devez modifier la `pdfbrochure` valeur dans CRXDE Lite. Pour ce faire, dans AEM, cliquez sur Outils **[UICONTROL &gt; Général &gt; CRXDE Lite]**. Dans l’arborescence de navigation du panneau de gauche, accédez à `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
Dans le volet inférieur droit, dans l’onglet **Propriétés** , sélectionnez la `jobParam` ligne. Définissez la valeur de `pdfbrochure` de `false` à `true`. Comme dans `pdfbrochure=true`le coin supérieur gauche de la page CRXDE Lite, cliquez sur **Enregistrer tout**.
Vous pouvez désormais créer des catalogues électroniques dans SPS.

**Démarrage rapide**

Cette section de démarrage rapide est conçue pour vous aider à maîtriser rapidement les opérations liées aux catalogues électroniques. Suivez les étapes 1 à 7. Chaque étape se termine par un renvoi à une rubrique contenant de plus amples informations.

**Cookie. Téléchargement des fichiers PDF**

En règle générale, un catalogue électronique est créé à partir de fichiers Adobe PDF. Les fichiers PDF étant destinés à l’impression, ils contiennent le plus souvent des images CMJN. Scene7 Publishing System détecte ces images et les convertit à l’aide d’un profil de couleurs CMJN standard. Cependant, vous pouvez être amené à télécharger et à utiliser un profil de couleurs personnalisé.

Cliquez sur Télécharger dans la barre de navigation globale pour commencer à télécharger des fichiers PDF ou des images pour votre catalogue électronique. Vous pouvez télécharger des fichiers depuis votre bureau ou via FTP, cette dernière méthode étant recommandée si les fichiers sont nombreux ou de taille supérieure à 100 Mo.

La section Options PDF de l’écran de téléchargement contient des options qui permettent de télécharger des fichiers PDF présentant l’espace colorimétrique adéquat et la résolution voulue. Une résolution de 150 pixels par pouce est recommandée. L’option Générer automatiquement un catalogue permet de créer un catalogue lors du téléchargement d’un fichier PDF.

Voir [Téléchargement des fichiers PDF](uploading-pdf-files.md#uploading_the_pdf_files).

**2. Création d’un catalogue électronique**

Pour créer un catalogue électronique, choisissez les fichiers PDF ou d’images voulus dans le panneau de navigation, cliquez sur le bouton Créer, puis choisissez l’option Catalogues électroniques. L’écran Catalogue électronique s’affiche.

Sous l’onglet Ordre des pages, cliquez sur un bouton Disposition (1 vignette, 2 vignettes ou Personnalisé) pour indiquer si vous souhaitez obtenir des planches d’une seule page, des planches en double page ou des planches personnalisées. Vous pouvez réorganiser les pages ou les planches en les faisant glisser ou, dans le cas de catalogues électroniques volumineux, en choisissant un nom de page dans le menu Déplacer vers.

Pour ajouter des pages, sélectionnez un dossier dans la bibliothèque de fichiers, puis faites glisser les fichiers PDF ou d’images dans l’écran Ordre des pages. Si les numéros de page par défaut ne vous conviennent pas, vous pouvez indiquer des noms de page personnalisés ou importer un grand nombre de noms de page.

Cliquez sur le bouton Enregistrer, nommez votre catalogue électronique, choisissez le dossier SPS dans lequel le stocker, puis cliquez sur Envoyer. Vous devez cliquer sur le bouton Enregistrer chaque fois que vous modifiez l’agencement des pages ou le catalogue électronique pour que vos modifications soient conservées.

Voir [Création d’un catalogue électronique](creating-ecatalog.md).

**Cookie. Création de zones cliquables**

Les zones cliquables ajoutent une nouvelle dimension aux pages des catalogues électroniques. Une zone cliquable correspond à une zone de la page permettant d’afficher d’autres informations sur un article. Lorsque les utilisateurs placent le pointeur sur une zone cliquable, une description de l’article en question s’affiche. La sélection d’une zone cliquable a pour effet d’activer une référence externe qui permet d’ouvrir une nouvelle page Web contenant des informations supplémentaires sur un article.

Pour créer une zone cliquable, ouvrez l’écran Catalogue électronique. Accédez ensuite à l’onglet Pages de zones de l’écran Catalogue électronique, puis tracez la zone à l’aide de l’outil de zone cliquable rectangulaire  ou de l’outil de zone cliquable polygonale. Vous pouvez ajuster la position et la taille d’une zone cliquable en faisant glisser ses bordures à l’aide de l’outil Panoramique.

Après avoir tracé la zone cliquable, indiquez l’URL à atteindre lorsque vous cliquez sur cette zone. Vous pouvez également indiquer le texte de survol qui s’affiche lorsque le pointeur se trouve sur la zone cliquable.

Voir [Création de zones cliquables dans un catalogue électronique](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

Voir [Utilisation des zones cliquables pour intégrer des médias enrichis dans un catalogue électronique](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

Vous pouvez configurer et gérer le texte de zone cliquable à l’aide des paramètres du panneau d’informations de l’écran Catalogue électronique.

Voir [Gestion du contenu du panneau d’informations](info-panel-content.md#managing-info-panel-content).

**4. Configuration des paramètres prédéfinis de la visionneuse de catalogue électronique**

Les utilisateurs finaux consultent votre catalogue dans la visionneuse de catalogue électronique. Si vous êtes un administrateur, vous avez la possibilité de configurer cette visionneuse. Vous pouvez modifier la couleur de son contour et sélectionner un nouvel habillage pour définir la marque de votre catalogue électronique. Dynamic Media Classic est fourni avec plusieurs paramètres prédéfinis de visionneuse de catalogue électronique de "bonnes pratiques". Vous pouvez choisir l’un de ces paramètres prédéfinis pour afficher vos catalogues électroniques. Vous pouvez également créer vous-même un paramètre prédéfini pour la visionneuse de catalogue électronique si vous êtes administrateur.

Pour créer un paramètre prédéfini de visionneuse de catalogue électronique, cliquez sur le bouton Configuration de la barre de navigation globale, puis choisissez Paramètres prédéfinis de la visionneuse. Then click Add, choose a platform, and choose **[UICONTROL eCatalog &gt; Viewer]**.

(Voir [Configuration des paramètres prédéfinis de la visionneuse de catalogue électronique](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).)

**5. Prévisualisation des catalogues électroniques dans la visionneuse de catalogue électronique**

Les paramètres prédéfinis de visionneuse de catalogue électronique déterminent le style et le comportement de vos visionneuses de catalogue électronique.

Pour découvrir de quelle manière les paramètres prédéfinis de visionneuse de catalogue électronique affichent votre catalogue, sélectionnez votre catalogue électronique dans le panneau de navigation et cliquez sur Prévisualiser. L’écran de prévisualisation s’ouvre dans la visionneuse par défaut.

Observez l’orientation des pages, la palette de couleurs, l’aspect des commandes permettant de changer de page et la manière dont les pages s’affichent lorsque vous les feuilletez.

Voir [Prévisualisation des catalogues électroniques dans la visionneuse de catalogue électronique](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

**6. Publication d’un catalogue électronique et des fichiers PDF associés**

Lorsque vous publiez votre catalogue électronique et le fichier PDF associé, il est placé sur les serveurs d’images Contenu multimédia dynamique afin de pouvoir être diffusé sur votre site Web et dans votre application. Scene7 Publishing System active la chaîne URL de votre catalogue électronique au cours du processus de publication. Utilisez cette URL pour appeler le catalogue électronique à partir des serveurs d’images de Contenu multimédia dynamique vers votre site Web ou votre application.

Après avoir marqué votre catalogue électronique et votre PDF pour publication dans le panneau de navigation, sélectionnez le bouton Publier de la barre de navigation globale pour lancer une publication. Dans l’écran Publier, cliquez sur Lancer publication.

Voir [Publication de catalogues électroniques et de fichiers PDF](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs)associés.

**7. Liaison d’un catalogue électronique à une page Web**

Dynamic Media Classic active la chaîne d’appel d’URL nécessaire pour afficher votre catalogue électronique lorsque vous le publiez sur les serveurs d’images de Contenu multimédia dynamique. Vous pouvez copier cette chaîne URL depuis l’écran de prévisualisation et le panneau de navigation (en mode Affichage des détails) en la sélectionnant dans le panneau. Une fois copiée, la chaîne URL peut être utilisée sur vos sites Web et dans vos applications.

Travaillez de concert avec votre équipe informatique pour décider de l’emplacement du lien vers le catalogue électronique au sein de votre page Web. Un clic sur ce lien entraîne l’ouverture de la visionneuse, permettant ainsi aux utilisateurs de parcourir votre catalogue électronique.

Voir [Liaison d’un catalogue électronique à une page Web](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
