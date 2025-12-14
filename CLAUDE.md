# Archive 44 Cours Charlemagne

Site web artistique présentant un appartement virtuel avec animations et interactions.

## Structure du projet

```
├── index.html          # Page d'accueil avec animations parallax
├── apropos.html        # Page à propos
├── chambre.html        # Galerie 3D avec images flottantes
├── cuisine.html        # Page cuisine avec scroll horizontal
├── atelier.html        # Page atelier avec boîtes d'info interactives
├── floorplan.html      # Navigation plan d'étage
└── style/
    ├── mobile-common.css    # Styles mobiles globaux
    ├── style_index.css
    ├── style_apropos.css
    ├── style_chambre.css
    ├── style_cuisine.css
    ├── style_atelier.css
    └── style_floorplan.css
```

## Travail en cours

Adaptation mobile du site - refonte complète avec conservation des animations.

### Ce qui a été fait

- Réactivation des animations sur mobile (suppression du bloc qui les désactivait)
- Correction des overflow horizontaux (`100vw` → `100%`)
- Désimbrication des media queries dans style_index.css
- Amélioration des zones tactiles (min 44px)
- Buildings en pleine hauteur avec animation sur la page d'accueil
- Fix du `transform: translateZ(0)` global qui cassait `position: fixed`

### Points d'attention

- Ne pas utiliser `transform` sur les parents d'éléments `position: fixed` (casse le comportement fixed)
- Breakpoints utilisés : 768px et 480px
- Les animations sont conservées sur mobile (choix utilisateur)

## Conventions

- Committer uniquement les fichiers modifiés
- Messages de commit en français
