---
title: Politique de confidentialité de Reforge
permalink: /reforge/privacy/
lang: fr
---

# Politique de confidentialité de Reforge

*Dernière mise à jour : 28 octobre 2026.* · [English version](../en/privacy/)

Reforge est une application Android de coaching de musculation. Cette page dit ce qu'elle enregistre, ce qui peut sortir de ton téléphone, vers qui, et comment tu gardes la main.

## En bref

- **Pas de compte, pas de serveur de Reforge.** L'éditeur ne reçoit, ne stocke et ne revend aucune de tes données.
- **Pas de publicité, pas de mesure d'audience, pas de pistage** par Reforge.
- **Tout reste sur ton téléphone** : ton profil, tes séances, ton poids, tes repas, ta conversation avec le coach et tes réglages.
- **Quatre choses peuvent en sortir** : les illustrations d'exercices téléchargées, ce que tu envoies à l'IA du coach quand elle passe par le cloud, c'est-à-dire si tu l'as activée sur un téléphone qui ne peut pas faire tourner Gemini Nano (messages, repas à estimer, photos de repas, et un résumé de ton profil, de ta santé et de ton entraînement), le code-barres d'un produit que tu cherches dans Open Food Facts, et ce que tu décides d'échanger avec Health Connect. Chacune est détaillée plus bas, et aucune n'est active sans toi.
- **Des informations techniques** que les bibliothèques de Google intégrées à l'application peuvent envoyer à Google pour fonctionner : voir « Informations techniques envoyées à Google ». Reforge n'en reçoit aucune.

## Ce que Reforge enregistre sur ton téléphone

