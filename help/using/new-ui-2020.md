---
title: Application de bureau Adobe Dynamic Media Classic
description: Les utilisateurs d’Adobe Dynamic Media Classic peuvent désormais effectuer une actualisation complète de l’interface utilisateur.
contentOwner: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: d61ea80a-a98e-43e6-9e2e-4389962134f1
topic: Administration
level: Intermediate
source-git-commit: 3f71adedf54832c4e7c4c46d4103d609a2fd9634
workflow-type: tm+mt
source-wordcount: '2934'
ht-degree: 0%

---

# Application de bureau Adobe Dynamic Media Classic : désormais disponible {#new-ui-2020}

Voir [Application de bureau Adobe Dynamic Media Classic](/help/using/dynamic-media-classic-desktop-app.md) pour examiner la configuration système requise, téléchargez et installez la nouvelle application, puis connectez-vous.

## _Dernière révision 30 juin 2020_

Les utilisateurs d’Adobe Dynamic Media Classic ont désormais accès à une nouvelle connexion qui ne repose plus sur la technologie de Flash d’Adobe dans le navigateur.

## Questions fréquentes

+++**_Lorsque les navigateurs cesseront de prendre en charge le Flash des Adobes le 31 décembre 2020, cela aura-t-il un impact sur Adobe Dynamic Media Classic (anciennement Scene7) ?_**
Adobe Flash Player était un module externe de navigateur Web qui permettait aux navigateurs Web d’utiliser le contenu développé sur Adobe Flash Platform. Interface utilisateur Web d’Adobe Dynamic Media Classic (actuellement étiquetée) [!DNL Scene7 Publishing System] ou [!DNL SPS] dans le produit) nécessitait le Flash Player d’Adobe. Lorsque le Flash Adobe sera abandonné le 31 décembre 2020, les clients Adobe Dynamic Media Classic ne pourront plus se connecter à l’interface utilisateur Web. En raison de cette modification, Adobe a fourni aux clients une appli de bureau qui remplace l’expérience du navigateur.
+++

+++**_Comment accéder à la nouvelle appli de bureau ?_**
La nouvelle appli de bureau est disponible sous la forme d’une `.dmg` programme d’installation pour macOS ou en tant que `.exe` pour Windows®.

Voir [Application de bureau Adobe Dynamic Media Classic](/help/using/dynamic-media-classic-desktop-app.md) pour examiner la configuration système requise, téléchargez et installez la nouvelle application, puis connectez-vous.
+++

