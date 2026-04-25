# 📸 Photos résultats

Dépose tes photos avant/après ici.

## Format recommandé
- Format : JPG ou WebP
- Ratio : 4:5 (portrait) → ex: 800x1000px
- Poids : < 500 Ko par photo (compresse sur squoosh.app)

## Nommage suggéré
- extensions-01.jpg
- extensions-02.jpg
- volume-russe-01.jpg
- lash-lift-01.jpg
- brow-lift-01.jpg

## Comment les afficher sur le site
Dans index.html, remplace un bloc `result-card-placeholder` par :

```html
<div class="result-card">
  <img src="images/resultats/extensions-01.jpg" alt="Extensions cils">
  <div class="result-tag">Extensions</div>
</div>
```
