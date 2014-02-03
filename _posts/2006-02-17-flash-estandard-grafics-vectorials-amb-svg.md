---
comments: true
date: 2006-02-16 11:48:19
layout: blog
slug: flash-estandard-grafics-vectorials-amb-svg
title: "Flash estàndard: Gràfics vectorials amb SVG"
categories: [estàndards, general, no-cita]
tags:
meta: "Flash estàndard: Gràfics vectorials amb SVG"
excerpt: "L'animació d'objectes a la web i el disseny utilitzant gràfics vectorials ha estat dominat els últims deu anys per Macromedia. "
author: oxygen
keywords: estàndards, web, w3c, html, xhtml, xml, css, xslt
---

#Flash estàndard: Gràfics vectorials amb SVG

##Del Flash al SVG

L'animació d'objectes a la web i el disseny utilitzant gràfics vectorials ha estat dominat els últims deu anys per Macromedia. Un llenguatge basat en XML desenvolupat pel World Wide Web Consortium (W3C) anomenat Scalable Vector Graphics (SVG) ha a aparegut com a competidor i sembla que està guanyant terreny.

La història de la interactivitat utilitzant gràfics vectorials comença a principis dels anys noranta quan Macromedia va desenvolupar el Shockwave, un producte que va permetre als desenvolupadors multimèdia crear les primeres animacions amb una interactivitat mai vista fins aleshores.

Els primers navegadors van començar a suportar Shockwave utilitzant plugins però molt aviat Macromedia va veure que una versió reduïda podia ser distribuïda directament. És així quan el 1996 Macromedia va comprar FutureWave que amb el seu producte FutureSplash es va convertir en el Flash 1.0.

A mitjans dels anys noranta, va aparèixer un nou actor en el món de les dades gràcies a la senzillesa d'organitzar-les. Molts tipus de dades es van començar a representar en XML: representació d'informació matemàtica utilitzant MathML, gestió del coneixement amb RDF per a representar catàlegs de biblioteques, notícies o col·leccions de música, fotografies o agendes. Aquesta forma d'organitzar les dades són la base la creació de l'SVG.

L'any 1999 va sortir la primera especificació de l'SVG. Proporciona una estructura per a una definició vectorial de gràfics utilitzant XML que inclouen l'animació temporal, la gestió d'events i la modifiació de documents. Tot això fa que l'SVG sigui un ferm competidor del Flash, lliure i estàndard.

El principal problema per a la generalització del SVG és poca implantació en navegadors i la manca d'una eina estàndard d'autor. L'aparició del Firefox 1.5 que suporta SVG de forma nativa i el ràpid creixement dels últims temps de la utilització d'estàndards com XHTML i CSS en el desenvolupament d'alicacions web, fa pensar en un creixement molt ràpid d'aquesta tecnologia.

###Taula De Comparació De Flash I SVG

&nbsp; |Macromedia Flash| SVG
--- | --- |
Llicència oberta i estàndard| No |Si
Especificació| Macromedia SWF |Llicència del World Wide Web Consortium
Tipus de format| Binari |Text (XML llegible per humans)
Tipus MIME| application/x-shockwave-flash |image/svg+xml
Possibilitat de Streamming| Si |No
Interactivitat| Si. Utilitzant Scripts i Events |Si. Utilitzant Scripts, SMIL, i events
DOM| Intern |SVGDOM conforme amb la recomenació DOM Nivell 1
Z-Order (Ordenació de gràfics)| L'element amb més profunditat queda a dalt. Es pot modificar |Utilitza l'estructura de SVGDOM per a col·locar els objectes. L'últim element queda a dalt i es pot modificar utilitzant DOM
Compressió| Si. ZLIB |Si. GZIP
Suport natiu en navegadors| No. Però el "plugin" està instal·lat en la majoria de sistemes operatius i navegadors |Parcialment implementat en alguns navegadors. Plugin d'Adobe disponible.
Indexat pels cercadors| Per la majoria |Només alguns
Estils| Específic de SWF (Subconjunt de CSS) |Específic de SVG. Molt similar i compatible amb CSS2 i XSL

##Més info

- [The Web Standards Project](http://www.webstandards.org/ 'The Web Standards Project')
- [World Wide Web Consortium](http://www.w3.org/ 'World Wide Web Consortium')
- [Web Standards Group](http://webstandardsgroup.org/ 'Web Standards Group')
- [Web Standards Awards](http://www.webstandardsawards.com/ 'Web Standards Awards')