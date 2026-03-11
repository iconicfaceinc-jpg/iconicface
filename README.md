# Iconic Face — Site Web

## Structure du projet

```
iconicface/
├── index.html           ← Page principale
├── extensions.html      ← Page détail Extensions de Cils
├── lash-brow.html       ← Page détail Lash Lift & Brow Lift
├── README.md            ← Ce fichier
└── images/
    ├── extensions-cils.png   ← Photo panneau Extensions
    ├── lash-brow.png         ← Photo panneau Lash Lift / Brow Lift
    ├── hero-video.mp4        ← Votre vidéo hero (à ajouter)
    └── iconic_face_logo.svg
```

---

## 🎬 Ajouter votre GIF ou vidéo dans le hero

### Option A — GIF

1. Placez votre fichier `.gif` dans le dossier `images/`
2. Dans `index.html`, trouvez cette ligne :
   ```html
   <div class="hero-dark"></div>
   ```
3. Ajoutez juste au-dessus :
   ```html
   <img class="hero-bg" src="images/votre-fichier.gif" alt="">
   ```
4. Supprimez la ligne `<div class="hero-dark"></div>`

---

### Option B — Vidéo (recommandé pour un résultat pro)

1. Préparez votre vidéo selon les specs ci-dessous
2. Placez-la dans `images/` et nommez-la `hero-video.mp4`
3. Dans `index.html`, trouvez cette ligne :
   ```html
   <div class="hero-dark"></div>
   ```
4. Remplacez-la par :
   ```html
   <video class="hero-bg" autoplay muted loop playsinline>
     <source src="images/hero-video.mp4" type="video/mp4">
   </video>
   ```

---

## 📐 Spécifications vidéo recommandées

| Paramètre     | Valeur recommandée                        |
|---------------|-------------------------------------------|
| Format        | MP4 (H.264, profil Baseline ou Main)      |
| Résolution    | 1920×1080 (Full HD) minimum               |
| Durée         | 10 à 30 secondes                          |
| Audio         | ❌ Aucun — supprimer impérativement       |
| Taille        | < 10 Mo (idéal), 20 Mo maximum            |
| FPS           | 24 ou 30 fps                              |
| Orientation   | Paysage (horizontal)                      |

> ⚠️ La vidéo DOIT être sans audio.
> Les navigateurs (Chrome, Safari) bloquent l'autoplay si une piste audio est détectée,
> même si le volume est à 0. Supprimez la piste audio à l'export.

---

## 🛠️ Supprimer l'audio avec un logiciel gratuit

### Avec HandBrake (gratuit, Mac/Windows/Linux)
1. Téléchargez HandBrake : https://handbrake.fr
2. Ouvrez votre vidéo
3. Dans l'onglet **Audio** → supprimez toutes les pistes
4. Dans l'onglet **Video** → choisissez H.264, qualité RF 28
5. Exportez en MP4

### Avec iMovie (Mac)
1. Importez votre vidéo
2. Clic droit sur le clip → **Détacher l'audio**
3. Supprimez la piste audio
4. Exportez en MP4 (Fichier → Partager → Fichier)

### Avec CapCut (mobile ou PC, gratuit)
1. Importez votre vidéo
2. Sélectionnez le clip → **Volume → 0**
3. Exportez — puis utilisez HandBrake pour supprimer
   définitivement la piste audio si nécessaire

### En ligne de commande (FFmpeg)
```bash
ffmpeg -i votre-video.mp4 -an -vcodec libx264 -profile:v baseline \
  -movflags +faststart -crf 28 hero-video.mp4
```

---

## 🔗 Liens à remplacer dans le code

Recherchez `https://share.google/kGYSKSPBKWj8OxEda` dans tous les fichiers HTML
et remplacez par votre lien Google My Business.

---

## 🚀 Déploiement

Le site est prêt pour Vercel, Netlify, ou tout hébergeur statique.
Uploadez simplement le dossier `iconicface/` complet.
