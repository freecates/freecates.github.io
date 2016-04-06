---
comments: true
date: 2015-04-07 11:48:19
og: true
og-type: article
layout: blog
slug: "webs-sense-connexio-el-cas-del-concurs-tram-disseny"
title: "Webs sense connexió a Internet! El cas del concurs TRAMdisseny"
categories: 
  - comunicació
  - treballs
  - "no-cita"
tags: "case-study"
"featured-img": true
"featured-img-url": "tram-disseny-case-study.png"
meta: "Webs sense connexió a Internet! El cas del concurs TRAMdisseny"
excerpt: "Per què és vol el retrat?. S’ha dit que el retrat és el substitut i/o el record de la presència de l’absent."
author: oxygen
published: true
keywords: "artinpocket, screens, digital, collection, polymer, restful, api, service, worker, google, forms"
---

>Concurs adreçat a estudiants de disseny gràfic amb el que es pretén ampliar la formació acadèmica de l’alumne amb un cas real.<footer>&mdash; <cite><a href="{{ page.url }}" title="{{ page.title }}">TRAMdisseny</a></cite></footer>

## TRAM

**[TRAM](http://www.tram.cat/ "TRAM - Barcelona")** és una empresa de transport públic que gestiona les dues xarxes actuals de tramvies a la Regió Metropolitana de Barcelona de la manera més eficient. Treballen per oferir el millor servei als viatgers que diàriament utilitzen el tramvia per desplaçar-se de manera ràpida, còmoda i segura.

Des de **TRAM** volen posar en marxa la seva línia de merxandatge. És en aquest sentit que s'emmarca **el nou web del concurs TRAMdisseny**.

### TRAMdisseny

[www.tramdisseny.cat](https://www.tramdisseny.cat/ "Concurs adreçat a estudiants de disseny gràfic amb el que es pretén ampliar la formació acadèmica de l’alumne amb un cas real. TRAM seleccionarà les proposte...") s'ha realitzat amb llenguatge HTML5 i l'aplicació del disseny web responsiu (en anglès: [responsive web design](http://en.wikipedia.org/wiki/Responsive_web_design "Responsive web desgin - Wikipedia the free encyclopedia")). Oxygen ha plantejat i realitzat un projecte innovador aplicant les últimes novetats en programació i disseny web, creant **una veritable webapp per a la recollida i gestió de les propostes del concurs**.

## CMS-free

A **Oxygen** apostem de totes totes per la construcció de webs [CMS-free](/oxygen-un-web-cms-free). Les lliçons apreses i les experiències visqudes durant 10 anys liderant projectes Magnolia són el rerafons de l'evolució d'un procés que ens condueix cap a nous webs simples, flexibles i fiables que permeten un enfocament renovat de disseny i estratègia.

<figure class="hidden-xs hidden-sm ox_animate_when_almost_visible ox_right-to-left"><img src="/assets/img/tram-disseny-full-width-snapshot.png" /><figcaption><p>Webs sense connexió a Internet! El cas del concurs TRAMdisseny</p></figcaption></figure>

## Tornar al bàsic

Mitjançant el desenvolupament de llocs web, com aplicacions de la banda client ("client-side") que només consten dels arxius utilitzables directament per un navegador web sense el treball addicional realitzat pels servidors de back-end, hom es capaç de traslladar l'**estalvi de costos als clients alhora que s'el·limina pràcticament el risc de caiguda de la pàgina web**. Per a funcionalitats addicionals no disponibles en les aplicacions "client-side", hom integra serveis externs.

## La fórmula amb Jekyll, Prose, Webcompoents, Service Worker i formularis de Google customitzats

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

Des del punt de vista tècnic, el web tramdisseny.cat fa ús també del "[service worker](http://www.html5rocks.com/en/tutorials/service-worker/introduction/)". Amb aquesta implementació, ara sí, el web es comporta com una veritable app ja que **funciona 100% offline sense els maldecaps de l'[appcache](http://alistapart.com/article/application-cache-is-a-douchebag)**! Aquesta funcionalitat es troba encara en una fase força [experimental](http://caniuse.com/#feat=serviceworkers) de l'HTML5  però de ben segur que aquest és el futur de les web apps.

### Formularis de Google customitzats

Per a la recollida de dades dels participants al Concurs **TRAM**disseny, hem optat per cusotmitzar un formulari de Google i lligar-lo a un full de càlcul al núvol, la qual cosa ens permet fer **un seguiment en temps real de totes les dades dels participants**.

## Millor difusió a xarxes socials i millor SEO

tramdisseny.cat presenta quatre detalls interessants que **faciliten la seva difusió a les xarxes socials i un millor posicionament SEO**:

- Ús de [metadades og](http://ogp.me/ "The Open Graph Protocol") que generen de manera automàtica **millors posts a Facebook i a Goolge Plus**.
- Ús de [Twitter Cards](https://dev.twitter.com/cards/overview "Twitter Cards | Twitter Developers") que generen de manera automàtica **resums ampliats en forma de tarjeta als tuits** sobre el Concurs.
- Ús d'[Schema Metadata](http://schema.org/docs/schemas.html "Schemas - schema.org") (Organization i Article) per **facilitar la indexació** dels contiguts a Google, **facilitar el poscionament** i donar **millors resultats de cerca**.
- SSL gràcies a Cloudflare. [Google](http://googlewebmastercentral.blogspot.com.es/2014/08/https-as-ranking-signal.html "Official Google Webmaster Central Blog: HTTPS as a ranking signal") aposta dedicidament per una Internet més segura i per tant ha decidit **premiar aquells webs que corrin sota https**!

A [Oxygen.cat](http://www.oxygen.cat/) tenim la voluntat d'intentar anar un pas per endavant, **oferint allò que els nostres clients es mereixen: bon servei i millor innovació**!