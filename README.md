# Le Chemin des Tons

Jeu mobile pour apprendre le tableau des intervalles (en tons) avec un thon. PWA : installable, utilisable hors ligne, mode clair/sombre.

Site statique, sans build : `index.html` + `manifest.webmanifest` + `sw.js` + `icons/`.

## Tester en local
    python3 -m http.server 8080   # puis http://localhost:8080

## Mettre en ligne
    git init && git add . && git commit -m "Le Chemin des Tons"
    gh repo create chemin-des-tons --public --source=. --push
    npx vercel --prod        # ou importer le repo sur vercel.com (Framework: Other, pas de build)

## À chaque mise à jour
Changer `VERSION` dans `sw.js` (ex. `cdt-v2`) pour que les appareils rechargent le jeu.

## Licence

[PolyForm Noncommercial 1.0.0](https://polyformproject.org/licenses/noncommercial/1.0.0) : usage, étude et adaptation libres pour tout usage non commercial (enseignement compris). Toute utilisation commerciale est exclue. Voir `LICENSE`.
