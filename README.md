# Tennis de l'Île aux Moines

Planning quotidien du court (9 h – 20 h), rotation des 10 familles, vacances scolaires A/B/C imprimables.

- Site : https://tennis-ile-aux-moines.vercel.app
- Tout est dans `index.html` : pas de base de données, le planning est recalculé à chaque ouverture.
- Familles et téléphones : objet `FAM` dans `index.html`.
- Ordre de rotation : tableau `CYCLE` (lu sur le planning de la Toussaint 2026).
- Vacances officielles : objet `OFFICIAL` (ajouter une année quand le ministère publie le calendrier).

Appli (PWA) : `manifest.webmanifest`, `sw.js` et les icônes `icon-*.png` / `apple-touch-icon.png` permettent d'installer le site sur l'écran d'accueil et de le consulter hors connexion. Après une modification importante, augmenter `VERSION` dans `sw.js` (tiam-v1 → tiam-v2) pour forcer le rafraîchissement chez tout le monde.

Mise à jour : modifier `index.html`, puis `git add . && git commit -m "..." && git push` — Vercel redéploie tout seul.
