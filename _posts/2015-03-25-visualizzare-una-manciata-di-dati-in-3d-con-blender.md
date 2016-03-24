---
id: 1860
title: 'Visualizzare una &#8220;manciata di dati&#8221; in 3D con Blender'
date: 2015-03-25T21:43:16+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=1860
permalink: /visualizzare-una-manciata-di-dati-in-3d-con-blender/
dsq_thread_id:
  - 3626489347
categories:
  - Blog
  - Hackers
  - Opendata
tags:
  - blender
  - dataviz
---
<p style="text-align: justify;">
  <a href="http://pratosmart.teo-soft.com/wp-content/uploads/2015/03/Schermata-2015-03-25-alle-20.51.29.png"><img class="alignleft  wp-image-1861" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/03/Schermata-2015-03-25-alle-20.51.29-312x1024.png" alt="Schermata 2015-03-25 alle 20.51.29" width="140" height="459" /></a>Da tempo mi sono fissato che sia sempre più necessario sviluppare metodi per rendere più fruibili i dati per porre i presupposti di una rapida applicazione del digitale nella nostra vita di tutti i giorni: questo vale per gli opendata, ma in modo più generale potremmo parlarne per i bigdata in generale. Per questo motivo (e per passione personale) sto dedicando un po’ di tempo per testare tecniche di visualizzazione dei dati in tre dimensioni.
</p>

<p style="text-align: justify;">
  Creare rappresentazioni di dati in 3D consente non solo di renderli visibili, ma anche di integrarli all’interno di infografiche tridimensionali, consente un’analisi più immediata del dato in sè e, infine, consente di creare modelli che oggi con stampanti 3D possono essere facilmente stampati e “toccati” con mano trasformando cosi l’informazione digitale in un oggetto.
</p>

<p style="text-align: justify;">
  Come già dimostrato anche <a href="http://pratosmart.teo-soft.com/fai-un-modello-3d-di-prato-con-openstreetmap-e-blender/">qui</a>, <a href="http://www.blender.org/">Blender </a>è un’ ottima risorsa per chi voglia cimentarsi nell’apprendere anche solo le basi del disegno 3D: i motivi sono essenzialmente dovuti al fatto che è un software opensource, integra la possibilità di eseguire script in linguaggio python nel proprio progetto e ha un’ampia community di utenti e sviluppatori diffusa sul web.
</p>

<p style="text-align: justify;">
  Detto questo oggi ho cercato di riassumere qui come è possibile ottenere una rappresentazione di dati digitali in 3 dimensioni a partire da un foglio di lavoro su <a href="http://www.google.com/docs/about/">Google Document</a>. Il risultato che otterremo è il seguente.
</p>

<p style="text-align: justify;">
  Io ho usato per esempio, per farvi capire il procedimento che sono riuscito a creare, una tabella con una lista di anni ed una lista di dati ad essi associati.
</p>

<ol style="text-align: justify;">
  <li>
    Creare un foglio di lavoro con i dati in <a href="http://www.google.com/docs/about/">Google Document</a> come quello che ho creato io <a href="https://github.com/TeoSoft80/datavizinblender/blob/master/data.csv" target="_blank">qui</a>. Nel mio caso la prima colonna rappresenta un anno e la seconda un dato associato a quell’anno. Esportare i dati in formato csv in un file data.csv
  </li>
  <li>
    Implementare lo script archiviato <a href="https://github.com/TeoSoft80/datavizinblender" target="_blank">qui</a> ed eseguire Run Script all’interno. Lo script è tutto commentato e si comprende abbastanza bene, ma spiegato in sintesi dopo aver importato due librerie carica i dati dal file csv che avete creato, setta le etichette prelevandole dalla prima colonna, e poi disegna i dati della seconda colonna creando dei cubi e posizionandoli nello spazio di Blender. [<a href="https://www.youtube.com/watch?v=D-pTF3KrTOQ" target="_blank">Questo</a> è un tutorial da cui sono partito.]
  </li>
</ol>

**Capite bene che se iniziate ad applicare lo stesso ragionamento per set di dati (o, ancora meglio, per dataset opendata) si prospettano interessanti applicazioni nel campo della visualizzazione e della “materializzazione” (tramite stampa 3D) delle informazioni.**

&nbsp;

[<img class="  wp-image-1862 aligncenter" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/03/Schermata-2015-03-25-alle-21.19.06.png" alt="Schermata 2015-03-25 alle 21.19.06" width="833" height="444" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/03/Schermata-2015-03-25-alle-21.19.06-300x160.png 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/03/Schermata-2015-03-25-alle-21.19.06-1024x546.png 1024w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/03/Schermata-2015-03-25-alle-21.19.06-150x80.png 150w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/03/Schermata-2015-03-25-alle-21.19.06.png 1530w" sizes="(max-width: 833px) 100vw, 833px" />](http://pratosmart.teo-soft.com/wp-content/uploads/2015/03/Schermata-2015-03-25-alle-21.19.06.png)