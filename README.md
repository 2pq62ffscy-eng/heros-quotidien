# Héros du Quotidien

Application PWA de gamification des habitudes quotidiennes, dans l'univers des Terres Centrales.

## Structure

```
heros-quotidien/
├── api/
│   └── chapter.js      ← Fonction serverless (proxy Groq)
├── public/
│   ├── index.html      ← App principale
│   ├── manifest.json   ← Config PWA
│   └── sw.js           ← Service Worker (offline)
├── vercel.json         ← Config Vercel
└── README.md
```

## Déploiement sur Vercel

### 1. Pusher sur GitHub
- Crée un nouveau repo GitHub (ex: `heros-quotidien`)
- Upload tous les fichiers dedans

### 2. Importer sur Vercel
- Va sur vercel.com → "Add New Project"
- Sélectionne ton repo GitHub
- Clique "Deploy" sans rien changer

### 3. Ajouter la clé Groq
- Dans Vercel → ton projet → "Settings" → "Environment Variables"
- Ajoute : `GROQ_API_KEY` = ta clé depuis console.groq.com
- Redéploie (Settings → Deployments → "Redeploy")

### 4. Installer la PWA
- Ouvre l'URL Vercel sur ton téléphone
- Safari (iOS) : bouton partage → "Sur l'écran d'accueil"
- Chrome (Android) : menu → "Ajouter à l'écran d'accueil"

## Coût
Groq est gratuit pour un usage personnel.
