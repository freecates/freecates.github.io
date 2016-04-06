---
comments: true
date: 2015-07-08 11:48:19
og: true
og-type: article
layout: blog
slug: "digital-art-barcelona-el-millor-web-possible-per-a-la-ii-mostra-simultania-d-art-digital"
title: "digitalartbarcelona, el millor web possible per a la II Mostra Simultània d'Art Digital"
categories: 
  - comunicació
  - treballs
  - "no-cita"
tags: "case-study"
"featured-img": true
"featured-img-url": "digital-art-barcelona-case-study.png"
meta: "digitalartbarcelona, el millor web possible per a la II Mostra Simultània d'Art Digital"
excerpt: "La mostra simultània d'art digital a Barcelona es presenta com una exposició simultània en espais i edificis de referència de la ciutat."
author: oxygen
published: true
keywords: "artinpocket, screens, digital, collection, polymer, restful, api, service, worker, google, forms, micorformat"
---

>... descobrir i experimentar amb l'art digital en entorns a priori fora del circuit expositiu tradicional d'art. Oci, cultura i patrimoni es fusionen per oferir una experiència entorn l'Art digital sense precedents a Barcelona.<footer>&mdash; <cite><a href="{{ page.url }}" title="{{ page.title }}">digitalartbarcelona.com</a></cite></footer>

## MAD BCN. II Mostra Simultània d'Art Digital

