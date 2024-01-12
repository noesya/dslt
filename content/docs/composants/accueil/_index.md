---
title: Accueil
weight: 1
---

## À la une

![](a-la-une.png)

```html {filename="HTML"}
<section class="home-section home-section--featured">
  <h2 class="home-section-title">À la une</h2>
  <ul class="articles is-mobile">...</ul>
  <ul class="articles featured-1">...</ul>
  <ul class="articles featured-2">...</ul>
  <aside class="home-section--aside">...</aside>
  <section class="home-section featured-3">...</section>
</section>
```

### Articles mobile

Non visible en desktop

```html {filename="HTML"}
<ul class="articles is-mobile">
  <li>
    <article class="post ">
      <div class="post__text">
        <h2 class="post__title">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 201.9 220.6" class="icon icon--premium">
            <title>Réservé aux abonnés</title>
            <path
              d="M201.9,57.8H199c-3.9-14.2-23.5-50.7-37.5-52.6a200.32,200.32,0,0,0-24.9-1.3H122.4v194c0,7.1,2.6,12.9,10,16.2,3.9,1.6,20.4,3.9,26.1,4.2v2.3H43.4v-2.3c5.8-.3,22-1.9,26.1-3.5,7.7-2.9,10-9.1,10-16.2V3.9H65.6A204.49,204.49,0,0,0,40.7,5.2C26.8,7.1,6.8,43.6,2.9,57.8H0V0H201.7l.2,57.8">
            </path>
          </svg>
          <a href="/monde/a-guayaquil-en-equateur-nous-souffrons-enormement-ici">A Guayaquil, en Equateur: «Nous
            souffrons énormément ici»</a>
        </h2>
        <div class="post__lead">
          <p>La plus grande ville d’Equateur est aussi l’une des plus violentes, gangrenée par le trafic de drogue
            et les conflits entre gangs locaux</p>
        </div>
      </div>
    </article>
  </li>
</ul>
```

### Articles aside

![](articles-aside.png)

```html {filename="HTML"}
<aside class="home-section--aside">
  <section>
    <h2 class="home-section-title">
      Chroniques
    </h2>
    <ul class="articles">
      <li>
        <article class="post post-opinion">...</article>
      </li>
      <li>
        <article class="post post-opinion">...</article>
      </li>
    </ul>
  </section>
  <section>
    <h2 class="home-section-title">
      Éditorial
    </h2>
    <ul class="articles">
      <li>
        <article class="post post-opinion">...</article>
      </li>
    </ul>
  </section>
  <div id="adnz_halfpage_1" class="aside__adzn" data-adnz-effect-tag="ad:adnz_halfpage_1"></div>
</aside>
```

## Articles featured

