---
comments: true
date: 2015-02-04 11:48:19
layout: blog
slug: "emocionart-un-altre-cop-jekyll-and-polymer"
title: "Jordi Pagès. Jekyll, Polymer, RESTful API i Service Worker"
categories: 
  - comunicació
  - treballs
  - "no-cita"
tags: "case-study"
"featured-img": true
"featured-img-url": "jordipages-case-study.png"
meta: "Jordi Pagès. Jekyll, Polymer, RESTful API i Service Worker"
excerpt: Jordi Pagès és un artista de Granollers (1951) amb una forta empremta a Cadaqués.
author: oxygen
published: true
keywords: "artinpocket, screens, digital, collection, polymer, restful, api, service, worker"
---

>Jordi Pagès és un artista de Granollers (1951) amb una forta empremta a Cadaqués.<footer>&mdash; <cite><a href="{{ page.url }}" title="{{ page.title }}">Artinpocket</a></cite></footer>

##El cas artinpocket

[artinpocket](/artipocket-la-comunitat-de-compra-venda-d-art-accessible-amb-un-sol-clic/ "Artinpocket, la comunitat de compra venda d'art accessible amb un sol clic") ofereix una comunitat de compra venda d'art accessible amb un sol clic. Ofereix una plataforma especialitzada en art que aglutina la promoció d'artistes i galeries amb un canal directe de venda i compra d'obres. Vol transformar i renovar el canal tradicional de projecció d'art utilitzant artinpocket com a suport, una xarxa social per a incentivar i estimular la compra d'art. 

És en aquest sentit que s'emmarca **el nou web de l'artista Jordi Pagès**.

###jordi Pagès

[jordipages.cat](http://www.jordipages.cat/ "Jordi Pagès és un artista de Granollers amb una forta empremta a Cadaqués") s'ha realitzat amb llenguatge HTML5 i l'aplicació del disseny web responsiu (en anglès: [responsive web design](http://en.wikipedia.org/wiki/Responsive_web_design "Responsive web desgin - Wikipedia the free encyclopedia")). Oxygen ha plantejat i realitzat un projecte innovador aplicant les últimes novetats en programació i disseny web, creant **una veritable webapp de portfoli professional**.

##CMS-free

A **Oxygen** apostem de totes totes per la construcció de webs [CMS-free](/oxygen-un-web-cms-free). Les lliçons apreses i les experiències visqudes durant 10 anys liderant projectes Magnolia són el rerafons de l'evolució d'un procés que ens condueix cap a nous webs simples, flexibles i fiables que permeten un enfocament renovat de disseny i estratègia.

<figure class="hidden-xs hidden-sm ox_animate_when_almost_visible ox_right-to-left"><img src="/assets/img/jordipages-full-width-snapshot.png" /><figcaption><p>Jordi Pagès. Jekyll, Polymeri Service Worker</p></figcaption></figure>

##Tornar al bàsic

Mitjançant el desenvolupament de llocs web, com aplicacions de la banda client ("client-side") que només consten dels arxius utilitzables directament per un navegador web sense el treball addicional realitzat pels servidors de back-end, hom es capaç de traslladar l'**estalvi de costos als clients alhora que s'el·limina pràcticament el risc de caiguda de la pàgina web**. Per a funcionalitats addicionals no disponibles en les aplicacions "client-side", hom integra serveis externs.

##La fórmula amb Jekyll, Prose, Webcompoents, RESTful API i Service Worker!

- [Jekyll](http://jekyllrb.com/ "Jekyll &bull; Simple, blog-aware, static sites") per a plantilles de pàgina i la generació d'arxius estàtics
- Fitxers HTML, CSS i Javascript
- El servidor de pàgines estàtiques GitHub
- APIs externes quan cal
- [Prose.io](http://prose.io/ "Prose &middot; A Content Editor for GitHub"), un editor de continguts web específicament dissenyat per treballar amb Jekyll

En aquest projecte emprem de nou [web components](http://webcomponents.org/ "WebComponents.org"), una veritable revolució en el desenvolupament web, per mitjà de [Polymer](http://www.polymer-project.org/ "Welcome - Polymer"), l'"opinionated framework" creat per Google.

<pre><code>&#60;core-image sizing="cover" class="core-image-size" preload fade src="&#123;&#123; work.featured_src &#125;&#125;"&#62;&#60;/core-image&#62;</code></pre>

Seguim emprant la [RESTful API](http://en.wikipedia.org/wiki/Representational_state_transfer "Representational state transfer - Wikipedia, the free encyclopedia") del portal principal, per obtenir les dades de les obres en venda de l'artista via [JSON](http://en.wikipedia.org/wiki/JSON "JSON - Wikipedia, the free encyclopedia"). D'aquesta manera creem **un sistema "automatitzat" per a l'emplenat de dades**.

###Service Worker

Des del punt de vista tècnic, el web jordipages.cat presenta **una darrera novetat molt innovadora**: l'ús del "[service worker](http://www.html5rocks.com/en/tutorials/service-worker/introduction/)". Amb aquesta implementació, ara sí, el web esc comporta com una veritable app ja que **funciona 100% offline sense els maldecaps de l'[appcache](http://alistapart.com/article/application-cache-is-a-douchebag)**! Aquesta funcionalitat es troba encara en una fase força [experimental](http://caniuse.com/#feat=serviceworkers) de l'HTML5 però tot sembla indicar que aquest és el futur de les web apps.

A Oxygen.cat **sempre anem un pas per endavant**! Ah, abans que se'ns oblidi! Un app [100% segura](/webs-segures-per-a-tothom-amb-ssl/), gràcies a Cloudflare!