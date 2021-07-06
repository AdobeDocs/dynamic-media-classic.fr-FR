---
title: '"Démarrage rapide : Catalogues électroniques"'
description: Cette section présente les catalogues électroniques et leur mise en route pour vous aider à maîtriser rapidement les techniques de catalogues électroniques.
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
feature: Dynamic Media Classic,Visionneuses,Catalogue électronique
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '1427'
ht-degree: 50%

---

# Démarrage rapide : Catalogues électroniques{#quick-start-ecatalogs}

Un catalogue électronique est une version en ligne numérique de documents imprimés, tels qu’un catalogue, une brochure, un dépliant, un guide de produits ou un prospectus. Un catalogue électronique s’affiche dans une visionneuse de catalogue électronique sur un site Web. Cette visionneuse simule le processus de lecture de documents imprimés. Selon les paramètres que vous choisissez pour votre catalogue électronique, la visionneuse peut vous permettre d’effectuer les opérations suivantes :

* Recherchez un mot-clé ou des mots-clés dans le catalogue. Les résultats de la recherche s’affichent sous la forme d’une liste de miniatures dans un panneau de recherche sur le côté gauche du catalogue. Chaque miniature cliquable représente une étendue de catalogue où le terme de recherche mis en surbrillance a été trouvé.

* Partagez le catalogue au moyen des médias sociaux ; télécharger le catalogue pour l’afficher hors ligne ; activez l’option Favoris pour marquer les éléments auxquels vous souhaitez revenir rapidement ou pour imprimer le catalogue.
* Naviguez dans le catalogue à l’aide de la table des matières ou de la vue Grille de page ; en avant ou en arrière en cliquant sur le bord central d’une page.
* effectuer un zoom avant, un zoom arrière ou un panoramique pour examiner des articles figurant sur une page ;
* Déplacez le pointeur au-dessus d’une zone de page (appelée zone cliquable) afin d’afficher une fenêtre contextuelle contenant des informations sur un élément.
* Cliquez sur une zone de page pour ouvrir une nouvelle page web contenant des informations supplémentaires sur un élément.
* rédiger un pense-bête et l’associer à une page du catalogue électronique ;
* Appuyez sur les icônes de zone cliquable si vous souhaitez lancer des pages web associées ou des panneaux d’informations contextuelles.
* utiliser les interactions de mouvement, y compris le zoom pincé et le feuilletage des pages ;
* effectuer des recherches par mot-clé.

![Le catalogue électronique tel qu’il s’affiche pour les utilisateurs. A) Page d’ouverture du catalogue électronique. B) Le catalogue électronique est passé à la page 2.](/help/assets/ec_cat_viewer_popup.png)

En règle générale, pour créer un catalogue électronique, vous utilisez des fichiers PDF haute résolution créés dans Adobe® Acrobat® ou un autre programme d’impression. Néanmoins, rien ne vous empêche d’avoir recours à des fichiers d’images.

Lorsque vous créez un catalogue électronique, vous agencez les pages ou les planches dans l’ordre de votre choix. Vous pouvez également indiquer si vous souhaitez obtenir des pages simples, des planches en double page ou des planches de plusieurs pages. A cela s’ajoute la possibilité de créer des zones cliquables à certains endroits de la page, afin que les utilisateurs puissent ouvrir une nouvelle page de votre site Web d’un simple clic. Vous pouvez gérer le texte de survol qui s’affiche à l’aide des paramètres du panneau d’informations dans l’écran Catalogue électronique. Vous disposez également de plus de 100 options de configuration différentes pour configurer la visionneuse de catalogue électronique à votre convenance. Vous pouvez ainsi adapter les fonctionnalités et l’aspect de votre visionneuse en fonction de votre clientèle.

