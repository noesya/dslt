---
title: Article - Teasers
---

## Analyse

Il y a une trentaine d'affichage différents pour les teasers. Une grande variété de taille de titres, et des informations optionnelles à afficher.

Actuellement il y a au moins 17 fichiers partiels pour gérer ces différents affichages. À notes que certains sont simplement des "passe-plats"

```rb {filename="articles/templates/podcast/_preview.html.erb"}
<!-- defaults to defaults template -->
<%= render "articles/templates/default/preview", article: article %>
```

## Article commun

### Titre 41/40 avec image, auteur et chapô

![](image-2.png)

### Titre 28/32 avec chapô

![](image.png)

### Titre 23/24 avec chapô

![](image-1.png)

### Titre 20/24 avec chevron

![](image-3.png)

### Titre 23/24 avec image, auteur et chapô

![](image-4.png)

### Titre 23/24 avec auteur mis en avant

![](image-5.png)

### Titre 23/24 avec image et catégorie

![](image-6.png)

### Titre 23/24 avec image, auteur et chapô

![](image-7.png)

### Titre 25/28 avec image et auteur

![](image-8.png)

### Titre 28/32 avec image, auteur et chapô

![](image-11.png)

### Titre 23/24 mode classement

![](image-9.png)

### Titre 20/24 mode classement

![Alt text](image-27.png)

### Titre 25/28 avec image

![](image-10.png)

### Titre 23/28

![](image-12.png)

### Titre 46/44 avec image, chapô et date

![](image-23.png)

### Titre 20/24 avec image, chapô et date

![](image-24.png)

### Titre 23/24 avec image et date

![Alt text](image-25.png)

### Titre 23/24 avec image, heure et chapô

![Alt text](image-26.png)

### Titre 23/24 avec image, auteur, chapô et date

![Alt text](image-28.png)

## Article Podcast

### Grand teaser accueil

![](image-13.png)

### Grand teaser index

![](image-14.png)

### Teaser grille

![](image-15.png)

### Teaser liste

![](image-18.png)

### Série simple

![](image-16.png)

### Série petit format

![](image-17.png)

## Article Vidéo

### Vidéo très grand teaser

![](image-21.png)

### Vidéo grand teaser

![](image-19.png)

### Vidéo teaser grille

![](image-22.png)

### Vidéo teaser liste

![](image-20.png)



## Actuellement : des partiels très proches avec quelques variations

```html {filename="articles/templates/default/_preview.html.erb"}
<% article_title ||= article.title %>
<% cache article do %>
  <article class="post <%= sponsor_html_classes(article) %>">
    <% if article.photo %>
      <figure class="post__cover is-16-9" data-ariato="Article.Cover">
        <%= link_to article_canonical_path(article), title: article_title do %>
          <picture>
            <%= render 'articles/photo_sources_large', photo: article.photo %>
            <img data-src="<%= small_photo_cdn_url(article.photo) %>" class="lazy" alt="<%= article.photo_caption if article.photo_caption.present? %>" />
          </picture>
        <% end %>
        <div class="post__meta">
          <%= render '/articles/post_genre_icon', article: article %>
        </div>
      </figure>
    <% end %>
    <div class="post__text">
      <%= render "articles/sponsors_small", sponsors: article.sponsors.commercial %>
      <h2 class="post__title">
        <% if article.is_active_live? %>
          <span class="post--live"><%= t("lives.article_label") %></span>
        <% elsif !article.photo %>
          <%= render '/articles/post_genre_icon', article: article %>
        <% end %>
        <% if !article.free %>
          <%= render 'articles/premium' %>
        <% end %>
        <%= link_to article_title, article_canonical_path(article) %>
      </h2>

      <%= render "articles/authors_list", article: article %>

      <% if article.description? %>
        <div class="post__lead"><%= markdown article.description %></div>
      <% end %>
      <time class="post__publication-date"><%= format_article_date article %></time>
      <%= render "articles/sponsors_small", sponsors: article.sponsors.not_commercial %>
    </div>
  </article>
<% end %>
```

