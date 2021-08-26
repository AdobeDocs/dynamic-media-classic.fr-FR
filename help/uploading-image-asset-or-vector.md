---
title: Transfert d’un fichier d’image ou d’un fichier vectoriel
description: Découvrez comment télécharger une ressource d’image ou vectorielle.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: 2ef78fe6-1e7c-4f48-86da-137ddaa55bbf
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '1495'
ht-degree: 77%

---

# Transfert d’un fichier d’image ou d’un fichier vectoriel{#uploading-an-image-asset-or-a-vector-asset}

Avant de transférer un fichier d’image, vous devez d’abord demander une clé de secret partagé. Cette clé vous permet de récupérer un jeton de téléchargement. Vous utilisez ensuite le jeton de téléchargement pour transférer les fichiers d’image ou vectoriels.

## Demande d’une clé de secret partagé {#requesting-a-shared-secret-key}

Demandez une *clé de secret partagé* par [à l’aide du Admin Console pour créer un cas de support.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) Dans votre cas de prise en charge, demandez une clé de secret partagé.

Dans le message électronique, indiquez le nom d’entreprise que vous voulez utiliser pour transférer les fichiers d’image. Une fois que vous avez reçu la clé d’Adobe Dynamic Media Classic, enregistrez-la localement pour une utilisation ultérieure.

## Récupération du jeton de téléchargement {#retrieving-the-upload-token}

Le *jeton de téléchargement* garantit que personne d’autre que vous n’utilisera la même clé de secret partagé pour télécharger des fichiers. Il garantit le caractère légitime et la fiabilité de la source du téléchargement.

Le jeton de téléchargement est une chaîne numérique uniquement disponible pendant une durée limitée. Utilisez les URL suivantes, en substituant votre clé de secret partagé, afin que vous puissiez récupérer le jeton de chargement.

* Image
   `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`Dans cet exemple, la clé de secret partagé est  `fece4b21-87ee-47fc-9b99-2e29b78b602`

* Vecteur
   `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`Dans cet exemple, la clé de secret partagé est  `2d19f60e-890a-4e79-a1a5-9ac2875429b9`

Par défaut, le jeton de téléchargement arrive à expiration au terme d’un délai de cinq minutes (300 secondes) après sa récupération. Pour demander plus de temps, incluez `expires` dans l’URL et le temps nécessaire en secondes. Par exemple, l’URL d’image suivante permet de récupérer un jeton de téléchargement valide pendant 1 800 secondes :

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

La réponse réussie des images s’affiche comme suit :

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
        <serviceName>User Generated Content - Images</serviceName> 
        <version>1.0.0</version> 
        <operationName>get_uploadtoken</operationName> 
        <serviceStatus>SUCCESS</serviceStatus> 
        <title>Upload Token for fece4b21-87ee-47fc-9b99-2e29b78b602</title> 
        <message> 
            <uploadtoken>aa2a378a-cd25-4c80-994d-312094e0ef20_1800</uploadtoken> 
            <expiration_in_seconds>1800</expiration_in_seconds> 
        </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Enregistrez le jeton de téléchargement sur l’ordinateur pour l’utiliser avec les futures requêtes.

Vous pouvez utiliser les champs suivants dans l’URL de requête pour récupérer un jeton de téléchargement :

| Paramètre de l’URL | Obligatoire ou facultatif | Valeur |
|--- |--- |--- |
| op | Obligatoire | get_uploadtoken |
| shared_secret | Obligatoire | La clé de secret partagé de l’entreprise qui procède au téléchargement. |
| expires | Facultatif | Durée de validité (en secondes) du jeton de téléchargement. Valeur par défaut : 300 secondes. |

**Exemple d’URL d’image :**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

