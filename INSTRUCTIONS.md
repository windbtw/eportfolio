# Guide de mise à jour du Portfolio

Voici comment ajouter tes propres fichiers (images, CVs) et liens vidéos.

## 1. Ajouter les CVs (PDF)

1.  Place tes fichiers PDF (ex: `cv-francais.pdf`, `cv-english.pdf`) dans le dossier :
    `d:\CODING\PERSO\portfolio\assets\docs\`
    *(J'ai créé ce dossier pour toi)*

2.  Ouvre le fichier `career.html`.
3.  Cherche la section "Resumes" (vers la ligne 44).
4.  Remplace le `#` par le chemin de ton fichier.

**Exemple :**
```html
<!-- Avant -->
<a href="#" class="btn">... Download Resume (French)</a>

<!-- Après -->
<a href="assets/docs/cv-francais.pdf" class="btn" target="_blank">... Download Resume (French)</a>
```

## 2. Ajouter la Vidéo YouTube

1.  Va sur ta vidéo YouTube.
2.  Clique sur **Partager** -> **Intégrer** (Embed).
3.  Copie tout le code qui commence par `<iframe ...`.
4.  Ouvre le fichier `career.html`.
5.  Cherche la section "Video Introduction" (vers la ligne 33).
6.  Remplace tout le bloc `<div ...> ... Video Placeholder ... </div>` par ton code iframe.

**Astuce :** Pour que la vidéo soit responsive, garde mon `div class="video-container"` et mets l'iframe dedans.

```html
<div class="video-container" ...>
    <!-- Colle ton iframe ici -->
    <iframe width="560" height="315" src="https://www.youtube.com/embed/TON_ID_VIDEO" ...></iframe>
</div>
```

## 3. Ajouter les Images (Hobbies)

1.  Place tes photos (ex: `figurine1.jpg`) dans le dossier :
    `d:\CODING\PERSO\portfolio\assets\images\`

2.  Ouvre le fichier `hobbies.html`.
3.  Cherche la "Gallery Grid" (vers la ligne 45).
4.  Remplace les `div` placeholders par des balises `img`.

**Exemple :**
```html
<!-- Avant -->
<div style="...">Image 1</div>

<!-- Après -->
<img src="assets/images/figurine1.jpg" alt="Description de la figurine" style="width: 100%; border-radius: 8px;">
```

## 4. Ajouter une photo de profil (Accueil)

1.  Mets ta photo (ex: `profile.jpg`) dans `assets/images/`.
2.  Ouvre `index.html`.
3.  Dans la section "Welcome", tu peux ajouter l'image à côté du texte.

```html
<div class="content-wrapper">
    <div class="text-content">...</div>
    
    <!-- Ajoute ceci -->
    <div class="image-content">
        <img src="assets/images/profile.jpg" alt="Martin Cornillad" style="max-width: 300px; border-radius: 50%;">
    </div>
</div>
```