```html {filename="HTML"}
<ul class="articles featured-1">
  <li>
    <article class="post ">
      <figure class="post__cover is-16-9" data-ariato="Article.Cover">
        <a title="En un graphique – enneigement et tarif du forfait, où aller skier ce week-end?"
          href="/sport/ski-snowboard/en-un-graphique-enneigement-et-tarif-du-forfait-ou-aller-skier-ce-week-end">
          <picture>
            <source type="image/avif" media="(min-width: 720px)"
              data-srcset="https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/large.avif 1x, https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/giant.avif 2x"
              srcset="https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/large.avif 1x, https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/giant.avif 2x">
            <source type="image/avif" media="(min-width: 480px)"
              data-srcset="https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/medium.avif 1x, https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/large.avif 2x"
              srcset="https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/medium.avif 1x, https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/large.avif 2x">
            <source type="image/avif" media="(min-width: 240px)"
              data-srcset="https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/small.avif 1x, https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/medium.avif 2x"
              srcset="https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/small.avif 1x, https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/medium.avif 2x">
            <source type="image/webp" media="(min-width: 720px)"
              data-srcset="https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/large.webp 1x, https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/giant.webp 2x"
              srcset="https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/large.webp 1x, https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/giant.webp 2x">
            <source type="image/webp" media="(min-width: 480px)"
              data-srcset="https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/medium.webp 1x, https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/large.webp 2x"
              srcset="https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/medium.webp 1x, https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/large.webp 2x">
            <source type="image/webp" media="(min-width: 240px)"
              data-srcset="https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/small.webp 1x, https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/medium.webp 2x"
              srcset="https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/small.webp 1x, https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/medium.webp 2x">
            <source type="image/jpeg" media="(min-width: 720px)"
              data-srcset="https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/large.jpg 1x, https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/giant.jpg 2x"
              srcset="https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/large.jpg 1x, https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/giant.jpg 2x">
            <source type="image/jpeg" media="(min-width: 480px)"
              data-srcset="https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/medium.jpg 1x, https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/large.jpg 2x"
              srcset="https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/medium.jpg 1x, https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/large.jpg 2x">
            <source type="image/jpeg" media="(min-width: 240px)"
              data-srcset="https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/small.jpg 1x, https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/medium.jpg 2x"
              srcset="https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/small.jpg 1x, https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/medium.jpg 2x">
            <img data-src="https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/small"
              class="lazy loaded" alt="© Photo: Jean-Christophe Bott/Keystone. Montage: Le&nbsp;Temps"
              src="https://letemps-17455.kxcdn.com/photos/6a939215-0ac7-489f-b36a-a4c83543d3b2/small"
              data-was-processed="true">
          </picture>
        </a>
        <div class="post__meta">
          <span class="post__category">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512" class="icon icon-infographie">
              <path
                d="m64 32c-35.3 0-64 28.7-64 64v320c0 35.3 28.7 64 64 64h320c35.3 0 64-28.7 64-64v-320c0-35.3-28.7-64-64-64zm64 192c17.7 0 32 14.3 32 32v96c0 17.7-14.3 32-32 32s-32-14.3-32-32v-96c0-17.7 14.3-32 32-32zm64-64c0-17.7 14.3-32 32-32s32 14.3 32 32v192c0 17.7-14.3 32-32 32s-32-14.3-32-32zm128 128c17.7 0 32 14.3 32 32v32c0 17.7-14.3 32-32 32s-32-14.3-32-32v-32c0-17.7 14.3-32 32-32z">
              </path>
            </svg>
          </span>
        </div>
      </figure>
      <h2 class="post__title">
        <a href="/sport/ski-snowboard/en-un-graphique-enneigement-et-tarif-du-forfait-ou-aller-skier-ce-week-end">En
          un graphique – enneigement et tarif du forfait, où aller skier ce week-end?</a>
      </h2>
      <div class="post__author">
        <a href="/profil/duc-quang-nguyen">Duc-Quang Nguyen</a>
      </div>
      <div class="post__lead">
        <p>Avec la neige qui s’est invitée jusqu’en plaine cette semaine en Suisse et des éclaircies prévues ce
          week-end, il est tentant de répondre à l’appel des pistes. Petit pointage de la quantité d’or blanc et du
          prix des forfaits dans différentes stations</p>
      </div>
      <time class="post__publication-date">Publié le 12 janvier 2024 à 13:28. / Modifié le 12 janvier 2024 à
        15:54.</time>
    </article>
  </li>
  <li class="is-desktop">
    <article class="post ">
      <figure class="post__cover is-16-9" data-ariato="Article.Cover">
        <a title="Sarrazin vainqueur, Pinturault blessé: la France des contrastes à Wengen"
          href="/sport/ski-snowboard/sarrazin-vainqueur-pinturault-blesse-la-france-des-contrastes-a-wengen">
          <picture>
            <source type="image/avif" media="(min-width: 240px)"
              data-srcset="https://letemps-17455.kxcdn.com/photos/9f1f5df9-e514-43fc-8632-8e245e72cfce/small.avif 1x, https://letemps-17455.kxcdn.com/photos/9f1f5df9-e514-43fc-8632-8e245e72cfce/small.avif 2x"
              srcset="https://letemps-17455.kxcdn.com/photos/9f1f5df9-e514-43fc-8632-8e245e72cfce/small.avif 1x, https://letemps-17455.kxcdn.com/photos/9f1f5df9-e514-43fc-8632-8e245e72cfce/small.avif 2x">
            <source type="image/webp" media="(min-width: 240px)"
              data-srcset="https://letemps-17455.kxcdn.com/photos/9f1f5df9-e514-43fc-8632-8e245e72cfce/small.webp 1x, https://letemps-17455.kxcdn.com/photos/9f1f5df9-e514-43fc-8632-8e245e72cfce/small.webp 2x"
              srcset="https://letemps-17455.kxcdn.com/photos/9f1f5df9-e514-43fc-8632-8e245e72cfce/small.webp 1x, https://letemps-17455.kxcdn.com/photos/9f1f5df9-e514-43fc-8632-8e245e72cfce/small.webp 2x">
            <source type="image/jpeg" media="(min-width: 240px)"
              data-srcset="https://letemps-17455.kxcdn.com/photos/9f1f5df9-e514-43fc-8632-8e245e72cfce/small.jpg 1x, https://letemps-17455.kxcdn.com/photos/9f1f5df9-e514-43fc-8632-8e245e72cfce/small.jpg 2x"
              srcset="https://letemps-17455.kxcdn.com/photos/9f1f5df9-e514-43fc-8632-8e245e72cfce/small.jpg 1x, https://letemps-17455.kxcdn.com/photos/9f1f5df9-e514-43fc-8632-8e245e72cfce/small.jpg 2x">
            <img data-src="https://letemps-17455.kxcdn.com/photos/9f1f5df9-e514-43fc-8632-8e245e72cfce/small"
              class="lazy loaded"
              alt="Cyprien Sarrazin déboule dans un nuage de neige. — © JEAN-CHRISTOPHE BOTT / keystone-sda.ch"
              src="https://letemps-17455.kxcdn.com/photos/9f1f5df9-e514-43fc-8632-8e245e72cfce/small"
              data-was-processed="true">
          </picture>
        </a>
        <div class="post__meta">
        </div>
      </figure>
      <div class="post__text">
        <h2 class="post__title">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 201.9 220.6" class="icon icon--premium">
            <title>Réservé aux abonnés</title>
            <path
              d="M201.9,57.8H199c-3.9-14.2-23.5-50.7-37.5-52.6a200.32,200.32,0,0,0-24.9-1.3H122.4v194c0,7.1,2.6,12.9,10,16.2,3.9,1.6,20.4,3.9,26.1,4.2v2.3H43.4v-2.3c5.8-.3,22-1.9,26.1-3.5,7.7-2.9,10-9.1,10-16.2V3.9H65.6A204.49,204.49,0,0,0,40.7,5.2C26.8,7.1,6.8,43.6,2.9,57.8H0V0H201.7l.2,57.8">
            </path>
          </svg>
          <a href="/sport/ski-snowboard/sarrazin-vainqueur-pinturault-blesse-la-france-des-contrastes-a-wengen">Sarrazin
            vainqueur, Pinturault blessé: la France des contrastes à Wengen</a>
        </h2>
        <div class="post__author">
          <a href="/profil/lionel-pittet">Lionel Pittet</a>
        </div>
        <div class="post__lead">
          <p>Cyprien Sarrazin a remporté le premier super-G de sa carrière vendredi sur le Lauberhorn, tandis que
            son compatriote Alexis Pinturault devait être évacué en hélicoptère après une lourde chute. La réalité
            de ce sport fait toujours «mal au ventre»</p>
        </div>
      </div>
    </article>
  </li>
  <li class="is-desktop">
    <article class="post ">
      <figure class="post__cover is-16-9" data-ariato="Article.Cover">
        <a title="Christoph Deluze, un air de blouse" href="/culture/musiques/christoph-deluze-un-air-de-blouse">
          <picture>
            <source type="image/avif" media="(min-width: 240px)"
              data-srcset="https://letemps-17455.kxcdn.com/photos/90d995a3-4a9d-4658-969b-7e50e5686fb4/small.avif 1x, https://letemps-17455.kxcdn.com/photos/90d995a3-4a9d-4658-969b-7e50e5686fb4/small.avif 2x"
              srcset="https://letemps-17455.kxcdn.com/photos/90d995a3-4a9d-4658-969b-7e50e5686fb4/small.avif 1x, https://letemps-17455.kxcdn.com/photos/90d995a3-4a9d-4658-969b-7e50e5686fb4/small.avif 2x">
            <source type="image/webp" media="(min-width: 240px)"
              data-srcset="https://letemps-17455.kxcdn.com/photos/90d995a3-4a9d-4658-969b-7e50e5686fb4/small.webp 1x, https://letemps-17455.kxcdn.com/photos/90d995a3-4a9d-4658-969b-7e50e5686fb4/small.webp 2x"
              srcset="https://letemps-17455.kxcdn.com/photos/90d995a3-4a9d-4658-969b-7e50e5686fb4/small.webp 1x, https://letemps-17455.kxcdn.com/photos/90d995a3-4a9d-4658-969b-7e50e5686fb4/small.webp 2x">
            <source type="image/jpeg" media="(min-width: 240px)"
              data-srcset="https://letemps-17455.kxcdn.com/photos/90d995a3-4a9d-4658-969b-7e50e5686fb4/small.jpg 1x, https://letemps-17455.kxcdn.com/photos/90d995a3-4a9d-4658-969b-7e50e5686fb4/small.jpg 2x"
              srcset="https://letemps-17455.kxcdn.com/photos/90d995a3-4a9d-4658-969b-7e50e5686fb4/small.jpg 1x, https://letemps-17455.kxcdn.com/photos/90d995a3-4a9d-4658-969b-7e50e5686fb4/small.jpg 2x">
            <img data-src="https://letemps-17455.kxcdn.com/photos/90d995a3-4a9d-4658-969b-7e50e5686fb4/small"
              class="lazy loaded" alt="Christoph Deluze à Genève, le 17 novembre 2023. — © Eddy Mottaz"
              src="https://letemps-17455.kxcdn.com/photos/90d995a3-4a9d-4658-969b-7e50e5686fb4/small"
              data-was-processed="true">
          </picture>
        </a>
        <div class="post__meta">
        </div>
      </figure>
      <div class="post__text">
        <h2 class="post__title">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 201.9 220.6" class="icon icon--premium">
            <title>Réservé aux abonnés</title>
            <path
              d="M201.9,57.8H199c-3.9-14.2-23.5-50.7-37.5-52.6a200.32,200.32,0,0,0-24.9-1.3H122.4v194c0,7.1,2.6,12.9,10,16.2,3.9,1.6,20.4,3.9,26.1,4.2v2.3H43.4v-2.3c5.8-.3,22-1.9,26.1-3.5,7.7-2.9,10-9.1,10-16.2V3.9H65.6A204.49,204.49,0,0,0,40.7,5.2C26.8,7.1,6.8,43.6,2.9,57.8H0V0H201.7l.2,57.8">
            </path>
          </svg>
          <a href="/culture/musiques/christoph-deluze-un-air-de-blouse">Christoph Deluze, un air de blouse</a>
        </h2>
        <div class="post__author">
          <a href="/profil/christian-lecomte">Christian Lecomte</a>
        </div>
        <div class="post__lead">
          <p>Il est pianiste virtuose et médecin rhumatologue. L’un n’empêche pas l’autre. En concert ou en
            consultation, il dit faire appel à la même rigueur et la même humilité</p>
        </div>
      </div>
    </article>
  </li>
</ul>
```

