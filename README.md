# Portfolio — Nathan Amian (React + Vite + Tailwind 4)

## Installation et lancement
```bash
npm install
npm run dev        # http://localhost:5173
npm run build      # génère /dist
```
Prérequis : Node.js 18+.

## Personnaliser
- **Tout le contenu** (textes, contacts, compétences, projets, parcours, galerie) : `src/data/content.js`.
- **Images** : placez vos fichiers dans `public/images/` puis utilisez `'/images/mon-fichier.jpg'` à la place de `img('seed')`.
- **Couleurs et polices** : bloc `@theme` dans `src/index.css` (`--color-volt` = vert d'accent).
- **Nouveau projet** : ajoutez un objet dans `projects` (catégorie : Réseaux, Design, Photo, Vidéo ou Communication).
- **SEO** : titre, description et Open Graph dans `index.html`.
- **Formulaire** : par défaut, ouvre la messagerie (mailto). Pour un envoi direct gratuit, créez un formulaire sur formspree.io et remplacez `submit` dans `Contact.jsx` par un `fetch('https://formspree.io/f/VOTRE_ID', { method: 'POST', body: new FormData(e.target) })`.

## Déployer gratuitement
- **Vercel** : poussez sur GitHub, « Add New Project », importez le dépôt (Vite détecté automatiquement).
- **Netlify** : build `npm run build`, dossier `dist`.
- **GitHub Pages** : ajoutez `base: '/nom-du-depot/'` dans `vite.config.js`, puis déployez `dist`.
