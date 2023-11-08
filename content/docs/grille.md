---
title: Grille
weight: 3
---

## 12 colonnes 

![Grille de 12 colonnes](/images/grille/grille.png)

```html {filename="HTML"}
<div class="container grid">
  <div>Une première colonne<div>
  <div>Une deuxième colonne<div>
  ...
</div>
```

```sass {filename="mixins.sass"}
@mixin grid($cols: 12, $gap-y: $grid-gutter, $gap-x: $grid-gutter)
    word-break: break-word
    display: grid
    grid-gap: $gap-y $gap-x
    grid-template-columns: repeat($cols, 1fr)
```


```sass {filename="functions.sass"}
// This must be used for content inside columns
@function col($quantity, $base: 12)
    $quantity-on-base: $quantity / $base * 12
    $width: calc( (100% + #{$grid-gutter}) / 12 * #{$quantity-on-base} - #{$grid-gutter} )
    @return #{$width}

// This must be used for offset, outside columns
@function offset($quantity, $base: 12)
    $quantity-on-base: $quantity / $base * 12
    $width: calc( (100% + #{$grid-gutter}) / 12 * #{$quantity-on-base} )
    @return #{$width}
```



## Unités d'espacement

Les unités d'espacement sont un moyen simple d'appliquer des dimensions d'espacement prédéfinies aux interfaces. L'utilisation d'unités d'espacement permet de créer des interfaces plus cohérentes et de simplifier la prise de décision concernant les marges et le remplissage, comme pour l'application des tailles de caractères.

Les développeurs définissent l'espace en unités rem (racine em). 1 rem équivaut normalement à 16px. Les unités rem sont particulièrement utiles pour maintenir des normes d'accessibilité élevées, car les sites web codés avec des unités rem seront compatibles avec le redimensionnement du texte dans les navigateurs. Les unités d'espacement sont très utiles car elles permettent aux concepteurs et aux développeurs de parler le même langage tout en valorisant la langue maternelle de chaque discipline, c'est-à-dire les pixels pour un concepteur et les unités rem pour un développeur.

