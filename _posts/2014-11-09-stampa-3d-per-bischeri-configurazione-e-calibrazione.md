---
id: 1440
title: Stampa 3D per bischeri – Configurazione e Calibrazione
date: 2014-11-09T17:33:00+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=1440
permalink: /stampa-3d-per-bischeri-configurazione-e-calibrazione/
dsq_thread_id:
  - 3207973634
categories:
  - Una Stampante 3D per Prato
tags:
  - prato
  - printrun
  - prusa
---
[<img class=" wp-image-1441 alignleft" src="http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/171-1024x589.jpg" alt="171" width="423" height="243" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/171-300x172.jpg 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/171-1024x589.jpg 1024w, http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/171-150x86.jpg 150w, http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/171.jpg 1034w" sizes="(max-width: 423px) 100vw, 423px" />](http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/171.jpg)Quando avrete terminato di montare la vostra <a title="Stampa 3D per bischeri : Cosa c’è dentro un KIT Prusa I3 Steel" href="http://pratosmart.teo-soft.com/stampa-3d-da-0-cosa-ce-dentro-un-kit-per-una-prusa-i3/" target="_blank">Prusa I3 con un kit </a>come il mio non vedrete l&#8217;ora di iniziare a stampare.

E invece no. Ancora c&#8217;è bisogno di fare il setup iniziale dello strumento e la sua calibrazione a modo altrimenti non stamperete un bel niente o comunque stamperete male.

Durante questa fase avrete necessità di usare questo software

  * Firmware <a href="https://github.com/ErikZalm/Marlin" target="_blank">Marlin</a> ovvero il programma che dovete caricare nella stampante
  * <a href="http://arduino.cc/en/Main/Software" target="_blank">IDE di Arduino</a> ovvero l&#8217;ambiente per caricare il firmware nella scheda Arduino della stampante
  * <a href="http://reprap.org/wiki/Printrun" target="_blank">Printrun</a> un programma che vi consentirà di pilotare i singoli componenti (motori, estrusore) della stampante da PC per verificarne il corretto funzionamento

Come si procede? Io mi sono servito di due tutorial online (dello stesso autore): seguiteli in sequenza:

  1. <a href="http://www.ivanbortolin.it/?p=360" target="_blank">Caricare e configurare il firmware<img class="wp-image-1443 alignright" src="http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/IMG_2486-1024x768.jpg" alt="IMG_2486" width="455" height="341" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/IMG_2486-300x225.jpg 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/IMG_2486-1024x768.jpg 1024w" sizes="(max-width: 455px) 100vw, 455px" /></a>
  2. <a href="http://www.ivanbortolin.it/?p=399" target="_blank">Taratura dei motori</a>

Due note a riguardo:

<p style="text-align: justify;">
  Non confondete la taratura degli step dei motori con la stampa vera e propria. Tutta la taratura dei motori va fatta A FREDDO cioè muovendo i motori senza la parte calda montata che va per l&#8217;occorrenza staccata dalla stampante.
</p>

<p style="text-align: justify;">
  Nel caso in cui (come a me è accaduto) vi si tappi l&#8217;estrusore di stampa mi è stato suggerito di smontare il finale dell&#8217;estrusore di stampa, scaldarlo portandolo a temperatura e con un filo di rame pulirlo internamente.
</p>

In bocca al lupo!

&nbsp;

PS. Una volta tarato un po&#8217; tutto per iniziare a stampare i primi oggetti utilizzate il software CURA che è illustrato in modo base molto bene <a href="http://www.stampa3d-forum.it/guida-a-cura-lo-slicer-di-ultimaker/" target="_blank">qui</a>.

&nbsp;