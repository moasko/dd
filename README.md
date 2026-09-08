# demo

Maquette HTML de démonstration d’un compte bancaire, préparée en PWA.

## Utilisation

Pour consulter la maquette, ouvrir index.html. Pour installer la PWA et activer le mode hors ligne, servir le dossier sur HTTPS (ou localhost en développement). Une ouverture directe du fichier ne permet pas l’installation.

Avec Python installé : `python -m http.server 8080 --bind 127.0.0.1`, puis ouvrir http://localhost:8080 dans Chrome ou Edge et choisir Installer dans le navigateur.

Sur téléphone, ouvrir la version hébergée en HTTPS, puis choisir Installer l’application (Android) ou Partager > Sur l’écran d’accueil (iPhone).

Le premier chargement nécessite une connexion. Attendre la fin du chargement pour que les fichiers soient mis en cache. L’application peut ensuite être ouverte hors ligne. Les modifications des textes restent enregistrées dans le navigateur utilisé ; elles ne sont pas synchronisées entre appareils.

## Mise à jour

Déployer tous les fichiers, y compris icons et sw.js. À chaque modification des fichiers mis en cache, incrémenter la version CACHE_NAME dans sw.js. Fermer les fenêtres de l’application puis la rouvrir pour activer la nouvelle version.