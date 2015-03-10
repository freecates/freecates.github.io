---
comments: true
date: 2015-01-09 11:48:19
layout: blog
og: true
og-type: article
slug: webs-segures-per-a-tothom-amb-ssl
title: "Webs segures per a tothom amb ssl. Millor posicionament"
categories: [programació, general, no-cita]
tags:
"featured-img": true
"featured-img-url": "ssl-case-study.jpg"
meta: "Webs segures per a tothom amb ssl"
excerpt: "Google ja fa temps que ha apostat per la seguretat com una prioritat màxima. Per tant, els nostres webs tindran majors possibilitats d'aparèixer al capdamunt dels resultats de cerca si fa ús del protocol HTTPS."
author: oxygen
keywords: ssl, github, clouflare, jekyll, SEO
---

A Oxygen apostem de totes totes per la construcció de webs [CMS-free](/oxygen-un-web-cms-free). Les lliçons apreses i les experiències visqudes durant 10 anys liderant projectes Magnolia són el rerafons de l'evolució d'un procés que ens condueix cap a nous webs simples, flexibles i fiables que permeten un enfocament renovat de disseny i estratègia. En essència la fórmula és:

- [Jekyll](http://jekyllrb.com/ "Jekyll &bull; Simple, blog-aware, static sites") per a plantilles de pàgina i la generació d'arxius estàtics
- Fitxers HTML, CSS i Javascript
- El servidor de pàgines estàtiques GitHub
- APIs externes quan cal
- [Prose.io](http://prose.io/ "Prose &middot; A Content Editor for GitHub")

##Google i la seguretat. Una prioritat de màxim nivell. Un millor posicionament

[Google](http://googlewebmastercentral.blogspot.com.es/2014/08/https-as-ranking-signal.html "Official Google Webmaster Central Blog: HTTPS as a ranking signal") ja fa temps que ha apostat per la seguretat com una prioritat màxima. En aquest sentit una Intenet més segura passa per l'adopció del que anomenen "[HTTPS a tot arreu](https://www.youtube.com/watch?v=cBhZ6S0PFCY "Google I/O 2014 - HTTPS Everywhere - YouTube")". Aquesta prioritat a més a més fa que Google consideri l'[HTTPS](http://ca.wikipedia.org/wiki/HTTPS "HTTPS - Viquipèdia, l'enciclopèdia lliure") com un indicador en el posicionament orgànic. És a dir, **els nostres webs tindran majors possibilitats d'aparèixer al capdamunt dels resultats de cerca si fem ús del protocol HTTPS**. És a dir, si estan certificats via [SSL](http://en.wikipedia.org/wiki/Transport_Layer_Security "Transport Layer Security - Wikipedia, the free encyclopedia").

##HTTPS a tot arreu. Com ho faig

Des de fa molt de temps hi ha empreses especialitzades en l'emissió de certificats de navegació segura. Aquestes empreses emeten diferents tipus de certificat amb diferents nivells d'encriptació. Algunes d'aquestes empreses són: Symantec, Thawte o GeoTrust. Els preus anuals d'emissió oscil·len entre els 150€ i els 400€. Un cop adquirit el nostre certificat caldrà configurar el nostre servidor web per tal d'acitivar-lo.

Ara bé, **i si hem apostat per la fórmula Jekyll [Github](https://konklone.com/post/github-pages-now-supports-https-so-use-it) amb domini propi? Doncs estem de sort!** Podem tenir els nostres webs segurs i millor posicionats, **com per exemple [#espaiSID](https://www.espaisid.com/)**, gràcies al servei universal SSL que ens ofereix [Cloudflare](https://www.cloudflare.com/index.html). I a més, sense cost addicional.

###Activant el servei universal SSL de Cloudflare

En primer lloc, hem de crear un compte a Cloudflare. No ens preocupem, és fàcil registrar-se! La part "difícil" és modificar el DNS al registrador de dominis, però si sabem allotjar el nostre codi a Github, sabem modificar registres DNS al registrador de dominis. Seguim les instruccions Cloudflare (hem d'apuntar els nostres servdidors de noms als de Cloudflare) i després configurem les nostres opcions preferides (per exemple podem "minimitzar" els nostres CSS i Javascript).

Hem d'habilitar SSL en la configuració Cloudflare i esperar-ne l'activació. L'última part és forçar HTTPS a totes les pàgines. Per fer això, hem d'anar a 'pages rules" i activar-ne l'opció. Molt fàcil!

##Per què és això important?

SSL és una capa de seguretat a través d'HTTP que impedeix que qualsevol un tercer pugui veure el contingut de les pàgines a les que accedim. Evita que les "escoltes" i per tant que get com la NSA sapiguen per on naveguem (o potser no :-)).

És una barrera de xifrat que és útil per evitar que algú sàpiga els nostres hàbits de navegació i les nostres que fem en un determinat lloc. Això és encara més rellevant quan ens connectem a xarxes wifi públiques, com la d'un aeroport o un hotel. 

A més a més, com hem dit al començament, **Google ha anunciat que millorarà el PageRank dels llocs web que tenen HTTPS!**



