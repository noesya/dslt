---
title: Architecture
weight: 1
---

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


