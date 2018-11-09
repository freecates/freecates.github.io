---
comments: true
date: 2018-11-09 09:48:19
og: true
og-type: article
layout: blog
slug: "beneficios-fanoc-pwa-headless-wp-with-nextjs"
title: "Beneficios FANOC, una PWA amb Nextjs i WordPress API"
categories: 
  - comunicació
  - treballs
  - "no-cita"
tags: "case-study"
class: blog-article
"featured-img": true
"featured-img-url": "beneficios-fanoc-una-wppwa-case-study.png"
meta: "Beneficios Familias Nombroses Catalanes, una PWA amb Nextjs i WordPress API"
excerpt: "La creació d'aplicacions web progressives, PWA, és el futur de la Web i el 30% de tots els webs són WordPress. I si ho ajuntem? Això és BenFamCaNum: una PWA gestionada amb WordPress i 'presentada' amb Nextjs!"
author: oxygen
published: true
keywords: "empresa, digital, app, progressive, api, service, worker, chrome, push, beneficis, nextjs, react, now"
---

<blockquote>
  <p>... La creació d'aplicacions web progressives, PWA, és el futur de la Web i el 30% de tots els webs són WordPress. I si ho ajuntem? Això és BenFamCaNum: una PWA gestionada amb WordPress i 'presentada' amb Nextjs!</p>
  <footer>&mdash; <cite><a href="{{ page.url }}" title="{{ page.title }}">Ramon Gil</a></cite></footer>
</blockquote>

## El passat

**Els desenvolupadors i dissenyadors segueixen utilitzant l'arquitectura de PC i la Web basada en el navegador d'escriptori** i continuen desitjant poder accelerar-la als mòbils. Veiem aquest enfocament en els "embolcalls" per a aplicacions natives, personificats a per exemple PhoneGap (IE, Apache Còrdova), on les aplicacions web i llocs web estan escrites en HTML i CSS i després "embolicades" amb propietats natives (API hooks per al sistema operatiu i el maquinari del telèfon mòbil). El terme a la indústria per a aquests beuratges és aplicacions "híbrides". A dia d'avui, aquest és **un enfocament erroni en el desenvolupament multiplataforma** i en la construcció de les millors experiències Web i app.

## El Present

Si heu anat seguint el desenvolupament web el darrer any, és probable que hagueu llegit les Aplicacions Web Progressives (en anglès **PWAs**). És un concepte general utilitzat per descriure experiències web tan avançades que competeixen amb les aplicacions natives: el ple funcionament offline, la capacitat d'instal·lació, la ràpidesa, el comportament "suau" de l'aplicació al navegador, les notificacions push i una gran interfície d'usuari.

Les Aplicacions web progressives ("progressive web apps") és un concepte [exposat per primer cop per l'enginyer de Google Alex Russell el juny de 2015](https://infrequently.org/2015/06/progressive-apps-escaping-tabs-without-losing-our-soul/ "Progressive Web Apps: Escaping Tabs Without Losing Our Soul &#8211; Infrequently Noted"). En poques paraules, les aplicacions web progressives comencen com pestanyes als navegadors (Chrome, Firefox i aviat Safari) i **esdevenen progressivament més "aplicació"** a mida que més persones les utilitzen, fins al punt en què poden ser afegides a la pantalla principal del telèfon i tenir accés a propietats d'aplicació com ara notificacions i ús sense connexió. Les aplicacions web progressives són "linkables" via URL, completament responsives i segures.

## "Service Workers"

Els "Service Workers" poden fer que els llocs web funcionin fora de línia o ajudar a accelerar el contingut "interceptant les sol·licituds de xarxa per oferir respostes programàtiques o emmagatzemades a la memòria cau."

L'interessant dels "Service Workers" és que si poden interceptar, emmagatzemar i lliurar continguts a partir de sol·licutds de xarxa, també poden **tenir sempre a disposició l'arquitectura de l'aplicació ("Appication Shell Architecture")**, és a dir, la interfície bàsica i el disseny de l'aplicació web emmagatzemats i llests per lliurar-los gairebé a l'instant.

No obstant això, tot i que la nova API dels Service Worker permet emmagatzemar a la memòria cau tots els actius del lloc web per a una segona càrrega gairebé instantània, com quan conèixer algú nou, la primera impressió és el que compta. **Si la primera càrrega triga més de 3 segons**, un estudi de [DoubleClick](https://www.doubleclickbygoogle.com/articles/mobile-speed-matters/) mostra que **més del 53% de tots els usuaris ens abandonarà**. La [velocitat](https://www.doubleclickbygoogle.com/articles/mobile-speed-adds-up/) al mòbil sí importa.

## Millor una PWA que una app nativa

Un dels [avantatges](https://www.youtube.com/watch?v=z2JgN6Ae-Bo) més importants d'un lloc web és l'entrada gairebé sense fricció - és a dir, sense el pas de la instal·lació i amb la càrrega gairebé instantània. **Un usuari web és sempre a tan sols un clic de distància**. Per realment beneficiar-nos d'aquesta oportunitat cal ser molt ràpids! Per mantenir-nos, cal ser atractius.

<figure class="hidden-xs hidden-sm ox_animate_when_almost_visible ox_right-to-left"><img src="/assets/img/beneficios-fanoc-una-wppwa-full-width-snapshot.png" /><figcaption><p>beneficios.fanoc.org una aplicació web avançada!</p></figcaption></figure>

Al final el que importa és aconseguir una experiència d'usuari ideal. Hem d'anar tenint, de manera progressiva, una experiència de navegació cada cop més atractiva.

Sona massa bo per ser veritat? Doncs **justament això és [BenFamCaNum](https://beneficios.fanoc.org/ "Beneficios FANOC"), una sòlida comibació de tres tecnologies: PWA + WordPress (WP API) + React (NextJS)**

## Beneficios FANOC, una PWA amb React i WordPress API

A **Oxygen** apostem de totes totes per la construcció d'app webs que dugin a la millor experiència possible als seus usuaris per mitjà de les millors tecnologies disponibles en cada moment. És per això que hem creat **[BenFamCaNum](https://beneficios.fanoc.org/ "Beneficios FANOC")**, una mostra de les possibilitats reals d'una aplicació web progressiva, gestionada pel CMS més estés, WordPress, i presentada per mitjà de NextJS:

- Plenament responsiva
- De càrrega gairebé instantània gràcies al SSR del NextJS
- Indepentent de la connectivitat, ja que funciona "offline"
- Instal·lable a la pantalla d'inici
- Autogestionable gràcies al WP.

A més a més, de **segura** (funciona sota https) i **moderna** ja que separa estrictament el gestor de les dades (WordPress  + WP API) de la seva visualiztació (ReactJS / NextJS).

Aquesta és la segona iteració del concepte que duen a terme a Oxygen. Els avantatges del model **ens permeten crear una experiència customitada** per a FANOC a partir de compartir la mateixa API que la Federación Española de Familias Numerosas.

---

A [Oxygen.cat](http://www.oxygen.cat/) tenim la voluntat d'intentar anar un pas per endavant, **oferint allò que els nostres clients es mereixen: el millor servei i la millor innovació**!
