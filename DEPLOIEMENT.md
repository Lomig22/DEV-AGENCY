# 🚀 Guide de Déploiement sur Vercel

Votre landing page est prête à être déployée ! Voici les différentes méthodes disponibles.

## ✅ Fichiers Préparés

- ✅ `vercel.json` - Configuration Vercel
- ✅ `.gitignore` - Fichiers à ignorer
- ✅ Git initialisé et commit créé
- ✅ Tous vos fichiers sont prêts

---

## 🎯 Méthode 1 : Via GitHub + Vercel (RECOMMANDÉ)

### Étape 1 : Créer un repository GitHub

1. Allez sur [github.com](https://github.com) et connectez-vous
2. Cliquez sur le bouton **"New"** (ou "+" en haut à droite)
3. Nommez votre repository : `landing-page-agence` (ou autre nom)
4. Laissez-le **Public** ou **Private**
5. **NE COCHEZ PAS** "Add README" ou autres options
6. Cliquez sur **"Create repository"**

### Étape 2 : Pousser votre code sur GitHub

GitHub vous donnera des commandes. Utilisez celles-ci dans votre terminal :

```bash
cd "/Users/admin/DEV AGENCY/LANDING PAGE/DEV-AGENCY-main"
git remote add origin https://github.com/VOTRE-USERNAME/VOTRE-REPO.git
git branch -M main
git push -u origin main
```

**Remplacez** `VOTRE-USERNAME` et `VOTRE-REPO` par vos informations !

### Étape 3 : Déployer sur Vercel

1. Allez sur [vercel.com](https://vercel.com)
2. Cliquez sur **"Sign Up"** (ou "Log In" si vous avez déjà un compte)
3. Choisissez **"Continue with GitHub"**
4. Autorisez Vercel à accéder à vos repositories
5. Cliquez sur **"Add New Project"** ou **"Import Project"**
6. Sélectionnez votre repository `landing-page-agence`
7. Vercel détectera automatiquement la configuration
8. Cliquez sur **"Deploy"**

🎉 **C'est tout !** Votre site sera en ligne en moins d'une minute !

Vercel vous donnera une URL comme : `https://landing-page-agence.vercel.app`

---

## 🎯 Méthode 2 : Via Vercel CLI (Si vous avez les droits admin)

Si vous pouvez installer des packages globalement :

```bash
# Installer Vercel CLI
sudo npm install -g vercel

# Naviguer vers votre projet
cd "/Users/admin/DEV AGENCY/LANDING PAGE/DEV-AGENCY-main"

# Déployer
vercel

# Suivez les instructions interactives
# - Connectez-vous avec votre compte
# - Confirmez les paramètres
# - Votre site sera déployé !
```

---

## 🎯 Méthode 3 : Drag & Drop (Le Plus Simple)

1. Allez sur [vercel.com](https://vercel.com) et connectez-vous
2. Sur le dashboard, cherchez **"Deploy"** ou **"Add New"**
3. Sélectionnez **"Deploy without Git"** ou cherchez l'option de drag & drop
4. **Glissez-déposez** tout le dossier `DEV-AGENCY-main` dans la zone
5. Vercel uploadera et déploiera automatiquement

⚠️ **Note** : Cette méthode ne permet pas les mises à jour automatiques via Git.

---

## 📝 Après le Déploiement

### Votre site sera accessible via :
- URL Vercel : `https://votre-projet.vercel.app`
- Vous pouvez ajouter un domaine personnalisé dans les paramètres Vercel

### Mises à jour futures :
- **Avec GitHub** : Faites vos modifications, puis :
  ```bash
  git add .
  git commit -m "Description des changements"
  git push
  ```
  Vercel déploiera automatiquement !

- **Sans GitHub** : Re-déployez manuellement via drag & drop ou CLI

---

## 🔧 Personnalisation du Domaine

1. Dans votre projet Vercel, allez dans **Settings**
2. Cliquez sur **Domains**
3. Ajoutez votre domaine personnalisé
4. Suivez les instructions pour configurer les DNS

---

## ❓ Problèmes Courants

### "Permission denied" lors de l'installation
- Utilisez `sudo npm install -g vercel`
- Ou utilisez la méthode GitHub (pas besoin d'installation)

### Le site ne s'affiche pas correctement
- Vérifiez que `profile.jpg` est bien dans le dossier
- Vérifiez la console du navigateur pour les erreurs

### La vidéo YouTube ne s'affiche pas
- Vérifiez que la vidéo est publique
- Vérifiez votre connexion internet

---

## 📞 Support

- Documentation Vercel : [vercel.com/docs](https://vercel.com/docs)
- Support Vercel : [vercel.com/support](https://vercel.com/support)

---

**🎉 Félicitations ! Votre landing page sera bientôt en ligne !**
