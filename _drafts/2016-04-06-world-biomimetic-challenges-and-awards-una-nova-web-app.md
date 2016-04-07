---
comments: true
date: 2016-04-06 11:48:19
og: true
og-type: article
layout: blog
slug: "world-biomimetic-challenges-and-awards-una-nova-web-app"
title: "World Biomimeitc Challenges and Awards. Una nova web app"
categories: 
  - comunicació
  - treballs
  - "no-cita"
tags: "case-study"
"featured-img": true
"featured-img-url": "world-biomimetic-challenges-and-awards-case-study.png"
meta: "World Biomimeitc Challenges and Awards. Una nova web app"
excerpt: "La creació d'aplicacions web progressives és el futur de la Web, ja que l'arquitectura d'aplicació tipus closca, el·liminarà la necessitat d'aplicacions híbrides."
author: oxygen
published: true
keywords: "biomimetics, screens, digital, app, challenges, polymer, api, service, worker, chrome, push, notifications"
---

>... the first edition of World Biomimetics Challenges & Awards... is well underway for the coming World Biomimetic Experience Summit 2017 that will get to know a new social, economic and industrial reality by a bioinspirer Cosmo vision.<footer>&mdash; <cite><a href="{{ page.url }}" title="{{ page.title }}">Daniel Fuentes</a></cite></footer>

El proper 22 de juny (2016) tindrà lloc la primera edició dels 'World Biomimetic Challenges and Awards'. Un esdeveniment de caire internacional que pretén: 

- Donar a conèixer la biomimètica per contribuir a la seva implementació en la societat, atenent al desenvolupament integral de l'ésser humà, de les comunitats que el formen i del planeta que el sustenta.
- Apropar la dimensió creativa de la Naturalesa als límits de la imaginació humana.
- Ser un altaveu de reconeixament de projectes que promouen la consciencia, el talent i la creativitat biomimètica per afrontar els desafiaments globals de futur.
- Donar coneixement del 1st World Biomimetics Experience Summit 2017.
- Fomentar un espai de consciència col·lectiva desde una cosmovisió biomimètica.

## Els WBChA, una sigle page web app

