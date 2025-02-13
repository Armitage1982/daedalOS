Le process pour publier le site est :

yarn install - Récupère les paquets et prépare l'application.
yarn build - Exécute les scripts et copie les fichiers depuis le dossier 'DaedalOS\public' vers 'DaedalOS\out'. C'est ce dernier dossier qui est à uploader.
(yarn deploy) - Réduit la taille du site en le minimisant.

Fichier à modifier pour ne plus référencer le mauvais propriétaire.
J'ai zippé l'essentiel dans une archive du même nom que ce fichier.

Dans le dossier 'DaedalOS\plublic' les fichiers y sont puisés, notamment :

- CREDITS.md - Qui contient la licence MIT et la référence à l'auteur
- favicon.ico
- Users\Public\Desktop\Demoscene Tribute.url - Le web desktop raccourcis vers une vidéo YouTube
- Users\Public\Desktop\GenAI.url - Le web desktop raccourcis vers le dossier suivant :
- GenAI\
- Users\Public\Pictures\slideshow.json - Une liste d'image pour le wallpaper slideshow.

Dans le dossier 'DaedalOS\utils' il y a 1 fichier Typescript :

- constants.ts

Toutes les infos de l'objet PACKAGE_DATA
La donnée npub est utilisée par l'apps Messenger afin d'envoyer un message au propriétaire.
Ma clé publique est : f473ad13216ab3be812d2b24bfd14e6c970c2b94cee41a8ef60f2b8dfa35aa05

Dans le dossier 'DaedalOS\scripts' il y a 2 scripts :

- robots.js
- rssBuilder.js

Principalement le ${author.url}

Dans le dossier 'DaedalOS\components\pages' il y a ce script :

- Metadata.tsx - Qui modifie également des infos pour les robots de navigateur

Dans le dossier 'daedalOS\components\apps\Browser' il y a ce script :

- config.ts - Permets de modifier / ajouter des raccourcis vers des sites web dans le navigateur intégré.

Dans le dossier 'daedalOS\2e2\components\apps' il y a ce script :

- constants.ts - Le nom de l'app