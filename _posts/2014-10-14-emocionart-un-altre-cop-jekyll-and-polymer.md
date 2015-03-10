---
comments: true
date: 2014-10-15 11:48:19
layout: blog
og: true
og-type: article
slug: "emocionart-un-altre-cop-jekyll-and-polymer"
title: "Emocionart. Un altre cop, Jekyll i Polymer i a més RESTful API"
categories: 
  - comunicació
  - treballs
  - "no-cita"
tags: "case-study"
"featured-img": true
"featured-img-url": "emocionart-case-study.png"
meta: "Un altre cop, Jekyll i Polymer i a més RESTful API"
excerpt: "#Emocionart' és una acció d'Artinpocket per promocionar i impulsar la compra d'art."
author: oxygen
published: true
keywords: "artinpocket, screens, digital, collection, polymer"
---

>'#Emocionart' és una acció d'Artinpocket per promocionar i impulsar la compra d'art.<footer>&mdash; <cite><a href="{{ page.url }}" title="{{ page.title }}">Artinpocket</a></cite></footer>

##El cas artinpocket

[artinpocket](/artipocket-la-comunitat-de-compra-venda-d-art-accessible-amb-un-sol-clic/ "Artinpocket, la comunitat de compra venda d'art accessible amb un sol clic") ofereix una comunitat de compra venda d'art accessible amb un sol clic. Ofereix una plataforma especialitzada en art que aglutina la promoció d'artistes i galeries amb un canal directe de venda i compra d'obres. Vol transformar i renovar el canal tradicional de projecció d'art utilitzant artinpocket com a suport, una xarxa social per a incentivar i estimular la compra d'art.

###Emocionart

Amb aquest nou projecte **[Artinpocket](http://www.artinpocket.cat/)**, duu a terme una acció per promocionar i impulsar la compra d'art. Durant tres mesos la plataforma impulsarà diferents accions amb l'objectiu d'apropar l'art i incentivar la compra obres originals a preus assequibles. Amb aquesta acció es pretén trencar falsos mites: l'art és car? No sempre! L'Art és per a una minoria? ¡Fals!

[emocio-nart.com](http://www.emocio-nart.com/ "#Emocionart &middot; Descubre, emociónate y compra obras de arte ") s'ha realitzat amb llenguatge HTML5 i l'aplicació del disseny web responsiu (en anglès: [responsive web design](http://en.wikipedia.org/wiki/Responsive_web_design "Responsive web desgin - Wikipedia the free encyclopedia")). Oxygen ha plantejat i realitzat un projecte innovador aplicant les últimes novetats en programació i disseny web, creant **una veritable webapp d'ecommerce**.

##CMS-free

A **Oxygen** apostem de totes totes per la construcció de webs [CMS-free](/oxygen-un-web-cms-free). Les lliçons apreses i les experiències visqudes durant 9 anys liderant projectes Magnolia són el rerafons de l'evolució d'un procés que ens condueix cap a nous webs simples, flexibles i fiables que permeten un enfocament renovat de disseny i estratègia.

<figure class="hidden-xs hidden-sm ox_animate_when_almost_visible ox_right-to-left"><img src="/assets/img/emocionart-full-width-snapshot.png" /><figcaption><p>Emocionart. Un altre cop, Jekyll and Polymer</p></figcaption></figure>

##Tornar al bàsic

Mitjançant el desenvolupament de llocs web, com aplicacions de la banda client ("client-side") que només consten dels arxius utilitzables directament per un navegador web sense el treball addicional realitzat pels servidors de back-end, hom es capaç de traslladar l'estalvi de costos als clients alhora que s'el·limina pràcticament el risc de caiguda de la pàgina web. Per a funcionalitats addicionals no disponibles en les aplicacions "client-side", hom integra serveis externs.

##La fórmula amb Jekyll, Prose, Webcompoents i RESTful API!

- [Jekyll](http://jekyllrb.com/ "Jekyll &bull; Simple, blog-aware, static sites") per a plantilles de pàgina i la generació d'arxius estàtics
- Fitxers HTML, CSS i Javascript
- El servidor de pàgines estàtiques GitHub
- APIs externes quan cal
- [Prose.io](http://prose.io/ "Prose &middot; A Content Editor for GitHub"), un editor de continguts web específicament dissenyat per treballar amb Jekyll

En aquest nou projecte emprem de nou [web components](http://webcomponents.org/ "WebComponents.org"), una veritable revolució en el desenvolupament web, per mitjà de [Polymer](http://www.polymer-project.org/ "Welcome - Polymer"), l'"opinionated framework" creat per Google.

<pre><code>&#60;core-image sizing="cover" class="core-image-size" preload fade src="&#123;&#123; work.featured_src &#125;&#125;"&#62;&#60;/core-image&#62;</code></pre>

A més a més hem començat a emprar la [RESTful API](http://en.wikipedia.org/wiki/Representational_state_transfer "Representational state transfer - Wikipedia, the free encyclopedia") del portal principal per obtenir les dades de les obres dels artistes via [JSON](http://en.wikipedia.org/wiki/JSON "JSON - Wikipedia, the free encyclopedia"). D'aquesta manera creem **un sistema "automatitzat" per l'emplenat de dades**. 

##artinpocket, segueix creixent

A més a més de la posta en marxa d'emocio-nart.com, des d'**Oxygen** seguim aportant per fer més gran l'ecosistema web d'**artinpocket**:

- [artinpocket.cat](http://www.artinpocket.cat/), la comunitat de compra venda d'art accessible amb un sol clic
- [artinpocket.cat/blog](http://www.artinpocket.cat/blog/), el blog general sobre el projecte
- [artinpocketregular.com](http://www.artinpocketregular.com/), el blog del verkami per a desenvolupar una tipografia pròpia i adequada per al món de les arts plàstiques i visuals
- [artelowcost.com](http://www.artelowcost.com/), un blog especialitzat en art contemporani de baix cost
- [arteeconomico.com](http://www.arteeconomico.com/), un blog especialitzat en art contemporani de baix cost
- [inpockettshirts.com](http://www.inpockettshirts.com/), la botiga d'art per emportar d'Artinpocket. Art per portar posat, art amb la gent, per a la gent i per la gent.
- [inpocketart.com](http://www.inpocketart.com/), ~~la botiga d'art digital d'edició limitada amb certificat digital d'autenticitat~~. Fusionada amb el portal principal, que conté ambdues tipologies d'art: analògic i digital amb certficiat digital d'autenticitat.
- [digitalartbarcelona.com](http://www.digitalartbarcelona.com/), la 1ª mostra simultània d'art digital a Barcelona.
- [emocio-nart.com](http://www.emocio-nart.com/), campanya per promocionar i impulsar la compra d'art.