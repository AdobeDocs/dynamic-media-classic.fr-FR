---
title: 'Démarrage rapide : catalogues électroniques'
description: Présentation et démarrage rapide des catalogues électroniques pour vous aider à maîtriser rapidement les techniques de catalogue électronique dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
topic: Integrations
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1470'
ht-degree: 25%

---

# Démarrage rapide : catalogues électroniques{#quick-start-ecatalogs}

Un catalogue électronique est une version numérique et web de documents imprimés, tels qu’un catalogue, une brochure, un prospectus, un manuel produit ou une circulaire publicitaire. Un catalogue électronique s’affiche dans une visionneuse de catalogue électronique sur un site Web. Cette visionneuse simule l’expérience de lecture de documents imprimés.

Consultez également les vidéos de formation suivantes :

* [Démarrage rapide 1 : catalogues électroniques](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/561_Quick%20Start%20-%20Part%201_converted%20renamed_eCatalogs-AVS)
* [Démarrage rapide 2 : catalogues électroniques](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/562_Quick%20Start%20-%20Part%202_converted%20renamed_eCatalogs-AVS)

Selon les paramètres que vous choisissez pour votre catalogue électronique, la visionneuse peut vous permettre d’effectuer les opérations suivantes :

* Recherchez un ou plusieurs mots-clés dans le catalogue. Les résultats de la recherche s’affichent sous la forme d’une liste de miniatures dans un panneau de recherche sur le côté gauche du catalogue. Chaque miniature cliquable représente une planche de catalogue où le terme de recherche en surbrillance a été trouvé.

* Partagez le catalogue par le biais des médias sociaux, téléchargez le catalogue pour l’afficher hors ligne, activez les Favoris pour marquer les éléments auxquels vous souhaitez revenir rapidement ou imprimez le catalogue.
* Parcourez le catalogue à l’aide de la table des matières ou de la vue de grille de page ; page vers l’avant ou vers l’arrière en sélectionnant le bord médian d’une page.
* effectuer un zoom avant, un zoom arrière ou un panoramique pour examiner des articles figurant sur une page ;
* Déplacez le pointeur sur une zone de la page (appelée zone cliquable) pour afficher une fenêtre pop-up contenant des informations sur un élément.
* Sélectionnez une zone géographique de page afin d&#39;ouvrir une nouvelle page Web contenant plus d&#39;informations sur un élément.
* rédiger un pense-bête et l’associer à une page du catalogue électronique ;
* Appuyez sur les icônes de zone cliquable pour lancer des pages web associées ou des panneaux d’informations contextuelles.
* utiliser les interactions de mouvement, y compris le zoom pincé et le feuilletage des pages ;
* effectuer des recherches par mot-clé.

![Le catalogue électronique tel qu’il apparaît aux utilisateurs. A) Page d’ouverture du catalogue électronique. B)Catalogue électronique tourné vers la page 2.](/help/using/assets/ec_cat_viewer_popup.png)

Pour créer un catalogue électronique, vous utilisez généralement des fichiers PDF haute résolution créés dans Adobe Acrobat ou un autre programme d’impression, mais vous pouvez également créer un catalogue électronique à partir de fichiers image.

Lorsque vous créez un catalogue électronique, vous agencez les pages ou les planches dans l’ordre de votre choix. Vous pouvez également indiquer si vous souhaitez obtenir des pages simples, des planches en double page ou des planches de plusieurs pages. Vous pouvez créer des zones cliquables pour les zones de page, de sorte que les visiteurs puissent, par exemple, sélectionner une zone de la page et ouvrir une nouvelle page de votre site Web. Vous pouvez gérer le texte de survol qui s’affiche à l’aide des paramètres du panneau d’informations dans l’écran Catalogue électronique. Vous disposez également de plus de 100 options de configuration différentes pour configurer la visionneuse de catalogue électronique à votre convenance. Vous pouvez ainsi adapter les fonctionnalités et l’aspect de votre visionneuse en fonction de votre clientèle.

