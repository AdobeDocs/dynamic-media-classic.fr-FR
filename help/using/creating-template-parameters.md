---
title: Création de paramètres de modèle
description: Découvrez comment créer des paramètres de modèle dans Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 118806ea-c8a7-4aaf-9ae3-739c6b04ea77
topic: Development
level: Experienced
source-git-commit: 00591bdbe721035e25d3dea245a2110f978d19aa
workflow-type: tm+mt
source-wordcount: '791'
ht-degree: 45%

---

# Création de paramètres de modèle{#creating-template-parameters}

Les paramètres vous permettent d’utiliser des modèles avec une flexibilité maximale. Ils vous permettent de personnaliser dynamiquement une image de modèle. Vous pouvez déterminer les calques de texte et d’image à inclure dans le modèle et, dans chacun des calques, les paramètres à afficher. Par exemple, pour attirer l’attention sur un produit qui est en vente, vous pouvez créer un calque de texte À la vente . Ultérieurement, vous pourrez supprimer ce calque tout en conservant le reste de l’image de modèle simplement en supprimant le paramètre Promotions.

Lorsque vous créez des paramètres de modèle, vous spécifiez en fait les parties du modèle à appeler dans une chaîne URL. Une URL créée avec des paramètres expose ces éléments dans la chaîne URL. Avec les paramètres exposés, vous pouvez créer des résultats personnalisés en vous basant sur le mode de création dynamique de l’image de modèle à partir du serveur Image Server. Ainsi, vous pouvez modifier un modèle dynamiquement puisque vous pouvez appeler la totalité ou une partie de ses paramètres dans une URL.

Dans les paramètres de calque de texte, vous pouvez également transformer la chaîne de texte en champ dynamique lié aux valeurs d’une base de données. Il est très pratique de pouvoir lier un texte à une base de données, notamment dans le cadre de promotions. Vous pouvez personnaliser les images de modèle pour qu’elles affichent le nom des clients. Vous pouvez également associer un paramètre de calque de texte à une base de données de prix pour afficher le prix d’un article dans une image de modèle.

Vous pouvez vous référer à un même paramètre plusieurs fois. Pour chaque commande de la boîte de dialogue des paramètres, sélectionnez un paramètre qui correspond à la commande concernée dans la zone combinée. Par exemple, tous les paramètres de taille sont disponibles pour la commande `size=`. Vous pouvez attribuer de nouveau la référence de paramètre à n’importe quel autre paramètre déjà existant dans la zone combinée à condition de lui donner un nouveau nom. Dans ce cas, le nom doit être unique. Dans le cas contraire, une erreur indique que le paramètre existe. Lorsque vous supprimez une référence de paramètre, le paramètre est supprimé de l’URL s’il n’est référencé nulle part ailleurs. Lorsque vous modifiez la valeur par défaut d’un paramètre de texte, toutes les références à ce paramètre sont mises à jour. Vous pouvez voir la mise à jour dans le tableau de calques, dans le rendu du modèle et dans l’URL. Lorsque vous modifiez un attribut de calque en manipulant les poignées de redimensionnement ou en saisissant des valeurs dans le panneau de propriétés, la valeur du paramètre est mise à jour et toutes les références au paramètre sont mises à jour. Par exemple, si vous avez paramétré la taille de deux calques à l’aide d’un seul paramètre, les dimensions des deux calques sont mises à jour simultanément lorsque vous modifiez les dimensions d’un seul des calques. Lorsque vous prévisualisez un modèle et modifiez un paramètre, toutes les références au paramètre en question sont mises à jour.

Voir aussi la vidéo de formation [Concepts de base des modèles](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS).

## Paramétrer un calque {#parameterizing-a-layer}

Pour créer des paramètres de modèle pour chacun des calques de votre modèle, procédez comme suit :

1. Dans la liste Calques, sélectionnez le bouton Paramètres situé en regard du nom du calque pour lequel vous souhaitez créer des paramètres. L’écran Paramètres apparaît. Il répertorie le nom de chaque paramètre sur le calque, sa valeur et son type.
1. Sélectionnez l’option Activé en regard du nom de chaque paramètre à inclure dans l’image du modèle.
1. Sélectionnez **[!UICONTROL Fermer]** pour quitter l’écran Paramètres.

>[!NOTE]
>
>Vous pouvez renommer les paramètres dans l’écran Paramètres. Un paramètre renommé est plus facile à identifier dans les chaînes URL et à utiliser comme valeur de base de données. Pour renommer un paramètre, sélectionnez son option **[!UICONTROL On]**, sélectionnez son nom, puis saisissez un nouveau nom dans le champ Nom .

Pour afficher la liste des paramètres que vous avez créés pour votre modèle, cliquez sur le bouton Résumé des paramètres dans l’écran Modèle. Dans l’écran Résumé des paramètres, le nom de chaque calque est répertorié et si vous avez créé des paramètres pour un calque, les noms et valeurs des paramètres.

## Création de paramètres de texte dynamique {#creating-dynamic-text-parameters}

Pour les calques de texte, vous pouvez également faire de la chaîne de texte un champ dynamique lié à une valeur de base de données. Procédez comme suit :

1. Sur l’écran Modèle, sélectionnez le bouton Paramètres situé en regard du nom de la couche de texte pour laquelle vous souhaitez créer des paramètres de texte dynamique. La page Paramètres s’ouvre.
1. Sélectionnez l’option **[!UICONTROL On]** en regard du nom de l’attribut text (textAttr).
1. Sélectionnez l’onglet **[!UICONTROL Texte]** dans l’écran Paramètres.
1. Sélectionnez **[!UICONTROL Ajouter un paramètre]**. Un nom de paramètre par défaut s’affiche. Pour remplacer ce nom, sélectionnez-le, puis saisissez un autre nom. La chaîne de texte courante devient le nouveau nom du paramètre.
1. Sélectionnez **[!UICONTROL Fermer]** pour fermer la page Paramètres.

Pour que le nom du paramètre utilise une valeur de base de données, ajoutez la chaîne suivante dans l’URL du modèle :

```as3
?$_2(parameter name)=(database value)
```

Les noms d’un champ de base de données ou du code Java™ remplacent les noms des paramètres. Cette fonctionnalité indique, par exemple, le prix actuel d’un article ou d’un nom de client.
