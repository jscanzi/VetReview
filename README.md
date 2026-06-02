# vetReview — Landing Page

Landing page pour vetReview, solution de gestion des avis Google pour vétérinaires et groupements de cliniques.

## Structure

```
vetreview/
├── index.html                  # Page principale
├── assets/
│   ├── logo.svg                # Logo vetReview (SVG)
│   ├── images/
│   │   ├── google-reviews-logo.png   # Logo Google Reviews
│   │   └── laptop-network.png        # Photo section groupements
│   └── screens/                # Screenshots carousel
│       ├── tableau-de-bord.jpg
│       ├── reponse-ia.jpg
│       ├── mentions-equipe.jpg
│       ├── comparateur.jpg
│       └── dashboard-reseau.jpg
└── README.md
```

## Dépendances externes (CDN)

- **Fonts** : Inter + DM Sans via Google Fonts
- **Icônes** : Hugeicons stroke-rounded via `cdn.hugeicons.com`
- **Photo hero** : Unsplash (à remplacer par une photo propriétaire)

## Remplacer la photo hero

Dans `index.html`, chercher `.hero-bg` dans le CSS et remplacer :

```css
background-image: url('https://images.unsplash.com/...');
/* → */
background-image: url('assets/images/photo-hero.jpg');
```

## Intégrer le lien Tol.d

Dans `index.html`, chercher `VOTRE_LIEN_TOLD` (2 occurrences : nav + section contact) et remplacer par l'URL de ton formulaire.

## Lancer en local

Ouvrir `index.html` directement dans un navigateur, ou via un serveur local :

```bash
npx serve .
# ou
python3 -m http.server 8080
```
