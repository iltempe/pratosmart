---
id: 1968
title: Fai una mappa 3D con Openstreetmap e Sketchfab
date: 2015-06-09T11:00:08+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=1968
permalink: /fai-una-mappa-3d-con-openstreetmap-e-sketchfab/
dsq_thread_id:
  - 3833753152
categories:
  - Blog
  - Hackers
  - Opendata
tags:
  - 3d
  - model
  - opendata
  - openstreetmap
  - prato
  - scketchfab
---
<p style="text-align: justify;">
  Chi mi conosce sa che da tempo amo mischiare gli opendata contenuti in <a href="http://www.openstreetmap.org" target="_blank">Openstreetmap</a> con altre forme di innovazione tecnologica. Già a suo tempo vi ho fatto vedere come produrre un modello 3D della vostra città con Blender tramite <a href="http://pratosmart.teo-soft.com/fai-un-modello-3d-di-prato-con-openstreetmap-e-blender/" target="_blank">questo post</a>. Oggi uniamo i dati di Openstreetmap alla piattaforma web <a href="https://sketchfab.com/" target="_blank">Sketchfab</a>, forse la più conosciuta piattaforma di condivisione e pubblicazione modelli 3D presente online.
</p>

<p style="text-align: justify;">
  Iniziate scaricando un file di dati da Openstreetmap del vostro quartiere (il mio è Galciana). Potete farlo tramite il pulsante <img class="  wp-image-1969 alignright" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/06/Schermata-2015-06-08-alle-22.43.10-1024x529.png" alt="Schermata 2015-06-08 alle 22.43.10" width="517" height="267" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/06/Schermata-2015-06-08-alle-22.43.10-300x155.png 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/06/Schermata-2015-06-08-alle-22.43.10-1024x529.png 1024w" sizes="(max-width: 517px) 100vw, 517px" />Esporta di Openstreetmap una volta posizionato lo zoom e la vista sull&#8217;area che volete riprodurre in 3D. Sul vostro computer verrà scaricata un file contenente tutti i dati dell&#8217;area denominato map.osm
</p>

Per usare il file .osm di Openstreetmap in Sketchfab occorre convertirlo in un modello 3D. Per fare questo useremo il software **<a href="http://wiki.openstreetmap.org/wiki/OSM2World" target="_blank">osm2world</a> **che potete scaricare <a href="http://osm2world.org/download/files/latest/" target="_blank">qui</a>.

Scaricate anche la cartella &#8216;example texture selection’ del programma osm2world <a href="http://osm2world.org/download/" target="_blank">qui</a>, per predisporre il software all&#8217;uso di texture per il disegno 3D.

Estraete tutto nella stessa cartella e copiate nella stessa cartella il file map.osm

Aprite una shell posizionatevi nella cartella contenente osm2world e digitate

<code class="prettyprint prettyprinted">&lt;span class="pun">./&lt;/span>&lt;span class="pln">osm2world&lt;/span>&lt;span class="pun">.&lt;/span>&lt;span class="pln">sh &lt;/span>&lt;span class="pun">-&lt;/span>&lt;span class="pln">i map&lt;/span>&lt;span class="pun">.&lt;/span>&lt;span class="pln">osm &lt;/span>&lt;span class="pun">-&lt;/span>&lt;span class="pln">o map&lt;/span>&lt;span class="pun">.&lt;/span>&lt;span class="pln">obj&lt;/span></code>

<img class="size-medium wp-image-1970 alignleft" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/06/Schermata-2015-06-08-alle-22.55.02-300x244.png" alt="Schermata 2015-06-08 alle 22.55.02" width="300" height="244" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/06/Schermata-2015-06-08-alle-22.55.02-300x244.png 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/06/Schermata-2015-06-08-alle-22.55.02-1024x832.png 1024w" sizes="(max-width: 300px) 100vw, 300px" />(potete settare altre opzioni di osm2world che sono specificate nella relativa pagina <a href="http://wiki.openstreetmap.org/wiki/OSM2World" target="_blank">wiki</a>).

A questo punto nella cartella avrete ottenuto due file map.obj con la geometria della mappa in 3D e map.obj.mtl che definisce i materiali.

Zippate tutto assieme alla cartella texture e fatene l&#8217;upload su Sketchfab.

<p style="text-align: justify;">
  Ecco fatto! adesso potete divertirvi a renderizzare il vostro modello in 3D usando materiali con <a href="https://help.sketchfab.com/hc/en-us/articles/202512446-Material-Editor" target="_blank">l&#8217;editor online</a>. L&#8217;editing di un materiale è molto semplice ed intuitivo basta usare il doppio click e effettuare i settaggi di texture o colore. Potete inoltre tramite l&#8217;editor rendere navigabile la vostra mappa 3D aggiungendo le vostre note direttamente sulla mappa, che diventeranno i punti di interesse visionabili con il navigatore. Ovviamente più i dati sono dettagliati più dettagliato e popolato sarà il modello. E questa è Galciana !
</p>



<p style="font-size: 13px; font-weight: normal; margin: 5px; color: #4a4a4a;">
  <a style="font-weight: bold; color: #1caad9;" href="https://sketchfab.com/models/b8d2e41030b042c2b795dace8e4112b5?utm_source=oembed&utm_medium=embed&utm_campaign=b8d2e41030b042c2b795dace8e4112b5" target="_blank">Galciana</a> by <a style="font-weight: bold; color: #1caad9;" href="https://sketchfab.com/pratosmart?utm_source=oembed&utm_medium=embed&utm_campaign=b8d2e41030b042c2b795dace8e4112b5" target="_blank">pratosmart</a> on <a style="font-weight: bold; color: #1caad9;" href="https://sketchfab.com?utm_source=oembed&utm_medium=embed&utm_campaign=b8d2e41030b042c2b795dace8e4112b5" target="_blank">Sketchfab</a>
</p>

<p style="font-size: 13px; font-weight: normal; margin: 5px; color: #4a4a4a;">
  (<a href="http://blog.sketchfab.com/post/107993471219/creating-interactive-3d-maps-with-openstreetmap" target="_blank">fonte</a>)
</p>