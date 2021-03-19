---
title: '"Début rapide : Catalogues électroniques"'
description: Une introduction et un Début rapide aux catalogues électroniques pour vous aider à maîtriser rapidement les techniques de catalogue électronique.
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
feature: Dynamic Media Classic, Visionneuses, Catalogue électronique
role: Professionnel
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '1453'
ht-degree: 63%

---


# Début rapide : Catalogues électroniques{#quick-start-ecatalogs}

Un catalogue électronique est une version en ligne numérique de documents imprimés, tels qu’un catalogue, une brochure, un dépliant, un guide de produits ou un prospectus. Un catalogue électronique s’affiche dans une visionneuse de catalogue électronique sur un site Web. Cette visionneuse simule le processus de lecture de documents imprimés. Selon les paramètres que vous choisissez pour votre catalogue électronique, la visionneuse peut vous permettre d’effectuer les opérations suivantes :

* Recherchez un mot-clé ou des mots-clés dans le catalogue. Les résultats de la recherche s’affichent sous la forme d’une liste de miniatures dans un panneau de recherche situé à gauche du catalogue. Chaque miniature cliquable représente une planche de catalogue dans laquelle le terme de recherche mis en surbrillance a été trouvé.

* partager le catalogue au moyen des médias sociaux ; télécharger le catalogue vers la vue hors ligne ; activez Favoris pour marquer les éléments auxquels vous souhaitez revenir rapidement ou pour imprimer le catalogue.
* Accédez au catalogue à l’aide de la table des matières ou de la vue de grille de pages ; en avant ou en arrière en cliquant sur le bord central d’une page.
* effectuer un zoom avant, un zoom arrière ou un panoramique pour examiner des articles figurant sur une page ;
* déplacer le pointeur sur une zone de la page (appelée zone cliquable) pour afficher une fenêtre contextuelle contenant des informations sur un article ;
* cliquer sur une zone de la page pour ouvrir une nouvelle page Web contenant d’autres informations sur un article ;
* rédiger un pense-bête et l’associer à une page du catalogue électronique ;
* cliquer sur les icônes d’images interactives pour lancer les pages Web associées ou les panneaux d’informations contextuels ;
* utiliser les interactions de mouvement, y compris le zoom pincé et le feuilletage des pages ;
* effectuer des recherches par mot-clé.

![Catalogue électronique présenté aux utilisateurs. A) Page d’ouverture du catalogue électronique. B)Le catalogue électronique est passé à la page 2.](/help/assets/ec_cat_viewer_popup.png)

En règle générale, pour créer un catalogue électronique, vous utilisez des fichiers PDF haute résolution créés dans Adobe® Acrobat® ou un autre programme d’impression. Néanmoins, rien ne vous empêche d’avoir recours à des fichiers d’images.

Lorsque vous créez un catalogue électronique, vous agencez les pages ou les planches dans l’ordre de votre choix. Vous pouvez également indiquer si vous souhaitez obtenir des pages simples, des planches en double page ou des planches de plusieurs pages. A cela s’ajoute la possibilité de créer des zones cliquables à certains endroits de la page, afin que les utilisateurs puissent ouvrir une nouvelle page de votre site Web d’un simple clic. Vous pouvez gérer le texte de survol qui s’affiche à l’aide des paramètres du panneau d’informations dans l’écran Catalogue électronique. Vous disposez également de plus de 100 options de configuration différentes pour configurer la visionneuse de catalogue électronique à votre convenance. Vous pouvez ainsi adapter les fonctionnalités et l’aspect de votre visionneuse en fonction de votre clientèle.