## Publicité

```html {filename="HTML"}
<div class="featured-ad">
  <div id="adnz_wideboard_2" data-adnz-effect-tag="ad:adnz_wideboard_2"></div>
</div>
```

## Le choix de la rédaction

```html {filename="HTML"}
<section class="home-section featured-4">
  <h2 class="home-section-title">
    Le choix de la rédaction
  </h2>
  <div class="width-limiter">
    <ul class="articles featured-4 articles--boxed">
      <li>
        <article class="post ">
          <figure class="post__cover is-16-9" data-ariato="Article.Cover">
            <a title="«Lolita malgré moi», le remake: la méchanceté n’a pas d’âge"
              href="/culture/ecrans/lolita-malgre-moi-le-remake-la-mechancete-n-a-pas-d-age">
              <picture>
                <source type="image/avif" media="(min-width: 720px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/ba8fa29c-4f0a-47e3-9518-c861d44df90a/large.avif 1x, https://letemps-17455.kxcdn.com/photos/ba8fa29c-4f0a-47e3-9518-c861d44df90a/giant.avif 2x">
                <source type="image/avif" media="(min-width: 480px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/ba8fa29c-4f0a-47e3-9518-c861d44df90a/medium.avif 1x, https://letemps-17455.kxcdn.com/photos/ba8fa29c-4f0a-47e3-9518-c861d44df90a/large.avif 2x">
                <source type="image/avif" media="(min-width: 240px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/ba8fa29c-4f0a-47e3-9518-c861d44df90a/small.avif 1x, https://letemps-17455.kxcdn.com/photos/ba8fa29c-4f0a-47e3-9518-c861d44df90a/medium.avif 2x">
                <source type="image/webp" media="(min-width: 720px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/ba8fa29c-4f0a-47e3-9518-c861d44df90a/large.webp 1x, https://letemps-17455.kxcdn.com/photos/ba8fa29c-4f0a-47e3-9518-c861d44df90a/giant.webp 2x">
                <source type="image/webp" media="(min-width: 480px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/ba8fa29c-4f0a-47e3-9518-c861d44df90a/medium.webp 1x, https://letemps-17455.kxcdn.com/photos/ba8fa29c-4f0a-47e3-9518-c861d44df90a/large.webp 2x">
                <source type="image/webp" media="(min-width: 240px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/ba8fa29c-4f0a-47e3-9518-c861d44df90a/small.webp 1x, https://letemps-17455.kxcdn.com/photos/ba8fa29c-4f0a-47e3-9518-c861d44df90a/medium.webp 2x">
                <source type="image/jpeg" media="(min-width: 720px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/ba8fa29c-4f0a-47e3-9518-c861d44df90a/large.jpg 1x, https://letemps-17455.kxcdn.com/photos/ba8fa29c-4f0a-47e3-9518-c861d44df90a/giant.jpg 2x">
                <source type="image/jpeg" media="(min-width: 480px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/ba8fa29c-4f0a-47e3-9518-c861d44df90a/medium.jpg 1x, https://letemps-17455.kxcdn.com/photos/ba8fa29c-4f0a-47e3-9518-c861d44df90a/large.jpg 2x">
                <source type="image/jpeg" media="(min-width: 240px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/ba8fa29c-4f0a-47e3-9518-c861d44df90a/small.jpg 1x, https://letemps-17455.kxcdn.com/photos/ba8fa29c-4f0a-47e3-9518-c861d44df90a/medium.jpg 2x">
                <img data-src="https://letemps-17455.kxcdn.com/photos/ba8fa29c-4f0a-47e3-9518-c861d44df90a/small"
                  class="lazy" alt="Bebe Wood, Reneé Rapp et Avantika dans «Mean Girls». — © Paramount Pictures">
              </picture>
            </a>
            <div class="post__meta">
            </div>
          </figure>
          <div class="post__text">
            <h2 class="post__title">
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 201.9 220.6" class="icon icon--premium">
                <title>Réservé aux abonnés</title>
                <path
                  d="M201.9,57.8H199c-3.9-14.2-23.5-50.7-37.5-52.6a200.32,200.32,0,0,0-24.9-1.3H122.4v194c0,7.1,2.6,12.9,10,16.2,3.9,1.6,20.4,3.9,26.1,4.2v2.3H43.4v-2.3c5.8-.3,22-1.9,26.1-3.5,7.7-2.9,10-9.1,10-16.2V3.9H65.6A204.49,204.49,0,0,0,40.7,5.2C26.8,7.1,6.8,43.6,2.9,57.8H0V0H201.7l.2,57.8">
                </path>
              </svg>
              <a href="/culture/ecrans/lolita-malgre-moi-le-remake-la-mechancete-n-a-pas-d-age">«Lolita malgré moi»,
                le remake: la méchanceté n’a pas d’âge</a>
            </h2>
            <div class="post__author">
              <a href="/profil/virginie-nussbaum">Virginie Nussbaum</a>
            </div>
            <div class="post__lead">
              <p>Sorti en salle cette semaine avant une mise en ligne prochaine sur Paramount+, la version revisitée
                de «Mean Girls», ce classique de 2004 avec Lindsay Lohan, adapte la recette à la sauce musicale. Le
                classique d’une génération qui n’a étonnamment pas vieilli</p>
            </div>
            <time class="post__publication-date">Publié le 12 janvier 2024 à 10:35. / Modifié le 12 janvier 2024 à
              16:01.</time>
          </div>
        </article>
      </li>
      <li>
        <article class="post ">
          <figure class="post__cover is-16-9" data-ariato="Article.Cover">
            <a title="Quand le consulting cherche à attirer les talents"
              href="/economie/carrieres/quand-le-consulting-cherche-a-attirer-les-talents">
              <picture>
                <source type="image/avif" media="(min-width: 720px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/6e6047f5-8f57-4613-8697-b8b6a4c30c56/large.avif 1x, https://letemps-17455.kxcdn.com/photos/6e6047f5-8f57-4613-8697-b8b6a4c30c56/giant.avif 2x">
                <source type="image/avif" media="(min-width: 480px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/6e6047f5-8f57-4613-8697-b8b6a4c30c56/medium.avif 1x, https://letemps-17455.kxcdn.com/photos/6e6047f5-8f57-4613-8697-b8b6a4c30c56/large.avif 2x">
                <source type="image/avif" media="(min-width: 240px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/6e6047f5-8f57-4613-8697-b8b6a4c30c56/small.avif 1x, https://letemps-17455.kxcdn.com/photos/6e6047f5-8f57-4613-8697-b8b6a4c30c56/medium.avif 2x">
                <source type="image/webp" media="(min-width: 720px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/6e6047f5-8f57-4613-8697-b8b6a4c30c56/large.webp 1x, https://letemps-17455.kxcdn.com/photos/6e6047f5-8f57-4613-8697-b8b6a4c30c56/giant.webp 2x">
                <source type="image/webp" media="(min-width: 480px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/6e6047f5-8f57-4613-8697-b8b6a4c30c56/medium.webp 1x, https://letemps-17455.kxcdn.com/photos/6e6047f5-8f57-4613-8697-b8b6a4c30c56/large.webp 2x">
                <source type="image/webp" media="(min-width: 240px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/6e6047f5-8f57-4613-8697-b8b6a4c30c56/small.webp 1x, https://letemps-17455.kxcdn.com/photos/6e6047f5-8f57-4613-8697-b8b6a4c30c56/medium.webp 2x">
                <source type="image/jpeg" media="(min-width: 720px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/6e6047f5-8f57-4613-8697-b8b6a4c30c56/large.jpg 1x, https://letemps-17455.kxcdn.com/photos/6e6047f5-8f57-4613-8697-b8b6a4c30c56/giant.jpg 2x">
                <source type="image/jpeg" media="(min-width: 480px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/6e6047f5-8f57-4613-8697-b8b6a4c30c56/medium.jpg 1x, https://letemps-17455.kxcdn.com/photos/6e6047f5-8f57-4613-8697-b8b6a4c30c56/large.jpg 2x">
                <source type="image/jpeg" media="(min-width: 240px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/6e6047f5-8f57-4613-8697-b8b6a4c30c56/small.jpg 1x, https://letemps-17455.kxcdn.com/photos/6e6047f5-8f57-4613-8697-b8b6a4c30c56/medium.jpg 2x">
                <img data-src="https://letemps-17455.kxcdn.com/photos/6e6047f5-8f57-4613-8697-b8b6a4c30c56/small"
                  class="lazy"
                  alt="L'entreprise Julhiet Sterwen fonctionne par «communautés» d’expertises. — © Wirestock / Getty Images">
              </picture>
            </a>
            <div class="post__meta">
            </div>
          </figure>
          <div class="post__text">
            <h2 class="post__title">
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 201.9 220.6" class="icon icon--premium">
                <title>Réservé aux abonnés</title>
                <path
                  d="M201.9,57.8H199c-3.9-14.2-23.5-50.7-37.5-52.6a200.32,200.32,0,0,0-24.9-1.3H122.4v194c0,7.1,2.6,12.9,10,16.2,3.9,1.6,20.4,3.9,26.1,4.2v2.3H43.4v-2.3c5.8-.3,22-1.9,26.1-3.5,7.7-2.9,10-9.1,10-16.2V3.9H65.6A204.49,204.49,0,0,0,40.7,5.2C26.8,7.1,6.8,43.6,2.9,57.8H0V0H201.7l.2,57.8">
                </path>
              </svg>
              <a href="/economie/carrieres/quand-le-consulting-cherche-a-attirer-les-talents">Quand le consulting
                cherche à attirer les talents</a>
            </h2>
            <div class="post__author">
              <a href="/profil/julie-eigenmann">Julie Eigenmann</a>
            </div>
            <div class="post__lead">
              <p>La société de conseil Julhiet Sterwen, qui compte un bureau à Nyon, mise sur plusieurs fronts pour
                être attractive: absence d’objectifs financiers, fonctionnement en «communautés» et choix des
                missions. Des modèles toujours plus fréquents</p>
            </div>
            <time class="post__publication-date">Publié le 12 janvier 2024 à 12:30. / Modifié le 12 janvier 2024 à
              16:01.</time>
          </div>
        </article>
      </li>
      <li>
        <article class="post ">
          <figure class="post__cover is-16-9" data-ariato="Article.Cover">
            <a title="Malgré les mesures de protection, les requins font toujours face au risque d’extinction"
              href="/sciences/environnement/malgre-les-mesures-des-requins-toujours-face-au-risque-d-extinction">
              <picture>
                <source type="image/avif" media="(min-width: 720px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/6b09cdc4-6dcd-4994-b917-94fff91cd871/large.avif 1x, https://letemps-17455.kxcdn.com/photos/6b09cdc4-6dcd-4994-b917-94fff91cd871/giant.avif 2x">
                <source type="image/avif" media="(min-width: 480px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/6b09cdc4-6dcd-4994-b917-94fff91cd871/medium.avif 1x, https://letemps-17455.kxcdn.com/photos/6b09cdc4-6dcd-4994-b917-94fff91cd871/large.avif 2x">
                <source type="image/avif" media="(min-width: 240px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/6b09cdc4-6dcd-4994-b917-94fff91cd871/small.avif 1x, https://letemps-17455.kxcdn.com/photos/6b09cdc4-6dcd-4994-b917-94fff91cd871/medium.avif 2x">
                <source type="image/webp" media="(min-width: 720px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/6b09cdc4-6dcd-4994-b917-94fff91cd871/large.webp 1x, https://letemps-17455.kxcdn.com/photos/6b09cdc4-6dcd-4994-b917-94fff91cd871/giant.webp 2x">
                <source type="image/webp" media="(min-width: 480px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/6b09cdc4-6dcd-4994-b917-94fff91cd871/medium.webp 1x, https://letemps-17455.kxcdn.com/photos/6b09cdc4-6dcd-4994-b917-94fff91cd871/large.webp 2x">
                <source type="image/webp" media="(min-width: 240px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/6b09cdc4-6dcd-4994-b917-94fff91cd871/small.webp 1x, https://letemps-17455.kxcdn.com/photos/6b09cdc4-6dcd-4994-b917-94fff91cd871/medium.webp 2x">
                <source type="image/jpeg" media="(min-width: 720px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/6b09cdc4-6dcd-4994-b917-94fff91cd871/large.jpg 1x, https://letemps-17455.kxcdn.com/photos/6b09cdc4-6dcd-4994-b917-94fff91cd871/giant.jpg 2x">
                <source type="image/jpeg" media="(min-width: 480px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/6b09cdc4-6dcd-4994-b917-94fff91cd871/medium.jpg 1x, https://letemps-17455.kxcdn.com/photos/6b09cdc4-6dcd-4994-b917-94fff91cd871/large.jpg 2x">
                <source type="image/jpeg" media="(min-width: 240px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/6b09cdc4-6dcd-4994-b917-94fff91cd871/small.jpg 1x, https://letemps-17455.kxcdn.com/photos/6b09cdc4-6dcd-4994-b917-94fff91cd871/medium.jpg 2x">
                <img data-src="https://letemps-17455.kxcdn.com/photos/6b09cdc4-6dcd-4994-b917-94fff91cd871/small"
                  class="lazy"
                  alt="Un requin-marteau halicorne pris dans un filet maillant. — © Ocean Image Bank/Toby Matthews">
              </picture>
            </a>
            <div class="post__meta">
            </div>
          </figure>
          <div class="post__text">
            <h2 class="post__title">
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 201.9 220.6" class="icon icon--premium">
                <title>Réservé aux abonnés</title>
                <path
                  d="M201.9,57.8H199c-3.9-14.2-23.5-50.7-37.5-52.6a200.32,200.32,0,0,0-24.9-1.3H122.4v194c0,7.1,2.6,12.9,10,16.2,3.9,1.6,20.4,3.9,26.1,4.2v2.3H43.4v-2.3c5.8-.3,22-1.9,26.1-3.5,7.7-2.9,10-9.1,10-16.2V3.9H65.6A204.49,204.49,0,0,0,40.7,5.2C26.8,7.1,6.8,43.6,2.9,57.8H0V0H201.7l.2,57.8">
                </path>
              </svg>
              <a href="/sciences/environnement/malgre-les-mesures-des-requins-toujours-face-au-risque-d-extinction">Malgré
                les mesures de protection, les requins font toujours face au risque d’extinction</a>
            </h2>
            <div class="post__author">
              <a href="/profil/pascaline-minet">Pascaline Minet</a>
            </div>
            <div class="post__lead">
              <p>Une nouvelle étude révèle que la mortalité globale des requins a augmenté au cours de la dernière
                décennie. Les réglementations destinées à prévenir le prélèvement de leurs ailerons ont eu des effets
                pervers. Mais il y a aussi eu des progrès</p>
            </div>
            <time class="post__publication-date">Publié le 12 janvier 2024 à 10:17. / Modifié le 12 janvier 2024 à
              16:01.</time>
          </div>
        </article>
      </li>
      <li>
        <article class="post ">
          <figure class="post__cover is-16-9" data-ariato="Article.Cover">
            <a title="L’Eglise réformée réunit une task force sur la question des abus sexuels"
              href="/suisse/l-eglise-reformee-reunit-une-task-force-sur-la-question-des-abus-sexuels">
              <picture>
                <source type="image/avif" media="(min-width: 720px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/0f2dbf77-440e-4e88-bef5-f64168b6ff53/large.avif 1x, https://letemps-17455.kxcdn.com/photos/0f2dbf77-440e-4e88-bef5-f64168b6ff53/giant.avif 2x">
                <source type="image/avif" media="(min-width: 480px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/0f2dbf77-440e-4e88-bef5-f64168b6ff53/medium.avif 1x, https://letemps-17455.kxcdn.com/photos/0f2dbf77-440e-4e88-bef5-f64168b6ff53/large.avif 2x">
                <source type="image/avif" media="(min-width: 240px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/0f2dbf77-440e-4e88-bef5-f64168b6ff53/small.avif 1x, https://letemps-17455.kxcdn.com/photos/0f2dbf77-440e-4e88-bef5-f64168b6ff53/medium.avif 2x">
                <source type="image/webp" media="(min-width: 720px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/0f2dbf77-440e-4e88-bef5-f64168b6ff53/large.webp 1x, https://letemps-17455.kxcdn.com/photos/0f2dbf77-440e-4e88-bef5-f64168b6ff53/giant.webp 2x">
                <source type="image/webp" media="(min-width: 480px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/0f2dbf77-440e-4e88-bef5-f64168b6ff53/medium.webp 1x, https://letemps-17455.kxcdn.com/photos/0f2dbf77-440e-4e88-bef5-f64168b6ff53/large.webp 2x">
                <source type="image/webp" media="(min-width: 240px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/0f2dbf77-440e-4e88-bef5-f64168b6ff53/small.webp 1x, https://letemps-17455.kxcdn.com/photos/0f2dbf77-440e-4e88-bef5-f64168b6ff53/medium.webp 2x">
                <source type="image/jpeg" media="(min-width: 720px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/0f2dbf77-440e-4e88-bef5-f64168b6ff53/large.jpg 1x, https://letemps-17455.kxcdn.com/photos/0f2dbf77-440e-4e88-bef5-f64168b6ff53/giant.jpg 2x">
                <source type="image/jpeg" media="(min-width: 480px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/0f2dbf77-440e-4e88-bef5-f64168b6ff53/medium.jpg 1x, https://letemps-17455.kxcdn.com/photos/0f2dbf77-440e-4e88-bef5-f64168b6ff53/large.jpg 2x">
                <source type="image/jpeg" media="(min-width: 240px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/0f2dbf77-440e-4e88-bef5-f64168b6ff53/small.jpg 1x, https://letemps-17455.kxcdn.com/photos/0f2dbf77-440e-4e88-bef5-f64168b6ff53/medium.jpg 2x">
                <img data-src="https://letemps-17455.kxcdn.com/photos/0f2dbf77-440e-4e88-bef5-f64168b6ff53/small"
                  class="lazy" alt="Rita Famos, en juin 2018. — © Ennio Leanza/Keystone">
              </picture>
            </a>
            <div class="post__meta">
            </div>
          </figure>
          <div class="post__text">
            <h2 class="post__title">
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 201.9 220.6" class="icon icon--premium">
                <title>Réservé aux abonnés</title>
                <path
                  d="M201.9,57.8H199c-3.9-14.2-23.5-50.7-37.5-52.6a200.32,200.32,0,0,0-24.9-1.3H122.4v194c0,7.1,2.6,12.9,10,16.2,3.9,1.6,20.4,3.9,26.1,4.2v2.3H43.4v-2.3c5.8-.3,22-1.9,26.1-3.5,7.7-2.9,10-9.1,10-16.2V3.9H65.6A204.49,204.49,0,0,0,40.7,5.2C26.8,7.1,6.8,43.6,2.9,57.8H0V0H201.7l.2,57.8">
                </path>
              </svg>
              <a href="/suisse/l-eglise-reformee-reunit-une-task-force-sur-la-question-des-abus-sexuels">L’Eglise
                réformée réunit une task force sur la question des abus sexuels</a>
            </h2>
            <div class="post__author">
              <a href="/profil/lucas-vuilleumier-protestinfo">Lucas Vuilleumier (Protestinfo)</a>
            </div>
            <div class="post__lead">
              <p>En amont de la publication des résultats de l’Eglise protestante allemande (EKD) portant sur les cas
                d’abus en son sein, l’Eglise réformée suisse (EERS) réunit&nbsp;les représentants des différentes
                Eglises cantonales en task force</p>
            </div>
            <time class="post__publication-date">Publié le 12 janvier 2024 à 09:25. / Modifié le 12 janvier 2024 à
              16:01.</time>
          </div>
        </article>
      </li>
    </ul>
  </div>
</section>
```