**Exemple d’URL de fichier vectoriel :**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000`

**Méthodes HTTP autorisées :**
`GET` et  `POST`

Vous pouvez maintenant transférer un fichier d’image.

Voir [Téléchargement d’un fichier d’image](uploading-image-asset-or-vector.md#uploading_an_image_asset).

## Téléchargement d’un fichier d’image {#uploading-an-image-asset}

Après avoir récupéré un jeton de téléchargement valide pendant une durée limitée, vous pouvez télécharger un fichier d’image. Vous téléchargez le fichier en tant que publication de formulaire ou publication en plusieurs parties tout en envoyant le reste des valeurs en tant que chaîne de requête d’URL, comme dans cet exemple :

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

Les champs `upload_token` et `company_name` sont obligatoires.

Voir [Récupération du jeton de téléchargement](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

Voir [Récupération d’une clé de secret partagé](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

Vous pouvez également envoyer d’autres valeurs facultatives comme chaînes de requête d’URL, comme dans cet exemple :

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

Le paramètre `file_limit` spécifie la limite de taille de fichier en octets. Le paramètre `file_exts` spécifie les extensions de nom de fichier admises pour le téléchargement. Ces deux valeurs sont facultatives.

Une limite globale est définie dans l’application pour la taille limite des fichiers et les extensions de nom de fichier autorisées. Si le contenu de votre requête se trouve dans les limites globales, celle-ci est satisfaite. Les limites globales sont les suivantes :

| Limite globale | Valeur |
|--- |--- |
| Taille du fichier pour tous les clients | 20 Mo |
| Formats de fichiers d’image pris en charge pour le téléchargement | BMP, GIF, JPG, PNG, PSD |

Le formulaire HTML suivant permet à un utilisateur de télécharger un fichier. L’utilisateur est invité à entrer les informations suivantes :

* Nom de l’entreprise.
* Jeton de téléchargement.
* Taille limite de fichier.
* Liste des extensions de nom de fichier.
* Permet de conserver le profil colorimétrique et le nom de fichier associés à la ressource.
* Indique s’il faut utiliser l’arrière-plan de masquage. Si vous activez l’option Masquer l’arrière-plan, définissez les méthodes Coin, Tolérance et Remplir.
Voir Masquer l’arrière-plan dans [Options d’édition d’images lors du téléchargement](image-editing-options-upload.md#image-editing-options-at-upload).
* Nom du fichier à télécharger.

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment> elements under &lt;adobefig>.</p>

 -->

Vous pouvez afficher le code source HTML associé au formulaire ci-dessus en cliquant sur [https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)

Dans Firefox, cliquez avec le bouton droit de la souris dans la fenêtre du navigateur, puis cliquez sur **[!UICONTROL Afficher la source de la page]**. Le code affiche la chaîne de requête d’URL correspondante et la méthode POST qui sont exécutées lorsque l’utilisateur clique sur **[!UICONTROL Envoyer]**.

Pour afficher la réponse XML dans Internet Explorer, cliquez sur **[!UICONTROL Affichage]** > **[!UICONTROL Source]**. Pour afficher la réponse XML dans Firefox, cliquez sur **[!UICONTROL Outils]** > **[!UICONTROL Outils de navigateur]** > **[!UICONTROL Outils de développement web]**. Firefox est recommandé pour afficher les réponses XML.

Vous trouverez ci-dessous un exemple de réponse à un téléchargement réussi :

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>upload</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Your file has been uploaded Successfully.</title> 
            <message> 
            <url>https://s7w2p1.scene7.com/is/image/ </url> 
            <path>000Company/ugc/1442564.tif</path> 
            <fullurl>https://s7w2p1.scene7.com/is/image/000Company/ugc/1442564.tif </fullurl> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

>[!NOTE]
>
>le fichier téléchargé (JPG, GIF, etc.) est converti au format PTIFF et un lien direct vers ce fichier PTIFF est envoyé dans la réponse.

Ce fichier est semblable à n’importe quelle autre ressource ImageServing ; vous pouvez lui appliquer des requêtes de traitement. Par exemple, l’URL suivante demande un fichier étiré à la largeur et à la hauteur spécifiées.

```as3
https://s7w2p1.scene7.com/is/image/S7WebUGC/ugc/9536356.tif?&wid=800&hei=100&fit=stretch
```

Envoyez le fichier à télécharger en tant que publication de formulaire ou en plusieurs parties tout en envoyant le reste des valeurs en tant que chaîne de requête d’URL. Vous pouvez utiliser les champs suivants dans la chaîne de requête d’URL pour télécharger un fichier :

| Paramètre de l’URL | Obligatoire ou facultatif | Valeur |
|--- |--- |--- |
| `op` | Obligatoire | charger |
| `upload_token` | Obligatoire | Jeton de téléchargement pour la clé de secret protégé associée à l’entreprise. |
| `company_name` | Obligatoire | Nom de l’entreprise qui réalise le téléchargement. |
| `file_limit` | Facultatif | Taille limite du fichier (en octets). |
| `file_exts` | Facultatif | Liste des extensions de fichiers d’image autorisées. |
| `preserve_colorprofile` | Facultatif | Conservation de tout profil de couleur incorporé avec conversion du fichier téléchargé au format PTIFF. Les valeurs possibles sont vrai ou faux. La valeur par défaut est faux. |
| `preserve_filename` | Facultatif | Conservation du nom du fichier téléchargé. Les valeurs possibles sont vrai ou faux. La valeur par défaut est faux. |

>[!NOTE]
>
>vous devez envoyer le fichier à télécharger en tant que champ unique dans la requête POST en plusieurs parties.

**Exemple d’URL :**

`https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company`

**Méthode HTTP autorisée :**

POST

### Obtention des métadonnées de fichier pour des images {#getting-asset-metadata-for-images}

Vous pouvez utiliser `image_info` pour récupérer les métadonnées d’un fichier que vous avez téléchargé, comme indiqué dans l’exemple suivant :

```as3
https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Voici un exemple de réponse réussie :

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>image_info</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>More information on 1442564.tif</title> 
            <message> 
            File created on Tue Sep 08 19:02:04 CDT 2009, File Size = 243494 bytes 
            <imageFormat>Tiff</imageFormat> 
            <colorSpace>Rgb</colorSpace> 
            <width>686</width> 
            <height>457</height> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Vous pouvez utiliser les champs suivants dans la chaîne de requête d’URL pour demander des informations sur un fichier :

