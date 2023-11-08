---
title: Grille
weight: 3
---

## Pourquoi une grille ?

Une grille en design interactif, souvent appelée "grille de mise en page" ou "grille de conception", est un élément clé de la conception web et de l'interface utilisateur. Elle sert de structure de base pour organiser et disposer les éléments d'une page web de manière cohérente.

### Structure visuelle cohérente
Une grille permet de créer une structure visuelle cohérente sur un site web. Cela signifie que les éléments tels que les en-têtes, les menus, le contenu principal et les pieds de page sont placés de manière prévisible, ce qui facilite la navigation pour les utilisateurs. Une structure cohérente aide également à renforcer la marque et l'identité visuelle d'un site.

[Source](https://bootcamp.uxdesign.cc/the-power-of-the-8pt-grid-system-in-design-1c9dbc683ad8)

### Alignement précis
Une grille permet d'aligner précisément les éléments sur la page, garantissant que les espacements, les marges et les dimensions sont uniformes. Cela crée une esthétique propre et professionnelle, ce qui améliore l'expérience utilisateur.

[Source](https://bootcamp.uxdesign.cc/the-importance-of-grid-systems-in-ui-ux-design-enhancing-user-experience-ff7d0a90b08e)

### Flexibilité responsive

Les grilles sont essentielles pour concevoir des sites web réactifs, qui s'adaptent à différents appareils et tailles d'écran. Une grille responsive permet de réorganiser les éléments de la page de manière à ce qu'ils s'ajustent automatiquement pour offrir une expérience optimale sur les ordinateurs de bureau, les tablettes et les smartphones.

[Source](https://www.smashingmagazine.com/2020/01/understanding-css-grid-container/)

### Hiérarchie de l'information

Une grille aide à définir la hiérarchie de l'information sur une page web. Les éléments importants peuvent être placés plus en évidence, tandis que les éléments moins importants peuvent être relégués vers le bas de la page. Cela guide l'attention des utilisateurs et améliore la lisibilité.

[Source](https://www.smashingmagazine.com/2017/12/building-better-ui-designs-layout-grids/)

### Conformité aux normes de conception

Les grilles sont conformes aux normes de conception web et d'accessibilité, ce qui signifie qu'elles contribuent à rendre un site plus convivial pour tous les utilisateurs, y compris ceux ayant des besoins spécifiques.

[Source](https://www.w3.org/TR/css-grid-1/)

### Conclusion

En résumé, une grille en design interactif est un outil fondamental pour créer des designs web esthétiquement agréables, cohérents et fonctionnels. Elle facilite la conception, l'alignement et l'adaptabilité tout en améliorant l'expérience de l'utilisateur. Les sources que j'ai fournies vous donneront davantage d'informations sur ces concepts et leur application.


## La grille du DSLT

### Design

![Grille de 12 colonnes](/images/grille/grille.png)

### Balisage HTML 

```html {filename="HTML"}
<div class="container grid">
  <div>Une première colonne<div>
  <div>Une deuxième colonne<div>
  ...
</div>
```

### Feuilles de styles

{{< filetree/container >}}
  {{< filetree/folder name="letemps" >}}
    {{< filetree/folder name="tools" >}}
      {{< filetree/file name="functions.sass" >}}
      {{< filetree/file name="mixins.sass" >}}
    {{< /filetree/folder >}}
  {{< /filetree/folder >}}
{{< /filetree/container >}}

```scss {filename="mixins.sass"}
@mixin grid($cols: 12, $gap-y: $grid-gutter, $gap-x: $grid-gutter)
    word-break: break-word
    display: grid
    grid-gap: $gap-y $gap-x
    grid-template-columns: repeat($cols, 1fr)
```

```scss {filename="functions.sass"}
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

