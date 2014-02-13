---
comments: true
date: 2013-12-24 11:48:19
layout: blog
slug: box-fort-un-web-tambe-cms-free
title: "Box-fort.com, un web també CMS-free"
categories: [comunicació, treballs, no-cita]
tags: "case-study"
"featured-img": true
"featured-img-url": "box-fort-case-study.png"
meta: "Box-fort.com, un web també CMS-free"
excerpt: "Amb Jekyll hem construït un web senzill, flexible, fiable i multi idioma sense el sobrecost del CMS."
author: oxygen
published: true
keywords: box-fort, web, cms, free, multilang
---

#Box-fort.com, un web també CMS-free

<blockquote>
	<p>Jekyll permet la construcció senzilla, flexible i fiable de webs sense el sobrecost del CMS. Fins i tot multi idioma</p>
	<footer>
		&mdash; <cite><a href="{{ page.url }}" title="{{ page.title }}">Oxygen</a></cite>
	</footer>
</blockquote>

A Oxygen apostem de totes totes per la contruscció de webs CMS-free. Les lliçons apreses i les experiències visqudes durant 9 anys liderant projectes Magnolia són el rerafons de l'evolució d'un procés que ens condueix cap a nous webs simples, flexibles i fiables que permeten un enfocament renovat de disseny i estratègia.

##L'era CMS. Magnolia un aliat

En el passat, la creació de llocs web "potents", significava la creació de complexos sistemes de gestió de continguts. Aquests CMSs necessitaven de la lògica de les plantilles, el codi d'aplicació i les bases de dades de contingut per poder "muntar" pàgines web cada vegada que eren sol·licitades pels visitants del web. Eren sistemes complexos que depenien d'aplicacions diferents treballant alhora, com un servidor web per conduir les peticions de pàgina cap a una aplicació Java, que emprava plantilles de disseny de pàgina predefinides per donar format a contingut emmagatzemat en una base de dades MySQL. Per servir una sola sol·licitud de pàgina calia almenys tres aplicacions separades treballant alhora.

Tant els frameworks de codi obert com ara Magnolia, Drupal o Wordpress com les aplicacions de codi propietari de milions d'euros que empren governs i grans empreses, produeixen exactament el mateix "output": arxius HTML, CSS i JavaScript que els navegadors web saben com "convertir" en les pàgines web que veiem.

Tot i la complexitat d'aquests sistemes, tots ells han de produir els mateixos formats de sortida: estàndards web.

##Tornar al bàsic

Mitjançant el desenvolupament de llocs web, com aplicacions de la banda client ("client-side") que només consten dels arxius utilitzables directament per un navegador web sense el treball addicional realitzat pels servidors de back-end, hom es capaç de traslladars l'estalvi de costos als clients alhora que s'elimina pràcticament el risc de caiguda de la pàgina web. Per a funcionalitats addicionals no disponibles en les aplicacions "client-side", hom integra serveis externs.

##La fórmula amb Jekyll i Prose

