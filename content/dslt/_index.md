---
title: L'ensemble Spyri 
layout: hextra-home
---

<div class="mt-6 mb-6">
{{< hextra/hero-headline >}}
  Du système au site configuré.
{{< /hextra/hero-headline >}}
</div>

<div class="mt-6"></div>

{{< hextra/feature-grid >}}
  {{< hextra/feature-card
    title="Système"
    subtitle="Les fondations et la philosophie de l'écosystème Spyri."
    class="aspect-auto md:aspect-[1.1/1] max-md:min-h-[340px]"
    imageClass="top-[40%] left-[24px] w-[180%] sm:w-[110%] dark:opacity-80"
    style="background: radial-gradient(ellipse at 50% 80%,rgba(194,97,254,0.15),hsla(0,0%,100%,0));"
  >}}
  {{< hextra/feature-card
    title="Le Temps"
    subtitle="Les particularités du site du Temps."
    class="aspect-auto md:aspect-[1.1/1] max-lg:min-h-[340px]"
    imageClass="top-[40%] left-[36px] w-[180%] sm:w-[110%] dark:opacity-80"
    style="background: radial-gradient(ellipse at 50% 80%,rgba(142,53,74,0.15),hsla(0,0%,100%,0));"
  >}}
  {{< hextra/feature-card
    title="Thème"
    subtitle="Le thème par défaut des sites de l'écosystème Spyri."
    class="aspect-auto md:aspect-[1.1/1] max-md:min-h-[340px]"
    imageClass="top-[40%] left-[36px] w-[110%] sm:w-[110%] dark:opacity-80"
    style="background: radial-gradient(ellipse at 50% 80%,rgba(221,210,59,0.15),hsla(0,0%,100%,0));"
  >}}
{{< /hextra/feature-grid >}}

## Architecture

### DSLT (core system)

Les grandes règles et utilitaires CSS : 
- Grilles
- Typographique
- Couleurs sémantiques
- Gestion des icônes
- Breakpoints
- Espacements (4px)
- Composants

### Thèmes

#### Sans thème Spyri
Approche pertinente s'il n'y a pas beaucoup de spécificités communes entre les 3 sites Heidi, Kometa et Geneva, au-dessus du DSLT.

```mermaid
graph TD;
    DSLT-->LT(Le Temps);
    DSLT-->Heidi;
    DSLT-->Kometa;
    DSLT-->Geneva;
    LT-->letemps.ch;
    LT-->LTs(Autres sites Le Temps);
```

#### Avec thème Spyri
Approche pertinente s'il y a un ensemble de spécificités à ajouter au DSLT et à utiliser dans les 3 sites Heidi, Kometa et Geneva.

```mermaid
graph TD;
    DSLT-->LT(Le Temps);
    DSLT-->Spyri;
    Spyri-->Heidi;
    Spyri-->Kometa;
    Spyri-->Geneva;
    LT-->letemps.ch;
    LT-->LTs(Autres sites Le Temps);
```

## Arborescence 

### HTML


### CSS



## Ressources

- L'intégralité du design est disponible et visible sur [Figma](https://www.figma.com/file/TCIWZid2yVpz05VOt72Azq/DSLT?type=design&node-id=0%3A1&mode=design&t=m5UbnUNG4ewQNNdc-1).