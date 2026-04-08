# 🚀 FINA Interview Web Legacy - Guide de Déploiement

## Option 1 : Déploiement sur Vercel (RECOMMANDÉ - 5 min)

### Étape 1 : Préparer le projet
```bash
# Extraire le ZIP
# Ouvrir un terminal dans le dossier fina-deploy

# Installer les dépendances
npm install
```

### Étape 2 : Tester en local (optionnel)
```bash
npm start
# Ouvre http://localhost:3000
```

### Étape 3 : Déployer sur Vercel

**Méthode A - Via GitHub (recommandé):**
1. Créer un compte sur https://github.com
2. Créer un nouveau repository "fina-app"
3. Pousser le code :
   ```bash
   git init
   git add .
   git commit -m "FINA V6"
   git remote add origin https://github.com/TON_USERNAME/fina-app.git
   git push -u origin main
   ```
4. Aller sur https://vercel.com
5. "Import Project" → Sélectionner ton repo GitHub
6. Cliquer "Deploy"
7. ✅ Ton site est en ligne !

**Méthode B - Glisser-déposer:**
1. ```bash
   npm run build
   ```
2. Aller sur https://vercel.com
3. Glisser le dossier `build` sur la page
4. ✅ Ton site est en ligne !

---

## Option 2 : Déploiement sur Netlify

1. ```bash
   npm run build
   ```
2. Aller sur https://app.netlify.com/drop
3. Glisser le dossier `build`
4. ✅ Ton site est en ligne !

---

## 📁 Structure du projet
```
fina-deploy/
├── package.json      # Dépendances
├── public/
│   └── index.html    # Page HTML
└── src/
    ├── index.js      # Point d'entrée React
    └── App.js        # Code FINA V6
```

## ⚠️ Prérequis
- Node.js 18+ (télécharger sur https://nodejs.org)
- npm (inclus avec Node.js)

## 🆘 Problèmes courants

**"npm not found"**
→ Installer Node.js depuis https://nodejs.org

**Erreurs de build**
→ Supprimer node_modules et réinstaller :
```bash
rm -rf node_modules
npm install
```

---

Créé avec ❤️ par FINA
