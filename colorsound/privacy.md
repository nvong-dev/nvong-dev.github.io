---
title: Politique de confidentialité de ColorSound
permalink: /colorsound/privacy/
lang: fr
---

# Politique de confidentialité de ColorSound

*Dernière mise à jour : 14 novembre 2026.* · [English version](../en/privacy/)

ColorSound est un visualiseur de spectre audio pour Windows. Cette page dit ce qu'il enregistre, ce qui peut sortir de ton PC, et comment tu gardes la main.

## En bref

- **Rien ne sort de ton PC par ColorSound.** Il n'utilise pas Internet : il n'envoie rien à l'éditeur ni à personne, et l'éditeur ne reçoit, ne stocke et ne revend aucune donnée sur toi.
- **Le son est analysé en mémoire, en temps réel**, pour animer les barres. Il n'est ni enregistré, ni conservé, ni envoyé.
- **Pas de compte, pas de publicité, pas de mesure d'audience, pas de pistage.**
- **Tes réglages et les journaux de diagnostic restent sur ton PC.**

## Le son

ColorSound capte le son que joue ton PC, sur la sortie par défaut de Windows ou sur le périphérique que tu choisis, avec l'API audio de Windows. Il n'utilise pas le microphone. À partir de ce son, il calcule plusieurs fois par seconde l'intensité de chaque bande de fréquences pour animer les barres. Le son lui-même n'est jamais écrit sur le disque ni transmis.

## Ce que ColorSound enregistre sur ton PC

- Tes réglages : thèmes et couleurs, nombre de barres et de LED, échelle, opacité, arrière-plan acrylique et rétroéclairage, position du widget à l'écran, source audio choisie, lancement au démarrage de Windows.
- Des journaux de diagnostic, utiles pour signaler un problème : version de ColorSound, démarrages et arrêts, état de la capture du son (avec le nom du périphérique audio) et erreurs. Ils ne contiennent rien de ce que tu écoutes.

Avec la version du Microsoft Store, ces fichiers sont dans le dossier privé de l'application, que Windows efface quand tu la désinstalles. La version portable les range dans `%LOCALAPPDATA%\ColorSound`.

Au premier lancement après une mise à jour de ColorSound 4, ColorSound reprend les réglages que la version 4 avait enregistrés sur ton PC. Ils ne quittent pas ton PC.

Si tu actives le lancement au démarrage de Windows, c'est Windows qui s'en charge : une tâche de démarrage pour la version du Microsoft Store, une entrée de démarrage du registre pour la version portable.

## Ce qui peut sortir de ton PC

ColorSound lui-même n'envoie rien. Deux choses relèvent de Microsoft, pas de ColorSound :

- **Le Microsoft Store**, qui installe ColorSound et ses mises à jour. La [déclaration de confidentialité de Microsoft](https://privacy.microsoft.com/fr-fr/privacystatement) s'y applique.
- **Les données de diagnostic de Windows** : Windows et ses composants, dont le Windows App Runtime sur lequel s'appuie ColorSound, peuvent envoyer des données de diagnostic à Microsoft selon tes réglages (Paramètres de Windows › Confidentialité et sécurité › Diagnostics et commentaires). ColorSound n'en reçoit aucune et ne peut pas les consulter.

Si le Windows App Runtime manque sur ton PC (version portable), ColorSound propose d'ouvrir sa page de téléchargement chez Microsoft : rien n'est téléchargé sans toi.

## Ce que ColorSound ne fait pas

ColorSound n'affiche pas de publicité, ne mesure pas ton usage, ne crée pas de profil, ne contient aucun traceur ni outil de mesure d'audience, et ne vend ni ne partage aucune donnée avec des tiers.

## Autorisations

La version du Microsoft Store déclare la capacité `runFullTrust`, que demande toute application de bureau Windows empaquetée pour fonctionner comme un programme classique. ColorSound n'utilise ni le microphone, ni la caméra, ni ta position, et ne lit pas tes fichiers.

## Tes choix

- Choisir le son affiché : Paramètres de ColorSound › Général › Source audio.
- Activer ou couper le lancement au démarrage : Paramètres de ColorSound › Général › Lancer au démarrage de Windows, ou Paramètres de Windows › Applications › Démarrage.
- Voir ou effacer les journaux de diagnostic : Paramètres de ColorSound › À propos › Journaux de diagnostic ouvre leur dossier.
- Tout supprimer : désinstaller ColorSound (Paramètres de Windows › Applications › Applications installées) efface ses réglages et ses journaux. Pour la version portable, supprime son dossier et `%LOCALAPPDATA%\ColorSound`.

L'éditeur ne détient aucune donnée sur toi. Pour ce qui relève de Microsoft (Microsoft Store, données de diagnostic de Windows), tes droits s'exercent auprès de Microsoft.

## Enfants

ColorSound ne collecte aucune donnée, quel que soit l'âge de la personne qui l'utilise.

## Changements

Quand cette politique change, la date en haut de la page change aussi, et les changements importants sont annoncés dans les notes de version.

## Contact

Une question sur cette politique ? Écris à [nvong.dev@gmail.com](mailto:nvong.dev@gmail.com).
