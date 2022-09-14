---
title: Chargement d’une ressource d’image pixellisée
description: Découvrez comment télécharger une ressource d’image pixellisée dans Adobe Dynamic Media Classic
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: 2ef78fe6-1e7c-4f48-86da-137ddaa55bbf
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 67%

---

# Chargement d’une ressource d’image pixellisée {#uploading-an-image-asset-or-a-vector-asset}

Avant de transférer un fichier d’image, vous devez d’abord demander une clé de secret partagé. Cette clé vous permet de récupérer un jeton de téléchargement. Vous pouvez ensuite utiliser le jeton de chargement pour charger des ressources d’image pixellisée.

>[!IMPORTANT]
>
>La prise en charge de ressources vectorielles UGC nouvelles ou existantes dans Adobe Dynamic Media Classic s’est terminée le 30 septembre 2021.

## Demande d’une clé de secret partagé {#requesting-a-shared-secret-key}

Demander une *clé secrète partagée* par [utilisation du Admin Console pour créer un cas d’assistance.](https://helpx.adobe.com/enterprise/using/support-for-experience-cloud.html) Dans votre cas de prise en charge, demandez une clé de secret partagé.

Dans le message électronique, indiquez le nom d’entreprise que vous voulez utiliser pour transférer les fichiers d’image. Une fois que vous avez reçu la clé d’Adobe Dynamic Media Classic, enregistrez-la localement pour une utilisation ultérieure.

## Récupération du jeton de chargement {#retrieving-the-upload-token}

Le *jeton de téléchargement* garantit que personne d’autre que vous n’utilisera la même clé de secret partagé pour télécharger des fichiers. Il garantit le caractère légitime et la fiabilité de la source du téléchargement.

Le jeton de téléchargement est une chaîne numérique uniquement disponible pendant une durée limitée. Utilisez les URL suivantes, en substituant votre clé de secret partagé, afin que vous puissiez récupérer le jeton de chargement.

* Image pixellisée
   `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`Dans cet exemple, la clé de secret partagé est `fece4b21-87ee-47fc-9b99-2e29b78b602`

<!-- * Vector
  `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`In this example, the shared-secret key is `2d19f60e-890a-4e79-a1a5-9ac2875429b9` -->

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
| --- | --- | --- |
| op | Obligatoire | get_uploadtoken |
| shared_secret | Obligatoire | La clé de secret partagé de l’entreprise qui procède au téléchargement. |
| expires | Facultatif | Durée de validité (en secondes) du jeton de téléchargement. Valeur par défaut : 300 secondes. |

**Exemple d’URL d’image pixellisée :**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000` -->

**Méthodes HTTP autorisées :**
`GET` et `POST`

Vous pouvez maintenant transférer un fichier d’image.

Voir [Chargement d’une ressource image](uploading-image-asset-or-vector.md#uploading_an_image_asset).

## Chargement d’une ressource d’image pixellisée {#uploading-an-image-asset}

Après avoir récupéré un jeton de téléchargement valide pendant une durée limitée, vous pouvez télécharger un fichier d’image. Vous téléchargez le fichier en tant que publication de formulaire ou publication en plusieurs parties tout en envoyant le reste des valeurs en tant que chaîne de requête d’URL, comme dans cet exemple :

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

Le `upload_token` et `company_name` sont obligatoires.

Voir [Récupération du jeton de chargement](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

Voir [Récupération d’une clé secrète partagée](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

Vous pouvez également envoyer d’autres valeurs facultatives comme chaînes de requête d’URL, comme dans cet exemple :

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

Le `file_limit` spécifie la limite de taille de fichier en octets. Le paramètre `file_exts` spécifie les extensions de nom de fichier admises pour le téléchargement. Ces deux valeurs sont facultatives.

Une limite globale est définie dans l’application pour la taille limite des fichiers et les extensions de nom de fichier autorisées. Si le contenu de votre requête se trouve dans les limites globales, celle-ci est satisfaite. Les limites globales sont les suivantes :

| Limite globale | Valeur |
| --- | --- |
| Taille du fichier pour tous les clients | 20 Mo |
| Formats de fichiers d’image pris en charge pour le téléchargement | BMP, GIF, JPG, PNG, PSD, TIFF |

Le formulaire HTML suivant permet à un utilisateur de télécharger un fichier. L’utilisateur est invité à entrer les informations suivantes :

* Nom de l’entreprise.
* Jeton de téléchargement.
* Taille limite de fichier.
* Liste des extensions de nom de fichier.
* Permet de conserver le profil colorimétrique et le nom de fichier associés à la ressource.
* Indique s’il faut utiliser l’arrière-plan de masquage. Si vous activez l’option Masquer l’arrière-plan, définissez les méthodes Coin, Tolérance et Remplir.
Voir Masquage de l’arrière-plan dans [Options d’optimisation des images lors du téléchargement](image-editing-options-upload.md#image-editing-options-at-upload).
* Nom du fichier à télécharger.

Vous pouvez afficher le code source du HTML associé au formulaire ci-dessus en sélectionnant [https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)

Dans Firefox, cliquez avec le bouton droit dans la fenêtre du navigateur, puis sélectionnez **[!UICONTROL Afficher la source de page]**. Le code affiche la chaîne de requête d’URL correspondante et la méthode POST qui sont exécutées lorsque l’utilisateur clique sur **[!UICONTROL Envoyer]**.

Pour afficher la réponse XML dans Internet Explorer, accédez à **[!UICONTROL Affichage]** > **[!UICONTROL Source]**. Pour afficher la réponse XML dans Firefox, accédez à **[!UICONTROL Outils]** > **[!UICONTROL Outils de navigateur]** > **[!UICONTROL Outils de développement web]**. Firefox est recommandé pour afficher les réponses XML.

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
| --- | --- | --- |
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

### Obtention des métadonnées de ressource pour les images {#getting-asset-metadata-for-images}

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
| --- | --- | --- |
| `op` | Obligatoire | image_info |
| `shared_secret` | Obligatoire | La clé de secret partagé de l’entreprise. |
| `image_name` | Obligatoire | Nom de l’image. |

**Exemple d’URL :**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Méthode HTTP autorisée :**

GET et POST

<!-- ## Upload a vector asset {#uploading-a-vector-asset}

>[!IMPORTANT]
>
>Support for new or existing UGC vector image assets in Adobe Dynamic Media Classic end on September 30, 2021.

After you retrieve an upload token that is valid for a specific amount of time, you can upload a vector asset. You upload the asset as a multipart/form post while sending the rest of the values as a URL query string, as shown in this example:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

The `upload_token` and `company_name` fields are required.

See [Retrieve the upload token](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

See [Retrieve a shared-secret key](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

You can also send other optional values as URL query strings, as in this example:

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

The `file_limit` parameter specifies the file-size limit in bytes. The `file_exts` parameter specifies the filename extensions that are allowed for upload. Both of these values are optional.

A global limit is set in the application for the file size limit and the filename extensions allowed. If what you send in the request is a subset of the global limits, it is honored. The global limits are the following:

| Global limit | Value |
| --- | --- |
| File size for all clients | 20 MB |
| Supported vector file formats for upload | AI, EPS, PDF (only when the PDF is previously opened and saved in Adobe Illustrator CS6) |

The following HTML form lets a user upload an asset. The form asks the user to enter the following information:

* A company name.
* An upload token.
* A file size limit.
* A list of filename extensions.
* Whether to preserve the color profile and file name associated with the asset.
* Whether to use Knockout Background. If you enable Knockout Background, set the Corner, Tolerance, and Fill Method.
See Knockout Background in [Image fine-tuning options at upload](image-editing-options-upload.md#image-editing-options-at-upload).
* The name of the file to upload.

The following HTML code is displayed when you right-click in the browser window, and then select **[!UICONTROL View Source]** for the form shown in the example. The code shows the corresponding URL query string and the POST method that are run when the user selects **[!UICONTROL Submit]**.

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
<td><strong>Select Submit to upload your Vector: </strong></td> 
<td><input type="submit" value="Submit"></td> 
</tr> 
</table> 
</form> 
</body>
```

To view the XML response in Internet Explorer, go to **[!UICONTROL View]** > **[!UICONTROL Source]**. To view XML response in Firefox, go to **[!UICONTROL Tools]** > **[!UICONTROL Browser Tools]** > **[!UICONTROL Page Source]**. Firefox is recommended for viewing XML responses.

The following is a sample response from a successful upload:

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
>The uploaded asset (AI, EPS, PDF so on) is converted to the FXG format and the response sends a direct link to that FXG asset.

The asset is like any other Web-to-print resource; you apply processing queries to it. For example, the following URL converts an FXG resource into a 500x500 png image.

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

Send the asset to upload as a multipart/form post while sending the rest of the values as a URL query string. You can use the following fields in the URL query string to upload an asset:

| URL Parameter | Required or Optional | Value |
| --- | --- | --- |
| `op` | Required | upload |
| `upload_token` | Required | Upload token for the shared-secret key associated with the company. |
| `company_name` | Required | Name of the company performing the upload. |
| `file_limit` | Optional | File size limit, in bytes, for the asset. |
| `file_exts` | Optional | List of allowable extensions for the asset file. |

>[!NOTE]
>
>You are required to send the asset to be uploaded as the only field in a multipart POST request.

**Sample URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**Allowed HTTP method:**

POST
 -->