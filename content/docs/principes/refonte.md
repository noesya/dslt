---
title: Refonte 2024
weight: 1
---

## Vues

### Imbrications
Structure de fichiers (multiples inclusions de partiels, nommage, ...)
2 exemples d’inclusions multiple

### Répétitions
multiples répétitions (manque de “composants”) 
2 exemples

## DOM

### A11y
Menu - role aria menuitem faux sur tous les liens de liste de navigation
Menu - role aria "none" faut sur tous les list item de liste de navigation
Menu - Bouton de validation de la recherche caché et sans aria label (indétectable par un lecteur d'écran)
Menu - Mauvaise compréhension des rôles ARIA menu, menuitem et separator sur des éléments de navigation, ce qui contredit complétement l'information réel pour un lecteur d'écran
Menu - aria-label="secondary" --> le lecteur d'écran va lire "Secondary"

### Optimisations
- plan de la homepage
- plan de page article ?
- SVG inlines
- sections 
- balisage en “series” pour la page folder

## CSS

### Calculs 

Voilà un exemple de calcul de taille typographique pour un teaser.
![](refonte/css-titre.png)
Et voilà la pile de styles qui s'applique :
![](refonte/css-style.png)

```css {filename="CSS"}
font-size: calc(var(--font-size-110) * var(--font-serif-scale));
```

Voilà les valeurs des variables ci-dessus :
```css {filename="CSS"}
--font-size-110: calc(var(--font-size-100) * var(--ratio));
--font-size-100: calc(var(--font-size-90) * var(--ratio));
--font-size-90: calc(var(--font-size-80) * var(--ratio));
--font-size-80: calc(var(--font-size-70) * var(--ratio));
--font-size-70: calc(var(--font-size-60) * var(--ratio));
--font-size-60: calc(var(--font-size-50) * var(--ratio));
--font-size-50: 1rem;
--font-serif-scale: 1;
--ratio: 1.125;
```

{{< callout type="error" >}}La taille en desktop est de 40.5457px.{{< /callout >}}
{{< callout type="error" >}}Cette taille est le produit de 7 multiplications en cascade.{{< /callout >}}
{{< callout type="error" >}}7 directives CSS sont empilées, dont 3 s'appuient sur le même type de calculs.{{< /callout >}}

{{< callout type="info" >}}
L'échelle modulaire ne correspond ni à un besoin graphique ni à un besoin technique, il suffit de l'enlever pour tout simplifier.
{{< /callout >}}


### Cloisonnements