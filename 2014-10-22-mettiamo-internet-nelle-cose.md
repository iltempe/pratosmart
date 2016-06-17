---
id: 1386
title: Mettiamo internet nelle cose
date: 2014-10-22T22:00:27+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=1386
permalink: /mettiamo-internet-nelle-cose/
dsq_thread_id:
  - 3145415925
categories:
  - Arduino
  - Internet Nelle Cose
  - Laboratorio
tags:
  - arduino yun
  - iot
---
##### Da oggi anche dato quanto presentato ad #<a title="#HACKTOSCANA : ha vinto la LEGO ;-)" href="http://pratosmart.teo-soft.com/hacktoscana-ha-vinto-la-lego/" target="_blank">hacktoscana</a> ho deciso di dar vita alla rubrica **Internet Nelle Cose** uno spazio dove sperimentare con voi cosa significa inserire internet negli oggetti.

Iniziamo col dire che inserire internet negli oggetti oggi è diventato cosa assai economica e di media complessità. Non ci credete?

<p style="text-align: justify;">
  Stasera vi presento la piattaforma su cui inizieremo a <em>smanettare</em>: <a href="http://arduino.cc/en/Main/ArduinoBoardYun?from=Products.ArduinoYUN" target="_blank">Arduino Yun</a>. Si tratta di una particolare versione Arduino che presenta già in forma integrata la gestione non solo di possibili sensori e attuatori ma anche di connessioni internet (cablata e wifi). La scelta ricade cu questa versione perché per un costo di circa 60 euro avete quindi in una scheda sola tutto quello che Arduino consente di fare più la possibilità di connettersi in rete con una applicazione client o server installata direttamente sul dispositivo.
</p>

<p style="text-align: justify;">
  Stasera ho provato a sviluppare un sito web su Arduino Yun. Avete capito bene. Dato che su Arduino Yun esiste un processore con un suo sistema operativo mi è venuto in mente un&#8217;idea per poter interfacciarsi con la parte di sensori di Arduino direttamente da una semplice applicazione web. Ovviamente nulla si inventa da 0, <a href="http://grallator.wordpress.com/2014/01/13/json-and-the-arduino-yun/" target="_blank">qui</a> trovate l&#8217;applicazione da cui sono partito e <a href="https://github.com/TeoSoft80/Yun-and-Json-Data" target="_blank">qui</a> il mio codice sorgente. Il codice è composto da uno sketch Arduino Yun e una applicazione web HTML5 e JS. Dateci un&#8217;occhiata.
</p>

<p style="text-align: justify;">
  L&#8217;idea di base è semplice: l&#8217;applicazione web consente di
</p>

<li style="text-align: justify;">
  definire per ogni pin la tipologia (input o output)
</li>
<li style="text-align: justify;">
  impostare il livello delle uscite
</li>
<li style="text-align: justify;">
  leggere gli input digitali e analogici
</li>

Il tutto, sebbene avvenga con i ritardi delle richieste dalla pagina web, permette di avere un semplice controllo della piattaforma via rete.

Le richieste verso Arduino sono fatte in Javascript ed i dati sono resi in forma JSON.

La app è utilizzabile connettendo Arduino alla vostra rete WIFI di casa e consente un controllo completo anche da dispositivi mobile: perdonate i tecnicismi spero sia chiaro il concetto di fondo, nelle prossime puntate per chiarire dove voglio andare a parare vedremo come si può espandere la dashboard e la piattaforma Arduino per creare degli oggetti connessi 😉

<!-- Flickr Photostream by Miro Mannino -->

