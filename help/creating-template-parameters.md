---
title: Création de paramètres de modèle
seo-title: Création de paramètres de modèle
description: 'null'
seo-description: Découvrez comment créer des paramètres de modèle.
uuid: d17168a8-4776-4761-b022-8258d5997604
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: d263f041-5a0d-4c4f-9266-aeff51a5a7e2
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '791'
ht-degree: 98%

---


# Création de paramètres de modèle{#creating-template-parameters}

Les paramètres permettent d’utiliser les modèles avec une extrême souplesse. Ils offrent la possibilité de personnaliser dynamiquement une image de modèle. Vous pouvez déterminer les calques de texte et d’image à inclure dans le modèle et, dans chacun des calques, les paramètres à afficher. Par exemple, pour mettre en lumière un produit soldé, vous pouvez créer un calque de texte Promotions. Ultérieurement, vous pourrez supprimer ce calque tout en conservant le reste de l’image de modèle simplement en supprimant le paramètre Promotions.

Lorsque vous créez des paramètres de modèle, vous spécifiez en fait les parties du modèle à appeler dans une chaîne URL. Une URL créée avec des paramètres expose ces éléments dans la chaîne URL. Avec les paramètres exposés, vous pouvez créer des résultats personnalisés en vous basant sur le mode de création dynamique de l’image de modèle à partir du serveur Image Server. Ainsi, vous pouvez modifier un modèle dynamiquement puisque vous pouvez appeler la totalité ou une partie de ses paramètres dans une URL.

Dans les paramètres de calque de texte, vous pouvez également transformer la chaîne de texte en champ dynamique lié aux valeurs d’une base de données. Il est très pratique de pouvoir lier un texte à une base de données, notamment dans le cadre de promotions. Vous pouvez personnaliser les images de modèle pour qu’elles affichent le nom des clients. A titre d’exemple, vous pouvez également lier un paramètre de calque de texte à une base de données de prix afin d’afficher le prix d’un article dans une image de modèle.

Vous pouvez vous référer à un même paramètre plusieurs fois. Pour chaque commande de la boîte de dialogue des paramètres, sélectionnez un paramètre qui correspond à la commande concernée dans la zone combinée. Par exemple, tous les paramètres de taille sont disponibles pour la commande size=, etc. Vous pouvez attribuer de nouveau la référence de paramètre à n’importe quel autre paramètre déjà existant dans la zone combinée à condition de lui donner un nouveau nom. Dans ce cas, le nom doit être unique. A défaut de nom unique, un message d’erreur indiquant que le paramètre existe déjà apparaît. Lorsque vous supprimez une référence de paramètre, le paramètre est supprimé de l’URL s’il n’est associé à aucune autre référence. Lorsque vous modifiez la valeur par défaut d’un paramètre de texte, toutes les références renvoyant à ce paramètre sont mises à jour. Vous pouvez voir la mise à jour dans le tableau de calques, dans le rendu du modèle et dans l’URL. Lorsque vous modifiez un attribut de calque en manipulant les poignées de redimensionnement ou en saisissant de nouvelles valeurs dans le panneau des propriétés, la valeur du paramètre ainsi que toutes les références au paramètre en question sont mises à jour. Par exemple, si vous avez paramétré la taille de deux calques à l’aide d’un seul paramètre, les dimensions des deux calques sont mises à jour simultanément lorsque vous modifiez les dimensions d’un seul des calques. Lorsque vous prévisualisez un modèle et modifiez un paramètre, toutes les références au paramètre en question sont mises à jour.

## Paramétrage d’un calque  {#parameterizing-a-layer}

Pour créer des paramètres de modèle pour chacun des calques de votre modèle, procédez comme suit :

1. Dans la liste Calques, sélectionnez le bouton Paramètres  situé en regard du nom du calque pour lequel vous souhaitez créer des paramètres. L’écran Paramètres apparaît. Il affiche la liste des noms de tous les paramètres du calque, leur valeur et leur type.
1. Sélectionnez l’option Oui située en regard du nom de chaque paramètre à inclure dans l’image de modèle.
1. Sélectionnez **Fermer** pour quitter l’écran Paramètres.

>[!NOTE]
>
>Vous pouvez renommer les paramètres dans l’écran Paramètres. Un paramètre renommé est plus facile à identifier dans les chaînes URL et à utiliser comme valeur de base de données. Pour renommer un paramètre, sélectionnez l’option Oui correspondante, cliquez sur son nom, puis entrez un nouveau nom dans le champ Nom.

Pour obtenir la liste des paramètres que vous avez créés pour votre modèle, sélectionnez le bouton Résumé des paramètres dans l’écran Modèle. L’écran Résumé des paramètres apparaît. Il répertorie le nom de tous les calques et, si vous avez créé des paramètres pour un calque, le nom et la valeur de ces paramètres.

## Création de paramètres de texte dynamique  {#creating-dynamic-text-parameters}

Pour les calques de texte, vous pouvez en outre transformer la chaîne de texte en champ dynamique lié à une valeur d’une base de données. Procédez comme suit :

1. Dans l’écran Modèle, sélectionnez le bouton Paramètres  situé en regard du nom du calque de texte pour lequel vous souhaitez créer des paramètres de texte dynamiques. L’écran Paramètres apparaît.
1. Sélectionnez l’option Oui située en regard du nom de l’attribut de texte (textAttr).
1. Sélectionnez l’onglet Texte dans l’écran Paramètres.
1. Cliquez sur le bouton Ajouter paramètre. Un nom de paramètre par défaut s’affiche. Pour remplacer ce nom, sélectionnez-le, puis saisissez un autre nom. La chaîne de texte courante devient le nouveau nom du paramètre.
1. Sélectionnez le bouton Fermer pour quitter l’écran Paramètres.

Pour que le nom du paramètre utilise une valeur de base de données, ajoutez la chaîne suivante dans l’URL du modèle :

```as3
?$_2(parameter name)=(database value)
```

Le nom du paramètre sera remplacé par des noms dans un champ de base de données ou un code Java indiquant, par exemple, le prix actuel d’un article ou le nom d’un client.