<!-- NEWSLETTER IS DEAD The download links are also available by way of the [Adobe Dynamic Media Classic newsletter subscription page.](https://www.adobe.com/subscription/dynamic-media-newsletter.html) -->

+++**_Comment fonctionne la nouvelle appli de bureau ?_**
Une fois que vous avez téléchargé, installé et lancé l’appli de bureau, une nouvelle connexion s’affiche. En saisissant votre nom d’utilisateur et votre mot de passe, puis en sélectionnant le serveur approprié en fonction de votre région, vous pouvez vous connecter à Adobe Dynamic Media Classic. L’expérience globale est la même que la version de navigateur Web à laquelle vous êtes habitué. Depuis l’appli de bureau, vous pouvez accéder aux environnements de production et d’évaluation Adobe Dynamic Media Classic. Vous pouvez également accéder à Media Portal si vous disposez des informations d’identification nécessaires à cette fonctionnalité.

>[!IMPORTANT]
>
>Une seule instance de l’appli de bureau peut être installée. *et* actif à la fois sur un ordinateur donné. Cependant, il n’existe aucune restriction quant au nombre d’installations que vous pouvez avoir sur plusieurs ordinateurs.

+++

+++**_Que se passe-t-il si j’utilise les API Adobe Dynamic Media Classic pour accéder au produit et que je ne me connecte pas par le biais de l’interface utilisateur web ?_**
Les API sous-jacentes d’Adobe Dynamic Media Classic ne sont pas modifiées.
+++

+++**_Cette nouvelle expérience de l’appli de bureau nécessite-t-elle des migrations ou des modifications pour les intégrations tierces ?_**
Non. Les clients Adobe Dynamic Media Classic n’ont pas à migrer ni à modifier des intégrations tierces pour utiliser la nouvelle appli de bureau.
+++

+++**_Cette modification affecte-t-elle mes scripts d’automatisation ?_**
Non. Les scripts d’automatisation n’ont aucun impact. La nouvelle appli de bureau agit et se comporte de manière similaire à l’expérience basée sur un navigateur que vous connaissez déjà.
+++

+++**_La nouvelle appli de bureau Adobe Dynamic Media Classic fonctionnera-t-elle sur les Mac et les ordinateurs personnels ?_**
Oui. La nouvelle appli de bureau est une solution multi-plateformes qui fonctionne sur Mac et PC. Linux® is *not* pris en charge.
+++

+++**_Mon entreprise a des exigences de sécurité strictes. Comment la nouvelle appli de bureau Adobe Dynamic Media Classic gère-t-elle ces exigences ?_**
Adobe s’engage à s’assurer que ses produits répondent aux exigences de sécurité de ses clients. La nouvelle appli de bureau Adobe Dynamic Media Classic continue de fournir aux clients une expérience hautement sécurisée, conforme à toutes les normes de sécurité d’Adobe.
+++

+++**_Mon entreprise ne me permet pas d&#39;installer des logiciels et des applications sur mon ordinateur. Comment me recommander l’accès à la nouvelle appli de bureau ?_**
Certaines sociétés ne vous permettent pas de télécharger et d’installer des logiciels et des applications sur votre système sans approbation. Dans ce cas, demandez à votre équipe informatique d’obtenir plus tôt l’autorisation d’accéder à la nouvelle appli de bureau Adobe Dynamic Media Classic. N’oubliez pas qu’après le 31 décembre 2020, la version du navigateur sera obsolète. Il est important d’éviter d’attendre la dernière minute pour télécharger la nouvelle appli de bureau.
+++

+++**_Plusieurs instances de la nouvelle appli de bureau peuvent-elles être ouvertes en même temps ?_**
Non. La technologie AIR sur laquelle la nouvelle application de bureau Adobe Dynamic Media Classic est créée empêche l’utilisateur d’ouvrir plusieurs instances de l’application à la fois.
+++

+++**_Existe-t-il des restrictions quant au nombre de fichiers pouvant être transférés vers Adobe Dynamic Media Classic par le biais d’un ordinateur local ?_**
Lorsque vous utilisez la nouvelle appli de bureau Adobe Dynamic Media Classic sous Windows®, vous pouvez charger un maximum de 150 fichiers à la fois à l’aide de la fonction **[!UICONTROL Télécharger]** de la boîte de dialogue Cette limitation a déjà été corrigée avant la fin de 2020. Il y a *non* restrictions de chargement sur la plateforme macOS.
+++

+++**_La nouvelle appli de bureau Adobe Dynamic Media Classic requiert-elle un nouveau SKU ? Y a-t-il un coût de licence impliqué ?_**
Non aux deux questions. Aucun SKU ou changement de licence n’est nécessaire pour utiliser la nouvelle appli de bureau Adobe Dynamic Media Classic.
+++

+++**_Comment les mises à niveau de l’appli de bureau Adobe Dynamic Media Classic sont-elles activées ?_**
Après la publication de l’appli de bureau Adobe Dynamic Media Classic le 30 juin 2020, si Adobe publie une nouvelle version, les clients doivent télécharger et installer la nouvelle version (remplacer l’application existante dans **[!UICONTROL Applications]**). Vous êtes informé de la nouvelle version par l’intermédiaire de votre équipe de compte d’Adobe et d’un mécanisme de notification de mise à niveau in-app qui avertit les utilisateurs d’une mise à niveau.
+++

+++**_Comment obtenir de l’aide pour tout problème lié à l’appli de bureau Adobe Dynamic Media Classic ?_**
Contactez l’assistance Adobe pour tout problème rencontré lors de l’utilisation de l’application.
+++

+++**_Je veux m&#39;assurer d&#39;optimiser ma stratégie de médias riches. Comment en savoir plus sur Adobe Dynamic Media Classic ?_**
Adobe Dynamic Media Classic est une solution puissante et riche en fonctionnalités, conçue pour améliorer vos stratégies multimédias riches. Pour tirer parti de toutes les fonctionnalités, veillez à explorer les ressources pratiques suivantes :

* [Tutoriel sur les bonnes pratiques d’Adobe Dynamic Media Classic](https://experienceleague.adobe.com/en/docs/experience-manager-learn/dynamic-media-classic-tutorial/overview)
* [Adobe de publications de blog](https://blog.adobe.com/)<!-- (https://blog.adobe.com/tag/dynamic-media/) -->
* [Archives de la newsletter Adobe Dynamic Media](https://experienceleague.adobe.com/en/docs/dynamic-media-classic/using/dynamic-media-newsletter)
+++

<!-- HIDDEN AUGUST 2, 2021 BECAUSE THE NEWSLETTER WAS DISCONTINUED Plus, [subscribe to the Dynamic Media newsletter](https://www.adobe.com/subscription/dynamic-media-newsletter.html) to stay current on the latest news, information, training opportunities, powerful features available to you such as [Smart Imaging](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html), and the complementary audit program. -->

+++**_Je souhaite en savoir plus sur la mise à niveau vers Adobe Dynamic Media avec Adobe Experience Manager Assets. Où puis-je trouver plus d’informations ?_**
Pour en savoir plus sur les avantages de la mise à niveau vers la nouvelle génération de la création, de la publication et de la diffusion dynamique de médias riches, consultez la page [Adobe du portail Dynamic Media pour la mise à niveau](/help/using/upgrade.md).
+++

### Ajout de plusieurs sous-titres et pistes audio à votre vidéo {#add-msma}

Avant d’ajouter plusieurs sous-titres et pistes audio à votre vidéo, assurez-vous que vous disposez déjà des éléments suivants :

* Dynamic Media est configuré dans un environnement AEM.
* A [Le profil vidéo Dynamic Media est appliqué au dossier dans lequel vos vidéos sont ingérées.].
* [Les pistes audio/multilégendes et les sous-titres générés par l’IA sont activés sur votre compte Dynamic Media.].

Les légendes ajoutées sont prises en charge avec les formats WebVTT et Adobe VTT. De plus, les fichiers de suivi audio ajoutés sont pris en charge au format MP3.

>[!IMPORTANT]
>
>Pour les vidéos chargées *before* activation de la prise en charge de plusieurs sous-titres/suivis audio ou sous-titres générés par l’IA sur votre compte Dynamic Media, [vous devez les retraiter.]. Cette étape de retraitement permet de s’assurer que ces vidéos peuvent utiliser plusieurs fonctions de sous-titres/suivi audio et de sous-titres générées par l’IA. Après le retraitement, les URL de la vidéo continuent à fonctionner et à être lues comme d’habitude.

**Pour ajouter plusieurs sous-titres et pistes audio à votre vidéo :**

1. [Chargement de la vidéo principale dans un dossier]) auquel est déjà affecté un profil vidéo. Vous n’avez pas besoin de publier la vidéo avant plus tard dans ces étapes.
1. Accédez à la ressource vidéo chargée à laquelle vous souhaitez ajouter plusieurs sous-titres et pistes audio.
1. En mode de sélection des ressources, en mode Liste ou Carte, sélectionnez la ressource vidéo.
1. Dans la barre d’outils, sélectionnez l’icône Propriétés (un cercle avec un &quot;i&quot; à l’intérieur).
1. Sur la page Propriétés de la vidéo, sélectionnez la variable **[!UICONTROL Sous-titres et suivi audio]** .

   >[!TIP]
   >Si vous ne voyez pas le **[!UICONTROL Sous-titres et suivi audio]** , cela signifie l’une des deux choses suivantes :
   >
   >* Aucun profil vidéo n’est affecté au dossier dans lequel se trouve la vidéo sélectionnée. Dans ce cas, voir [Application d’un profil vidéo au dossier]
   >* Ou, la vidéo doit être retraitée par Dynamic Media. Dans ce cas, voir [Retraiter des ressources Dynamic Media dans un dossier].
   >
   >Une fois l’une des tâches ci-dessus terminée, revenez à ces étapes.

1. Pour ajouter une ou plusieurs pistes audio à une vidéo, procédez comme suit :
   1. Sélectionner **[!UICONTROL Chargement de suivi audio]**.
   1. Accédez à un ou plusieurs fichiers .mp3 et sélectionnez-les, puis ouvrez-les.
   1. Pour que les pistes audio soient visibles dans le **[!UICONTROL Sélection de l’audio ou de la légende]** liste contextuelle sur le lecteur multimédia, vous *must* ajout des détails requis *each* fichier de suivi audio que vous avez ajouté. Sélectionnez l’icône représentant un crayon à droite du nom d’un fichier de suivi audio. Dans le **Modifier la piste audio** , saisissez les détails requis suivants :

      | Métadonnées de suivi audio | Description |
      |--- |--- |
      | Nom de fichier | Le nom de fichier par défaut est dérivé du nom de fichier d’origine. Le nom du fichier ne peut être modifié que lors du chargement et ne peut pas l’être plus tard. Les exigences en termes de caractères de nom de fichier sont les mêmes que pour AEM Assets.<br>Le même nom de fichier ne peut pas être utilisé pour d’autres fichiers de suivi audio ou de sous-titres. |
      | Langue | Sélectionnez la langue correcte de la piste audio. |
      | Type | Sélectionnez le type de piste audio que vous utilisez.<br>**Original** - La piste audio initialement jointe à la vidéo et représentée sous la forme `[Original]` dans le libellé avec `English` langue sélectionnée par défaut. while **[!UICONTROL Libellé]** et **[!UICONTROL Langue]** peut être modifié dans la variable **[!UICONTROL Modifier la piste audio]** , les valeurs d’origine sont utilisées par défaut si la vidéo principale est retraitée.<br>**Standard** - Une piste audio complémentaire pour une langue autre que l’original.<br>**Audio-description** - Une piste audio qui comprend également une narration descriptive des actions et gestes non verbaux dans la vidéo, rendant le contenu plus accessible pour les personnes malvoyantes. |
      | Etiquette | Le texte affiché comme nom de la piste audio dans la variable **[!UICONTROL Sélection de l’audio ou de la légende]** liste déroulante dans le lecteur multimédia. Le libellé correspond à ce qu’un client voit qui correspond à une piste audio. Par exemple : `English [Original]`. Le libellé audio associé à une vidéo est défini sur `[Original]` par défaut. |

      Vous pouvez modifier ou modifier ces métadonnées de suivi audio ultérieurement, si nécessaire. Lorsque la vidéo est publiée, ces détails sont reflétés dans les URL publiques des vidéos publiées.

   1. Dans le coin supérieur droit de la page, dans la **[!UICONTROL Enregistrer et fermer]** menu déroulant, cliquez sur **[!UICONTROL Enregistrer]**.
   1. Effectuez l’une des opérations suivantes :
      * Répétez cette procédure pour chaque fichier de piste audio que vous chargez.
      * Passez à l’étape suivante pour ajouter des sous-titres à une vidéo.

1. Pour ajouter un ou plusieurs fichiers de sous-titres à une vidéo, sélectionnez l’un des cas d’utilisation suivants qui correspond le mieux à votre scénario :

   |  | Cas pratique |
   | --- | --- |
   | **Option 1** | J&#39;ai mes propres fichiers de sous-titres préexistants dans les langues que je veux utiliser.<br>Voir **Option 1** à l’étape 8 ci-dessous. |
   | **Option 2** | Je veux que l’IA génère mes fichiers de sous-titres en plusieurs langues.<br>Voir **Option 2** à l’étape 8 ci-dessous. |
   | **Option 3** | Le texte d’un fichier de légende (.vtt) doit être corrigé, rechargé pour remplacer l’ancien fichier .vtt, puis le fichier corrigé doit être traduit par AI.<br>Voir **Option 3** à l’étape 8 ci-dessous. |

+++**Option 1 :** *J&#39;ai mes propres fichiers de sous-titres préexistants dans les langues que je veux utiliser.*

   1. Dans le coin supérieur droit de la page, cliquez sur **[!UICONTROL Créer une légende]** > **[!UICONTROL Chargement de fichiers]**.
   1. Accédez à un ou plusieurs de vos fichiers .vtt (Video Text Tracks) préexistants, sélectionnez-les, puis ouvrez-les.
   1. Pour que les sous-titres soient visibles sur le lecteur multimédia, vous *must* ajoutez les détails requis sur *each* fichier de sous-titres que vous chargez. Sélectionnez l’icône représentant un crayon à droite du nom d’un fichier de légende. Dans le **Modifier la légende** , saisissez les informations requises suivantes sur le fichier :

      | Métadonnées de légende | Description |
      |--- |--- |
      | Nom de fichier | Le nom de fichier par défaut est dérivé du nom de fichier d’origine. Le nom du fichier ne peut être modifié que lors du chargement et ne peut pas l’être plus tard. Les exigences en termes de caractères de nom de fichier sont les mêmes que pour AEM Assets.<br>Le même nom de fichier ne peut pas être utilisé pour des fichiers de sous-titres et de suivi audio supplémentaires. |
      | Langue | Sélectionnez la langue de la légende. Après le traitement d’un fichier de légende, ce champ de langue devient non modifiable (grisé). |
      | Type | Sélectionnez le type de légende que vous utilisez.<br>**Sous-titre** - Texte de la légende affiché avec la vidéo qui traduit ou transcrit la boîte de dialogue.<br>**Légende** - Le texte de la légende comprend également des bruits de fond, la différenciation des locuteurs et d’autres informations pertinentes, ainsi que la traduction ou la transcription du dialogue, ce qui rend le contenu plus accessible aux personnes sourdes ou malentendantes. |
      | Etiquette | Le texte affiché pour le nom de la légende dans le champ **[!UICONTROL Sélection de l’audio ou de la légende]** liste déroulante dans le lecteur multimédia. Le libellé correspond à ce qu’un client voit et correspond à un suivi de sous-titre ou de légende. Par exemple : `English (CC)`. |

      Si nécessaire, vous pourrez modifier les métadonnées de légende ultérieurement. Lorsque la vidéo est publiée, ces détails sont reflétés dans les URL publiques des vidéos publiées.

   1. Dans le coin supérieur droit de la page, dans la **[!UICONTROL Enregistrer et fermer]** menu déroulant, cliquez sur **[!UICONTROL Enregistrer]**. Les fichiers sont chargés et le traitement des métadonnées commence, comme le montre la section **État** de l’interface.

      >[!NOTE]
      >
      >Selon les paramètres de mise en cache de votre instance, le traitement des métadonnées peut prendre plusieurs minutes avant qu’elles ne soient reflétées dans l’aperçu et dans les URL publiées.

   1. Si vous avez sélectionné **[!UICONTROL Enregistrer et fermer]** à l’étape précédente au lieu de sélectionner **[!UICONTROL Enregistrer]**, vous pouvez toujours afficher l’état du traitement des fichiers chargés. Voir [Afficher l’état de cycle de vie des fichiers de sous-titres et de suivi audio chargés].
   1. Passez à l’étape 9.
+++

+++**Option 2 :** *Je veux que l’IA génère mes fichiers de sous-titres en plusieurs langues.*

   1. Dans le coin supérieur droit de la page, cliquez sur **[!UICONTROL Créer une légende]** > **[!UICONTROL Conversion de pistes audio]**.
   1. Dans le **Convertir les pistes audio** , définissez les options suivantes :

      | Option | Description |
      |--- |--- |
      | Suivi audio à convertir | Dans la liste déroulante, sélectionnez le fichier de suivi audio téléchargé à partir duquel l’IA doit générer les sous-titres. |
      | Langues de sortie | Dans la liste déroulante, sélectionnez une ou plusieurs langues dans lesquelles le fichier de sous-titres doit apparaître.<br>Pour supprimer une langue sélectionnée, cliquez sur **X**.<br>Pendant la lecture vidéo, la liste des langues s’affiche dans le lecteur multimédia dans l’ordre dans lequel vous les sélectionnez ici. |

   1. Cliquez sur **[!UICONTROL Terminé]**.
   1. Dans le coin supérieur droit de la page, dans la **[!UICONTROL Enregistrer et fermer]** menu déroulant, cliquez sur **[!UICONTROL Enregistrer]**. Un ou plusieurs fichiers de sous-titres sont créés et le traitement commence, comme le montre la section **État** de l’interface. Voir aussi [Afficher l’état de cycle de vie des fichiers de sous-titres et de suivi audio chargés].

      >[!NOTE]
      >
      >Selon les paramètres de mise en cache de votre instance, le traitement des métadonnées peut prendre plusieurs minutes avant qu’elles ne soient reflétées dans l’aperçu et dans les URL publiées.

   1. (Facultatif) Sélectionnez l’icône représentant un crayon à droite du nom d’un fichier de sous-titres. Dans le **Modifier la légende** , vous pouvez modifier les détails suivants sur le fichier :

      | Métadonnées de légende | Description |
      | --- | --- |
      | Type | Sélectionnez le type de légende que vous utilisez.<br>**Sous-titre** - Texte de la légende affiché avec la vidéo qui traduit ou transcrit la boîte de dialogue.<br>**Légende** - Le texte de la légende comprend également des bruits de fond, la différenciation des locuteurs et d’autres informations pertinentes, ainsi que la traduction ou la transcription du dialogue, ce qui rend le contenu plus accessible aux personnes sourdes ou malentendantes. |
      | Etiquette | Le texte affiché pour le nom de la légende dans le champ **[!UICONTROL Sélection de l’audio ou de la légende]** liste déroulante dans le lecteur multimédia. Le libellé correspond à ce qu’un client voit et correspond à un suivi de sous-titre ou de légende. Par exemple : `English (CC)`. |

      Vous pouvez modifier ou modifier ultérieurement certaines métadonnées de légende, si nécessaire. Lorsque la vidéo est publiée, ces détails de métadonnées sont répercutés sur les URL publiques dans les vidéos publiées.
   1. Passez à l’étape 9.
+++

+++**Option 3 :** *Le texte d’un fichier de légende (.vtt) doit être corrigé, rechargé pour remplacer l’ancien fichier .vtt, puis le fichier corrigé doit être traduit par AI.*

   1. Cliquez sur **[!UICONTROL Créer une légende]** > **[!UICONTROL Traduire les légendes]**.
   1. Dans le **Traduire la légende** , définissez les options suivantes :

      | Option | Description |
      |--- |--- |
      | Légende à traduire | Dans la liste déroulante, choisissez un fichier de sous-titres à partir duquel l’IA doit traduire le texte de la sous-titrage. |
      | Langues de sortie | Dans la liste déroulante, sélectionnez une ou plusieurs langues dans lesquelles le fichier de sous-titres doit apparaître.<br>Pour supprimer une langue sélectionnée, cliquez sur **X**.<br>Pendant la lecture vidéo, la liste des langues s’affiche dans le lecteur multimédia dans l’ordre dans lequel vous les sélectionnez ici. |

   1. Cliquez sur **[!UICONTROL Terminé]**.
   1. Dans le coin supérieur droit de la page, dans la **[!UICONTROL Enregistrer et fermer]** menu déroulant, cliquez sur **[!UICONTROL Enregistrer]**. Un ou plusieurs fichiers de sous-titres sont créés et le traitement commence, comme le montre la section **État** de l’interface. Voir aussi [Afficher l’état de cycle de vie des fichiers de sous-titres et de suivi audio chargés].

      >[!NOTE]
      >
      >Selon les paramètres de mise en cache de votre instance, le traitement des métadonnées peut prendre plusieurs minutes avant qu’elles ne soient reflétées dans l’aperçu et dans les URL publiées.

   1. (Facultatif) Sélectionnez l’icône représentant un crayon à droite du nom d’un fichier de sous-titres. Dans le **Modifier la légende** , vous pouvez modifier les détails suivants sur le fichier :

      | Métadonnées de légende | Description |
      | --- | --- |
      | Type | Sélectionnez le type de légende que vous utilisez.<br>**Sous-titre** - Texte de la légende affiché avec la vidéo qui traduit ou transcrit la boîte de dialogue.<br>**Légende** - Le texte de la légende comprend également des bruits de fond, la différenciation des locuteurs et d’autres informations pertinentes, ainsi que la traduction ou la transcription du dialogue, ce qui rend le contenu plus accessible aux personnes sourdes ou malentendantes. |
      | Etiquette | Le texte affiché pour le nom de la légende dans le champ **[!UICONTROL Sélection de l’audio ou de la légende]** liste déroulante dans le lecteur multimédia. Le libellé correspond à ce qu’un client voit et correspond à un suivi de sous-titre ou de légende. Par exemple : `English (CC)`. |

      Vous pouvez modifier ou modifier ultérieurement certaines métadonnées de légende, si nécessaire. Lorsque la vidéo est publiée, ces détails de métadonnées sont répercutés sur les URL publiques dans les vidéos publiées.

   1. Passez à l’étape 9.
+++

1. (Facultatif) Prévisualisez la vidéo avant de la publier pour vous assurer que les sous-titres et le son fonctionnent comme prévu. Voir [Prévisualiser une vidéo comportant plusieurs sous-titres et pistes audio].

>[!MORELIKETHIS]
>
>* [Connexion à et déconnexion de l’application de bureau Adobe Dynamic Media Classic](/help/using/signing-out.md)
>* [Téléchargement et installation de l’appli de bureau Adobe Dynamic Media Classic](/help/using/dynamic-media-classic-desktop-app.md)

<!-- SAVE: OLD LINK TO BEST PRACTICES GUIDE IN PDF https://www.adobe.com/content/dam/www/us/en/marketing/experience-manager-assets/dynamic-media/adobe-dynamic-media-classic-best-practices-guide.pdf -->