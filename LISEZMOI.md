# Bordereaux CNAS / CASNOS — application Android

Cette application fonctionne **hors connexion** (sauf l'import Excel si la bibliothèque n'est pas chargée : elle est incluse).
Les données restent **sur le téléphone** (stockage local de l'application). Faites régulièrement
« Exporter (JSON) » pour sauvegarder.

## Obtenir l'APK (gratuit, sans installer Android Studio)

1. Créez un compte gratuit sur https://github.com puis un **nouveau dépôt** (ex. `bordereaux-apk`), en **public** si vous voulez un lien de téléchargement ouvert à tous.
2. Envoyez tout le contenu de ce dossier dans le dépôt (bouton **Add file > Upload files**).
   - Si le dossier caché `.github` n'est pas pris en compte : **Add file > Create new file**, nom `.github/workflows/build-apk.yml`, puis collez le contenu du fichier `build-apk.yml` fourni.
3. Onglet **Actions** > « Construire l'APK » > **Run workflow**. Attendez 5 à 10 minutes.
4. Récupérez l'APK dans **Releases** (colonne de droite du dépôt) : fichier `Bordereaux-CNAS-CASNOS.apk`.

## Installer sur le téléphone

Ouvrez le fichier APK téléchargé et autorisez l'installation depuis cette source si Android le demande
(« Installer des applications inconnues »). C'est un APK de type *debug* : il s'installe normalement, mais n'est pas publié sur le Play Store.

## Mettre à jour l'application

Remplacez `www/index.html` dans le dépôt : l'APK est reconstruit automatiquement.
Pensez à exporter vos données avant de désinstaller l'ancienne version.