```html {filename="articles/templates/default/_preview_small.html.erb"}
<!-- 2 differences with _preview: larger images + lead -->
<% cache article do %>
  <article class="post <%= sponsor_html_classes(article) %>">
    <% if article.photo %>
      <figure class="post__cover is-16-9" data-ariato="Article.Cover">
        <%= link_to article_canonical_path(article) do %>
          <picture>
            <%= render 'articles/photo_sources_small', photo: article.photo %>
            <img data-src="<%= small_photo_cdn_url(article.photo) %>" class="lazy" alt="<%= article.photo_caption if article.photo_caption.present? %>" />
          </picture>
        <% end %>
        <div class="post__meta">
          <%= render '/articles/post_genre_icon', article: article %>
        </div>
      </figure>
    <% end %>
    <div class="post__text">
      <%= render "articles/sponsors_small", sponsors: article.sponsors.commercial %>
      <h2 class="post__title">
        <% if article.is_active_live? %>
          <span class="post--live"><%= t("lives.article_label") %></span>
        <% elsif !article.photo %>
          <%= render '/articles/post_genre_icon', article: article %>
        <% end %>
        <% if !article.free %>
          <%= render 'articles/premium' %>
        <% end %>
        <%= link_to article.title, article_canonical_path(article) %>
      </h2>

      <%= render "articles/authors_list", article: article %>   
      <time class="post__publication-date"><%= format_article_date article %></time>
      <%= render "articles/sponsors_small", sponsors: article.sponsors.not_commercial %>
    </div>
  </article>
<% end %>
```

```html {filename="articles/templates/default/_preview_dated.html.erb"}
<% cache article do %>
  <article class="post post-dated <%= sponsor_html_classes(article) %>">
    <aside>
      <time class="post__publication-date">
        <%= article.publication_date.to_s(:time) %>
      </time>
    </aside>
    <% if article.photo %>
      
      <figure class="post__cover is-16-9" data-ariato="Article.Cover">
        <%= link_to article_canonical_path(article) do %>
          <picture>
            <%= render 'articles/photo_sources_mini', photo: article.photo %>
            <img data-src="<%= small_photo_cdn_url(article.photo) %>" class="lazy" alt="<%= article.photo_caption if article.photo_caption.present? %>" />
          </picture>
        <% end %>
        <div class="post__meta">
          <%= render '/articles/post_genre_icon', article: article %>
        </div>
      </figure>
    <% end %>
    <div class="post__text">
      <%= render "articles/sponsors_small", sponsors: article.sponsors.commercial %>
      <h2 class="post__title">
        <% if article.is_active_live? %>
          <span class="post--live"><%= t("lives.article_label") %></span>
        <% elsif !article.photo %>
          <%= render '/articles/post_genre_icon', article: article %>
        <% end %>
        <% if !article.free %>
          <%= render 'articles/premium' %>
        <% end %>
        <%= link_to article.title, article_canonical_path(article) %>
      </h2>
      <% if article.description? %>
        <div class="post__lead"><%= markdown article.description %></div>
      <% end %>      
      <%= render "articles/sponsors_small", sponsors: article.sponsors.not_commercial %>
    </div>
  </article>
<% end %>
```

## Solution

“Un partiel pour les gouverner tous.“

```html {filename="app/views/sites/letemps/articles/_teaser.html.erb"}
<% hide_image ||= false %>
<% hide_description ||= false %>
<% show_date ||= false %>
<% show_time ||= false %>
<% show_authors ||= false %>
<% show_category ||= false %>

<% item_class = article.free ? "" : "article-item--premium" %>

<article class="article-item <%= item_class %>">

  <h3><%= link_to article, article_canonical_path(article) %></h3>

  <% if show_date %>
    <time class="article-item__date" datetime="<%= article.publication_date %>"><%= format_article_date article %></time>
  <% end %>

  <% if show_time %>
    <time class="article-item__date" datetime="<%= article.publication_date %>"><%= article.publication_date.to_s(:time) %></time>
  <% end %>

  <% if show_category && article.category %>
    <div class="article-item__category">
      <%= link_to article.category, url_for_category(article.category) %>
    </div>
  <% end %>

  <% if show_authors %>
    <%= render "articles/authors_list", article: article %>
  <% end %>

  <% if !hide_description && article.description %>
    <div class="article-item__description"><%= markdown article.description %></div>
  <% end %>

  <% if !hide_image && article.photo %>
    <figure>
      <picture>
        <%= render 'articles/photo_sources', photo: article.photo %>
        <img src="<%= medium_photo_cdn_url(article.photo) %>" class="lazy" alt="<%= article.photo_caption if article.photo_caption.present? %>" />
      </picture>
    </figure>
  <% end %>

</article>
```

### Utilisation 

```html
<%= render 'articles/article', 
    article: block.article,
    hide_description: true,
    hide_image: true,
    show_authors: true,
    show_category: true,
    show_date: true,
    show_time: true,
    %>
```
