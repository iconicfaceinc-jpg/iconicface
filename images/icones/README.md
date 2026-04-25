# 🎨 Icônes des prestations

Dépose tes images ici avec exactement ces noms de fichier :

| Fichier                          | Prestation            |
|----------------------------------|-----------------------|
| `extensions-classique.png`       | Extensions classique  |
| `extensions-mixte.png`           | Extensions mixte      |
| `volume-russe.png`               | Volume russe          |
| `lash-lift.png`                  | Lash lift + teinture  |
| `brow-lift.png`                  | Brow lift             |
| `brow-lift-teinture.png`         | Brow lift + teinture  |

## Format recommandé
- Format : PNG avec fond transparent
- Taille : 200×200px ou 400×400px (carré)
- Les images sur fond lavande violet arrondi que tu as déjà sont parfaites !

## Comment activer
Dans `index.html`, dans chaque `.prestation-icon`, remplace la ligne de commentaire :

**Avant (emoji) :**
```html
<div class="prestation-icon">
  <!-- Remplace par : <img src="images/icones/extensions-classique.png" alt=""> -->
  🪶
</div>
```

**Après (image) :**
```html
<div class="prestation-icon">
  <img src="images/icones/extensions-classique.png" alt="">
</div>
```

## Pour le favicon (icône onglet navigateur)
Dépose un fichier `favicon.png` directement dans `images/`
- Taille : 512×512px (PNG carré)
- Le cercle violet "if" que tu as est parfait !