| Paramètre de l’URL | Obligatoire ou facultatif | Valeur |
|--- |--- |--- |
| `op` | Obligatoire | image_info |
| `shared_secret` | Obligatoire | La clé de secret partagé de l’entreprise. |
| `image_name` | Obligatoire | Nom de l’image. |

**Exemple d’URL :**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Méthode HTTP autorisée :**

GET et POST

## Transfert d’un fichier vectoriel {#uploading-a-vector-asset}

Après avoir récupéré un jeton de téléchargement valide pendant une durée limitée, vous pouvez transférer un fichier vectoriel. Vous téléchargez le fichier en tant que publication de formulaire ou publication en plusieurs parties tout en envoyant le reste des valeurs en tant que chaîne de requête d’URL, comme dans cet exemple :

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

Les champs `upload_token` et `company_name` sont obligatoires.

Voir [Récupération du jeton de téléchargement](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

Voir [Récupération d’une clé de secret partagé](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

Vous pouvez également envoyer d’autres valeurs facultatives comme chaînes de requête d’URL, comme dans cet exemple :

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

Le paramètre `file_limit` spécifie la limite de taille de fichier en octets. Le paramètre `file_exts` spécifie les extensions de nom de fichier admises pour le téléchargement. Ces deux valeurs sont facultatives.

Une limite globale est définie dans l’application pour la taille limite des fichiers et les extensions de nom de fichier autorisées. Si le contenu de votre requête se trouve dans les limites globales, celle-ci est satisfaite. Les limites globales sont les suivantes :

| Limite globale | Valeur |
|--- |--- |
| Taille du fichier pour tous les clients | 20 Mo |
| Formats de fichiers vectoriels pris en charge pour le transfert | AI, EPS, PDF (uniquement si le fichier PDF est déjà ouvert et enregistré dans Adobe Illustrator CS6) |

Le formulaire HTML suivant permet à un utilisateur de télécharger un fichier. L’utilisateur est invité à entrer les informations suivantes :

* Nom de l’entreprise.
* Jeton de téléchargement.
* Taille limite de fichier.
* Liste des extensions de nom de fichier.
* Permet de conserver le profil colorimétrique et le nom de fichier associés à la ressource.
* Indique s’il faut utiliser l’arrière-plan de masquage. Si vous activez l’option Masquer l’arrière-plan, définissez les méthodes Coin, Tolérance et Remplir.
Voir Masquer l’arrière-plan dans [Options d’édition d’images lors du téléchargement](image-editing-options-upload.md#image-editing-options-at-upload).
* Nom du fichier à télécharger.

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment> elements under &lt;adobefig>.</p>

 -->

Le code HTML suivant s’affiche lorsque vous cliquez avec le bouton droit de la souris dans la fenêtre du navigateur, puis cliquez sur **[!UICONTROL Afficher la source]** pour le formulaire affiché dans l’exemple. Le code affiche la chaîne de requête d’URL correspondante et la méthode POST qui sont exécutées lorsque l’utilisateur clique sur **[!UICONTROL Envoyer]**.

```as3
<body> 
<script language="javascript"> 
function uploadImage() 
{ 
document.image_upload.action="vector?op=upload&company_name="+document.image_upload.company_name.value+"&upload_token="+document.image_upload.upload_token.value+"&file_limit="+document.image_upload.file_limit.value+"&file_exts="+document.image_upload.file_exts.value; 
return true; 
} 
</script> 
<form method="POST" enctype="multipart/form-data" name="image_upload" id="image_upload" onSubmit="return uploadImage();"> 
<table> 
<tr><td colspan="2"><strong> UGC Vector Upload Test Page: </strong></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr><td><strong> Company Name</strong></td><td><input type="text" size="40" name="company_name"></td></tr> 
<tr><td><strong> Upload Token </strong></td><td><input type="text" size="40" name="upload_token"></td></tr> 
<tr><td><strong> File Size Limit (in bytes) </strong></td><td><input type="text" size="40" name="file_limit"> bytes</td></tr> 
<tr><td><strong> File Extensions allowed </strong></td><td><input type="text" size="40" name="file_exts"></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>File to upload: : </strong></td> 
<td><input name="filename" type="file" id="filename" size="58" maxlength="1024" /></td> 
</tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>Click Submit to upload your Vector: </strong></td> 
<td><input type="submit" value="Submit"></td> 
</tr> 
</table> 
</form> 
</body>
```

Pour afficher la réponse XML dans Internet Explorer, cliquez sur **[!UICONTROL Affichage]** > **[!UICONTROL Source]**. Pour afficher la réponse XML dans Firefox, cliquez sur **[!UICONTROL Outils]** > **[!UICONTROL Outils de navigateur]** > **[!UICONTROL Source de page]**. Firefox est recommandé pour afficher les réponses XML.

Vous trouverez ci-dessous un exemple de réponse à un téléchargement réussi :

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
    <scene7> 
    <user_generated_content> 
    <response> 
    <serviceName>User Generated Content -Vector</serviceName> 
    <version>1.0.0</version> 
    <operationName>upload</operationName> 
    <serviceStatus>SUCCESS</serviceStatus> 
    <title>Your file has been uploaded Successfully.</title> 
    <message> 
    <url>https://s7w2p1.scene7.com/is/agm</url> 
    <path>W2PTest/ugc/8875744.fxg</path> 
    <fullurl> 
        https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg 
    </fullurl> 
</message> 
</response> 
</user_generated_content> 
</scene7>
```

>[!NOTE]
>
>le fichier transféré (AI, EPS, PDF, etc.) est converti au format FXG et un lien direct vers ce fichier FXG est envoyé dans la réponse.

La ressource est semblable à toute autre ressource d’impression en ligne ; vous lui appliquez des requêtes de traitement. Par exemple, l’URL suivante convertit une ressource FXG en image PNG 500 x 500.

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

Envoyez le fichier à télécharger en tant que publication de formulaire ou en plusieurs parties tout en envoyant le reste des valeurs en tant que chaîne de requête d’URL. Vous pouvez utiliser les champs suivants dans la chaîne de requête d’URL pour télécharger un fichier :

| Paramètre de l’URL | Obligatoire ou facultatif | Valeur |
|--- |--- |--- |
| `op` | Obligatoire | charger |
| `upload_token` | Obligatoire | Jeton de téléchargement pour la clé de secret protégé associée à l’entreprise. |
| `company_name` | Obligatoire | Nom de l’entreprise qui réalise le téléchargement. |
| `file_limit` | Facultatif | Taille limite du fichier (en octets). |
| `file_exts` | Facultatif | Liste des extensions de fichiers autorisées. |

>[!NOTE]
>
>vous devez envoyer le fichier à télécharger en tant que champ unique dans la requête POST en plusieurs parties.

**Exemple d’URL :**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**Méthode HTTP autorisée :**

POST
