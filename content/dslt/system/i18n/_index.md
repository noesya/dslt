---
title: i18n
weight: 3
---

## Traduction

Architecture :

L'architecture des fichiers de traductions est symétrique à l'architecture des fichiers des modèles. On ajoute à cette symétrie un fichier admin pour l'espace d'administration.

{{< filetree/container >}}
  {{< filetree/folder name="config" >}}
    {{< filetree/folder name="locales" >}}
      {{< filetree/folder name="fr" >}}
        {{< filetree/folder name="article" >}}
          {{< filetree/file name="article" >}}
        {{< /filetree/folder >}}

        {{< filetree/file name="admin.yml" >}}

        {{< filetree/file name="article.yml" >}}

        {{< filetree/folder name="sites" >}}
          {{< filetree/file name="letemps.yml" >}}
          {{< filetree/file name="heidi.yml" >}}
          {{< filetree/file name="kometa.yml" >}}
        {{< /filetree/folder >}}
      {{< /filetree/folder >}}
    {{< /filetree/folder >}}
  {{< /filetree/folder >}}
{{< /filetree/container >}}

Les clés à l'intérieur des fichiers sont ordonnées par ordre alphabétique.

```yaml {filename="article.yml"}
fr:
  activerecord:
    attributes:
      article:
        authors: Auteurs
        body: Corps
        cover_embed_url: Embed de couverture
        description: Chapô
        event_location: Lieu de l'événement
```

