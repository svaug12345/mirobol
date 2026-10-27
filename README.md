# mirobol.fr — bac à sable

Site de **test** (banc d'essai) des projets, séparé de `baiji.fr` (la vitrine).
Hébergé sur GitHub Pages, domaine perso `mirobol.fr`.

## Ajouter un test

1. Créer un dossier à la racine (ex. `essai-jeu/`) avec au moins un `index.html`.
2. Ajouter une ligne dans la liste `TESTS` de `index.html` :
   `{ nom: "Essai jeu", desc: "…", url: "essai-jeu/" }`
3. Le test devient accessible à `mirobol.fr/essai-jeu/`.

Quand un projet est prêt, on le promeut vers `baiji.fr`.

## Serrure d'accès + journal

`gate.js` affiche une petite serrure (code `aaaa`) et « ping » un Google Apps Script
à chaque visite pour tenir un journal (dans un Google Sheet).
Sécurité faible par nature (site statique, code visible dans la source) : décourage
un regard indiscret, rien de plus. L'URL du script se règle dans `gate.js` (`LOG_URL`).
Pour protéger une page de test : ajouter `<script src="/gate.js"></script>` en haut de son `<head>`.

## Identité visuelle

Charte « SV » : teal `#0f7c7b`, neutres vert-bleu, police Manrope, le « geste » comme logo.
