---
title: Intégration d’Adobe Dynamic Media Classic à Adobe Target Standard/Premium
description: Découvrez comment intégrer Adobe Dynamic Media Classic à Adobe Target Standard/Premium.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: c6f217fb-89cb-4c8d-aa7f-309fc42f7d46
topic: Integrations, Development
level: Experienced
source-git-commit: 914fde11270dc731a261da3305b29dd573584d93
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---

# Intégration d’Adobe Dynamic Media Classic à Adobe Target Standard/Premium {#integrating-dmc-with-target}

Avant d’intégrer [!DNL Adobe Dynamic Media Classic] avec [!DNL Target Standard/Premium], vous devez saisir votre URL cible dans la variable [!DNL Adobe Dynamic Media Classic] Écran Paramètres généraux de l’application. Pour obtenir votre URL Target et la saisir dans la page Paramètres généraux de l’application, procédez comme suit :

1. Dans [!DNL Adobe Experience Cloud], connectez-vous à [!DNL Target Standard/Premium] compte .
1. Une fois connecté, copiez l’URL dans la barre d’adresse de votre navigateur, y compris `.com`.

   Par exemple, si la variable *fiction* URL (les chemins d’accès aux URL contiennent toujours des barres obliques, et non des barres obliques inversées comme dans cet exemple) dans la barre d’adresse est : `https:\\www.myfictionalsite.com/categories/admin/home.do`, ne copiez que cette partie de la variable *fiction* URL : `https:\\www.myfictionalsite.com`.

1. Dans [!DNL Adobe Dynamic Media Classic], accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Configuration de l’application]**.
1. Sur la page Paramètres généraux de l’application, dans le **[!UICONTROL Nom du serveur Test&amp;Target]** collez l’URL que vous avez copiée à l’étape 2.
1. Sélectionner **[!UICONTROL Fermer]**.
