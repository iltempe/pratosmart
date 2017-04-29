---
id: 2236
title: 'Notifiche sul PC con gli opendata: Linux e Allerte Meteo'
date: 2015-10-29T12:31:52+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=2236
permalink: /notifiche-sul-pc-con-gli-opendata-linux-e-allerte-meteo/
dsq_thread_id:
  - 4270408201
categories:
  - Blog
  - Hackers
  - Opendata
tags:
  - emergenzeprato
  - linux
  - opendata
  - opensource
  - ubuntu
---
<p style="text-align: justify;">
  Immaginate una scuola. Interamente attrezzata con PC. Oppure un insieme di uffici pubblici pieni zeppi di scrivanie con computer ed immaginate di voler far arrivare a tutti una certa notifica con un certo formato. Non vi basta una mail, volete essere sicuri che appaia sul desktop di tutti un certo avviso come avvertimento.
</p>

Ho rispolverato le mie conoscenze di <a href="https://it.wikipedia.org/wiki/Linux" target="_blank">Linux</a> per questo tutorial.

<p style="text-align: justify;">
  Linux è un sistema operativo che si presta molto bene a queste personalizzazioni per la sua filosofia di fornire completo accesso alle risorse del computer perchè la conoscenza relativa al suo sviluppo è aperta. Per cui se avete necessità di configurare dei computer che abbiano carattestiche custom come quella che vogliamo implementare è l&#8217;ambiente ideale. Nella sua versione <a href="http://www.ubuntu-it.org/" target="_blank">Ubuntu</a> consente anche un buon utilizzo da utente oltre che da sviluppatore per cui chiunque può inziare a prenderci confidenza.
</p>

<p style="text-align: justify;">
  <a href="http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/1.png"><img class="alignleft wp-image-2238" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/1-1024x576.png" alt="1" width="477" height="268" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/1-300x169.png 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/1-1024x576.png 1024w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/1.png 1366w" sizes="(max-width: 477px) 100vw, 477px" /></a>Vantaggi di usare Ubuntu? Ubuntu vi mette a disposizione il tool &#8220;notify-send&#8221; uno strumento che consente di mostrare un&#8217;avviso personalizzato (con poche righe di codice). Potete provarlo installandolo con questa istruzione
</p>

<div class="bbcode_container">
  <pre class="bbcode_code">sudo apt-get install notify-osd</pre>
</div>

<p style="text-align: justify;">
  e poi testarlo con
</p>

<div class="bbcode_container">
  <pre class="bbcode_code">notify-send CIAO! "Ciao Mondo"
</pre>
  
  <p class="bbcode_code">
    dove la prima stringa è il titolo e la seconda il messaggio del testo da mostrare in notifica. Il comando vi consente tra le varie opzioni di definire una criticità per l&#8217;avviso da mostrare, un&#8217;icona personalizzata e un tempo di visualizzazione.
  </p>
  
  <p class="bbcode_code">
    <strong>A questo punto arriva la magia degli opendata. Ho realizzato tre semplici script che in sostanza fanno questo:</strong>
  </p>
  
  <ul>
    <li class="bbcode_code">
      Prelevano un file archiviato contenente i dati (TXT o XML)
    </li>
    <li class="bbcode_code">
      Individuano l&#8217;informazione da notificare all&#8217;interno del file
    </li>
    <li class="bbcode_code">
       Notificano il dato con un tempo definito e una particolare icona.
    </li>
  </ul>
  
  <p style="text-align: justify;">
    In particolare il primo file notifica aggiornamenti della protezione civile di Prato leggendoli da un file TXT, il secondo va a notificare il rischio di una zona della Toscana (prendendo in input la zona e tipo di rischio) ed il terzo fornisce il meteo del giorno. Tutto è archiviato su <a href="https://github.com/iltempe/Emergenzeprato" target="_blank">Emergenzeprato</a> in forma opensource ovviamente, non vi resta altro che personalizzare i link ai dati e le chiavi di ricerca per prelevare le informazioni di vostro interesse ed il gioco è fatto.
  </p>
  
  <p style="text-align: justify;">
    Gli script possono essere lanciati da shell con (i parametri servono solo per il 2 e il 3)
  </p>
  
  <pre style="text-align: justify;">sh scritp.sh $parametro1 $parametro2
</pre>
  
  <p style="text-align: justify;">
    Ma possono anche essere eseguiti periodicamente con il comando cron oppure allo startup del vostro computer con
  </p>
  
  <pre style="text-align: justify;">sudo chmod a+x /percorso/allo/script.sh
</pre>
  
  <pre style="text-align: justify;">sudo nano /etc/rc.local
</pre>
  
  <p style="text-align: justify;">
    inserendo prima di
  </p>
  
  <pre style="text-align: justify;">exit 0
</pre>
  
  <p style="text-align: justify;">
    l&#8217;istruzione
  </p>
  
  <pre style="text-align: justify;">/percorso/allo/script.sh</pre>
</div>

<span style="color: #555555; font-family: Monaco, 'Andale Mono', 'Courier New', Courier, mono; font-size: 12.15px; line-height: 15.795px; background-color: #f4f4f4;">In bocca al lupo!</span>

&nbsp;

[<img class="size-large wp-image-2240 aligncenter" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/3-1024x576.png" alt="3" width="640" height="360" />](http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/3-e1446113550293.png)

&nbsp;