>[!NOTE]
>
>Si vous êtes un utilisateur de Dynamic Media en mode Scene7 et souhaitez utiliser des catalogues électroniques, modifiez la valeur `pdfbrochure` dans CRXDE Lite. Pour ce faire, dans Adobe Experience Manager, accédez à **[!UICONTROL Outils]** > **[!UICONTROL Général]** > **[!UICONTROL CRXDE Lite]**. Dans l’arborescence de navigation du panneau de gauche, accédez à `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>Dans le volet inférieur droit, sous l’onglet **[!UICONTROL Propriétés]**, sélectionnez la ligne `jobParam`. Définissez la valeur de `pdfbrochure` de `false` à `true`. Comme dans `pdfbrochure=true`
>
>Dans le coin supérieur gauche de la page CRXDE Lite, sélectionnez **[!UICONTROL Enregistrer tout]**.
>
>Vous pouvez désormais créer des catalogues électroniques dans Adobe Dynamic Media Classic.

Cette section de démarrage rapide est conçue pour vous aider à maîtriser rapidement les opérations liées aux catalogues électroniques. Suivez les étapes 1 à 7. Après chaque étape, il existe une référence croisée à un en-tête de rubrique dans laquelle vous pouvez trouver plus d’informations.

## &#x200B;1. Chargez les fichiers PDF

En règle générale, un catalogue électronique est créé à partir de fichiers Adobe PDF. Les fichiers PDF étant destinés à l’impression, ils contiennent le plus souvent des images CMJN. Adobe Dynamic Media Classic détecte ces images et les convertit à l’aide d’un profil colorimétrique CMJN standard. Cependant, vous devez charger et utiliser un profil de couleurs personnalisé.

Sur la barre de navigation générale, sélectionnez **[!UICONTROL Télécharger]** pour commencer à télécharger des fichiers PDF ou des images pour votre catalogue électronique. Vous pouvez télécharger des fichiers depuis votre bureau ou par FTP ; le protocole FTP est recommandé si vous téléchargez de nombreux fichiers ou des fichiers de plus de 100 Mo.

La section Options PDF de l’écran de téléchargement contient des options qui permettent de télécharger des fichiers PDF présentant l’espace colorimétrique adéquat et la résolution voulue. Une résolution de 150 pixels par pouce est recommandée. Vous pouvez sélectionner l’option **[!UICONTROL Générer automatiquement un catalogue électronique]** pour créer un catalogue électronique lorsque vous chargez un fichier PDF.

Voir [Charger les fichiers PDF](uploading-pdf-files.md#uploading_the_pdf_files).

## &#x200B;2. Créer un catalogue électronique

Créez votre catalogue électronique en sélectionnant des fichiers PDF ou image dans le panneau de navigation. Sélectionnez **[!UICONTROL Créer]**, puis choisissez **[!UICONTROL Catalogues électroniques]**.

Sur la page Catalogue électronique, dans l’onglet **[!UICONTROL Pages de commande]**, sélectionnez une option de mise en page : **[!UICONTROL 1 vers le haut]**, **[!UICONTROL 2 vers le haut]** ou **[!UICONTROL Personnalisé]**. Vous pouvez réorganiser les pages ou les planches en les faisant glisser ou, dans le cas de catalogues électroniques volumineux, en choisissant un nom de page dans le menu Déplacer vers.

Pour ajouter des pages, sélectionnez un dossier dans la bibliothèque de fichiers, puis faites glisser les fichiers PDF ou d’images dans l’écran Ordre des pages. Au lieu des numéros de page par défaut, vous pouvez fournir des noms de page personnalisés ou importer de nombreux noms de page.

Sélectionnez **[!UICONTROL Enregistrer]**, saisissez un nom pour votre catalogue électronique, choisissez un dossier Adobe Dynamic Media Classic pour le stocker, puis sélectionnez **[!UICONTROL Enregistrer]**. Chaque fois que vous modifiez l’ordre des pages ou votre catalogue électronique, enregistrez vos modifications en sélectionnant **[!UICONTROL Enregistrer]**.

Voir [Création d’un catalogue électronique](creating-ecatalog.md).

## &#x200B;3. Création de zones cliquables

Les zones cliquables ajoutent un autre aspect aux pages de catalogue électronique. Une zone cliquable correspond à une zone de la page permettant d’afficher d’autres informations sur un article. Lorsque les utilisateurs placent le pointeur sur une zone cliquable, une description de l’article en question s’affiche. Cliquer sur une zone cliquable active une référence externe qui ouvre une nouvelle page web dans laquelle vous pouvez en savoir plus sur un élément.

Pour créer une zone cliquable, ouvrez l’écran Catalogue électronique. Accédez ensuite à l’onglet **[!UICONTROL Pages de carte]** de l’écran Catalogue électronique et encadrez la carte à l’aide de l’outil de zone cliquable Rectangle ou de l’outil de zone cliquable Polygone. Vous pouvez ajuster la position et la taille des zones cliquables en faisant glisser les bordures des zones cliquables à l’aide de l’outil Panoramique.

Après avoir encadré la zone cliquable, saisissez l’adresse URL à laquelle accéder lorsque vous sélectionnez la zone cliquable. Vous pouvez également indiquer le texte de survol qui s’affiche lorsque le pointeur se trouve sur la zone cliquable.

Voir [Création de zones cliquables de catalogue électronique](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

Voir [&#x200B; Utilisation de zones cliquables pour incorporer des médias riches dans un catalogue électronique](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

Vous pouvez configurer et gérer le texte de la zone cliquable à l’aide des paramètres du panneau Informations dans l’écran Catalogue électronique.

Voir [Gérer le contenu du panneau Informations dans les catalogues électroniques](/help/using/info-panel-content-ecatalog.md).

## &#x200B;4. Configurer les paramètres prédéfinis de la visionneuse de catalogue électronique

Les utilisateurs finaux consultent votre catalogue dans la visionneuse de catalogue électronique. Si vous êtes un administrateur, vous avez la possibilité de configurer cette visionneuse. Vous pouvez modifier sa couleur de contour et sélectionner une nouvelle « apparence » pour marquer votre catalogue électronique. Adobe Dynamic Media Classic s’accompagne de plusieurs paramètres prédéfinis de visionneuse de catalogue électronique correspondant aux bonnes pratiques. Vous pouvez choisir l’un de ces paramètres prédéfinis pour afficher vos catalogues électroniques. Vous pouvez également créer vous-même un paramètre prédéfini pour la visionneuse de catalogue électronique si vous êtes administrateur.

Pour créer un paramètre prédéfini de la visionneuse de catalogue électronique, sur la barre de navigation générale, sélectionnez **[!UICONTROL Configuration]**, puis choisissez **[!UICONTROL Paramètres prédéfinis de la visionneuse]**. Sélectionnez **[!UICONTROL Ajouter]**, choisissez une plateforme, puis sélectionnez **[!UICONTROL Catalogue électronique]** > **[!UICONTROL Visionneuse]**.

Voir [Configuration des paramètres prédéfinis de la visionneuse de catalogue électronique](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

## &#x200B;5. Aperçu des catalogues électroniques dans la visionneuse de catalogues électroniques

Les paramètres prédéfinis de visionneuse de catalogue électronique déterminent le style et le comportement de vos visionneuses de catalogue électronique.

Pour découvrir comment les paramètres prédéfinis de la visionneuse de catalogue électronique affichent votre catalogue électronique, sélectionnez votre catalogue électronique dans le panneau de navigation, puis sélectionnez **[!UICONTROL Aperçu]**. L’écran de prévisualisation s’ouvre dans la visionneuse par défaut.

Observez l’orientation des pages, la palette de couleurs, l’aspect des commandes permettant de changer de page et la manière dont les pages s’affichent lorsque vous les feuilletez.

Voir [Aperçu des catalogues électroniques dans la visionneuse de catalogue électronique](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

## &#x200B;6. Publier le catalogue électronique et les fichiers PDF associés

La publication de votre catalogue électronique et des PDF associées le place sur les serveurs d’images Dynamic Media afin qu’il puisse être diffusé sur votre site Web et votre application. Dans le cadre du processus de publication, Adobe Dynamic Media Classic active la chaîne d’URL de votre catalogue électronique. Utilisez cette URL pour appeler le catalogue électronique depuis les serveurs d’images Dynamic Media vers votre site web ou votre application.

Après avoir marqué votre catalogue électronique et votre PDF pour publication dans le panneau de navigation, sélectionnez le bouton Publier sur la barre de navigation générale pour lancer une publication. Sur la page Publication, sélectionnez **[!UICONTROL Envoyer la publication]**.

Voir [&#x200B; Publication de catalogues électroniques et de fichiers PDF associés](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

## &#x200B;7. Lier un catalogue électronique à une page Web

Adobe Dynamic Media Classic active la chaîne de légende d’URL nécessaire pour afficher votre catalogue électronique lorsque vous le publiez sur les serveurs d’images Dynamic Media. Vous pouvez copier cette chaîne d’URL à partir de l’écran de prévisualisation et du panneau de navigation (dans la vue détaillée) en sélectionnant les URL dans le panneau. Une fois la chaîne d’URL copiée, elle est disponible pour vos sites web et applications.

Contactez votre équipe informatique pour placer le lien vers le catalogue électronique à l’emplacement approprié dans votre page web. Lorsque les utilisateurs sélectionnent le lien, la visionneuse de catalogue électronique s’affiche et les utilisateurs peuvent parcourir votre catalogue électronique.

Voir [Liaison d’un catalogue électronique à une page web](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
