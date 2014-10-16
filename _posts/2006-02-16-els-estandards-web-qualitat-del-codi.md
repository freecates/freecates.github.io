---
comments: true
date: 2006-02-16 11:48:19
layout: blog
slug: els-estandards-web-qualitat-del-codi
title: "Els estàndards web: qualitat del codi"
categories: [estàndards, general, no-cita]
tags:
meta: "Els estàndards web: qualitat del codi"
excerpt: "Per als estàndards HTML i XHTML, la declaració de tipus de document, DOCTYPE informa al validador de quina versió de (X)HTML esteu utilitzant"
author: oxygen
keywords: estàndards, web, w3c, html, xhtml, xml, css, xslt
---

##Utilització d'un Doctype correcte

Per als estàndards **HTML** i **XHTML**, la declaració de tipus de document, DOCTYPE informa al validador de quina versió de (X)HTML esteu utilitzant. Ha d'aparèixer com a principi de qualsevol pàgina i són un component clau per a que les pàgines compleixin amb els estàndards;  per exemple que es validin els CSS. Són essencials per tal que les pàgines web funcionin i es vegin correctament amb browsers com Mozilla, IE5/Mac, and IE6/Win.

Utilitzar un [DOCTYPE](http://www.w3.org/QA/2002/04/Web-Quality 'W3C QA - How to achieve Web standards and quality on your Web site?') incorrecte o incomplet o no utilitzar-ne, fa que aquests browsers passin a utilitzar el mode **“Quirks”**, on assumeixen que esteu utilitzant un codi invàlid i intentarà “parsejar” les pàgines i els CSS tal i com s'haurien visialitzat en navegadors antics com l'IE4 o el Netscape6.

##Utilització d'un joc de caràcters.

Els documents transmesos amb HTTP que són de tipus text, com per exemple text/html, text/plain, etc.. han de tenir el paràmetre charset establert per tal d'especificar la codificació de caracters del document.

És molt important etiquetar els documents web de forma explícita. L'**HTTP 1.1** especifica que el charset per defecte és l' **ISO-8859-1**. El que passa és que els navegadors utilitzen la codificació seleccionada per l'usuari en la configuració quan el document no està etiquetat.

En les capceleres HTTP, normalment hi està especificat de la forma següent:

- Content-Type: text/html; charset=iso-8859-1

En teoria, es pot utilitzar qualsevol codificació que ha estat registrada per l'[IANA](http://www.iana.org/assignments/character-sets/character-sets.xhtml 'Character Sets'), però no hi ha cap navegador3 que els tingui tots inclosos.

Per a l'XML i l'HTML 4.0, el charset és Unicode (aka ISO 10646). Això vol dir que els navegadors HTML i els processadors XML, s'han de comportar com si utilitzessin internament Unicode. Però això no vol dir forçosament que els documents hagin estat transmesos utilitzant Unicode.

És molt important que la codificació de caràcters estigui fixada a tots els documents XML o (X)HTML i es pot fer d'una de les maneres següents:

1. Utilitzar el paràmetre 'charset' a la capçalera Content-Type de l'HTTP. Content-Type: text/html; charset=EUC-JP
2. Pera l'XML, utilitzar un atribut a la decleració d'XML a l'inic del document:<?xml version="1.0" encoding="iso-8859-1" ?>
3. Pe-r a l'HTML utilitzar un tage <meta> a l'interior del <head>. <meta http-equiv="Content-Type" content="text/html;charset=utf-8" >
4. Per a XHTML: <meta http-equiv="Content-Type" content="text/html;charset=utf-8" />

Amb aquesta informació, els clients podran mapejar fàcilment aquesta codificació a Unicode. A la pràctica molt poques codificacions es poden utilitzar: UTF-8 , ISO-8859-1 (Latin-1), US-ASCII, UTF-16, i altres codificacions a les sèries ISO-8859, iso-2022-jp, euc-kr.

##Utilització d'un (X)HTML vàlid

Podem utilitzar bàsicament dos tipus d'HTML:

- **HTML 4**: Es pot definir l'HTML 4 com una aplicació de l'**SGML** (Standard Generalized Markup Language) un estàndar internacional: ISO 8879 i és plenament reconegut com l'estàndard per a la publicació de pàgines a la web. L'SGML és un llenguatge per a descriure i intercanviar electrònicament documents, l'HTML és un exemple d'un llenguatge definit en **SGML**. L'SGML, definit a mitjans dels 80, és molt flexible i s'ha matingut molt estable; aquesta flexibilitat, ens fa pagar el preu que s'ha arribat a un nivell de complexitat en els documents en el moment que s'ha adoptat en entorns com la web. L'HTML va ser concebut per a l'intercanvi de documents científics, simplificant l'SGML amb un subconjunt de “tags” semàntics molt útils per a crear documents molt símples i afegint suport per a l'hipertext (enllaç simbòlic entre documents).

	En molt poc temps, l'HTML s'ha popularitzat molt i ha superat el seu propòsit inicial, adoptant funcions multimèdia i molts elements molt especialitzats. Tots aquests nous elements, ha portat a molts problemes d'interoperatibilitat per a documents entre plataformes diferents.

- **XHTML**: XHTML és un una reformulació molt més estricte de l'HTML4 basat en XML, per tant, els documents XHTML poden ser visualitzat, editats i validats utilitzant totes les eines XML. També, els documents XHTML es poden escriure per a que operin tant bé o millor amb els navegadors pensats per a HTML 4 com a nous navegadors ja pensats per a XHTML. Amb una sintaxi més esticta però amb les mateixes possibilitats d'expresió que l'HTML, permet que els documents siguin tractats amb les llibreries estàndards de XML; un “parser” molt més senzill que els de l'HTML que han de ser específics. L'XHTML 1.0 és un estàndard del World Wide Web Consortium4 (W3C), des del 26 de gener de l'any 2000.

##Més info

- [The Web Standards Project](http://www.webstandards.org/ 'The Web Standards Project')
- [World Wide Web Consortium](http://www.w3.org/ 'World Wide Web Consortium')
- [Web Standards Group](http://webstandardsgroup.org/ 'Web Standards Group')
- [Web Standards Awards](http://www.webstandardsawards.com/ 'Web Standards Awards')