[Els WBChA](https://www.biomimeticchallengesandawards.com/) estan concebuts com una single page web app, de manera què **en un sol "html" hi troben tot el que cal per posicionar l'esdevinent a Internet**. És a dir, en accedir a [https://www.biomimeticchallengesandawards.com/](https://www.biomimeticchallengesandawards.com/) ho tenim tot: el què, el qui, el quan i l'on harmònicament distribuït amb diferents "call to action."

Hem desenvolupat la pàgina d'un esdeveniment i l'hem dotat d'elements de "[progressive web app](/progressive-web-apps-el-futur-de-la-web/)": **notificacions push i accés offline**.

## El passat

**Els desenvolupadors i dissenyadors segueixen utilitzant l'arquitectura de PC i la Web basada en el navegador d'escriptori** i continuen desitjant poder accelerar-la als mòbils. Veiem aquest enfocament en els "embolcalls" per a aplicacions natives, personificats a per exemple PhoneGap (IE, Apache Còrdova), on les aplicacions web i llocs web estan escrites en HTML i CSS i després "embolicades" amb propietats natives (API hooks per al sistema operatiu i el maquinari del telèfon mòbil). El terme a la indústria per a aquests beuratges és aplicacions "híbrides". A dia d'avui, aquest és **un enfocament erroni en el desenvolupament multiplataforma** i en la construcció de les millors experiències Web i app.

## El Futur

Hi ha yna nova arquitectura que ajudarà a tancar la bretxa entre el rendiment de la web i el de les aplicacions natives i, finalment, pot proporcionar **la solució per a la creació d'aplicacions i llocs web que són ràpids i fiables a l'era mòbil**.

Les Aplicacions web progressives ("progressive web apps") és un concepte [exposat per primer cop per l'enginyer de Google Alex Russell el juny de 2015](https://infrequently.org/2015/06/progressive-apps-escaping-tabs-without-losing-our-soul/ "Progressive Web Apps: Escaping Tabs Without Losing Our Soul &#8211; Infrequently Noted"). En poques paraules, les aplicacions web progressives comencen com pestanyes al navegador Chrome i **esdevenen progressivament més "aplicació"** a mida que més persones les utilitzen, fins al punt en què poden ser afegides a la pantalla principal del telèfon i tenir accés a propietats d'aplicació com ara notificacions i ús sense connexió. Les aplicacions web progressives són "linkables" via URL, completament responsives i segures.

Per a la velocitat i funcionalitat, les aplicacions web progressistes **es basen en dues funcions: l'[arquitectura d'aplicació tipus closca](https://developers.google.com/web/updates/2015/11/app-shell "Instant Loading Web Apps with An Application Shell Architecture | Web Updates - Google Developers") ("Application Shell Architecture") i els "[Service Workers](http://blog.chromium.org/2014/12/chrome-40-beta-powerful-offline-and.html "Chromium Blog: Chrome 40 Beta: Powerful Offline and Lightspeed Loading with Service Workers")"**.

## "Service Workers" i "Application Shell Architecture"

Els "Service Workers" poden fer que els llocs web funcionen fora de línia o ajudar a accelerar el contingut "interceptant les sol·licituds de xarxa per oferir respostes programàtiques o emmagatzemades a la memòria cau."

L'interessant dels "Service Workers" és que si poden interceptar, emmagatzemar i lliurar continguts a partir de sol·licutds de xarxa, també poden **tenir sempre a disposició l'arquitectura de l'aplicació ("Appication Shell Architecture")**, és a dir, la interfície bàsica i el disseny de l'aplicació web emmagatzemats i llests per lliurar-los gairebé a l'instant.

D'aquesta manera, la "closca" ("shell") de l'aplicació és **lliurada de manera instantània en el mateix moment que algú fa una petició des del seu mòbil**.


<figure class="hidden-xs hidden-sm ox_animate_when_almost_visible ox_right-to-left"><img src="/assets/img/world-biomimetic-challenges-and-awards-full-width-snapshot.png" /><figcaption><p>digitalartbarcelona.com, el millor web possible per a la II Mostra Simultània d'Art Digital</p></figcaption></figure>

## Com a mostra un botó: ArtinpocketShowcase

La implementació dels "Service Workers" juntament amb l'arquitectura tipus "closca" tot just està començant. Ara bé, totes les eines ja estan disponibles (en diversos graus de maduresa). Tot és a punt per als desenvolupadors que ja vulguin fer el pas.

A **Oxygen** apostem de totes totes per la construcció d'app webs que dugin a la millor experiència possible als seus usuaris per mitjà de les millors tecnologies disponibles en cada moment. És per això que hem creat **[Artinpocketshowcase](https://artinpocketshowcase.appspot.com/)**, una mostra de les possibilitats reals d'una aplicació web progressiva. Artinpocketshowcase és<sup><a href="#fn1" id="r1">[1]</a></sup>:

- Plenament responsiva
- De càrrega gairebé instantània
- Indepentent de la connectivitat, ja que funciona "offline"
- Instal·lable
- Atractiva ja que disposa de la capacitat per retenir els usuaris via notifacions no intrusives de nous contignuts.
- Modular via Polymer

En aquest projecte hem seguit apostant pels [web components](http://webcomponents.org/ "WebComponents.org"), una veritable revolució en el desenvolupament web, per mitjà de [Polymer](http://www.polymer-project.org/ "Welcome - Polymer"), l'"opinionated framework" creat per Google.

<pre>
  <code>
        &#60;template is="dom-if" if="&#123;&#123;article.categoryaday&#125;&#125;" restamp="true"&#62;
          &#60;section class="main"&#62;
              &#60;template is="dom-repeat" items="&#123;&#123;article.desc&#125;&#125;"&#62;
                &#60;dl&#62;
                  &#60;dt&#62;&#60;strong&#62;&#123;&#123;item.pregunta&#125;&#125;&#60;/strong&#62;&#60;/dt&#62;
                  &#60;dd&#62;&#123;&#123;item.resposta&#125;&#125;&#60;/dd&#62;
                &#60;/dl&#62;
              &#60;/template&#62;
            &#60;/section&#62;
        &#60;/template&#62;
  </code>
</pre>

A [Oxygen.cat](http://www.oxygen.cat/) tenim la voluntat d'intentar anar un pas per endavant, **oferint allò que els nostres clients es mereixen: el millor servei i la millor innovació**!

---

<section>
 <p id="fn1"><small><a href="#r1">[1]</a> Les funcionalitats d'aquesta app estan optimitzades per als navegador Chrome Desktop i Chrome Android a partir de la versió 47.</small></p>
</section>

---