>[!NOTE]
>
>Si vous êtes un utilisateur AEM mode Dynamic Media - Scene7 et que vous souhaitez utiliser des catalogues électroniques, vous devez modifier la valeur `pdfbrochure` dans CRXDE Lite. Pour ce faire, dans AEM, cliquez sur **[!UICONTROL Outils > Général > CRXDE Lite]**. Dans l’arborescence de navigation du panneau de gauche, accédez à `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>Dans le volet inférieur droit, dans l&#39;onglet **[!UICONTROL Propriétés]**, sélectionnez la ligne `jobParam`. Définissez la valeur de `pdfbrochure` de `false` sur `true`. Comme dans `pdfbrochure=true`
>
>Dans le coin supérieur gauche de la page du CRXDE Lite, cliquez sur **[!UICONTROL Enregistrer tout]**.
>
>Vous pouvez désormais créer des catalogues électroniques dans Dynamic Media Classic.

**Début rapide**

Cette section de démarrage rapide est conçue pour vous aider à maîtriser rapidement les opérations liées aux catalogues électroniques. Suivez les étapes 1 à 7. Chaque étape se termine par un renvoi à une rubrique contenant de plus amples informations.

**1. Téléchargement des fichiers PDF**

En règle générale, un catalogue électronique est créé à partir de fichiers Adobe PDF. Les fichiers PDF étant destinés à l’impression, ils contiennent le plus souvent des images CMJN. Dynamic Media Classic détecte ces images et les convertit à l’aide d’un profil de couleurs CMJN standard. Cependant, vous pouvez être amené à télécharger et à utiliser un profil de couleurs personnalisé.

Cliquez sur Télécharger dans la barre de navigation globale pour début de télécharger des fichiers PDF ou des images pour votre catalogue électronique. Vous pouvez télécharger des fichiers depuis votre bureau ou via FTP, cette dernière méthode étant recommandée si les fichiers sont nombreux ou de taille supérieure à 100 Mo.

La section Options PDF de l’écran de téléchargement contient des options qui permettent de télécharger des fichiers PDF présentant l’espace colorimétrique adéquat et la résolution voulue. Une résolution de 150 pixels par pouce est recommandée. L’option Générer automatiquement un catalogue permet de créer un catalogue lors du téléchargement d’un fichier PDF.

Voir [Téléchargement des fichiers PDF](uploading-pdf-files.md#uploading_the_pdf_files).

**2. Création d’un catalogue électronique**

Pour créer un catalogue électronique, choisissez les fichiers PDF ou d’images voulus dans le panneau de navigation, cliquez sur le bouton Créer, puis choisissez l’option Catalogues électroniques. L’écran Catalogue électronique s’affiche.

Sous l’onglet Ordre des pages, cliquez sur un bouton Disposition (1 vignette, 2 vignettes ou Personnalisé) pour indiquer si vous souhaitez obtenir des planches d’une seule page, des planches en double page ou des planches personnalisées. Vous pouvez réorganiser les pages ou les planches en les faisant glisser ou, dans le cas de catalogues électroniques volumineux, en choisissant un nom de page dans le menu Déplacer vers.

Pour ajouter des pages, sélectionnez un dossier dans la bibliothèque de fichiers, puis faites glisser les fichiers PDF ou d’images dans l’écran Ordre des pages. Si les numéros de page par défaut ne vous conviennent pas, vous pouvez indiquer des noms de page personnalisés ou importer un grand nombre de noms de page.

Cliquez sur **[!UICONTROL Enregistrer]**, attribuez un nom à votre catalogue électronique, choisissez un dossier Dynamic Media Classic pour le stocker, puis cliquez sur **[!UICONTROL Enregistrer]**. Chaque fois que vous modifiez l’ordre des pages ou votre catalogue électronique, enregistrez vos modifications en cliquant sur **[!UICONTROL Enregistrer]**.

Voir [Création d’un catalogue électronique](creating-ecatalog.md).

**Cookie. Création de zones cliquables**

Les zones cliquables ajoutent une nouvelle dimension aux pages des catalogues électroniques. Une zone cliquable correspond à une zone de la page permettant d’afficher d’autres informations sur un article. Lorsque les utilisateurs placent le pointeur sur une zone cliquable, une description de l’article en question s’affiche. La sélection d’une zone cliquable a pour effet d’activer une référence externe qui permet d’ouvrir une nouvelle page Web contenant des informations supplémentaires sur un article.

Pour créer une zone cliquable, ouvrez l’écran Catalogue électronique. Accédez ensuite à l’onglet **[!UICONTROL Pages de zones]** de l’écran Catalogue électronique, puis tracez la zone à l’aide de l’outil Zone cliquable rectangulaire ou de l’outil Zone cliquable polygonale. Vous pouvez ajuster la position et la taille d’une zone cliquable en faisant glisser ses bordures à l’aide de l’outil Panoramique.

Après avoir tracé la zone cliquable, indiquez l’URL à atteindre lorsque vous cliquez sur cette zone. Vous pouvez également indiquer le texte de survol qui s’affiche lorsque le pointeur se trouve sur la zone cliquable.

Voir [Création de zones cliquables dans un catalogue électronique](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

Voir [Utilisation des zones cliquables pour intégrer des médias enrichis dans un catalogue électronique](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

Vous pouvez configurer et gérer le texte de zone cliquable à l’aide des paramètres du panneau d’informations de l’écran Catalogue électronique.

Voir [Gestion du contenu du panneau d’informations](info-panel-content.md#managing-info-panel-content).

**4. Configuration des paramètres prédéfinis de la visionneuse de catalogue électronique**

Les utilisateurs finaux consultent votre catalogue dans la visionneuse de catalogue électronique. Si vous êtes un administrateur, vous avez la possibilité de configurer cette visionneuse. Vous pouvez modifier la couleur de son contour et sélectionner un nouvel habillage pour définir la marque de votre catalogue électronique. Dynamic Media Classic est fourni avec plusieurs paramètres prédéfinis de visionneuse de catalogue électronique &quot;recommandés&quot;. Vous pouvez choisir l’un de ces paramètres prédéfinis pour l’affichage de vos catalogues électroniques. Vous pouvez également créer vous-même un paramètre prédéfini pour la visionneuse de catalogue électronique si vous êtes administrateur.

Pour créer un paramètre prédéfini de visionneuse de catalogue électronique, sur la barre de navigation globale, cliquez sur **[!UICONTROL Configuration]** et choisissez **[!UICONTROL Paramètres prédéfinis de la visionneuse]**. Cliquez ensuite sur **[!UICONTROL Ajouter]**, choisissez une plate-forme, puis cliquez sur **[!UICONTROL Catalogue électronique > Visionneuse]**.

(Voir [Configuration des paramètres prédéfinis de la visionneuse de catalogue électronique](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).)

**5. Prévisualisation des catalogues électroniques dans la visionneuse de catalogue électronique**

Les paramètres prédéfinis de visionneuse de catalogue électronique déterminent le style et le comportement de vos visionneuses de catalogue électronique.

Pour découvrir comment les paramètres prédéfinis de la visionneuse de catalogue électronique affichent votre catalogue électronique, sélectionnez votre catalogue électronique dans le panneau de navigation, puis cliquez sur **[!UICONTROL Prévisualisation]**. L’écran de prévisualisation s’ouvre dans la visionneuse par défaut.

Observez l’orientation des pages, la palette de couleurs, l’aspect des commandes permettant de changer de page et la manière dont les pages s’affichent lorsque vous les feuilletez.

Voir [Prévisualisation des catalogues électroniques dans la visionneuse de catalogue électronique](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

**6. Publication d’un catalogue électronique et des fichiers PDF associés**

Lorsque vous publiez votre catalogue électronique et le fichier PDF associé, il est placé sur les serveurs Dynamic Media Image Server afin de pouvoir être diffusé sur votre site Web et dans votre application. Dans le cadre du processus de publication, Dynamic Media Classic active la chaîne URL de votre catalogue électronique. Utilisez cette URL pour appeler le catalogue électronique à partir des serveurs Dynamic Media Image Server vers votre site Web ou votre application.

Après avoir marqué votre catalogue électronique et votre fichier PDF pour publication dans le panneau de navigation, cliquez sur le bouton Publier de la barre de navigation globale pour lancer une publication. Dans l’écran Publier, cliquez sur **[!UICONTROL Publier par Début]**.

Voir [Publication de catalogues électroniques et de fichiers PDF associés](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

**7. Liaison d’un catalogue électronique à une page Web**

Dynamic Media Classic active la chaîne d’appel d’URL nécessaire à l’affichage de votre catalogue électronique lorsque vous le publiez sur les serveurs Dynamic Media Image Server. Vous pouvez copier cette chaîne URL depuis l’écran de prévisualisation et le panneau de navigation (en mode Affichage des détails) en la sélectionnant dans le panneau. Une fois copiée, la chaîne URL peut être utilisée sur vos sites Web et dans vos applications.

Travaillez de concert avec votre équipe informatique pour décider de l’emplacement du lien vers le catalogue électronique au sein de votre page Web. Un clic sur ce lien entraîne l’ouverture de la visionneuse, permettant ainsi aux utilisateurs de parcourir votre catalogue électronique.

Voir [Liaison d’un catalogue électronique à une page Web](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
