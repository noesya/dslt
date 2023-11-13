---
title: Typographie
weight: 2
---

## Système typographique

Pour que la lecture du contenu du site soit optimale, peu importe la taille de l’écran utilisé, nous divisons nos systèmes typographiques en trois sections : large, medium et extra small.

`Large` correspond à un écran d’une taille supérieure ou égale à 1280px (pour les écrans d'ordinateur).
`Medium` correspond à un écran d’une taille comprise entre la référence large et 768px (pour les tablettes ou les téléphones à l'horizontale).
`Extra small` correspond aux écrans d’une taille inférieure à la référence medium (principalement ceux de téléphones).

### Conventions de nommage

Plutôt que de créer des ensemble de valeurs typographiques correspondant aux utilisations principales (par exemple : h1, h2, lead), il semble plus pérenne de nommer ces ensembles selon les normes typographiques traditionnelles. Ces conventions s’appliquaient en fonction de la hauteur en point d’une police et fournissent des nom spécifiques à chaque taille.

Ces noms existent dans plusieurs langues, dont le français, mais il semble plus cohérent, étant donné que le code est anglophone, de nous fonder sur les noms anglais.

[Source](https://en.wikipedia.org/wiki/Traditional_point-size_names)

### Tailles de police

Les tailles de police ci-dessous sont indiquées en pixels, mais nous les convertissons ensuite en rem, ce qui permet aux utilisateurs et utilisatrices de redimensionner sans problème la taille de la police, en plus de créer d'uniformiser les textes pour chaque contexte d’utilisation.

Pour chaque système typographique, nous indicons la taille de la police et la hauteur de la ligne, de cette façon : `font-size`/`line-height`.

| Dénommination    | Medium    | Extra small  |
| ---------------- | --------- | ------------ |
| Double Canon     | 58/56     | 46/44        |
| Small Canon      | 40/42     | 24/29        |
| Trafalgar        | 32/36     | 20/25        |
| Paragon          | 28/32     | 20/30        |
| Double Pica      | 24/26     | 18/20        |
| Chapo            | 23/23     | 18/25        |
| Body Copy        | 23/32     | 18/25        |
| Pica             | 18/18     |              |
| Long Primer      | 14/18     |              |
| Minion           | 12/16     |              |

## Emploi technique

Afin de pouvoir utiliser nos typographies facilement dans plusieurs contexte de lecture, nous employons du SCSS, à la racine de notre document HTML, pour définir le même ensemble de polices que celui listé dans le tableau ci-dessus, dans un fichier de configuration :

{{< filetree/container >}}
  {{< filetree/folder name="letemps" >}}
    {{< filetree/folder name="configuration" >}}
      {{< filetree/file name="type-sizes.sass" >}}
    {{< /filetree/folder >}}
  {{< /filetree/folder >}}
{{< /filetree/container >}}

```scss {filename="type-sizes.sass"}
:root {
  @include set-type-size('double-canon', (
    'xs': ('font-size': 46, 'line-height': 44),
    'md': ('font-size': 58, 'line-height': 56)
  ));

  @include set-type-size('small-canon', (
    'xs': ('font-size': 24, 'line-height': 29),
    'md': ('font-size': 40, 'line-height': 42)
  ));

  @include set-type-size('trafalgar', (
    'xs': ('font-size': 22, 'line-height': 25),
    'md': ('font-size': 32, 'line-height': 36)
  ));

  @include set-type-size('paragon', (
    'xs': ('font-size': 20, 'line-height': 30),
    'md': ('font-size': 28, 'line-height': 32)
  ));

  @include set-type-size('double-pica', (
    'xs': ('font-size': 18, 'line-height': 20),
    'md': ('font-size': 24, 'line-height': 26)
  ));

  @include set-type-size('chapo', (
    'xs': ('font-size': 18, 'line-height': 25),
    'md': ('font-size': 23, 'line-height': 23)
  ));

  @include set-type-size('body-copy', (
    'xs': ('font-size': 18, 'line-height': 25),
    'md': ('font-size': 22, 'line-height': 32)
  ));

  @include set-type-size('pica', (
    'xs': ('font-size': 18, 'line-height': 24)
  ));

  @include set-type-size('long-primer', (
    'xs': ('font-size': 14, 'line-height': 18)
  ));

  @include set-type-size('minion', (
    'xs': ('font-size': 12, 'line-height': 16)
  ));
}
```

Nous récupérons ces données dans deux mixins SASS :

{{< filetree/container >}}
  {{< filetree/folder name="letemps" >}}
    {{< filetree/folder name="tools" >}}
      {{< filetree/file name="fonts.sass" >}}
    {{< /filetree/folder >}}
  {{< /filetree/folder >}}
{{< /filetree/container >}}

* Le premier va permettre de gérer les breakpoints (donc le changement de taille de police en fonction de la taille de l'écran) et surtout de prendre les différentes valeurs indiquées au-dessus, pour en faire des propriétés CSS.

```scss {filename="fonts.sass"}
@mixin set-type-size($name, $type)
    @each $breakpoint, $settings in $type
      @include media-breakpoint-up($breakpoint)
          @each $property, $value in $settings
              --#{$name}-#{$property}: #{pxToRem($value)}
```

* Le deuxième va quant à lui permettre d'appeler ces propriétés, en faisant le lien entre le mixin `set-type-size` et le fichier `type-sizes.scss`.

```scss {filename="fonts.sass"}
@mixin type-size($name)
  font-size: var(--#{$name}-font-size)
  line-height: var(--#{$name}-line-height)
```

Nous employons ensuite ce mixin aux différents endroits nous intéressant, comme, par exemple, pour définir les tailles du titre de niveau 1 du site :

{{< filetree/container >}}
  {{< filetree/folder name="letemps" >}}
    {{< filetree/folder name="design-system" >}}
      {{< filetree/file name="typography.sass" >}}
    {{< /filetree/folder >}}
  {{< /filetree/folder >}}
{{< /filetree/container >}}

```scss {filename="typography.sass"}
@mixin h1
    font-family: $h1-font-family
    font-weight: $h1-weight
    text-transform: $h1-text-transform
    @include type-size(double-canon)
```

Ici, le mixin `type-size` va checher à l'intérieur du fichier `type-sizes.sass` la valeur de police et de hauteur de ligne (si elle est définie) correspondant au nom (ici "double-canon") qu'on lui passe en paramètre.

Cette méthode permet de gérer directement les différents contextes de visionnage du site, mais aussi de garder un nommage cohérent des différentes tailles de police.

## Exemple d'utilisation

![Exemple : Les typographies sur un article](/images/typography/typo-01.jpg)

Ce qui correspond, dans le style du site (en terme de typographie uniquement), au style du fichier suivant :

{{< filetree/container >}}
  {{< filetree/folder name="letemps" >}}
    {{< filetree/folder name="articles" >}}
      {{< filetree/file name="show.sass" >}}
    {{< /filetree/folder >}}
  {{< /filetree/folder >}}
{{< /filetree/container >}}

```scss {filename="show.sass"}
.articles-show
  .article-header, .article-authors, .article-meta, .article-body
    .lead
      font-family: $lead-font-family
      font-size: $lead-size
      font-weight: $lead-weight
      @include type-size(body-copy)
  .article-meta
    font-family: $meta-font-family
    font-weight: $meta-weight
    @include type-size(minion)
  .article-body
    font-family: $article-body-font-family
    font-weight: $article-body-weight
    @include type-size(body-copy)
  .article-links
    font-family: $article-body-font-family
    font-weight: $article-body-weight
    @include type-size(body-copy)

.article-date
  font-family: $meta-font-family
  font-weight: $meta-weight
  @include type-size(minion)
```

Nous avons ainsi un équilibre entre des variables définies en SASS (`font-family`et `font-weight`) et celles utilisées grâce au mixin `type-size`. Ces deux usages nous permettent d'obtenir un design system cohérent et adaptable en fonction des besoins et des contextes.
