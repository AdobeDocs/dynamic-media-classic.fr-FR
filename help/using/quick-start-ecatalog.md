---
title: "Démarrage rapide : catalogues électroniques"
description: Introduction aux catalogues électroniques et démarrage rapide pour vous aider à maîtriser rapidement les techniques de catalogue électronique dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
topic: Integrations
level: Experienced
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '1470'
ht-degree: 25%

---

# Démarrage rapide : catalogues électroniques{#quick-start-ecatalogs}

Un catalogue électronique est une version numérique Web d’un document imprimé (un catalogue, une brochure, un prospectus, un manuel de produit ou une circulaire publicitaire, par exemple). Un catalogue électronique s’affiche dans une visionneuse de catalogue électronique sur un site Web. Cette visionneuse simule l’expérience de lecture de documents imprimés.

Visionnez également les vidéos de formation suivantes :

* [Démarrage rapide 1 : catalogues électroniques](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/561_Quick%20Start%20-%20Part%201_converted%20renamed_eCatalogs-AVS)
* [Démarrage rapide 2 : catalogues électroniques](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/562_Quick%20Start%20-%20Part%202_converted%20renamed_eCatalogs-AVS)

Selon les paramètres que vous choisissez pour votre catalogue électronique, la visionneuse peut vous permettre d’effectuer les opérations suivantes :

* Recherchez un mot-clé ou des mots-clés dans le catalogue. Les résultats de la recherche s’affichent sous la forme d’une liste de miniatures dans un panneau de recherche sur le côté gauche du catalogue. Chaque miniature cliquable représente une étendue de catalogue où le terme de recherche mis en surbrillance a été trouvé.

* Partagez le catalogue par le biais des médias sociaux ; téléchargez le catalogue pour l’afficher hors ligne ; activez Favoris pour marquer les éléments auxquels vous souhaitez revenir rapidement ou imprimez le catalogue.
* Naviguez dans le catalogue à l’aide de la table des matières ou de la vue Grille de page ; en sélectionnant le bord central d’une page.
* effectuer un zoom avant, un zoom arrière ou un panoramique pour examiner des articles figurant sur une page ;
* Déplacez le pointeur au-dessus d’une zone de page (appelée zone cliquable) afin d’afficher une fenêtre contextuelle contenant des informations sur un élément.
* Sélectionnez une zone de page afin d’ouvrir une nouvelle page Web contenant plus d’informations sur un élément.
* rédiger un pense-bête et l’associer à une page du catalogue électronique ;
* Appuyez sur les icônes de zone cliquable si vous souhaitez lancer des pages Web associées ou des panneaux d’informations contextuelles.
* utiliser les interactions de mouvement, y compris le zoom pincé et le feuilletage des pages ;
* effectuer des recherches par mot-clé.

![Le catalogue électronique tel qu’il s’affiche pour les utilisateurs. A) Page d’ouverture du catalogue électronique. B) Le catalogue électronique est devenu page 2.](/help/using/assets/ec_cat_viewer_popup.png)

Pour créer un catalogue électronique, vous utilisez généralement des fichiers de PDF haute résolution créés dans Adobe Acrobat ou dans un autre programme d’impression, mais vous pouvez également créer un catalogue électronique à partir de fichiers image.

Lorsque vous créez un catalogue électronique, vous agencez les pages ou les planches dans l’ordre de votre choix. Vous pouvez également indiquer si vous souhaitez obtenir des pages simples, des planches en double page ou des planches de plusieurs pages. Vous pouvez créer des zones cliquables pour les zones de page, de sorte que les visiteurs puissent, par exemple, sélectionner une zone de la page et ouvrir une nouvelle page sur votre site Web. Vous pouvez gérer le texte de survol qui s’affiche à l’aide des paramètres du panneau d’informations dans l’écran Catalogue électronique. Vous disposez également de plus de 100 options de configuration différentes pour configurer la visionneuse de catalogue électronique à votre convenance. Vous pouvez ainsi adapter les fonctionnalités et l’aspect de votre visionneuse en fonction de votre clientèle.

