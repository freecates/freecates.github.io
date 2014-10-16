---
comments: true
date: 2014-07-31 11:48:19
layout: blog
slug: "barcelona-digital-art-jekyll-and-polymer"
title: "Barcelona Digital Art. Jekyll and Polymer"
categories: 
  - comunicació
  - treballs
  - "no-cita"
tags: "case-study"
"featured-img": true
"featured-img-url": "barcelona-digital-art-case-study.png"
meta: "Barcelona Digital Art. Jekyll and Polymer"
excerpt: "La mostra simultània d'art digital a Barcelona es presenta com una exposició simultània en espais i edificis de referència de la ciutat"
author: oxygen
published: true
keywords: "artinpocket, screens, digital, collection, convert"
---

#Barcelona Digital Art. Jekyll and Polymer


>La mostra simultània d'art digital a Barcelona es presenta com una exposició simultània en espais i edificis de referència de la ciutat.<footer>&mdash; <cite><a href="{{ page.url }}" title="{{ page.title }}">Artinpocket</a></cite></footer>

##El cas artinpocket

[artinpocket](/artipocket-la-comunitat-de-compra-venda-d-art-accessible-amb-un-sol-clic/ "Artinpocket, la comunitat de compra venda d'art accessible amb un sol clic") ofereix una comunitat de compra venda d'art accessible amb un sol clic. Ofereix una plataforma especialitzada en art que aglutina la promoció d'artistes i galeries amb un canal directe de venda i compra d'obres. Vol transformar i renovar el canal tradicional de projecció d'art utilitzant artinpocket com a suport, una xarxa social per a incentivar i estimular la compra d'art.

###Barcelona Digital Art

Amb aquest nou projecte **Artinpocket**, crea la 1ª mostra simultània d'art digital a Barcelona. Una exposició simultània en espais i edificis de referència de la ciutat. La mostra neix amb l'objectiu d'oferir al públic la possibilitat de descobrir i experimentar amb l'art digital en entorns a priori fora del circuit expositiu tradicional d'art. Oci, cultura i patrimoni es fusionen per oferir una experiència entorn l'Art digital sense precedents a Barcelona. Amb la finalitat de divulgar la disciplina de l'art digital; projectar i promocionar el treball de joves artistes i obrir nous espais i formats expositius a Barcelona [Artinpocket](http://www.artinpocket.cat/), el [Convent de Sant Agustí](http://www.digitalartbarcelona.com/patrocinadors/2014/07/24/convent-sant-agusti/), amb la col·laboració de [IDODI](http://www.digitalartbarcelona.com/patrocinadors/2014/07/26/idodi/) i [BlaNZ](http://www.digitalartbarcelona.com/patrocinadors/2014/07/25/blanz/), han reunit més de 20 creadors d'art digital per crear una mostra simultània a diferents locals de Barcelona.

