---
title: '« Démarrage rapide : Publication de modèles »'
seo-title: '« Démarrage rapide : Publication de modèles »'
description: 'null'
seo-description: Une introduction et une publication rapide à modèles pour vous aider à maîtriser rapidement les opérations.
uuid: 101 b 6211-2421-4565-8635-944315 a 5 c 512
contentOwner: admin
content-type: référence
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/template-publishing
discoiquuid: 03671 fc 1-ce 3 b -4 fae-ad 1 f -53 c 99 abcabde
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Quick Start: Template publishing{#quick-start-template-publishing}

Adobe Dynamic Media Classic Web-to-Print vous permet de créer du contenu d'impression professionnel qui est facile à personnaliser pour vos clients, vos clients et votre personnel. Vous pouvez conserver le contenu et l’identité de marque de l’entreprise tout au long du processus de publication. Les utilisateurs finals peuvent personnaliser le contenu d’impression, mais uniquement la partie du contenu dont vous avez autorisé la personnalisation. Papeterie personnalisée, cartes de visite, affiches, cartes de vœux, étiquettes, tickets, cadeaux, vêtements, calendriers, scrapbooks et albums photos sont autant d’exemples de produits d’impression personnalisés que vous pouvez présenter. Les entreprises peuvent conserver une identité de marque commune avec une enseigne qui peut être adaptée à différentes régions, franchises boutiques et succursales.

Vous commencez par créer un modèle dans Adobe Illustrator. Le modèle définit avec précision les éléments permanents ou variables ; les éléments variables sont ceux qui pourront être personnalisés. Par exemple, une fois qu’une zone de texte est paramétrée dans un fichier Illustrator, les utilisateurs finals peuvent saisir le texte de leur choix. De la même façon, une couleur de fond paramétrée en tant qu’élément variable peut être modifiée.

Dynamic Media Classic propose deux flux de travaux de publication à l'aide de modèles prédéfinis, un pour les cas d'utilisation de base et un pour les cas d'utilisation avancés. Les cas d'utilisation de base consistent à créer une conception dans Adobe Illustrator, à la télécharger vers Dynamic Media Classic et à définir des éléments variables avec des paramètres dans SPS. Une utilisation avancée nécessite une définition plus détaillée de la variabilité. Les cas d'utilisation avancés consistent à créer des éléments variables dans Adobe Illustrator, transférer le fichier vers Dynamic Media Classic et manipuler directement les éléments au niveau du code XML avec des appels d'URL. Ce scénario est appelé *`*DOM manipulation*`*.

>[!NOTE]
>
>For more information about Dynamic Media Classic web-to-print workflows, template creation, parameterization, DOM manipulation, and more, see the Web-to-Print Workflow Guide here: [www.adobe.com/go/learn_s7_webtoprint_en](https://www.adobe.com/go/learn_s7_webtoprint_en) . Téléchargez le fichier ZIP sur votre disque dur local et extrayez son contenu (le document de didacticiel de flux de travaux Web Dynamic Media Classic et les ressources tutorielles).

**Démarrage rapide**

Cette section de démarrage rapide décrit le flux de travail de base en vue d’utiliser des fichiers Illustrator pour créer des produits d’impression personnalisables de haute qualité.

**Cookie. Conception d’un fichier Illustrator pour le module de publication à l’aide de modèles prédéfinis**

Dans Illustrator, créez votre modèle. Si vous souhaitez utiliser la méthode de manipulation avancée DOM pour personnaliser votre modèle, définissez des identifiants d’élément Scene7 pour les éléments variables dans Illustrator.

Voir les sections [Création d’un modèle initial dans Illustrator](create-initial-template-illustrator.md#create_the_initial_template_in_illustrator) et [Manipulation DOM](dom-manipulation.md#dom_manipulation).

**2. Convert your template to Dynamic Media Classic FXG and upload it to Scene7 Publishing System**

Les utilisateurs d’Adobe Creative Cloud peuvent utiliser le module externe d’Adobe Illustrator pour l’impression en ligne. Ce module externe convertit les modèles au format FXG Dynamic Media Classic. Si un modèle comporte des polices de caractères, les fichiers de police correspondants doivent être téléchargés vers SPS avant le téléchargement du fichier FXG.

Voir [Téléchargement de fichiers pour le module de publication à l’aide de modèles prédéfinis](upload-files-template-publishing.md#upload_files_for_template_publishing).

**Cookie. Affichage, définition ou redéfinition de paramètres dans Dynamic Media Classic**

Dans les écrans de prévisualisation et de création du module de publication à l’aide de modèles prédéfinis, vous pouvez définir et affiner des éléments variables à l’aide des fonctions de paramétrage, prévisualisation des résultats et test des résultats. Dans ces écrans, vous pouvez effectuer les actions suivantes :

* Créer et modifier des paramètres.
* Indiquer des valeurs par défaut pour les attributs et les propriétés des paramètres.
* Pour copier l’URL de prévisualisation dans le Presse-papiers et prévisualiser le résultat dans un navigateur, cliquez sur Copier l’URL.

Voir [Paramétrage d'un modèle dans Dynamic Media Classic](parameterizing-template-scene7.md#parameterizing_a_template_in_scene7).

**4. Publication du modèle FXG**

Après avoir défini et testé les paramètres et attributs, publiez le fichier. Lorsque vous publiez votre modèle FXG, il est placé sur les serveurs d'images de médias dynamiques et l'URL est activée.

Assurez-vous de publier toutes les images et polices associées à votre modèle FXG.

Voir [Publication de modèles FXG](dom-manipulation.md#publish_fxg_templates).

**5. Obtention de l’URL**

A l’aide de son URL, le modèle est maintenant prêt à être intégré à votre site Web pour que les utilisateurs finals puissent en personnaliser le contenu variable.

Voir [Liaison d’un modèle FXG à une page Web](linking-fxg-template-web-page.md#linking_an_fxg_template_to_a_web_page).