- [Jekyll](http://jekyllrb.com/ "Jekyll &bull; Simple, blog-aware, static sites") per a plantilles de pàgina i la generació d'arxius estàtics
- Fitxers HTML, CSS i Javascript
- El servidor de pàgines estàtiques GitHub
- APIs externes quan cal
- [Prose.io](http://prose.io/ "Prose &middot; A Content Editor for GitHub"), un editor de continguts web específicament dissenyat per treballar amb Jekyll

Per a plantilles i per a la generació de llocs web, hom pot emprar Jekyll, un projecte de codi obert iniciat a GitHub fa gairebé cinc anys. Jekyll emmagatzema tot el contingut en arxius de text simple. Les metadades que descriuen el contingut es troben sobre el contingut en el mateix arxiu de text. Aquestes metadades associades al contingut amb les plantilles de disseny, permeten un format avançat com ara el filtratge de categories o etiquetes, i podem emmagatzemar dades estructurades arbitràries com l'associació d'articles amb autors, fotos del moment, o qualsevol altra cosa que el desenvolupador de la plantilla estableixi.

Si volem que un tercer sense coneixements tècnics pugui mantenir i administrar un web creat amb Jekyll, cal trobar un editor de continguts amb interfície web. [Prose.io](http://prose.io/ "Prose &middot; A Content Editor for GitHub"), és un editor de continguts web específicament dissenyat per treballar bé amb Jekyll. Prose permet editar arxius de text allotjats a GitHub, on emmagatzemem el nostre codi. Ofereix una elegant interfície que se centra en l'escriptura.

<figure class="hidden-xs hidden-sm ox_animate_when_almost_visible ox_right-to-left"><img src="/assets/img/box-fort-full-width-snapshot.png" /><figcaption><p>Captura de "Maletes de plàstic, Doble paret" — Box-fort.com, un web també CMS-free</p></figcaption></figure>

##I si el fem multi idioma?

Amb [Box fort](http://www.box-fort.com/ "Boxfort, maletes i contenidors professionals"), hme fet un pas més en la creció de webs CMS-free. Hem fet un web CMS-free multi idioma. A la <abbr title="World Wide Web">WWW</abbr>, hi ha molts de recursos que parlen de com afrontar un web multi idioma fet amb Jekyll. Alguns d'ells són:

- [G. Garron - Multi language site with Jekyll](http://www.garron.me/en/blog/jekyll-multi-language.html "G. Garron - Multi language site with Jekyll")
- [Building a multilanguage Jekyll blog](http://nicoespeon.com/en/2013/04/building-a-multinlingual-jekyll-blog/ "Building a multilanguage Jekyll blog | @nicoespeon")
- [Multilingual Jekyll](http://developmentseed.org/blog/multilingual-jekyll-sites/ "Multilingual Jekyll | Development Seed")

En el cas que ens ocupa hem optat per treure el màxim de pròfit de les metadades <abbr title="YAML Ain't Markup Language">YAML</abbr> per assignar l'idioma i una estructura separada dins d'una carpeta amb el nom corresponent al codi ISO de l'idioma que estem fent:

	---
	lang: es
	---

	|-- _includes/      # Partials included in other files
	|-- _layouts/       # Templates of the website
	|-- _plugins/       # Plugins to override Jekyll workflow
	|-- assets/         # LESS/CSS, JS, images, ...
	|-- es/             # Spanish category
	|   |-- index.html  # French html files
	|   |-- (...)
	|-- index.html      # Default html files (CA)
	|-- (...)
	|-- _config.yml     # Jekyll configuration file

A partir d'aquí podem també tenir els nostres includes amb les diferents opcions idiomàtiques del nostre web:

<pre><code>&#60;li&#62;
	&#123;% if page.lang == 'es' &#37;&#125;
		&#60;a href="&#123;&#123; site.base_url &#125;&#125;/es/maletas/aluminio/standard.html"&#62;
			&#123;&#37; if page.box == "standard" &#37;&#125;
				&#60;strong&#62;
					&#60;em&#62;
						Standard
					&#60;/em&#62;
				&#60;/strong&#62;
			&#123;&#37; else &#37;&#125;
				Standard
			&#123;&#37; endif &#37;&#125;
		&#60;/a&#62;
	&#123;&#37; else if &#37;&#125;
		&#60;a href="&#123;&#123; site.base_url &#125;&#125;/maletes/alumini/standard.html"&#62;
			&#123;&#37; if page.box == "standard" &#37;&#125;
				&#60;strong&#62;
					&#60;em&#62;
						Standard
					&#60;/em&#62;
				&#60;/strong&#62;
			&#123;&#37; else &#37;&#125;
				Standard
			&#123;&#37; endif &#37;&#125;
		&#60;/a&#62;
	&#123;&#37; endif %&#125;
&#60;/li&#62;</code></pre>

