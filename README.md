# Gestion Locative – Application PWA

Application de gestion locative (résidences, appartements, locataires, loyers, travaux, parcelles et finance).

## Installation rapide depuis le téléphone

### Option A – StackBlitz (le plus simple)

1. Va sur https://stackblitz.com
2. Clique sur **Import from GitHub** (ou crée un projet React puis remplace les fichiers)
3. Une fois le projet ouvert :
   - Dans le terminal : `npm install`
   - Clique sur **Open in New Tab**
4. Dans Chrome → menu ⋮ → **Installer l’application**

### Option B – GitHub + Netlify (gratuit)

1. Crée un compte sur GitHub (app mobile ou navigateur)
2. Crée un nouveau dépôt (repository) public nommé `gestion-locative`
3. Uploade **tous les fichiers** de ce dossier dans le dépôt
4. Va sur https://app.netlify.com
5. Connecte ton compte GitHub et choisis le dépôt
6. Netlify déploie automatiquement
7. Ouvre le lien fourni par Netlify dans Chrome → **Installer l’application**

## Structure du projet

```
gestion-locative-pwa/
├── index.html
├── package.json
├── vite.config.js
├── public/
│   ├── manifest.json
│   └── icon-512.svg          ← icône (tu peux la remplacer par un PNG)
├── src/
│   ├── App.jsx               ← tout le code de l’application
│   ├── main.jsx
│   └── index.css
└── README.md
```

## Icône

L’icône actuelle est un SVG (immeuble stylisé or/sombre).

Pour une meilleure compatibilité PWA, télécharge une icône PNG 512×512 et place-la dans `public/icon-512.png`, puis mets à jour `manifest.json` si besoin.

## Commandes (si tu as un ordinateur plus tard)

```bash
npm install
npm run dev      # développement
npm run build    # production
```

## Notes

- Les données sont pour l’instant en mémoire (elles se réinitialisent au rechargement).
- Plus tard on pourra ajouter le stockage local (localStorage ou SQLite via Capacitor).

Bon courage !
