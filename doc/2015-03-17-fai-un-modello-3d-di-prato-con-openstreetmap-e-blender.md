---
id: 1837
title: Fai un modello 3D di Prato con Openstreetmap e Blender
date: 2015-03-17T23:06:06+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=1837
permalink: /fai-un-modello-3d-di-prato-con-openstreetmap-e-blender/
dsq_thread_id:
  - 3604042663
categories:
  - Blog
  - Hackers
  - Makers
tags:
  - 3d
  - blender
  - openstreetmap
---
<p style="text-align: justify;">
  Oggi un semplice tutorial alla portata di tutti su come ottenere un modello 3D della città di Prato a partire dai dati di <a href="www.openstreetmap.org" target="_blank">Openstreetmap</a> e usando il software di modellazione 3d opensource <a href="http://www.blender.org/" target="_blank">Blender</a>. Il tutorial è un punto di partenza per capire le potenzialità che possono provenire combinando una piattaforma di dati georeferenziati aperti, come è Openstreetmap ed il disegno 3D. Pensate alle infinite applicazioni per la visualizzazione in filmati, videogiochi, ma anche a tutte le possibilità nel mondo dei makers tramite la stampa in 3D di mappe per plastici, souvenir per il turismo e chi più ne ha più ne metta. Come si procede? Semplice.
</p>

<li style="text-align: justify;">
  Installate Blender scaricando l&#8217;ultima versione <a href="http://www.blender.org/download/" target="_blank">qui</a>.
</li>
  1. Esportate i dati da Openstreetmap della città di Prato da <a href="http://www.openstreetmap.org/#map=15/43.8822/11.1021" target="_blank">qui</a> facendo click su Esporta. Scaricherete un file .osm dei dati Openstreetmap ovvero il database dei dati corrispondenti alla mappa che state visualizzando sullo schermo.
  2. Scaricate il file <a href="https://raw.githubusercontent.com/vvoovv/blender-geo/master/io_import_scene_osm.py" target="_blank">io_import_scene_osm.py</a> parte del plugin blender <a href="https://github.com/vvoovv/blender-geo" target="_blank">BlenderGeo</a>
  3. Installare il plugin tramite il menu di Blender <ul class="task-list">
      <li>
        <em>File → User Preferences&#8230; → Addons → Install from File&#8230;</em>
      </li>
      <li>
        Cercare il file .py appena scaricato e selezionare<em> Install from File&#8230;</em>
      </li>
      <li>
        Abilitare il plugin con l&#8217;opzione <em>Enable an addon</em>
      </li>
    </ul>

<img class=" size-large wp-image-1840 alignleft" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/03/Schermata-2015-03-17-alle-22.58.24-1024x530.jpg" alt="Schermata 2015-03-17 alle 22.58.24" width="656" height="340" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/03/Schermata-2015-03-17-alle-22.58.24-300x155.jpg 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/03/Schermata-2015-03-17-alle-22.58.24-1024x530.jpg 1024w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/03/Schermata-2015-03-17-alle-22.58.24-150x78.jpg 150w" sizes="(max-width: 656px) 100vw, 656px" />Adesso avete tutti gli elementi per creare un modello 3D in Blender della città. E&#8217; consigliabile partire da piccole porzioni di città e lavorare su file nuovo per importare i dati la prima volta e capire come siano strutturati. Le istruzioni sono riprese da [qui](https://github.com/vvoovv/blender-geo/wiki/Import-OpenStreetMap-(.osm)).

Procedete come scritto sotto:

<ul class="task-list">
  <li>
    <em>Dal menu File → Import → OpenStreetMap (.osm)</em>
  </li>
  <li>
    Trovate il file .osm sul vostro computer
  </li>
  <li>
    Se l&#8217;opzione <em>Ignore existing georeferencing </em>è selezionata<em> </em>la georeferenziazione presente è ignorata e una nuova è costruita da Blender
  </li>
  <li>
    Se l&#8217;opzione <em>Import as a single mesh </em>è selezionata, gli oggetti OSM sono importati in un singolo oggetto invece che separatamente (utile se avete moltissimi edifici da importare)
  </li>
  <li>
    Selezionate <em>Import buildings</em> per importare gli edifici
  </li>
  <li>
    Selezionate <em>Import roads and paths</em> per importare strade e percorsi
  </li>
  <li>
    Scegliete una &#8220;thickness&#8221; diversa da 0 se volete dare volume agli edifici
  </li>
  <li>
    Premete <em>Import OpenStreetMap</em>
  </li>
</ul>

[<img class="  wp-image-1839 alignright" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/03/Schermata-2015-03-17-alle-22.59.44.jpg" alt="Schermata 2015-03-17 alle 22.59.44" width="305" height="224" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/03/Schermata-2015-03-17-alle-22.59.44-150x110.jpg 150w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/03/Schermata-2015-03-17-alle-22.59.44.jpg 658w" sizes="(max-width: 305px) 100vw, 305px" />](http://pratosmart.teo-soft.com/wp-content/uploads/2015/03/Schermata-2015-03-17-alle-22.59.44.jpg)Ecco fatto. Avete la città in forma 3D davanti a voi. Chi conosce Blender può divertirsi a cambiare texture, punti luce ed inserire sfondi e colori.

Solo una nota: ogni edificio ed oggetto importato dal file .osm ha un set di Custom Properties corrispondenti ai dati di Openstreetmap, ovvero state visualizzando i vostri opendata in 3D.

Restate sintonizzati andremo avanti su questo argomento!

&nbsp;