- Ton profil : objectif, niveau, âge, taille, poids, matériel, lieux d'entraînement, zones sensibles et notes que tu saisis.
- Ton programme, tes exercices personnels, tes séances et chaque série réalisée (charge, répétitions, effort ressenti).
- Tes pesées et ta masse grasse, saisies ou importées de Health Connect.
- Tes mensurations (tour de taille, hanches, bras…), si tu en saisis : elles restent sur ton téléphone et dans tes sauvegardes, et ne sont pas envoyées à l'IA.
- Tes photos de progression, si tu en prends ou en choisis : elles restent dans l'espace privé de l'application et ne vont nulle part ailleurs, ni à l'IA, ni dans l'export, ni dans la sauvegarde automatique, ni dans la sauvegarde cloud d'Android. Seul un transfert direct vers un nouveau téléphone (Android 12 et plus, par câble ou Wi-Fi) les copie. « Enregistrer une copie » écrit la photo à l'endroit que tu choisis dans le sélecteur d'Android ; une photo supprimée dans Reforge est effacée du téléphone.
- Tes repas (heure, description, aliments et leurs apports estimés), tes repas favoris et tes réglages de nutrition, dont ton régime alimentaire, tes allergies et les aliments que tu évites s'ils sont renseignés : ce sont des données de santé, que tu choisis de saisir (ou non), qui restent sur ton téléphone et dans tes sauvegardes. Les photos de repas ne sont pas gardées : celle prise avec l'appareil photo de Reforge (ou avec l'application d'appareil photo du téléphone, si celui de Reforge ne peut pas s'ouvrir) est écrite dans le cache de l'application, puis effacée dès que Reforge l'a lue.
- La conversation avec le coach, que tu peux effacer avec « Nouvelle conversation ».
- Tes réglages (thème, unités, minuteur de repos, rappels d'entraînement, IA activée ou non, opacité et couleurs de chaque widget) et tes habitudes de repos.

Ces données sont dans l'espace privé de l'application : les autres applications n'y ont pas accès.

### Widgets de l'écran d'accueil

Si tu ajoutes un widget de Reforge à ton écran d'accueil, il y affiche une partie de ces données : ton poids et ta masse grasse du dernier mois (« Poids et masse grasse »), tes apports du jour face à tes objectifs (« Apports du jour »), ou tes séances de la semaine et celle du jour (« Ma semaine »). Le widget est dessiné par ton téléphone et rien n'est envoyé à personne, mais toute personne qui voit ton écran d'accueil voit aussi ce qu'il affiche. Aucun widget n'est ajouté sans toi, et le retirer de l'écran d'accueil suffit pour ne plus rien montrer.

## Ce qui peut sortir de ton téléphone

### Illustrations des exercices

Quand tu ouvres la fiche d'un exercice ou les conseils d'une séance, Reforge télécharge ses illustrations depuis le serveur de [RepDB](https://repdb.co) (`exercise-dataset.com`), puis les garde sur le téléphone. Cette requête révèle l'exercice consulté et ton adresse IP, comme toute requête web. RepDB ne reçoit rien d'autre.

### IA du coach

L'IA est facultative et éteinte tant que tu ne l'as pas activée : à la fin du premier lancement, dans Réglages › Intelligence artificielle, ou avec le bouton « Activer l'IA » du coach. Un écran dit d'abord ce qu'elle fait et où va ce que tu écris. Tu ne choisis pas le modèle et tu n'as aucune clé à saisir : Reforge prend Gemini Nano si ton téléphone peut le faire tourner, et le cloud de Reforge sinon.

- **Gemini Nano (sur le téléphone)**, si ton téléphone peut le faire tourner (les Pixel 9 et 10, entre autres) : le texte est traité par ton téléphone, rien de ce que tu écris n'est envoyé. Le modèle est téléchargé par les services Google du téléphone (AICore), pas par Reforge, et le cloud ne prend jamais le relais pendant ce téléchargement. Gemini Nano ne lit pas les photos : estimer un repas en photo n'est pas proposé dans ce cas.
- **Le cloud de Reforge**, si ton téléphone ne peut pas faire tourner Gemini Nano et que ta version l'inclut : pour te répondre, tes messages au coach, tes notes, les repas que tu fais estimer (description, liste ou photo) et un résumé de ton profil, de ton entraînement et de ta nutrition (sexe, âge, taille, tendance du poids et de la masse grasse, zones sensibles, programme, dernières séances, repas saisis, objectifs du jour, régime alimentaire, allergies et aliments à éviter si tu les as renseignés, activité lue dans Health Connect si la synchronisation est active, date et heure locales) sont envoyés à l'API Gemini de Google, par le service Firebase de l'éditeur. C'est l'offre payante de l'API : Google n'utilise pas ces contenus pour entraîner ses modèles. Google garde tes messages et les réponses pendant une durée limitée, uniquement pour détecter les usages interdits par son règlement, et ces données peuvent être conservées ou mises en cache dans tout pays où Google ou ses agents ont des installations : cette API n'offre qu'un accès mondial aux modèles, et l'éditeur ne peut pas choisir la région où ta requête est traitée. Google reçoit aussi des informations techniques (nombre de jetons, erreurs, identifiants d'appareil ou de jeton, adresse IP), qu'il traite selon ses propres règles de confidentialité. L'éditeur ne consulte ni ne conserve ces échanges. Ce cloud est réservé aux personnes de 18 ans et plus : Reforge te demande de le confirmer avant de l'activer, et ne le propose pas si l'année de naissance de ton profil indique moins de 18 ans. Un jeton technique (Firebase App Check, Play Integrity) accompagne les requêtes pour que Google vérifie qu'elles viennent de l'application officielle et limite les abus. Rien n'est envoyé tant que tu n'as pas activé l'IA, puis que tu n'écris pas au coach ou ne fais pas estimer un repas.
- **Pas d'IA** : tant qu'elle est éteinte, ou si ni Gemini Nano ni le cloud de Reforge ne sont disponibles, le coach répond avec sa base de connaissances, hors ligne.

L'écran qui précède l'activation dit lequel des deux répond sur ton téléphone, et ce qui part quand c'est le cloud. Ni une sauvegarde (le fichier d'export, ou celle d'Android quand tu changes de téléphone) ne rallume l'IA : tu l'actives sur chaque téléphone. Les charges et les progressions sont toujours calculées par les règles de Reforge sur ton téléphone, jamais par l'IA.

### Produits trouvés par leur code-barres

Quand tu cherches un produit emballé par son code-barres (« Code-barres » dans l'onglet Nutrition), Reforge envoie ce code, et lui seul, à [Open Food Facts](https://world.openfoodfacts.org), une base de données ouverte gérée par une association à but non lucratif, pour recevoir les valeurs nutritionnelles et les allergènes de l'étiquette. La requête ne contient ni ton profil, ni tes repas, ni aucun identifiant ; comme pour toute connexion, le serveur d'Open Food Facts voit l'adresse IP de ton téléphone. Les valeurs reçues deviennent un repas que tu vérifies avant de l'enregistrer, sur ton téléphone.

Le code est lu par le lecteur de codes-barres des services Google Play (Google code scanner, ML Kit) : la caméra s'ouvre dans ces services, qui ne donnent à Reforge que le code lu, sans passer par l'autorisation « Appareil photo » de Reforge. Google indique que l'image est analysée sur le téléphone. Tu peux aussi taper le code à la main.

### Health Connect

C'est facultatif et désactivé par défaut : au premier lancement, une fois ton programme prêt, Reforge te le propose (tu peux répondre « Plus tard »), et tu peux l'activer plus tard dans les réglages. Si tu l'actives, Reforge **écrit** chaque séance terminée dans Health Connect (séance de musculation : date, durée, nom, exercices) avec l'énergie qu'il estime qu'elle a dépensée (calories actives, environ 3 MET au-dessus du repos pour la durée de la séance), sauf si ta montre ou une autre application en a déjà enregistré pour ce moment : sa mesure prime alors, et Reforge n'ajoute rien ou retire son estimation ; il **lit** ton poids et ta masse grasse pour compléter ta courbe, et **lit** ton activité des 7 derniers jours (pas, calories actives, activités enregistrées par d'autres applications) quand le coach ou l'onglet Nutrition en ont besoin, sans la conserver. Ces données sont gérées par Health Connect, sur ton téléphone : Reforge ne les envoie à personne, sauf la tendance du poids et de la masse grasse et l'activité récente qui accompagnent tes questions quand l'IA passe par le cloud. Quand tu supprimes une séance dans Reforge, Reforge supprime aussi, dans Health Connect, la séance et l'énergie qu'il y avait écrites (jamais les mesures d'une montre ou d'une autre application). Tu peux retirer ces autorisations à tout moment dans Health Connect.

### Informations techniques envoyées à Google

Reforge s'appuie sur deux bibliothèques de Google qui peuvent envoyer à Google des informations techniques, sans rapport avec ce que tu saisis dans l'application :

- **ML Kit**, pour Gemini Nano sur le téléphone : des mesures de fonctionnement et de performance, avec des informations sur l'appareil et sur l'application (version de l'application, modèle du téléphone, version d'Android). Elles peuvent partir dès que l'application demande à ton téléphone si Gemini Nano est disponible, donc à chaque lancement, même si l'IA est éteinte.
- **Firebase**, seulement si tu utilises le cloud de Reforge : des informations sur l'application (sa version, celle de la bibliothèque, son identifiant Firebase) et un jeton d'attestation Play Integrity (Firebase App Check) qui permet à Google de vérifier que la requête vient de l'application officielle.

Ces informations servent à faire fonctionner, diagnostiquer et protéger ces services de Google. Reforge n'en reçoit aucune et ne peut pas les consulter. Le détail est dans la documentation de Google sur [ML Kit](https://developers.google.com/ml-kit/android-data-disclosure) et sur [Firebase](https://firebase.google.com/docs/android/play-data-disclosure).

### Signaler une réponse du coach

Si tu signales une réponse de l'IA, Reforge prépare un message (la réponse signalée, le motif, ton commentaire éventuel, la version de l'application et le modèle utilisé) que tu relis dans ton application de messagerie avant de l'envoyer à l'éditeur. Rien n'est envoyé sans ton accord, et ce message ne contient ni ton profil ni tes séances.

### Sauvegardes et exports

- Si la sauvegarde Android est activée sur ton téléphone, Android peut sauvegarder les données de Reforge (base de données et réglages) dans ton compte Google, selon tes paramètres Android.
- « Exporter mes données » crée un fichier JSON que tu enregistres où tu veux : Reforge n'en garde aucune copie.
- « Sauvegarde automatique » est éteinte tant que tu n'as pas choisi un dossier dans le sélecteur d'Android (sur le téléphone, une carte mémoire, ou un cloud dont l'application le propose). Reforge y écrit alors le même fichier qu'un export, après chaque séance et une fois par jour, et garde les 7 derniers ; il n'a accès qu'à ce dossier, pas au reste du stockage. Si ce dossier est synchronisé avec un cloud, c'est l'application de ce cloud qui y envoie le fichier, pas Reforge. L'arrêter rend l'accès au dossier, et les fichiers déjà écrits y restent.

## Ce que Reforge ne fait pas

Reforge n'affiche pas de publicité, ne mesure pas ton usage, ne crée pas de profil publicitaire, ne contient aucun traceur publicitaire ni outil de mesure d'audience, et ne vend ni ne partage tes données avec des tiers.

## Autorisations Android

- **Internet** : télécharger les illustrations, chercher un produit dans Open Food Facts par son code-barres, et joindre l'IA dans le cloud quand tu l'as activée sur un téléphone qui ne peut pas faire tourner Gemini Nano.
- **Notifications, vibration, alarmes exactes** : te prévenir à la fin du temps de repos, même écran éteint.
- **Rappels d'entraînement** (facultatifs, éteints tant que tu ne les actives pas) : une notification les jours où une séance est prévue, faite sur ton téléphone avec ton programme et tes séances, sans rien envoyer à personne. Android te demande l'autorisation des notifications au moment où tu les actives, et la catégorie « Rappels d'entraînement » de ses réglages de notifications te laisse les couper. Reforge remet l'alarme du prochain rappel en place quand le téléphone redémarre (autorisation « Recevoir au démarrage », sans danger : elle ne donne accès à rien).
- **Health Connect** (écriture des séances et de leur énergie ; lecture du poids, de la masse grasse, des pas, des calories actives et des activités) : facultatif, voir plus haut.
- **Appareil photo** (facultatif) : Android te le demande la première fois que tu prends une photo depuis Reforge. Il sert à prendre tes photos avec l'appareil photo de Reforge : un repas toujours sur l'objectif arrière, une photo de progression sur l'objectif de ton choix, avec un retardateur si tu veux. Si celui de Reforge ne peut pas s'ouvrir, ton application d'appareil photo prend le relais (Android ne laisse une application qui a son propre appareil photo ouvrir celle du téléphone qu'avec cette autorisation). Reforge n'utilise la caméra que lorsque son appareil photo est ouvert à l'écran, et l'image suit le chemin décrit plus haut : jamais gardée pour un repas, gardée sur le téléphone seulement pour une photo de progression. Refusé, tu peux toujours choisir une photo dans ta galerie.
- **Codes-barres** : le lecteur des services Google Play ouvre sa propre caméra et ne donne à Reforge que le code lu ; il n'utilise pas l'autorisation « Appareil photo » de Reforge.
- **Galerie** : Reforge ne demande pas l'accès à tes photos : le sélecteur de photos d'Android ne lui donne que la photo choisie.

## Tes choix

- Activer ou éteindre l'IA : Réglages › Intelligence artificielle (ou « Activer l'IA » dans le coach).
- Renseigner, changer ou effacer ton régime et tes allergies : onglet Nutrition ou Réglages › Alimentation › Régime et allergies (« Tout effacer »).
- Activer, régler ou couper les rappels d'entraînement : Réglages › Rappels d'entraînement, ou la catégorie « Rappels d'entraînement » dans les réglages de notifications d'Android.
- Retirer les autorisations Health Connect : dans Health Connect.
- Retirer l'accès à l'appareil photo : réglages d'Android (Applications › Reforge › Autorisations).
- Supprimer une séance : Progrès › Historique › la séance › corbeille. Elle est aussi retirée de Health Connect.
- Exporter ou importer une sauvegarde, choisir ou arrêter la sauvegarde automatique : Réglages › Données.
- Ne plus afficher tes données sur l'écran d'accueil : retirer le widget, avec un appui long sur lui.
- Tout supprimer : désinstaller l'application, ou effacer son stockage dans les réglages Android (Applications › Reforge › Stockage). Les séances écrites dans Health Connect y restent : supprime-les dans Health Connect, ou une à une dans Reforge avant de le désinstaller (supprimer une séance dans Reforge la retire aussi de Health Connect).

Reforge ne détient aucune donnée sur toi en dehors de ton téléphone : il n'y a donc rien à demander à l'éditeur. Pour ce qui est envoyé à Google (IA dans le cloud, quand elle est activée), tes droits s'exercent auprès de Google.

## Santé

Reforge donne des repères d'entraînement et de nutrition ; ce n'est pas un avis médical. En cas de douleur, de blessure, de grossesse ou de maladie, demande l'avis d'un professionnel de santé avant de t'entraîner. Le filtre sur les allergies écarte les aliments de sa table qui contiennent d'ordinaire l'allergène, mais il ne connaît ni les traces, ni les produits transformés, ni les plats d'un restaurant : il ne remplace ni la lecture des étiquettes, ni l'avis d'un allergologue ou d'un médecin.

## Enfants

Reforge n'est pas destinée aux enfants et ne collecte aucune donnée à leur sujet.

## Changements

Quand cette politique change, la date en haut de la page change aussi, et les changements importants sont annoncés dans les notes de version.

## Contact

Une question sur cette politique ? Écris à l'adresse de contact indiquée sur la fiche Google Play de Reforge.