[digitalartbarcelona.com](http://www.digitalartbarcelona.com/ "Barcelona Digital Art &middot; 1st simultaneous digital art show in Barcelona") s'ha realitzat amb llenguatge HTML5 i l'aplicació del disseny web responsiu (en anglès: [responsive web design](http://en.wikipedia.org/wiki/Responsive_web_design "Responsive web desgin - Wikipedia the free encyclopedia")). Oxygen ha plantejat i realitzat un projecte innovador aplicant les últimes novetats en programació i disseny web, creant **una veritable webapp d'ecommerce**.

##CMS-free

A **Oxygen** apostem de totes totes per la construcció de webs [CMS-free](/oxygen-un-web-cms-free). Les lliçons apreses i les experiències visqudes durant 9 anys liderant projectes Magnolia són el rerafons de l'evolució d'un procés que ens condueix cap a nous webs simples, flexibles i fiables que permeten un enfocament renovat de disseny i estratègia.

<figure class="hidden-xs hidden-sm ox_animate_when_almost_visible ox_right-to-left"><img src="/assets/img/barcelona-digital-art-full-width-snapshot.png" /><figcaption><p>Barcelona Digital Art. Jekyll and Polymer</p></figcaption></figure>

##Tornar al bàsic

Mitjançant el desenvolupament de llocs web, com aplicacions de la banda client ("client-side") que només consten dels arxius utilitzables directament per un navegador web sense el treball addicional realitzat pels servidors de back-end, hom es capaç de traslladar l'estalvi de costos als clients alhora que s'el·limina pràcticament el risc de caiguda de la pàgina web. Per a funcionalitats addicionals no disponibles en les aplicacions "client-side", hom integra serveis externs.

##La fórmula amb Jekyll, Prose i... Webcompoents!

- [Jekyll](http://jekyllrb.com/ "Jekyll &bull; Simple, blog-aware, static sites") per a plantilles de pàgina i la generació d'arxius estàtics
- Fitxers HTML, CSS i Javascript
- El servidor de pàgines estàtiques GitHub
- APIs externes quan cal
- [Prose.io](http://prose.io/ "Prose &middot; A Content Editor for GitHub"), un editor de continguts web específicament dissenyat per treballar amb Jekyll

En aquest nou projecte hem començat a emprar [web components](http://webcomponents.org/ "WebComponents.org"), una veritable revolució en el desenvolupament web, per mitjà de [Polymer](http://www.polymer-project.org/ "Welcome - Polymer"), l'"opinionated framework" creat per Google que n'ha fet un impressionant desplegament al [I/O 2014](https://www.google.com/events/io/schedule/session/de22e147-07b6-e311-8491-00155d5066d7).


<pre><code>&#60;google-map latitude&#61;&#34;41.3804463&#34; longitude&#61;&#34;2.1800922&#34; disableDefaultUI fitToMarkers zoom&#61;&#34;15&#34;&#62;
      &#123;% for place in site.data.places %&#125;
      &#60;google-map-marker latitude&#61;&#34;&#123;&#123; place.latitude &#125;&#125;&#34; longitude&#61;&#34;&#123;&#123; place.longitude &#125;&#125;&#34;
                         title&#61;&#34;&#123;&#123; place.name &#125;&#125;&#34; draggable&#61;&#34;false&#34; icon&#61;&#34;/public&#47;favicon.ico&#34;&#62;
           &#60;p class&#61;&#34;text-center&#34;&#62;&#60;a href&#61;&#34;&#123;&#123; place.url-in &#125;&#125;&#34;&#62;&#60;img src&#61;&#34;&#47;public&#47;img&#47;&#123;&#123; place.logo &#125;&#125;&#34;&#62;&#60;&#47;a&#62;&#60;&#47;p&#62;
           &#60;p&#62;
	      &#60;strong&#62;&#60;a href&#61;&#34;&#123;&#123; place.url-in &#125;&#125;&#34;&#62;&#123;&#123; place.name &#125;&#125;&#60;&#47;a&#62;&#60;&#47;strong&#62;&#60;br&#47;&#62;
	      &#60;strong&#62;Direcció&#60;&#47;strong&#62; &#47; &#60;em&#62;Address&#60;&#47;em&#62;: &#123;&#123; place.address &#125;&#125;&#60;br&#47;&#62;
	      &#60;strong&#62;Horari projecció&#60;&#47;strong&#62; &#47; &#60;em&#62;Screening timetable&#60;&#47;em&#62;: &#60;strong&#62;&#123;&#123; place.screening-ca &#125;&#125;&#60;&#47;strong&#62; &#47; &#60;em&#62;&#123;&#123; place.screening-en &#125;&#125;&#60;&#47;em&#62;&#60;br&#47;&#62;
	    &#60;&#47;p&#62;
      &#60;&#47;google-map-marker&#62;
      &#123;% endfor %&#125;
  &#60;&#47;google-map&#62;</code></pre> 

##artinpocket, segueix creixent

A més a més de la posta en marxa d'digitalartbarcelona.com, des d'**Oxygen** seguim aportant per fer més gran l'ecosistema web d'**artinpocket**:

- [artinpocket.cat](http://www.artinpocket.cat/), la comunitat de compra venda d'art accessible amb un sol clic
- [artinpocket.cat/blog](http://www.artinpocket.cat/blog/), el blog general sobre el projecte
- [artinpocketregular.com](http://www.artinpocketregular.com/), el blog del verkami per a desenvolupar una tipografia pròpia i adequada per al món de les arts plàstiques i visuals
- [artelowcost.com](http://www.artelowcost.com/), un blog especialitzat en art contemporani de baix cost
- [arteeconomico.com](http://www.arteeconomico.com/), un blog especialitzat en art contemporani de baix cost
- [inpockettshirts.com](http://www.inpockettshirts.com/), la botiga d'art per emportar d'Artinpocket. Art per portar posat, art amb la gent, per a la gent i per la gent.
- [inpocketart.com](http://www.inpocketart.com/), la botiga d'art digital d'edició limitada amb certificat digital d'autenticitat.
- [digitalartbarcelona.com](http://www.digitalartbarcelona.com/), la 1ª mostra simultània d'art digital a Barcelona.