## Flux

```html {filename="HTML"}
<section class="home-section home-section--flux home-section--teasers teasers--3">
  <h2 class="home-section-title">
    Dry January
  </h2>
  <div class="width-limiter">
    <ul class="articles">
      <li>
        <article class="post ">
          <figure class="post__cover is-16-9" data-ariato="Article.Cover">
            <a title="Le boom des alternatives à l’alcool, la bière 0% en tête"
              href="/societe/le-boom-des-alternatives-a-l-alcool-la-biere-0-en-tete">
              <picture>
                <source type="image/avif" media="(min-width: 720px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/d9aba915-4d09-44fe-87cb-cc60bc56b0b0/large.avif 1x, https://letemps-17455.kxcdn.com/photos/d9aba915-4d09-44fe-87cb-cc60bc56b0b0/giant.avif 2x">
                <source type="image/avif" media="(min-width: 480px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/d9aba915-4d09-44fe-87cb-cc60bc56b0b0/medium.avif 1x, https://letemps-17455.kxcdn.com/photos/d9aba915-4d09-44fe-87cb-cc60bc56b0b0/large.avif 2x">
                <source type="image/avif" media="(min-width: 240px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/d9aba915-4d09-44fe-87cb-cc60bc56b0b0/small.avif 1x, https://letemps-17455.kxcdn.com/photos/d9aba915-4d09-44fe-87cb-cc60bc56b0b0/medium.avif 2x">
                <source type="image/webp" media="(min-width: 720px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/d9aba915-4d09-44fe-87cb-cc60bc56b0b0/large.webp 1x, https://letemps-17455.kxcdn.com/photos/d9aba915-4d09-44fe-87cb-cc60bc56b0b0/giant.webp 2x">
                <source type="image/webp" media="(min-width: 480px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/d9aba915-4d09-44fe-87cb-cc60bc56b0b0/medium.webp 1x, https://letemps-17455.kxcdn.com/photos/d9aba915-4d09-44fe-87cb-cc60bc56b0b0/large.webp 2x">
                <source type="image/webp" media="(min-width: 240px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/d9aba915-4d09-44fe-87cb-cc60bc56b0b0/small.webp 1x, https://letemps-17455.kxcdn.com/photos/d9aba915-4d09-44fe-87cb-cc60bc56b0b0/medium.webp 2x">
                <source type="image/jpeg" media="(min-width: 720px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/d9aba915-4d09-44fe-87cb-cc60bc56b0b0/large.jpg 1x, https://letemps-17455.kxcdn.com/photos/d9aba915-4d09-44fe-87cb-cc60bc56b0b0/giant.jpg 2x">
                <source type="image/jpeg" media="(min-width: 480px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/d9aba915-4d09-44fe-87cb-cc60bc56b0b0/medium.jpg 1x, https://letemps-17455.kxcdn.com/photos/d9aba915-4d09-44fe-87cb-cc60bc56b0b0/large.jpg 2x">
                <source type="image/jpeg" media="(min-width: 240px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/d9aba915-4d09-44fe-87cb-cc60bc56b0b0/small.jpg 1x, https://letemps-17455.kxcdn.com/photos/d9aba915-4d09-44fe-87cb-cc60bc56b0b0/medium.jpg 2x">
                <img data-src="https://letemps-17455.kxcdn.com/photos/d9aba915-4d09-44fe-87cb-cc60bc56b0b0/small"
                  class="lazy"
                  alt="La production de bière sans alcool a augmenté de 5,3% durant l’année brassicole 2022-2023 en Suisse. — © Tobias Schwarz / AFP Photo">
              </picture>
            </a>
            <div class="post__meta">
            </div>
          </figure>
          <div class="post__text">
            <h2 class="post__title">
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 201.9 220.6" class="icon icon--premium">
                <title>Réservé aux abonnés</title>
                <path
                  d="M201.9,57.8H199c-3.9-14.2-23.5-50.7-37.5-52.6a200.32,200.32,0,0,0-24.9-1.3H122.4v194c0,7.1,2.6,12.9,10,16.2,3.9,1.6,20.4,3.9,26.1,4.2v2.3H43.4v-2.3c5.8-.3,22-1.9,26.1-3.5,7.7-2.9,10-9.1,10-16.2V3.9H65.6A204.49,204.49,0,0,0,40.7,5.2C26.8,7.1,6.8,43.6,2.9,57.8H0V0H201.7l.2,57.8">
                </path>
              </svg>
              <a href="/societe/le-boom-des-alternatives-a-l-alcool-la-biere-0-en-tete">Le boom des alternatives à
                l’alcool, la bière 0% en tête</a>
            </h2>
            <div class="post__author">
              <a href="/profil/julie-eigenmann">Julie Eigenmann</a>
            </div>
            <div class="post__lead">
              <p>Alors que certains s’apprêtent à entamer un «Dry January», la part de la bière sans alcool sur
                l’ensemble du marché a atteint 6% sur l’année brassicole 2022-2023. Le vin et d’autres substituts
                suivent le même chemin, même s’ils sont moins aboutis et que l’offre est moins importante</p>
            </div>
            <time class="post__publication-date">Publié le 01 janvier 2024 à 18:55. / Modifié le 11 janvier 2024 à
              18:30.</time>
          </div>
        </article>
      </li>
      <li>
        <article class="post ">
          <figure class="post__cover is-16-9" data-ariato="Article.Cover">
            <a title="Dans la vie de Catherine, brillante scientifique le jour, alcoolique la nuit"
              href="/podcasts/brise-glace/vie-catherine-brillante-scientifique-jour-alcoolique-nuit">
              <picture>
                <source type="image/avif" media="(min-width: 720px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/dfd00d4f-74d9-41b3-9f8b-f945886ba214/large.avif 1x, https://letemps-17455.kxcdn.com/photos/dfd00d4f-74d9-41b3-9f8b-f945886ba214/giant.avif 2x">
                <source type="image/avif" media="(min-width: 480px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/dfd00d4f-74d9-41b3-9f8b-f945886ba214/medium.avif 1x, https://letemps-17455.kxcdn.com/photos/dfd00d4f-74d9-41b3-9f8b-f945886ba214/large.avif 2x">
                <source type="image/avif" media="(min-width: 240px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/dfd00d4f-74d9-41b3-9f8b-f945886ba214/small.avif 1x, https://letemps-17455.kxcdn.com/photos/dfd00d4f-74d9-41b3-9f8b-f945886ba214/medium.avif 2x">
                <source type="image/webp" media="(min-width: 720px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/dfd00d4f-74d9-41b3-9f8b-f945886ba214/large.webp 1x, https://letemps-17455.kxcdn.com/photos/dfd00d4f-74d9-41b3-9f8b-f945886ba214/giant.webp 2x">
                <source type="image/webp" media="(min-width: 480px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/dfd00d4f-74d9-41b3-9f8b-f945886ba214/medium.webp 1x, https://letemps-17455.kxcdn.com/photos/dfd00d4f-74d9-41b3-9f8b-f945886ba214/large.webp 2x">
                <source type="image/webp" media="(min-width: 240px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/dfd00d4f-74d9-41b3-9f8b-f945886ba214/small.webp 1x, https://letemps-17455.kxcdn.com/photos/dfd00d4f-74d9-41b3-9f8b-f945886ba214/medium.webp 2x">
                <source type="image/jpeg" media="(min-width: 720px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/dfd00d4f-74d9-41b3-9f8b-f945886ba214/large.jpg 1x, https://letemps-17455.kxcdn.com/photos/dfd00d4f-74d9-41b3-9f8b-f945886ba214/giant.jpg 2x">
                <source type="image/jpeg" media="(min-width: 480px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/dfd00d4f-74d9-41b3-9f8b-f945886ba214/medium.jpg 1x, https://letemps-17455.kxcdn.com/photos/dfd00d4f-74d9-41b3-9f8b-f945886ba214/large.jpg 2x">
                <source type="image/jpeg" media="(min-width: 240px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/dfd00d4f-74d9-41b3-9f8b-f945886ba214/small.jpg 1x, https://letemps-17455.kxcdn.com/photos/dfd00d4f-74d9-41b3-9f8b-f945886ba214/medium.jpg 2x">
                <img data-src="https://letemps-17455.kxcdn.com/photos/dfd00d4f-74d9-41b3-9f8b-f945886ba214/small"
                  class="lazy" alt="">
              </picture>
            </a>
            <div class="post__meta">
              <span class="post__category">
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512" class="icon">
                  <path
                    d="m319.4 372c48.5-31.3 80.6-85.9 80.6-148 0-97.2-78.8-176-176-176s-176 78.8-176 176c0 62.1 32.1 116.6 80.6 148 1.2 17.3 4 38 7.2 57.1l.2 1c-80-34.3-136-113.6-136-206.1 0-123.7 100.3-224 224-224s224 100.3 224 224c0 92.5-56 171.9-136 206.1l.2-1.1c3.1-19.2 6-39.8 7.2-57zm-2.3-38.1c-1.6-5.7-3.9-11.1-7-16.2-5.8-9.7-13.5-17-21.9-22.4 19.5-17.6 31.8-43 31.8-71.3 0-53-43-96-96-96s-96 43-96 96c0 28.3 12.3 53.8 31.8 71.3-8.4 5.4-16.1 12.7-21.9 22.4-3.1 5.1-5.4 10.5-7 16.2-31.1-26.4-50.9-65.9-50.9-109.9 0-79.5 64.5-144 144-144s144 64.5 144 144c0 44-19.8 83.5-50.9 109.9zm-93.1-21.9c32.9 0 64 8.6 64 43.8 0 33-12.9 104.1-20.6 132.9-5.1 19-24.5 23.4-43.4 23.4s-38.2-4.4-43.4-23.4c-7.8-28.5-20.6-99.7-20.6-132.8 0-35.1 31.1-43.8 64-43.8zm0-144a56 56 0 1 1 0 112 56 56 0 1 1 0-112z">
                  </path>
                </svg>
              </span>
            </div>
          </figure>
          <div class="post__text">
            <h2 class="post__title">
              <a href="/podcasts/brise-glace/vie-catherine-brillante-scientifique-jour-alcoolique-nuit">Dans la vie de
                Catherine, brillante scientifique le jour, alcoolique la nuit</a>
            </h2>
            <div class="post__author">
              <div class="authors-list"><a href="/profil/celia-heron">Célia Héron</a>, <a
                  href="/profil/virginie-nussbaum">Virginie Nussbaum</a></div>
            </div>
            <div class="post__lead">
              <p>Tout a commencé, ado, avec un verre de vin blanc bu cul sec. Au fil des années et des alcools,
                l'engrenage a emmené Catherine tout près de la noyade. Une double vie de brillante scientifique le
                jour, et d'alcoolique la nuit, qu'elle raconte au micro de «Brise Glace»</p>
            </div>
            <time class="post__publication-date">Publié le 31 juillet 2020 à 11:24. / Modifié le 11 janvier 2024 à
              18:30.</time>
          </div>
        </article>
      </li>
      <li>
        <article class="post ">
          <figure class="post__cover is-16-9" data-ariato="Article.Cover">
            <a title="Quel vin pour son Dry January?" href="/opinions/chroniques/quel-vin-pour-son-dry-january">
              <picture>
                <source type="image/avif" media="(min-width: 720px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/cbbcdc29-acd1-4173-9396-016aef1aad67/large.avif 1x, https://letemps-17455.kxcdn.com/photos/cbbcdc29-acd1-4173-9396-016aef1aad67/giant.avif 2x">
                <source type="image/avif" media="(min-width: 480px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/cbbcdc29-acd1-4173-9396-016aef1aad67/medium.avif 1x, https://letemps-17455.kxcdn.com/photos/cbbcdc29-acd1-4173-9396-016aef1aad67/large.avif 2x">
                <source type="image/avif" media="(min-width: 240px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/cbbcdc29-acd1-4173-9396-016aef1aad67/small.avif 1x, https://letemps-17455.kxcdn.com/photos/cbbcdc29-acd1-4173-9396-016aef1aad67/medium.avif 2x">
                <source type="image/webp" media="(min-width: 720px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/cbbcdc29-acd1-4173-9396-016aef1aad67/large.webp 1x, https://letemps-17455.kxcdn.com/photos/cbbcdc29-acd1-4173-9396-016aef1aad67/giant.webp 2x">
                <source type="image/webp" media="(min-width: 480px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/cbbcdc29-acd1-4173-9396-016aef1aad67/medium.webp 1x, https://letemps-17455.kxcdn.com/photos/cbbcdc29-acd1-4173-9396-016aef1aad67/large.webp 2x">
                <source type="image/webp" media="(min-width: 240px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/cbbcdc29-acd1-4173-9396-016aef1aad67/small.webp 1x, https://letemps-17455.kxcdn.com/photos/cbbcdc29-acd1-4173-9396-016aef1aad67/medium.webp 2x">
                <source type="image/jpeg" media="(min-width: 720px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/cbbcdc29-acd1-4173-9396-016aef1aad67/large.jpg 1x, https://letemps-17455.kxcdn.com/photos/cbbcdc29-acd1-4173-9396-016aef1aad67/giant.jpg 2x">
                <source type="image/jpeg" media="(min-width: 480px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/cbbcdc29-acd1-4173-9396-016aef1aad67/medium.jpg 1x, https://letemps-17455.kxcdn.com/photos/cbbcdc29-acd1-4173-9396-016aef1aad67/large.jpg 2x">
                <source type="image/jpeg" media="(min-width: 240px)"
                  data-srcset="https://letemps-17455.kxcdn.com/photos/cbbcdc29-acd1-4173-9396-016aef1aad67/small.jpg 1x, https://letemps-17455.kxcdn.com/photos/cbbcdc29-acd1-4173-9396-016aef1aad67/medium.jpg 2x">
                <img data-src="https://letemps-17455.kxcdn.com/photos/cbbcdc29-acd1-4173-9396-016aef1aad67/small"
                  class="lazy" alt="Illustration originale. — © Hector de La Vallée pour Le&nbsp;Temps">
              </picture>
            </a>
            <div class="post__meta">
            </div>
          </figure>
          <div class="post__text">
            <h2 class="post__title">
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 201.9 220.6" class="icon icon--premium">
                <title>Réservé aux abonnés</title>
                <path
                  d="M201.9,57.8H199c-3.9-14.2-23.5-50.7-37.5-52.6a200.32,200.32,0,0,0-24.9-1.3H122.4v194c0,7.1,2.6,12.9,10,16.2,3.9,1.6,20.4,3.9,26.1,4.2v2.3H43.4v-2.3c5.8-.3,22-1.9,26.1-3.5,7.7-2.9,10-9.1,10-16.2V3.9H65.6A204.49,204.49,0,0,0,40.7,5.2C26.8,7.1,6.8,43.6,2.9,57.8H0V0H201.7l.2,57.8">
                </path>
              </svg>
              <a href="/opinions/chroniques/quel-vin-pour-son-dry-january">Quel vin pour son Dry January?</a>
            </h2>
            <div class="post__author">
              <a href="/profil/gregoire-baur">Grégoire Baur</a>
            </div>
            <div class="post__lead">
              <p>Peut-être êtes-vous en train de réaliser le défi du moins de janvier sans alcool. Et – toujours
                peut-être – la dégustation d’une bonne bouteille de vin vous manque. Pas de souci! On a la solution
              </p>
            </div>
            <time class="post__publication-date">Publié le 06 janvier 2024 à 10:10. / Modifié le 11 janvier 2024 à
              18:30.</time>
          </div>
        </article>
      </li>
    </ul>
  </div>
</section>
```

