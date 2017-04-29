---
id: 1446
title: Abbiamo bisogno di dati, ma anche di dashboard
date: 2014-11-12T00:38:24+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=1446
permalink: /abbiamo-bisogno-di-dati-ma-anche-di-dashboard/
dsq_thread_id:
  - 3215558170
categories:
  - Hackers
  - Internet Nelle Cose
tags:
  - freeboard
  - iot
  - node-red
  - raspberry
---
<p style="text-align: justify;">
  Oggi riflettevo su un concetto: noi non possiamo limitarci a lavorare sul rendere digitali i dati aprendoli tramite sensori e persone che ci lavorino. Occorre di più: occorrono tutti gli strumenti per poterli leggere e interpretare e serve rendere semplice il loro utilizzo.
</p>

<p style="text-align: justify;">
  E&#8217; questo che agevola il riuso e la decision making in merito a ciò che vediamo.
</p>

<p style="text-align: justify;">
  Insomma, per citare un intervento di&nbsp;<a href="http://www.michelecamp.it/" target="_blank">Michele Vianello</a>&nbsp;che rivedevo in questi giorni&nbsp;noi &#8220;avremo sempre più bisogno di dashboard&#8221;: cioè servono spazi per visualizzare in modo semplice le informazioni (o una parte di esse) con le quali vogliamo interagire.
</p>

<p style="text-align: justify;">
  Chi mi ha ascoltato quando dicevo che gli opendata vanno spiegati ha capito bene cosa intendo.
</p>

<p style="text-align: justify;">
  Non sono qui a presentarvi un prodotto, ma una soluzione.
</p>

<h6 style="text-align: justify;">
  Ecco perché oggi mi son servito della mia piattaforma IOT per provare a spiegare come sarebbe fatta <strong>la dashboard di pratosmart</strong>. Iniziamo col dire che dietro la dashboard vive un <a title="Come si fa il primo setup di un Raspberry B+" href="http://pratosmart.teo-soft.com/come-si-fa-il-primo-setup-di-un-raspberry-b/" target="_blank">Raspberry B+</a>&nbsp;su cui si è installato <a href="http://nodered.org/" target="_blank">Node-Red</a> e <a href="https://freeboard.io/" target="_blank">Freeboard</a>. Come mai questa scelta? Ci sono vari motivi:
</h6>

<li style="text-align: justify;">
  In primis questo ci consente di avere una piattaforma indipendente su cui installare dei &#8220;job&#8221; che vengono eseguiti in tempo reale e sono completamente svincolati dai nostri dispositivi di comune utilizzo.
</li>
<li style="text-align: justify;">
  Raspberry è una piattaforma aperta su cui è possibile (volendo) ampliare Node-Red installando altri &#8220;nodi&#8221;
</li>
<li style="text-align: justify;">
  Raspberry è altamente portabile come oggetto
</li>
<li style="text-align: justify;">
  Raspberry nasce per connettere oggetti in internet
</li>

Una volta <a title="Come si fa il primo setup di un Raspberry B+" href="http://pratosmart.teo-soft.com/come-si-fa-il-primo-setup-di-un-raspberry-b/" target="_blank">configurata la piattaforma</a>, installate Node-Red e Freeboard e interagiteci da un normalissimo browser. Potete usare fonti di dati di vario tipo Feed Rss, Tweet, dati archiati in formato CSV. Pensate quindi di usare tutte le fonti di dati (aperte e no) riguardanti la vostra città così da aggrgarle.

<p style="text-align: justify;">
  <img class="size-large wp-image-1447 alignleft" src="http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/1-1024x379.jpg" alt="1" width="656" height="242" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/1-300x111.jpg 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/1-1024x379.jpg 1024w" sizes="(max-width: 656px) 100vw, 656px" />Avrete la possibilità di agire (in modo grafico utilizzando metodi drag and drop) da una parte in un backend che fungerà da server sul quale creerete la vostra applicazione (nel prototipo di esempio si tratta banalmente di una applicazione che raccoglie tweet con alcuni hashtag definiti come #pratosmart o #prato). Ovviamente in questo backend dovrete predisporre elementi di websocket laddove volete trasferire le informazioni dal back al front. In secondo luogo avrete una pagina dove con Freeboard potrete configurare la vostra dashboard e visualizzare le informazioni che vi occorrono.
</p>

<p style="text-align: justify;">
  Freeboard è un&#8217;ottima soluzione, altamente configurabile, che vi consente di definire un set di fonti da cui prelevare i dati (in questo caso dai vostri websocket, ma potete prelevarli anche da fonti web di diverso tipo) e visualizzarli tramite degli widget di vari formati. Per il momento mi sono limitato ad un semplice prototipo ma capite bene che cominciando a connettere Raspberry ad altri dispositivi elettronici o sensori le potenzialità diventano enormi.
</p>

<p style="text-align: justify;">
  <a href="https://github.com/iltempe/Dashboard">Questo</a> il repository github con un esperimento fatto e le indicazioni per rifarlo in casa vostra.
</p>

<p style="text-align: justify;">
  Ps una volta che avrete implementato la vostra soluzione su raspberry vi sarà facile creare il vostro canale degli opendata connettendolo via HDMI alla vostra tv di casa.
</p>

[<img class="aligncenter size-large wp-image-1448" src="http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/2-1024x502.jpg" alt="2" width="656" height="321" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/2-300x147.jpg 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/2-1024x502.jpg 1024w, http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/2.jpg 2636w" sizes="(max-width: 656px) 100vw, 656px" />](http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/2.jpg)

&nbsp;

&nbsp;

&nbsp;

&nbsp;