>[!NOTE]
>
>Si vous êtes un utilisateur en mode Dynamic Media - Scene7 et que vous souhaitez utiliser des catalogues électroniques, vous devez modifier la valeur `pdfbrochure` dans CRXDE Lite. Pour ce faire, dans Adobe Experience Manager, cliquez sur **[!UICONTROL Outils]** > **[!UICONTROL Général]** > **[!UICONTROL CRXDE Lite]**. Dans l’arborescence de navigation du panneau de gauche, accédez à `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>Dans le volet inférieur droit, dans l’onglet **[!UICONTROL Propriétés]**, sélectionnez la ligne `jobParam`. Définissez la valeur de `pdfbrochure` de `false` sur `true`. Comme dans `pdfbrochure=true`
>
>Dans le coin supérieur gauche de la page du CRXDE Lite, cliquez sur **[!UICONTROL Enregistrer tout]**.
>
>Vous pouvez désormais créer des catalogues électroniques dans Dynamic Media Classic.

Cette section de démarrage rapide est conçue pour vous aider à maîtriser rapidement les opérations liées aux catalogues électroniques. Suivez les étapes 1 à 7. Chaque étape se termine par un renvoi à une rubrique contenant de plus amples informations.

## 1. Téléchargement des fichiers PDF

En règle générale, un catalogue électronique est créé à partir de fichiers Adobe PDF. Les fichiers PDF étant destinés à l’impression, ils contiennent le plus souvent des images CMJN. Dynamic Media Classic détecte ces images et les convertit à l’aide d’un profil colorimétrique CMJN standard. Cependant, vous devez charger et utiliser un profil colorimétrique personnalisé.

Dans la barre de navigation globale, cliquez sur **[!UICONTROL Télécharger]** pour commencer à charger des fichiers PDF ou des images pour votre catalogue électronique. Vous pouvez télécharger des fichiers depuis votre bureau ou via FTP, cette dernière méthode étant recommandée si les fichiers sont nombreux ou de taille supérieure à 100 Mo.

La section Options PDF de l’écran de téléchargement contient des options qui permettent de télécharger des fichiers PDF présentant l’espace colorimétrique adéquat et la résolution voulue. Une résolution de 150 pixels par pouce est recommandée. L’option Générer automatiquement un catalogue permet de créer un catalogue lors du téléchargement d’un fichier PDF.

Voir [Téléchargement des fichiers PDF](uploading-pdf-files.md#uploading_the_pdf_files).

## 2. Création d’un catalogue électronique

Créez votre catalogue électronique en sélectionnant des fichiers PDF ou image dans le panneau de navigation. Cliquez sur **[!UICONTROL Créer]**, puis sélectionnez **[!UICONTROL Catalogues électroniques]**.

Sur la page Catalogue électronique, dans l’onglet **[!UICONTROL Classer les pages]**, sélectionnez une option Disposition : **[!UICONTROL 1 Up]**, **[!UICONTROL 2 Up]** ou **[!UICONTROL Custom]**. Vous pouvez réorganiser les pages ou les planches en les faisant glisser ou, dans le cas de catalogues électroniques volumineux, en choisissant un nom de page dans le menu Déplacer vers.

Pour ajouter des pages, sélectionnez un dossier dans la bibliothèque de fichiers, puis faites glisser les fichiers PDF ou d’images dans l’écran Ordre des pages. Au lieu des numéros de page par défaut, vous pouvez indiquer des noms de page personnalisés ou importer de nombreux noms de page.

Cliquez sur **[!UICONTROL Enregistrer]**, saisissez un nom pour votre catalogue électronique, choisissez un dossier Dynamic Media Classic pour le stocker, puis cliquez sur **[!UICONTROL Enregistrer]**. Chaque fois que vous modifiez l’ordre des pages ou l’ordre de votre catalogue électronique, enregistrez vos modifications en cliquant sur **[!UICONTROL Enregistrer]**.

Voir [Création d’un catalogue électronique](creating-ecatalog.md).

## 3. Création de zones cliquables

Les zones cliquables ajoutent un autre aspect aux pages de catalogue électronique. Une zone cliquable correspond à une zone de la page permettant d’afficher d’autres informations sur un article. Lorsque les utilisateurs placent le pointeur sur une zone cliquable, une description de l’article en question s’affiche. La sélection d’une zone cliquable a pour effet d’activer une référence externe qui permet d’ouvrir une nouvelle page Web contenant des informations supplémentaires sur un article.

Pour créer une zone cliquable, ouvrez l’écran Catalogue électronique. Ensuite, accédez à l’onglet **[!UICONTROL Pages de mappage]** de l’écran Catalogue électronique, puis encadrez la carte à l’aide de l’outil de zone cliquable Rectangle ou de l’outil de zone cliquable polygone. Vous pouvez ajuster la position et la taille d’une zone cliquable en faisant glisser ses bordures à l’aide de l’outil Panoramique.

Après avoir encadré la zone cliquable, saisissez l’adresse URL à laquelle vous souhaitez accéder lorsque vous cliquez sur la zone cliquable. Vous pouvez également indiquer le texte de survol qui s’affiche lorsque le pointeur se trouve sur la zone cliquable.

Voir [Création de zones cliquables dans un catalogue électronique](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

Voir [Utilisation des zones cliquables pour intégrer des médias enrichis dans un catalogue électronique](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

Vous pouvez configurer et gérer le texte de zone cliquable à l’aide des paramètres du panneau d’informations de l’écran Catalogue électronique.

Voir [Gestion du contenu du panneau d’informations](info-panel-content.md#managing-info-panel-content).

## 4. Configuration des paramètres prédéfinis de la visionneuse de catalogue électronique

Les utilisateurs finaux consultent votre catalogue dans la visionneuse de catalogue électronique. Si vous êtes un administrateur, vous avez la possibilité de configurer cette visionneuse. Vous pouvez modifier la couleur de son contour et sélectionner un nouvel habillage pour définir la marque de votre catalogue électronique. Dynamic Media Classic est fourni avec plusieurs paramètres prédéfinis de visionneuse de catalogue électronique &quot;recommandés&quot;. Vous pouvez choisir l’un de ces paramètres prédéfinis pour l’affichage de vos catalogues électroniques. Vous pouvez également créer vous-même un paramètre prédéfini pour la visionneuse de catalogue électronique si vous êtes administrateur.

Pour créer un paramètre prédéfini de visionneuse de catalogue électronique, dans la barre de navigation globale, cliquez sur **[!UICONTROL Configuration]** et sélectionnez **[!UICONTROL Paramètres prédéfinis de la visionneuse]**. Cliquez ensuite sur **[!UICONTROL Ajouter]**, choisissez une plateforme, puis cliquez sur **[!UICONTROL Catalogue électronique > Visionneuse]**.

(Voir [Configuration des paramètres prédéfinis de la visionneuse de catalogue électronique](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).)

## 5. Aperçu des catalogues électroniques dans la visionneuse de catalogue électronique

Les paramètres prédéfinis de visionneuse de catalogue électronique déterminent le style et le comportement de vos visionneuses de catalogue électronique.

Pour découvrir comment les paramètres prédéfinis de la visionneuse de catalogue électronique affichent votre catalogue électronique, sélectionnez votre catalogue électronique dans le panneau de navigation, puis cliquez sur **[!UICONTROL Aperçu]**. L’écran de prévisualisation s’ouvre dans la visionneuse par défaut.

Observez l’orientation des pages, la palette de couleurs, l’aspect des commandes permettant de changer de page et la manière dont les pages s’affichent lorsque vous les feuilletez.

Voir [Prévisualisation des catalogues électroniques dans la visionneuse de catalogue électronique](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

## 6. Publication d’un catalogue électronique et des fichiers PDF associés

La publication de votre catalogue électronique et du fichier PDF associé le place sur les serveurs d’images Dynamic Media afin qu’il puisse être diffusé sur votre site web et dans votre application. Dans le cadre du processus de publication, Dynamic Media Classic active la chaîne URL de votre catalogue électronique. Utilisez cette URL pour appeler le catalogue électronique à partir des serveurs d’images Dynamic Media vers votre site web ou votre application.

Après avoir marqué le catalogue électronique et le fichier PDF en vue de leur publication dans le panneau de navigation, cliquez sur le bouton Publier de la barre de navigation globale pour lancer une publication. Dans l’écran Publier, cliquez sur **[!UICONTROL Envoyer la publication]**.

Voir [Publication de catalogues électroniques et de fichiers PDF associés](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

## 7. Liaison d’un catalogue électronique à une page web

Dynamic Media Classic active la chaîne d’appel d’URL nécessaire à l’affichage de votre catalogue électronique lorsque vous le publiez sur les serveurs d’images Dynamic Media. Vous pouvez copier cette chaîne URL depuis l’écran de prévisualisation et le panneau de navigation (en mode Affichage des détails) en la sélectionnant dans le panneau. Une fois copiée, la chaîne URL peut être utilisée sur vos sites Web et dans vos applications.

Travaillez de concert avec votre équipe informatique pour décider de l’emplacement du lien vers le catalogue électronique au sein de votre page Web. Un clic sur ce lien entraîne l’ouverture de la visionneuse, permettant ainsi aux utilisateurs de parcourir votre catalogue électronique.

Voir [Liaison d’un catalogue électronique à une page Web](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