>[!NOTE]
>
>Si vous êtes un utilisateur du mode Dynamic Media : Scene7 et souhaitez utiliser des catalogues électroniques, modifiez la variable `pdfbrochure` dans CRXDE Lite. Pour ce faire, dans Adobe Experience Manager, accédez à **[!UICONTROL Outils]** > **[!UICONTROL Général]** > **[!UICONTROL CRXDE Lite]**. Dans l’arborescence de navigation du panneau de gauche, accédez à `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>Dans le volet inférieur droit, dans **[!UICONTROL Propriétés]** , sélectionnez l’onglet `jobParam` ligne. Définissez la valeur de `pdfbrochure` de `false` to `true`. Comme dans `pdfbrochure=true`
>
>Dans le coin supérieur gauche de la page du CRXDE Lite, sélectionnez **[!UICONTROL Enregistrer tout]**.
>
>Vous pouvez désormais créer des catalogues électroniques dans Adobe Dynamic Media Classic.

Cette section de démarrage rapide est conçue pour vous aider à maîtriser rapidement les opérations liées aux catalogues électroniques. Suivez les étapes 1 à 7. Après chaque étape, il existe une référence croisée à un en-tête de rubrique dans lequel vous trouverez plus d’informations.

## 1. Télécharger les fichiers du PDF

En règle générale, un catalogue électronique est créé à partir de fichiers Adobe PDF. Les fichiers PDF étant destinés à l’impression, ils contiennent le plus souvent des images CMJN. Adobe Dynamic Media Classic détecte ces images et les convertit à l’aide d’un profil colorimétrique CMJN standard. Cependant, vous devez charger et utiliser un profil colorimétrique personnalisé.

Dans la barre de navigation globale, sélectionnez **[!UICONTROL Télécharger]** pour commencer à charger des fichiers ou des images de PDF pour votre catalogue électronique. Vous pouvez transférer des fichiers depuis votre bureau ou par FTP. Il est conseillé d’opter pour le FTP si vous chargez de nombreux fichiers ou fichiers de plus de 100 Mo.

La section Options PDF de l’écran de téléchargement contient des options qui permettent de télécharger des fichiers PDF présentant l’espace colorimétrique adéquat et la résolution voulue. Une résolution de 150 pixels par pouce est recommandée. Vous pouvez sélectionner l’option **[!UICONTROL Génération automatique du catalogue électronique]** pour créer un catalogue électronique lorsque vous chargez un fichier de PDF.

Voir [Chargement des fichiers du PDF](uploading-pdf-files.md#uploading_the_pdf_files).

## 2. Création d’un catalogue électronique

Créez votre catalogue électronique en sélectionnant des fichiers de PDF ou d’image dans le panneau de navigation. Sélectionner **[!UICONTROL Build]**, puis choisissez **[!UICONTROL Catalogues électroniques]**.

Sur la page Catalogue électronique, sur la page **[!UICONTROL Pages de commande]** , sélectionnez une option Disposition : **[!UICONTROL 1 haut]**, **[!UICONTROL 2 en haut]**, ou **[!UICONTROL Personnalisé]**. Vous pouvez réorganiser les pages ou les planches en les faisant glisser ou, dans le cas de catalogues électroniques volumineux, en choisissant un nom de page dans le menu Déplacer vers.

Pour ajouter des pages, sélectionnez un dossier dans la bibliothèque de fichiers, puis faites glisser les fichiers PDF ou d’images dans l’écran Ordre des pages. Au lieu des numéros de page par défaut, vous pouvez indiquer des noms de page personnalisés ou importer de nombreux noms de page.

Sélectionner **[!UICONTROL Enregistrer]**, saisissez un nom pour votre catalogue électronique, choisissez un dossier Adobe Dynamic Media Classic pour le stocker, puis sélectionnez **[!UICONTROL Enregistrer]**. Chaque fois que vous modifiez l’ordre des pages ou le catalogue électronique, enregistrez vos modifications en sélectionnant **[!UICONTROL Enregistrer]**.

Voir [Créer un catalogue électronique](creating-ecatalog.md).

## 3. Création de zones cliquables

Les zones cliquables ajoutent un autre aspect aux pages de catalogue électronique. Une zone cliquable correspond à une zone de la page permettant d’afficher d’autres informations sur un article. Lorsque les utilisateurs placent le pointeur sur une zone cliquable, une description de l’article en question s’affiche. Cliquer sur une zone cliquable active une référence externe qui ouvre une nouvelle page Web dans laquelle vous pouvez en savoir plus sur un élément.

Pour créer une zone cliquable, ouvrez l’écran Catalogue électronique. Ensuite, accédez au **[!UICONTROL Pages de mappage]** de l’écran Catalogue électronique, et encadrez la carte à l’aide de l’outil de zone cliquable Rectangle ou zone cliquable polygone. Vous pouvez ajuster la position et la taille des zones cliquables en faisant glisser les bordures des zones à l’aide de l’outil Panoramique .

Après avoir encadré la zone cliquable, saisissez l’adresse URL à laquelle vous souhaitez accéder lorsque vous sélectionnez la zone cliquable. Vous pouvez également indiquer le texte de survol qui s’affiche lorsque le pointeur se trouve sur la zone cliquable.

Voir [Création de zones cliquables de catalogue électronique](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

Voir [Utilisation de zones cliquables pour incorporer des médias riches dans un catalogue électronique](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

Vous pouvez configurer et gérer le texte de la zone cliquable à l’aide des paramètres du panneau d’informations de l’écran Catalogue électronique.

Voir [Gestion du contenu du panneau Informations dans les catalogues électroniques](/help/using/info-panel-content-ecatalog.md).

## 4. Configuration des paramètres prédéfinis de la visionneuse de catalogue électronique

Les utilisateurs finaux consultent votre catalogue dans la visionneuse de catalogue électronique. Si vous êtes un administrateur, vous avez la possibilité de configurer cette visionneuse. Vous pouvez modifier la couleur de son contour et sélectionner un nouvel &quot;habillage&quot; pour personnaliser votre catalogue électronique. Adobe Dynamic Media Classic est fourni avec plusieurs paramètres prédéfinis de visionneuse de catalogue électronique &quot;recommandés&quot;. Vous pouvez choisir l’un de ces paramètres prédéfinis pour l’affichage de vos catalogues électroniques. Vous pouvez également créer vous-même un paramètre prédéfini pour la visionneuse de catalogue électronique si vous êtes administrateur.

Pour créer un paramètre prédéfini de visionneuse de catalogue électronique, dans la barre de navigation globale, sélectionnez **[!UICONTROL Configuration]**, puis choisissez **[!UICONTROL Paramètres prédéfinis de la visionneuse]**. Sélectionner **[!UICONTROL Ajouter]**, choisissez une plateforme, puis sélectionnez **[!UICONTROL Catalogue électronique]** > **[!UICONTROL Visionneuse]**.

Voir [Configuration des paramètres prédéfinis de la visionneuse de catalogue électronique](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

## 5. Aperçu des catalogues électroniques dans la visionneuse de catalogue électronique

Les paramètres prédéfinis de visionneuse de catalogue électronique déterminent le style et le comportement de vos visionneuses de catalogue électronique.

Pour découvrir comment les paramètres prédéfinis de la visionneuse de catalogue électronique affichent votre catalogue électronique, sélectionnez votre catalogue électronique dans le panneau de navigation, puis sélectionnez **[!UICONTROL Aperçu]**. L’écran de prévisualisation s’ouvre dans la visionneuse par défaut.

Observez l’orientation des pages, la palette de couleurs, l’aspect des commandes permettant de changer de page et la manière dont les pages s’affichent lorsque vous les feuilletez.

Voir [Aperçu des catalogues électroniques dans la visionneuse de catalogue électronique](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

## 6. Publier le catalogue électronique et les PDF associés

La publication de votre catalogue électronique et du PDF associé le place sur les serveurs d’images Dynamic Media afin qu’il puisse être diffusé sur votre site Web et dans votre application. Dans le cadre du processus de publication, Adobe Dynamic Media Classic active la chaîne URL de votre catalogue électronique. Utilisez cette URL pour appeler le catalogue électronique à partir des serveurs d’images Dynamic Media vers votre site web ou votre application.

Après avoir marqué votre catalogue électronique et votre PDF pour publication dans le panneau de navigation, cliquez sur le bouton Publier de la barre de navigation globale pour lancer une publication. Sur la page Publication, sélectionnez **[!UICONTROL Envoyer la publication]**.

Voir [Publication de catalogues électroniques et de PDF associés](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

## 7. Associer un catalogue électronique à une page Web

Adobe Dynamic Media Classic active la chaîne d’légende d’URL nécessaire à l’affichage de votre catalogue électronique lorsque vous le publiez sur les serveurs d’images Dynamic Media. Vous pouvez copier cette chaîne d’URL à partir de l’écran de prévisualisation et du panneau de navigation (dans le mode Affichage des détails) en sélectionnant les URL dans le panneau. Une fois la chaîne d’URL copiée, elle est disponible sur vos sites Web et applications.

Contactez votre équipe informatique pour placer le lien vers le catalogue électronique au bon endroit dans votre page web. Lorsque les utilisateurs sélectionnent le lien, la visionneuse de catalogue électronique s’affiche et ils peuvent parcourir votre catalogue électronique.

Voir [Lier un catalogue électronique à une page Web](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
