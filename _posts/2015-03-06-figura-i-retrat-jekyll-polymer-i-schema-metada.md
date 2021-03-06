---
comments: true
date: 2015-03-06 11:48:19
og: true
og-type: article
layout: blog
slug: "figura-i-retrat-jekyll-polymer-i-schema-metada"
title: "Figura i retrat. Jekyll, Polymer i Schema metadata"
categories: 
  - comunicació
  - treballs
  - "no-cita"
tags: "case-study" 
class: blog-article
"featured-img": true
"featured-img-url": "figura-i-retrat-case-study.png"
meta: "Figura i retrat. Jekyy, Polymer i Schema metadata"
excerpt: "Per què és vol el retrat?. S’ha dit que el retrat és el substitut i/o el record de la presència de l’absent."
author: oxygen
published: true
keywords: "artinpocket, screens, digital, collection, polymer, restful, api, service, worker"
---

>Per què és vol el retrat?. S’ha dit que el retrat és el substitut i/o el record de la presència de l’absent: amb el retrat es vol que l’absent, el recordat, sigui present.<footer>&mdash; <cite><a href="{{ page.url }}" title="{{ page.title }}">Arnau Puig</a></cite></footer>

## La Fundació Iluro

La [Fundació Iluro](http://www.fundacioiluro.cat/) té una remarcable col·lecció de pintura, escultura, dibuix i gravat que configura el seu fons artístic. El Patronat de la Fundació té clar que fer-lo accessible al públic ha de ser una de les seves prioritats.

És en aquest sentit que s'emmarca **el nou web de l'exposició Figura i Retrat**.

### Figura i Retrat

[figurairetrat.fundacioiluro.cat](http://figurairetrat.fundacioiluro.cat/ "L'exposició “La figura i el retrat en els fons d'art de la Fundació Iluro” es configura com una mostra de les obres més destacades del fons.") s'ha realitzat amb llenguatge HTML5 i l'aplicació del disseny web responsiu (en anglès: [responsive web design](http://en.wikipedia.org/wiki/Responsive_web_design "Responsive web desgin - Wikipedia the free encyclopedia")). Oxygen ha plantejat i realitzat un projecte innovador aplicant les últimes novetats en programació i disseny web, creant **una veritable webapp d'esdeveniments artístics**.

## CMS-free

A **Oxygen** apostem de totes totes per la construcció de webs [CMS-free](/oxygen-un-web-cms-free). Les lliçons apreses i les experiències visqudes durant 10 anys liderant projectes Magnolia són el rerafons de l'evolució d'un procés que ens condueix cap a nous webs simples, flexibles i fiables que permeten un enfocament renovat de disseny i estratègia.

<figure class="hidden-xs hidden-sm ox_animate_when_almost_visible ox_right-to-left"><img src="/assets/img/figura-i-retrat-full-width-snapshot.png" /><figcaption><p>Figura i retrat. Jekyy, Polymer i Schema metadata</p></figcaption></figure>

## Tornar al bàsic

Mitjançant el desenvolupament de llocs web, com aplicacions de la banda client ("client-side") que només consten dels arxius utilitzables directament per un navegador web sense el treball addicional realitzat pels servidors de back-end, hom es capaç de traslladar l'**estalvi de costos als clients alhora que s'el·limina pràcticament el risc de caiguda de la pàgina web**. Per a funcionalitats addicionals no disponibles en les aplicacions "client-side", hom integra serveis externs.

## La fórmula amb Jekyll, Prose, Webcompoents i Schema metadata!

- [Jekyll](http://jekyllrb.com/ "Jekyll &bull; Simple, blog-aware, static sites") per a plantilles de pàgina i la generació d'arxius estàtics
- Fitxers HTML, CSS i Javascript
- El servidor de pàgines estàtiques GitHub
- APIs externes quan cal
- [Prose.io](http://prose.io/ "Prose &middot; A Content Editor for GitHub"), un editor de continguts web específicament dissenyat per treballar amb Jekyll

En aquest projecte seguim apostant pels [web components](http://webcomponents.org/ "WebComponents.org"), una veritable revolució en el desenvolupament web, per mitjà de [Polymer](http://www.polymer-project.org/ "Welcome - Polymer"), l'"opinionated framework" creat per Google.

<pre>
  <code>&#60;google-map latitude="41.5499299" longitude="2.4512864" fitToMarkers disableDefaultUI zoom="15" id="mapa"&#62;
    &#123;% assign place_data = site.data.places | where:"id", 2 %&#125;
    &#123;% assign place = place_data | first %&#125;
        &#60;google-map-marker latitude="&#123;&#123; place.latitude &#125;&#125;" longitude="&#123;&#123; place.longitude &#125;&#125;"
        title="&#123;&#123; place.name &#125;&#125;" draggable="false" icon="/favicon.ico"&#62;
            &#60;p&#62;&#60;strong&#62;&#123;&#123; place.name &#125;&#125;&#60;/strong&#62;&#60;/p&#62;
            &#60;p&#62;&#60;small&#62;&#60;strong&#62;Adreça:&#60;/strong&#62; &#123;&#123; place.address &#125;&#125;&#60;br/&#62;&#60;strong&#62;Telèfon:&#60;/strong&#62; &#60;a href="tel:&#123;&#123; place.phone &#125;&#125;"&#62;&#123;&#123; place.phone &#125;&#125;&#60;/a&#62; | &#60;strong&#62;&#60;a href="&#123;&#123; place.getdirections &#125;&#125;"&#62;Com arribar-hi?&#60;/a&#62;&#60;/strong&#62;&#60;/small&#62;&#60;/p&#62;
            &#60;p&#62;&#60;small&#62;&#60;a href="&#123;&#123; place.url &#125;&#125;" title="&#123;&#123; place.name &#125;&#125;" rel="external"&#62;url&#60;/a&#62; | &#60;a href="https://twitter.com/&#123;&#123; place.twitter &#125;&#125;" title="@&#123;&#123; place.twitter &#125;&#125; rel="external""&#62;t&#60;/a&#62; | &#60;a href="&#123;&#123; place.facebook &#125;&#125;" title="&#123;&#123; place.name &#125;&#125; en Facebook" rel="external"&#62;f&#60;/a&#62; | &#60;a href="mailto:&#123;&#123; place.email &#125;&#125;" title="Correo-e &#123;&#123; place.email &#125;&#125;" rel="external"&#62;e&#60;/a&#62;&#60;/small&#62;&#60;/p&#62;
        &#60;/google-map-marker&#62;
    &#60;/google-map&#62;
  </code>
</pre>

En aquest projecte no fem ús de la [RESTful API](http://en.wikipedia.org/wiki/Representational_state_transfer "Representational state transfer - Wikipedia, the free encyclopedia") del portal principal, per obtenir les dades de les obres, donat que aquestes no estan a la venda. En aquest cas construim les dades a mida en format [YAML](http://en.wikipedia.org/wiki/YAML "YAML - Wikipedia, the free encyclopedia"). Una altra forma de crear **un sistema "automatitzat" per a l'emplenat de dades**.

## Millor difusió a xarxes socials i millor SEO

Des del punt de vista tècnic, el web figuraitretrat.fundacioiluro.cat presenta tres detalls interessants que **faciliten la seva difusió a les xarxes socials i un millor posicionament SEO**:

- Ús de [metadades og](http://ogp.me/ "The Open Graph Protocol") tant a les obres com als esdeveniments, que generen de manera automàtica **millors posts a Facebook i a Goolge Plus**.
- Ús de [Twitter Cards](https://dev.twitter.com/cards/overview "Twitter Cards | Twitter Developers") tant a les obres com als esdeveniments, que generen de manera automàtica **resums ampliats en forma de tarjeta als tuits** sobre l'exposició.
- Ús d'[Schema Metadata](http://schema.org/docs/schemas.html "Schemas - schema.org") (Organization, IndividualProduct i Event) per **facilitar la indexació** dels contiguts a Google, **facilitar el poscionament** i donar **millors resultats de cerca**.

A [Oxygen.cat](http://www.oxygen.cat/) **tenim la voluntat d'anar un pas per endavant**!