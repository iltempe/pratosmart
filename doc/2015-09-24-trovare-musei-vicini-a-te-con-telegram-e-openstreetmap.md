---
id: 2159
title: Trovare musei vicini a te con Telegram e Openstreetmap
date: 2015-09-24T15:08:25+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=2159
permalink: /trovare-musei-vicini-a-te-con-telegram-e-openstreetmap/
dsq_thread_id:
  - 4161042669
categories:
  - Blog
  - Hackers
  - Opendata
tags:
  - opendata
  - opensource
  - openstreetmap
  - telegram
---
<p style="text-align: justify;">
  Oggi un semplice tutorial su come creare una &#8220;guida robot&#8221; con <a href="https://telegram.org/" target="_blank">Telegram </a>che ti dica quali sono i Musei più vicini a te utilizzando la base di dati di <a href="https://www.openstreetmap.org/#map=14/43.8796/11.0854&layers=H" target="_blank">Openstreetmap</a>. Si tratta di un tutorial per spiegare come si può partendo dalla posizione inviata ad un robot Telegram associare dati geografici (nel caso di OSM dati aperti) e riusarli per creare un semplice servizio.
</p>

<p style="text-align: justify;">
  Ho creato un robot che si chiama <strong>MuseiBot</strong> potete aprire una chat con lui con il link <a href="http://telegram.me/MuseiBot" target="_blank">http://telegram.me/MuseiBot</a> o cercando l&#8217;utente @MuseiBot dentro Telegram stesso
</p>

<p style="text-align: justify;">
  Il robot si usa <strong>semplicemente inviando la propria posizione tramite la &#8220;molletta&#8221; in basso a sinistra nella chat</strong>.
</p>

<p style="text-align: justify;">
  <a href="http://pratosmart.teo-soft.com/wp-content/uploads/2015/09/Immagine1.jpg"><img class="alignleft  wp-image-2161" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/09/Immagine1.jpg" alt="Immagine1" width="373" height="352" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/09/Immagine1-300x283.jpg 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/09/Immagine1.jpg 534w" sizes="(max-width: 373px) 100vw, 373px" /></a>
</p>

<p style="text-align: justify;">
  Nel momento in cui riceve la vostra posizione il robot interroga il database di Openstreetmap, andando a cercare i luoghi identificati con il TAG <strong><em>tourism=museum </em></strong>e vi restituisce la loro posizione geografica e il loro nome.
</p>

<p style="text-align: justify;">
  Tutto tramite opendata di Openstreetmap per cui aggiungendo dati taggati come musei alla mappa di Openstreetmap permettete ai luoghi di essere visti.
</p>

<p style="text-align: justify;">
  L&#8217;applicazione ricorda molto il principio dei social come Foursquare, ma la base dei dati in questo caso è completamente aperta e più viene aumentata dai mappatori Openstreetmap più il servizio diventa efficiente.
</p>

<p style="text-align: justify;">
  C&#8217;è un limite massimo di musei che al momento vengono restituiti (5 nel raggio di 5km), ma teoricamente potrebbe essere rimosso oppure impostato ad un valore molto alto.
</p>

<p style="text-align: justify;">
  Attualmente la applicazione visualizza i NODI di Openstreetmap (quindi i punti di interesse), ma non è complesso aggiungere edifici e/o strade.
</p>

<p style="text-align: justify;">
  Non fate caso se vedete la mappa di Google dentro il robot (sono le mappe che nativamente usa Telegram sul vostro smartphone) i dati sono effettivamente prelevati da Openstreetmap come riportato nei crediti.
</p>

<p style="text-align: justify;">
  <p style="text-align: justify;">
    <span style="text-decoration: underline;"><strong>Per gli smanettoni che volessero creare un&#8217;applicazione analoga</strong></span>
  </p>
  
  <p style="text-align: justify;">
    &#8211; Come creare un robot è già descritto in questo <a href="http://pratosmart.teo-soft.com/come-fare-una-mappa-di-segnalazioni-usando-telegram/" target="_blank">post</a>
  </p>
  
  <p style="text-align: justify;">
     &#8211; Per usare il robot potete farlo in modo manuale col comando <em>php start.php getupdates</em> o in webhook usando il comando <em>php start.php sethook</em> avendo impostato il link al file start.php sul vostro server (occorre connessione SSL).
  </p>
  
  <p>
    Il tutto funziona ed è riusabile perchè configurabile in un file in un file <em>settings.php</em> dove imposterete per Openstreetmap
  </p>
  
  <ul>
    <li>
      un numero massimo di luoghi da restituire;
    </li>
    <li>
      un raggio massimo in metri in cui volete cercare;
    </li>
    <li>
      il tag del tipo di luogo che state cercando;
    </li>
  </ul>
  
  <p style="text-align: justify;">
    &#8211; Sorgenti rilasciati in formato opensource su <a href="https://github.com/iltempe/TelegramMusei" target="_blank">Github </a>(naturalmente)
  </p>
  
  <p style="text-align: justify;">
    Non scordatevi di citare la fonte dei dati ovvero Openstreetmap.
  </p>
  
  <p style="text-align: justify;">
    In bocca al lupo!
  </p>