## Articles les plus lus

```html {filename="HTML"}
<section class="home-section home-section--most-read">
  <header class="home-section__header">
    <h2 class="home-section-title">
      Articles les plus lus
    </h2>
  </header>
  <div class="width-limiter">
    <ol class="articles">
      <li>
        <article class="post ">
          <div class="post__text">
            <h2 class="post__title">
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 201.9 220.6" class="icon icon--premium">
                <title>Réservé aux abonnés</title>
                <path
                  d="M201.9,57.8H199c-3.9-14.2-23.5-50.7-37.5-52.6a200.32,200.32,0,0,0-24.9-1.3H122.4v194c0,7.1,2.6,12.9,10,16.2,3.9,1.6,20.4,3.9,26.1,4.2v2.3H43.4v-2.3c5.8-.3,22-1.9,26.1-3.5,7.7-2.9,10-9.1,10-16.2V3.9H65.6A204.49,204.49,0,0,0,40.7,5.2C26.8,7.1,6.8,43.6,2.9,57.8H0V0H201.7l.2,57.8">
                </path>
              </svg>
              <a href="/sciences/une-vaste-civilisation-amazonienne-devoilee-par-les-yeux-percants-d-un-laser">Une
                vaste civilisation amazonienne dévoilée par les yeux perçants d’un laser</a>
            </h2>
          </div>
        </article>
      </li>
      <li>
        <article class="post ">
          <div class="post__text">
            <h2 class="post__title">
              <a href="/societe/gastronomie-vins/a-carouge-un-nouveau-repaire-pour-les-amateurs-de-viande">A Carouge,
                un nouveau repaire pour les amateurs de viande</a>
            </h2>
          </div>
        </article>
      </li>
      <li>
        <article class="post ">
          <div class="post__text">
            <h2 class="post__title">
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 201.9 220.6" class="icon icon--premium">
                <title>Réservé aux abonnés</title>
                <path
                  d="M201.9,57.8H199c-3.9-14.2-23.5-50.7-37.5-52.6a200.32,200.32,0,0,0-24.9-1.3H122.4v194c0,7.1,2.6,12.9,10,16.2,3.9,1.6,20.4,3.9,26.1,4.2v2.3H43.4v-2.3c5.8-.3,22-1.9,26.1-3.5,7.7-2.9,10-9.1,10-16.2V3.9H65.6A204.49,204.49,0,0,0,40.7,5.2C26.8,7.1,6.8,43.6,2.9,57.8H0V0H201.7l.2,57.8">
                </path>
              </svg>
              <a
                href="/monde/europe/en-france-rachida-dati-est-la-principale-surprise-du-nouveau-gouvernement-attal-qui-penche-a-droite">En
                France, Rachida Dati est la principale surprise du nouveau gouvernement Attal, qui penche à droite</a>
            </h2>
          </div>
        </article>
      </li>
      <li>
        <article class="post ">
          <div class="post__text">
            <h2 class="post__title">
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 201.9 220.6" class="icon icon--premium">
                <title>Réservé aux abonnés</title>
                <path
                  d="M201.9,57.8H199c-3.9-14.2-23.5-50.7-37.5-52.6a200.32,200.32,0,0,0-24.9-1.3H122.4v194c0,7.1,2.6,12.9,10,16.2,3.9,1.6,20.4,3.9,26.1,4.2v2.3H43.4v-2.3c5.8-.3,22-1.9,26.1-3.5,7.7-2.9,10-9.1,10-16.2V3.9H65.6A204.49,204.49,0,0,0,40.7,5.2C26.8,7.1,6.8,43.6,2.9,57.8H0V0H201.7l.2,57.8">
                </path>
              </svg>
              <a href="/economie/personne-meme-amazon-ne-resiste-face-a-l-expansion-de-digitec-galaxus">Personne, même
                Amazon, ne résiste face à l’expansion de Digitec Galaxus</a>
            </h2>
          </div>
        </article>
      </li>
      <li>
        <article class="post ">
          <div class="post__text">
            <h2 class="post__title">
              <a href="/sciences/des-enigmes-mathematiques-pour-entrer-dans-2024-avec-l-esprit-aiguise">Des énigmes
                mathématiques pour entrer dans 2024 avec l’esprit aiguisé</a>
            </h2>
          </div>
        </article>
      </li>
      <li>
        <article class="post ">
          <div class="post__text">
            <h2 class="post__title">
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 201.9 220.6" class="icon icon--premium">
                <title>Réservé aux abonnés</title>
                <path
                  d="M201.9,57.8H199c-3.9-14.2-23.5-50.7-37.5-52.6a200.32,200.32,0,0,0-24.9-1.3H122.4v194c0,7.1,2.6,12.9,10,16.2,3.9,1.6,20.4,3.9,26.1,4.2v2.3H43.4v-2.3c5.8-.3,22-1.9,26.1-3.5,7.7-2.9,10-9.1,10-16.2V3.9H65.6A204.49,204.49,0,0,0,40.7,5.2C26.8,7.1,6.8,43.6,2.9,57.8H0V0H201.7l.2,57.8">
                </path>
              </svg>
              <a href="/culture/ecrans/corbeaux-et-corneilles-hommage-a-nos-noirs-compagnons-ailes">«Corbeaux et
                corneilles», hommage à nos noirs compagnons ailés</a>
            </h2>
          </div>
        </article>
      </li>
      <li>
        <article class="post ">
          <div class="post__text">
            <h2 class="post__title">
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 201.9 220.6" class="icon icon--premium">
                <title>Réservé aux abonnés</title>
                <path
                  d="M201.9,57.8H199c-3.9-14.2-23.5-50.7-37.5-52.6a200.32,200.32,0,0,0-24.9-1.3H122.4v194c0,7.1,2.6,12.9,10,16.2,3.9,1.6,20.4,3.9,26.1,4.2v2.3H43.4v-2.3c5.8-.3,22-1.9,26.1-3.5,7.7-2.9,10-9.1,10-16.2V3.9H65.6A204.49,204.49,0,0,0,40.7,5.2C26.8,7.1,6.8,43.6,2.9,57.8H0V0H201.7l.2,57.8">
                </path>
              </svg>
              <a href="/societe/comment-le-porno-banalise-la-violence-et-detruit-l-amour">Comment le porno banalise la
                violence et détruit l’amour</a>
            </h2>
          </div>
        </article>
      </li>
      <li>
        <article class="post ">
          <div class="post__text">
            <h2 class="post__title">
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 201.9 220.6" class="icon icon--premium">
                <title>Réservé aux abonnés</title>
                <path
                  d="M201.9,57.8H199c-3.9-14.2-23.5-50.7-37.5-52.6a200.32,200.32,0,0,0-24.9-1.3H122.4v194c0,7.1,2.6,12.9,10,16.2,3.9,1.6,20.4,3.9,26.1,4.2v2.3H43.4v-2.3c5.8-.3,22-1.9,26.1-3.5,7.7-2.9,10-9.1,10-16.2V3.9H65.6A204.49,204.49,0,0,0,40.7,5.2C26.8,7.1,6.8,43.6,2.9,57.8H0V0H201.7l.2,57.8">
                </path>
              </svg>
              <a href="/suisse/vaud/l-udc-vaud-appelle-a-refuser-la-13e-rente-avs">L’UDC Vaud appelle à refuser la 13e
                rente AVS</a>
            </h2>
          </div>
        </article>
      </li>
    </ol>
  </div>
</section>
```