La Plataforma **[Artinpocket](http://www.artinpocekt.cat/)** juntament amb el **Convent de Sant Agustí** i en col·laboració amb **Blanz** com a entitats conscients de les transformacions en la creació, difusió i exhibició de l'art han ceat la segona Mostra d'art digital de Barcelona (MAD Barcelona) que es pot veure del 8 al 19 de juliol a diferents espais de Barcelona. 

MAD Barcelona té com a objectiu oferir al públic la possibilitat de descobrir i experimentar amb l'art digital en entorns a priori fora del circuit expositiu tradicional d'art. Per assolir-ho es compta amb **Canon**, que realitzarà un taller on es mostraran els últims avenços tecnològics de les seves impressores vehiculant-les amb el món de l'art, així com el suport de **TRAM**, que projectarà vídeos de la mostra als monitors de les seves línies de transport.

Des de MAD Barcelona es promou la divulgació i normalització del consum de l'art digital fora dels circuits habituals i per aquest motiu la part educativa de la Mostra, que serà dirigida pel Convent de Sant Agustí de Barcelona, resulta essencial. Aquesta consistirà en la realització de deu càpsules formatives relacionades amb la creació digital i multimèdia i que es portaran a terme del 6 al 19 juliol al mateix convent.

### digitalartbarcelona

[www.digitalartbarcelona.com](https://www.digitalartbarcelona.com/ "MAD Barcelona &middot; II Simultaneous Digital Art Show") s'ha realitzat amb llenguatge HTML5 i l'aplicació del disseny web responsiu (en anglès: [responsive web design](http://en.wikipedia.org/wiki/Responsive_web_design "Responsive web desgin - Wikipedia the free encyclopedia")). Oxygen ha plantejat i realitzat un projecte innovador aplicant les últimes novetats en programació i disseny web, creant **una veritable webapp per a la recollida i gestió de les propostes del I Premi Internacional Digital Art Barcelona 2015, ruta dels espais d'exposició, agenda dels tallers i activitats paral·leles i tot plegat amb notificacions push**.

## CMS-free

A **Oxygen** apostem de totes totes per la construcció de webs [CMS-free](/oxygen-un-web-cms-free). Les lliçons apreses i les experiències visqudes durant 10 anys liderant projectes Magnolia són el rerafons de l'evolució d'un procés que ens condueix cap a nous webs simples, flexibles i fiables que permeten un enfocament renovat de disseny i estratègia.

<figure class="hidden-xs hidden-sm ox_animate_when_almost_visible ox_right-to-left"><img src="/assets/img/digital-art-barcelona-full-width-snapshot.png" /><figcaption><p>digitalartbarcelona.com, el millor web possible per a la II Mostra Simultània d'Art Digital</p></figcaption></figure>

## Tornar al bàsic

Mitjançant el desenvolupament de llocs web, com aplicacions de la banda client ("client-side") que només consten dels arxius utilitzables directament per un navegador web sense el treball addicional realitzat pels servidors de back-end, hom es capaç de traslladar l'**estalvi de costos als clients alhora que s'el·limina pràcticament el risc de caiguda de la pàgina web**. Per a funcionalitats addicionals no disponibles en les aplicacions "client-side", hom integra serveis externs.

## La fórmula amb Jekyll, Prose, Webcompoents, Service Worker, formularis de Google customitzats i notificacions push!

- [Jekyll](http://jekyllrb.com/ "Jekyll &bull; Simple, blog-aware, static sites") per a plantilles de pàgina i la generació d'arxius estàtics
- Fitxers HTML, CSS i Javascript
- El servidor de pàgines estàtiques GitHub
- APIs externes quan cal
- [Prose.io](http://prose.io/ "Prose &middot; A Content Editor for GitHub"), un editor de continguts web específicament dissenyat per treballar amb Jekyll

En aquest projecte seguim apostant pels [web components](http://webcomponents.org/ "WebComponents.org"), una veritable revolució en el desenvolupament web, per mitjà de [Polymer](http://www.polymer-project.org/ "Welcome - Polymer"), l'"opinionated framework" creat per Google.

<pre>
  <code>&#60;google-map latitude="41.389329" longitude="2.172469" disableDefaultUI zoom="14"&#62;
      &#123;% for place in site.data.places %&#125;
      &#60;google-map-marker latitude="&#123;&#123; place.latitude &#125;&#125;" longitude="&#123;&#123; place.longitude &#125;&#125;"
                         title="&#123;&#123; place.name &#125;&#125;" draggable="false" icon="/favicon.ico"&#62;
           &#60;p class="text-center"&#62;&#60;a href="&#123;&#123; place.url-in &#125;&#125;"&#62;&#60;img src="/public/img/&#123;&#123; place.logo &#125;&#125;"&#62;&#60;/a&#62;&#60;/p&#62;
           &#60;p&#62;
        &#60;strong&#62;&#60;a href="&#123;&#123; place.url-in &#125;&#125;"&#62;&#123;&#123; place.name &#125;&#125;&#60;/a&#62;&#60;/strong&#62;&#60;br/&#62;
        &#60;strong&#62;Adreça&#60;/strong&#62; / &#60;em&#62;Address&#60;/em&#62; / Dirección: &#123;&#123; place.address &#125;&#125;&#60;br/&#62;
        &#60;strong&#62;&#60;a href="&#123;&#123; place.getdirections &#125;&#125;"&#62;Com arribar-hi?&#60;/a&#62;&#60;/strong&#62; / &#60;em&#62;&#60;a href="&#123;&#123; place.getdirections &#125;&#125;"&#62;Get directions&#60;/a&#62;&#60;/em&#62; / &#60;a href="&#123;&#123; place.getdirections &#125;&#125;"&#62;¿Cómo llegar?&#60;/a&#62;&#60;br/&#62;
        &#60;strong&#62;Horari projecció&#60;/strong&#62; / &#60;em&#62;Screening timetable&#60;/em&#62;: &#60;strong&#62;&#123;&#123; place.screening-ca &#125;&#125;&#60;/strong&#62; / &#60;em&#62;&#123;&#123; place.screening-en &#125;&#125;&#60;/em&#62;&#60;br/&#62;
      &#60;/p&#62;
      &#60;/google-map-marker&#62;
      &#123;% endfor %&#125;
  &#60;/google-map&#62;
  </code>
</pre>

Des del punt de vista tècnic, el web digitalartbarcelona.com fa ús també del "[service worker](http://www.html5rocks.com/en/tutorials/service-worker/introduction/)". Amb aquesta implementació, ara sí, el web es comporta com una veritable app ja que **funciona 100% offline sense els maldecaps de l'[appcache](http://alistapart.com/article/application-cache-is-a-douchebag)**! Aquesta funcionalitat es troba encara en una fase força [experimental](http://caniuse.com/#feat=serviceworkers) de l'HTML5  però de ben segur que aquest és el futur de les web apps. A més a més, gràcies a la versió 1.0 de Polymer, la implementació és força més senzilla.

### Formularis de Google customitzats

Per a la recollida de dades dels participants al I Premi Internacional Digital Art Barcelona 2015, hem optat de nou per cusotmitzar dos formularis de Google i lligar-lo a un full de càlcul al núvol, la qual cosa ens ha permés fer **un seguiment en temps real de totes les dades dels participants**.

### Notificacions push

Cal destacar com a gran novetat, la incorporació de notificacions push. La incorporació d'aquesta nova API HTML5 als navegadors Chrome (tant entorn escriptori com mòbil i tauletes), donen un nou gran valor afegit a les webapp, pertement **una comunicació més directe amb els nostres usuaris**. Tot plegat gràcies al servei [goroost.com](http://goroost.com). 

## Millor difusió a xarxes socials i millor SEO

digitalartbarcelona.com presenta quatre detalls interessants que **faciliten la seva difusió a les xarxes socials i un millor posicionament SEO**:

- Ús de [metadades og](http://ogp.me/ "The Open Graph Protocol") que generen de manera automàtica **millors posts a Facebook i a Goolge Plus**.
- Ús de [Twitter Cards](https://dev.twitter.com/cards/overview "Twitter Cards | Twitter Developers") que generen de manera automàtica **resums ampliats en forma de tarjeta als tuits** sobre el Concurs.
- Ús d'[Schema Metadata](http://schema.org/docs/schemas.html "Schemas - schema.org") (Organization i Article) per **facilitar la indexació** dels contiguts a Google, **facilitar el poscionament** i donar **millors resultats de cerca**.
- SSL gràcies a Cloudflare. [Google](http://googlewebmastercentral.blogspot.com.es/2014/08/https-as-ranking-signal.html "Official Google Webmaster Central Blog: HTTPS as a ranking signal") aposta dedicidament per una Internet més segura i per tant ha decidit **premiar aquells webs que corrin sota https**!

A [Oxygen.cat](http://www.oxygen.cat/) tenim la voluntat d'intentar anar un pas per endavant, **oferint allò que els nostres clients es mereixen: el millor servei i la millor innovació**!