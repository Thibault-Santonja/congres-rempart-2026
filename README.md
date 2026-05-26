# Congrès REMPART, 60ᵉ Anniversaire

Site officiel du **Congrès REMPART 60ᵉ Anniversaire**, organisé par
l'**AMVCC** (Association de Mise en Valeur du Château de Coucy) du
**23 au 25 mai 2026** à **Coucy-le-Château-Auffrique** (Aisne).

🌐 **En ligne :** <https://thibault-santonja.github.io/congres-rempart-2026/>

---

## Structure

Site statique HTML/CSS/JS vanille, déployé sur GitHub Pages.

| Page | Contenu |
|------|---------|
| `index.html` | Accueil : carrousel photo + navigation |
| `timeline.html` | Planning détaillé (gantt desktop, vertical mobile) |
| `menu.html` | Menus des trois repas du week-end |
| `contact.html` | Trombinoscope des organisateurs + référente |
| `credits.html` | Remerciements aux associations et partenaires |
| `map.html` | Carte régionale + plan de Coucy (toggle plan/stylisé) |
| `album.html` | Galerie photo (lightbox) |
| `planning.html` | Version A4 paysage du planning (source du PDF) |

## Dossiers

```
assets/
├── css/style.css       Palette Seigneurie + classes partagées
└── photos/             30 WebP optimisées (1920px, q82)

.github/workflows/
└── build-pdf.yml       CI Puppeteer : génère planning.pdf à chaque
                        push de planning.html
```

## Outils & technos

- HTML/CSS/JS vanille : aucun framework
- Polices : Fraunces (titres) + Lato (corps), Google Fonts
- Palette « Seigneurie » : garance `#8b2a1a`, or `#b8892e`, parchemin
  `#faf5ee`, pierre, encre
- SVG inline pour les cartes (Picardie + plan de Coucy)
- Schema.org JSON-LD (Event, WebPage, ImageGallery, BreadcrumbList)

## Déploiement

GitHub Pages depuis la branche `main`. Chaque push redéploie
automatiquement.

Le workflow `build-pdf.yml` régénère `planning.pdf` lorsque
`planning.html` est modifié.

## Droits

- **Photographies** : © Thibault Santonja
  ([thibaultsan.com](https://thibaultsan.com)), voir
  [`NOTICE-PHOTOS.md`](NOTICE-PHOTOS.md). Reproduction interdite sans
  autorisation écrite.
- **Contenu rédactionnel & code** : © 2026 AMVCC.

## Crédits

- Conception et photographies : **Thibault Santonja**
- Organisation : **AMVCC** et bénévoles du congrès
- Union nationale : [REMPART](https://www.rempart.com/fr)
- Partenaires : APPEVA, ASPAM, Abbaye de Valsery, AROEVEN, Les Corbacs
  du Nord (musique)

## Contact

Référente du congrès : **Adeline Kadri**, `adeline.kadri@amvcc.com`
- 03 23 52 69 41