<div id="flickrGal9" class="justified-gallery" >
  <a href="https://www.flickr.com/photos/125814874@N05/15579629936/in/set-72157646588168074/lightbox" target="_blank" title="Schermata 2014-10-22 alle 22.44.48"><img alt="Schermata 2014-10-22 alle 22.44.48" src="https://farm6.static.flickr.com/5612/15579629936_4e73d89c3a_m.jpg" data-safe-src="https://farm6.static.flickr.com/5612/15579629936_4e73d89c3a_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15603303855/in/set-72157646588168074/lightbox" target="_blank" title="Schermata 2014-10-22 alle 22.45.02"><img alt="Schermata 2014-10-22 alle 22.45.02" src="https://farm6.static.flickr.com/5600/15603303855_3fef3cb4ff_m.jpg" data-safe-src="https://farm6.static.flickr.com/5600/15603303855_3fef3cb4ff_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15604139372/in/set-72157646588168074/lightbox" target="_blank" title="Schermata 2014-10-22 alle 22.45.12"><img alt="Schermata 2014-10-22 alle 22.45.12" src="https://farm4.static.flickr.com/3946/15604139372_72ffb34413_m.jpg" data-safe-src="https://farm4.static.flickr.com/3946/15604139372_72ffb34413_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/14983208043/in/set-72157646588168074/lightbox" target="_blank" title="IMG_2458"><img alt="IMG_2458" src="https://farm4.static.flickr.com/3935/14983208043_02022d4e12_m.jpg" data-safe-src="https://farm4.static.flickr.com/3935/14983208043_02022d4e12_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15603352995/in/set-72157646588168074/lightbox" target="_blank" title="IMG_2459"><img alt="IMG_2459" src="https://farm4.static.flickr.com/3949/15603352995_cac2b575bf_m.jpg" data-safe-src="https://farm4.static.flickr.com/3949/15603352995_cac2b575bf_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15600689361/in/set-72157646588168074/lightbox" target="_blank" title="IMG_2460"><img alt="IMG_2460" src="https://farm6.static.flickr.com/5600/15600689361_b599dfba0a_m.jpg" data-safe-src="https://farm6.static.flickr.com/5600/15600689361_b599dfba0a_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15720806012/in/set-72157646588168074/lightbox" target="_blank" title="IMG_2502"><img alt="IMG_2502" src="https://farm6.static.flickr.com/5616/15720806012_c9bb74d19e_m.jpg" data-safe-src="https://farm6.static.flickr.com/5616/15720806012_c9bb74d19e_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15534421040/in/set-72157646588168074/lightbox" target="_blank" title="IMG_2503"><img alt="IMG_2503" src="https://farm6.static.flickr.com/5597/15534421040_99d6477e17_m.jpg" data-safe-src="https://farm6.static.flickr.com/5597/15534421040_99d6477e17_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15720819782/in/set-72157646588168074/lightbox" target="_blank" title="IMG_2505"><img alt="IMG_2505" src="https://farm6.static.flickr.com/5604/15720819782_7bebe2192d_m.jpg" data-safe-src="https://farm6.static.flickr.com/5604/15720819782_7bebe2192d_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15099877873/in/set-72157646588168074/lightbox" target="_blank" title="IMG_2504"><img alt="IMG_2504" src="https://farm4.static.flickr.com/3955/15099877873_b2fb04e46c_m.jpg" data-safe-src="https://farm4.static.flickr.com/3955/15099877873_b2fb04e46c_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15099323254/in/set-72157646588168074/lightbox" target="_blank" title="IMG_2511"><img alt="IMG_2511" src="https://farm8.static.flickr.com/7529/15099323254_1a49048837_m.jpg" data-safe-src="https://farm8.static.flickr.com/7529/15099323254_1a49048837_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15719274115/in/set-72157646588168074/lightbox" target="_blank" title="IMG_2512"><img alt="IMG_2512" src="https://farm6.static.flickr.com/5603/15719274115_af5aaf4267_m.jpg" data-safe-src="https://farm6.static.flickr.com/5603/15719274115_af5aaf4267_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15533392009/in/set-72157646588168074/lightbox" target="_blank" title="IMG_2513"><img alt="IMG_2513" src="https://farm8.static.flickr.com/7474/15533392009_ce6d079bdd_m.jpg" data-safe-src="https://farm8.static.flickr.com/7474/15533392009_ce6d079bdd_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15534416540/in/set-72157646588168074/lightbox" target="_blank" title="IMG_2514"><img alt="IMG_2514" src="https://farm4.static.flickr.com/3956/15534416540_78e7af851d_m.jpg" data-safe-src="https://farm4.static.flickr.com/3956/15534416540_78e7af851d_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15534062957/in/set-72157646588168074/lightbox" target="_blank" title="IMG_2515"><img alt="IMG_2515" src="https://farm4.static.flickr.com/3939/15534062957_678bcf5a1a_m.jpg" data-safe-src="https://farm4.static.flickr.com/3939/15534062957_678bcf5a1a_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15099885193/in/set-72157646588168074/lightbox" target="_blank" title="IMG_2517"><img alt="IMG_2517" src="https://farm8.static.flickr.com/7537/15099885193_5e2537e86d_m.jpg" data-safe-src="https://farm8.static.flickr.com/7537/15099885193_5e2537e86d_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15533370079/in/set-72157646588168074/lightbox" target="_blank" title="IMG_2518"><img alt="IMG_2518" src="https://farm6.static.flickr.com/5600/15533370079_b0e2b3ca06_m.jpg" data-safe-src="https://farm6.static.flickr.com/5600/15533370079_b0e2b3ca06_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15549320348/in/set-72157646588168074/lightbox" target="_blank" title="Raspberry Send Mail"><img alt="Raspberry Send Mail" src="https://farm6.static.flickr.com/5605/15549320348_f284f85b34_m.jpg" data-safe-src="https://farm6.static.flickr.com/5605/15549320348_f284f85b34_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15549320808/in/set-72157646588168074/lightbox" target="_blank" title="Raspberry Send Mail"><img alt="Raspberry Send Mail" src="https://farm6.static.flickr.com/5600/15549320808_a3e6887c17_m.jpg" data-safe-src="https://farm6.static.flickr.com/5600/15549320808_a3e6887c17_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15734770435/in/set-72157646588168074/lightbox" target="_blank" title="Raspberry Send Mail"><img alt="Raspberry Send Mail" src="https://farm6.static.flickr.com/5608/15734770435_274fa8bab7_m.jpg" data-safe-src="https://farm6.static.flickr.com/5608/15734770435_274fa8bab7_m.jpg" /></a>
</div>

&nbsp;