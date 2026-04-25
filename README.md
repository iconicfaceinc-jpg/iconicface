# 🐰 Iconic Face — Site Web

Site mobile-first prêt pour Vercel.

---

## 📁 Structure du projet

```
iconic-face/
├── index.html          ← Page principale (tout le contenu est ici)
├── vercel.json         ← Config déploiement Vercel
├── images/
│   ├── logo.png        ← Logo Iconic Face (remplace ce fichier)
│   ├── favicon.svg     ← Icône onglet navigateur
│   └── resultats/      ← 📸 Dossier photos avant/après
│       ├── extensions-01.jpg
│       ├── volume-russe-01.jpg
│       ├── lash-lift-01.jpg
│       └── ...
```

---

## ✏️ Modifier le contenu

### Changer les tarifs
Ouvre `index.html` et cherche le commentaire :
```
<!-- Ajouter / modifier les prestations ici -->
```
Modifie les valeurs dans les `.prestation-card`.

### Ajouter des photos résultats
1. Dépose tes photos dans `images/resultats/`
2. Dans `index.html`, remplace les blocs `result-card-placeholder` par :
```html
<div class="result-card">
  <img src="images/resultats/extensions-01.jpg" alt="Extensions cils avant après">
  <div class="result-tag">Extensions</div>
</div>
```

### Ajouter des avis clients
Cherche le commentaire :
```
<!-- Ajouter d'autres avis en copiant un bloc .avis-card -->
```
Et copie-colle un nouveau bloc `avis-card`.

### Changer le lien Google Reviews
Cherche `VOTRE_ID_GOOGLE_MAPS` dans index.html et remplace par ton vrai lien Google Maps reviews.

---

## 🚀 Déployer sur Vercel

1. Va sur [vercel.com](https://vercel.com) → New Project
2. Importe depuis GitHub (ou glisse le dossier en drag & drop)
3. Framework Preset → **Other**
4. Deploy ✅

---

## 📞 Contact WhatsApp
Lien : `https://wa.me/33767508332`
Pour modifier le message pré-rempli, cherche `text=` dans les liens WhatsApp et modifie le texte (encodé URL).
