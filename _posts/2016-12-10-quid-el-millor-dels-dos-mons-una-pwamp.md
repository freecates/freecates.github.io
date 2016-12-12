---
comments: true
date: 2016-12-10 11:48:19
og: true
og-type: article
layout: blog
slug: "quid-el-millor-dels-dos-mons-una-pwamp"
title: "QUID, el millor dels dos móns: una PWAMP"
categories: 
  - comunicació
  - treballs
  - "no-cita"
tags: "case-study"
"featured-img": true
"featured-img-url": "quid-una-pwamp-case-study.png"
meta: "QUID, el millor dels dos móns: una PWAMP"
excerpt: "La creació d'aplicacions web progressives és el futur de la Web, la carrega instantània al mòbil una abosluta necessitat. La combinació és una PWAMP. I això és QUID, el millor dels dos móns!"
author: oxygen
published: true
keywords: "quid, cultura. empresa, screens, digital, app, progressive, api, service, worker, chrome, push, notifications, travis, gulp, amp"
---

<blockquote>
  <p>... La creació d'aplicacions web progressives és el futur de la Web, la carrega instantània al mòbil una abosluta necessitat. La combinació és una PWAMP. I això és QUID, el millor dels dos móns!</p>
  <footer>&mdash; <cite><a href="{{ page.url }}" title="{{ page.title }}">Ramon Gil</a></cite></footer>
</blockquote>

## El passat

**Els desenvolupadors i dissenyadors segueixen utilitzant l'arquitectura de PC i la Web basada en el navegador d'escriptori** i continuen desitjant poder accelerar-la als mòbils. Veiem aquest enfocament en els "embolcalls" per a aplicacions natives, personificats a per exemple PhoneGap (IE, Apache Còrdova), on les aplicacions web i llocs web estan escrites en HTML i CSS i després "embolicades" amb propietats natives (API hooks per al sistema operatiu i el maquinari del telèfon mòbil). El terme a la indústria per a aquests beuratges és aplicacions "híbrides". A dia d'avui, aquest és **un enfocament erroni en el desenvolupament multiplataforma** i en la construcció de les millors experiències Web i app.

## El Present

Si heu anat seguint el desenvolupament web aquests darrers mesos, és probable que hagueu llegit les Aplicacions Web Progressives (en anglès **PWAs**). És un concepte general utilitzat per descriure experiències web tan avançades que competeixen amb les aplicacions natives: el ple funcionament offline, la capacitat d'instal·lació, "Retina", la ràpidesa, el comportament "suau" de l'aplicació al navegador, les notificacions push i una gran interfície d'usuari.

Les Aplicacions web progressives ("progressive web apps") és un concepte [exposat per primer cop per l'enginyer de Google Alex Russell el juny de 2015](https://infrequently.org/2015/06/progressive-apps-escaping-tabs-without-losing-our-soul/ "Progressive Web Apps: Escaping Tabs Without Losing Our Soul &#8211; Infrequently Noted"). En poques paraules, les aplicacions web progressives comencen com pestanyes al navegador Chrome i **esdevenen progressivament més "aplicació"** a mida que més persones les utilitzen, fins al punt en què poden ser afegides a la pantalla principal del telèfon i tenir accés a propietats d'aplicació com ara notificacions i ús sense connexió. Les aplicacions web progressives són "linkables" via URL, completament responsives i segures.

## "Service Workers"

Els "Service Workers" poden fer que els llocs web funcionen fora de línia o ajudar a accelerar el contingut "interceptant les sol·licituds de xarxa per oferir respostes programàtiques o emmagatzemades a la memòria cau."

L'interessant dels "Service Workers" és que si poden interceptar, emmagatzemar i lliurar continguts a partir de sol·licutds de xarxa, també poden **tenir sempre a disposició l'arquitectura de l'aplicació ("Appication Shell Architecture")**, és a dir, la interfície bàsica i el disseny de l'aplicació web emmagatzemats i llests per lliurar-los gairebé a l'instant.

No obstant això, tot i que la nova API dels Service Worker permet emmagatzemar a la memòria cau tots els actius del lloc web per a una segona càrrega gairebé instantània, com quan conèixer algú nou, la primera impressió és el que compta. **Si la primera càrrega triga més de 3 segons**, l'últim estudi de [DoubleClick](https://www.doubleclickbygoogle.com/articles/mobile-speed-matters/) mostra que **més del 53% de tots els usuaris ens abandonarà**.

## AMP, per a Pàgines Mòbils Accelerades

Un dels avantatges més importants d'un lloc web és l'entrada gairebé sense fricció - és a dir, sense el pas de la instal·lació i amb la càrrega gairebé instantània. Un usuari és sempre a un clic de distància. Per realment beneficiar-nos d'aquesta oportunitat l'únic que **necessitem és un lloc web "fotudament" ràpid!** [AMP](https://www.ampproject.org/), abreviatura de pàgines mòbils accelerades, la clava en això. De fet, és la seva raó de ser! ... tot i que a costa d'haver de ser extramadament respectuosos a l'hora de desenvolupar amb les restriccions que imposa.

<figure class="hidden-xs hidden-sm ox_animate_when_almost_visible ox_right-to-left"><img src="/assets/img/quid-una-pwamp-full-width-snapshot.png" /><figcaption><p>QUID.cat el millor dels dos móns!</p></figcaption></figure>

## [QUID.cat](https://www.quid.cat/ "QUID, Connectem Empresa i Cultura") el millor dels dos móns!

Al final el que importa és aconseguir una experiència d'usuari ideal. Més o menys hauria de ser així:

1. Un usuari descobreix un enllaç cap al nostre web i fa clic.
2. El contingut es carrega gairebé instantàniament i és un plaer consumir-lo.
3. Automàticament es convida l'usuari a una experiència encara més rica, amb les notificacions push i el funcionament offline.
4. L'usuari exclama: "I tant, és clar que sí!" I en un instant el redirigim a una experiència similar al d'una app nativa i se'l pot instal·lar a la pantalla d'inici.

La primera càrrega del nostre web l'hem de sentir com gairebé instantània, i després hem d'anar tenint una experiència de navegació cada cop més atractiva.

Sona massa bo per ser veritat? Doncs **justament això és [QUID](https://www.quid.cat/ "QUID, Connectem Empresa i Cultura"), el millor dels dos móns! Una sòlida comibació de les dues tecnologies: PWA + AMP**

A **Oxygen** apostem de totes totes per la construcció d'app webs que dugin a la millor experiència possible als seus usuaris per mitjà de les millors tecnologies disponibles en cada moment. És per això que hem creat **[QUID](https://www.quid.cat/ "QUID, Connectem Empresa i Cultura")**, una mostra de les possibilitats reals d'una aplicació web progressiva amb pàgines mòbils accelerades. **QUID és una PWAMP!** (PWA + AMP):

- Plenament responsiva
- De càrrega gairebé instantània en qualsevol escenari
- Indepentent de la connectivitat, ja que funciona "offline"
- Instal·lable a la pantalla d'inici
- Atractiva ja que disposa de la capacitat per retenir els usuaris via notifacions no intrusives de nous contignuts.

A més a més, de **segura** (funciona sota https) i **moderna** ja que té un flux de publicació basat en 2 respositoris **github** i compilació via **travis** amb **gulp**. D'això en seguirem parlant en una altra ocasió.

---

A [Oxygen.cat](http://www.oxygen.cat/) tenim la voluntat d'intentar anar un pas per endavant, **oferint allò que els nostres clients es mereixen: el millor servei i la millor innovació**!