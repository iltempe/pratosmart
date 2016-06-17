---
id: 2016
title: Come farsi un sottobicchiere partendo dalla mappa Openstreetmap del centro di Prato (parte 1)
date: 2015-07-02T11:05:23+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=2016
permalink: /come-farsi-un-sottobicchiere-partendo-dalla-mappa-openstreetmap-del-centro-di-prato/
dsq_thread_id:
  - 3897408060
categories:
  - Laboratorio
  - Makers
  - Opendata
tags:
  - makers
  - opendata
  - openstreetmap
  - prato
---
<p style="text-align: justify;">
  <a href="http://pratosmart.teo-soft.com/wp-content/uploads/2015/07/1.jpg"><img class="alignleft size-medium wp-image-2017" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/07/1-258x300.jpg" alt="1" width="258" height="300" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/07/1-258x300.jpg 258w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/07/1.jpg 716w" sizes="(max-width: 258px) 100vw, 258px" /></a> Chi mi segue sa quanto sono appassionato della piattaforma Openstreetmap ed in particolare della possibilità di sperimentare applicazioni di questa piattaforma e dei dati che essa contiene per cercare contaminazioni con altre discipline.
</p>

<p style="text-align: justify;">
  Oggi vediamo un semplice tutorial su come creare un accessorio di cucina partendo dalla mappa del centro di Prato su Openstreetmap. Per semplicità faremo un sottobicchiere ma in base alla dimensione potete trasformare l’oggetto anche in un sottopiatto, in un sottovaso o in un sottopentola.
</p>

<p style="text-align: justify;">
  Se avete una stampante 3D potete crearvi veramente l’oggetto stampandolo, se non la possedete una volta realizzato il disegno in formato 3d potete affidarvi a Fablab o servizi online per farvi stampare la vostra creazione (<a href="http://www.shapeways.com/">Shapeways</a> è il più famoso).
</p>

<p style="text-align: justify;">
  Iniziamo prelevando i dati e creando l’immagine vettoriale che rappresenti il nostro oggetto.
</p>

<p style="text-align: justify;">
  Esiste un semplice strumento software creato da uno spazio MapTime Amsterdam per creare pattern partendo da porzioni di mappa <a href="https://www.openstreetmap.org/" target="_blank">Openstreetmap</a>. Il tool si chiama <a href="http://maptime-ams.github.io/street-patterns/">Street Patterns</a> .
</p>

<p style="text-align: justify;">
  Dalla pagina del Tool seguite le indicazioni in modo guidato per ritagliare la zona che più vi interessa. In particolare al primo step io ho scelto la città di Prato e posto la piantina centrandola sulla zona del centro: indicativamente da Via L. Muzzi a Viale Piave.
</p>

<p style="text-align: justify;">
  Al passo successivo Street Patterns vi permette di eseguire una query per scegliere quali dati esportare della zona selezionata. Creando una query con <a href="http://overpass-turbo.eu/">Overpass Turbo</a> io ho selezionato solo le strade taggate come <i>highway</i>.
</p>

<p style="text-align: justify;">
  <i>[out:json];</i>
</p>

<p style="text-align: justify;">
  <i>way[&#8220;highway&#8221;](around:200,43.880259353326394,11.097280383110046);</i>
</p>

<p style="text-align: justify;">
  <i>(._;>;);</i>
</p>

<p style="text-align: justify;">
  <i>out;<img class="size-medium wp-image-2019 alignright" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/07/3-300x300.jpg" alt="3" width="300" height="300" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/07/3-150x150.jpg 150w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/07/3-300x300.jpg 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/07/3.jpg 518w" sizes="(max-width: 300px) 100vw, 300px" /></i>
</p>

<p style="text-align: justify;">
  Una volta estratti i dati selezionati potrete visualizzare la mappa con le strade evidenziate che sono presenti nella porzione di città che avete ritagliato.
</p>

<p style="text-align: justify;">
  Nel passaggio successivo (grazie all’uso di <a href="http://turfjs.org/">Turf.js</a>) i punti e le linee della mappa vengono automaticamente  interpolati ai bordi con un’area che ne permetta la produzione (altrimenti non potreste creare un oggetto, dato che i DATI non hanno di per sè una dimensione). Succesivamente l’area scelta viene contornata in un cerchio.
</p>

<p style="text-align: justify;">
  A questo punto, al fine di realizzare un disegno tramite i software di grafica vettoriale potete esportare l’immagine in formato SVG. A questo punto il tool vi consiglia di intagliare questa immagine nel legno con macchine tipo CNC mill che si trovano nei makers space. Nella prossima parte del tutorial vedremo come creare una semplice produzione artigianale dell’oggetto vero e quindi passare dai dati agli oggetti. Non mancate!
</p>