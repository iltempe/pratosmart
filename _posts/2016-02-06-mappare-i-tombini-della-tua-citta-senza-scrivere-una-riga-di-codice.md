---
id: 2399
title: Mappare i tombini della tua città senza scrivere una riga di codice
date: 2016-02-06T10:18:55+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=2399
permalink: /mappare-i-tombini-della-tua-citta-senza-scrivere-una-riga-di-codice/
dsq_thread_id:
  - 4556310566
categories:
  - Blog
  - Hackers
  - Opendata
tags:
  - googl drive
  - hackers
  - ifttt
  - opendata
  - openstreetmap
---
<p style="text-align: justify;">
  Da tempo ragionavo su un metodo semplice per mappare dei punti su un territorio. L&#8217;idea nasce dal fatto che molto spesso ci sono informazioni che se pur &#8220;ovvie&#8221; non sono disponibili alla città in formato digitale aperto e accessibile. A volte le pubbliche amministrazioni le hanno in formato analogico a volte no. A volte tali informazioni sono in mano ad alcuni privati. Altre volte queste informazioni aggiornate non esistono proprio e sarebbe utilissimo produrle. Come fare in questi casi?
</p>

<p style="text-align: justify;">
  Qui descrivo&nbsp;un metodo semplice per poter creare dati di punti georeferenziati senza programmare. Nel mio tutorial ho immaginato una campagna cittadina per mappare i tombini delle fognature. La stessa logica può essere applicata per mappare qualunque tipo di informazione e per registrare la sua posizione online.
</p>

<p style="text-align: justify;">
  Per fare questa campagna vi occorre solo:
</p>

<li style="text-align: justify;">
  Un account ad&nbsp;<a href="https://ifttt.com/recipes" target="_blank">IFTTT</a>&nbsp;: questa&nbsp;applicazione vi consente di creare semplici ricette automatizzate in cloud mettendo in relazione vari servizi web;
</li>
<li style="text-align: justify;">
  Uno spazio <a href="https://www.google.it/intl/it/drive/" target="_blank">GOOGLE DRIVE</a>&nbsp;: il servizio cloud di google per gestione documenti;
</li>
<li style="text-align: justify;">
  Uno smatphone con installata la app <a href="https://ifttt.com/products/do/button" target="_blank">DO</a>&nbsp;: una app (affiliata ad IFTTT) per dispositivi mobile che consente con la semplice pressione di un pulsante di eseguire un&#8217;operazione pianificata con IFTTT. Abilitate nella app DO nella sezione permission la possibilità di inviare la propria posizione (Location). Il tutorial è testato su Iphone 6.
</li>

<p style="text-align: justify;">
  Come si procede per creare tutto il sistema per mappare?
</p>

<li style="text-align: justify;">
  Accedete a IFTTT e create una ricetta DO Button ovvero un bottone personalizzato. La ricetta deve essere del tipo DO Button &#8211; Google Drive come quella illustrata in figura. Vi verrà chiesto le credenziali di accesso a Google Drive. Potete farlo partendo una ricetta esistente come <a href="Track your journey https://ifttt.com/recipes/192141?z=5720169">questa</a>.&nbsp;<img class="wp-image-2400 aligncenter" src="http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-05-alle-22.15.35-1024x556.png" alt="Schermata 2016-02-05 alle 22.15.35" width="623" height="338" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-05-alle-22.15.35-300x163.png 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-05-alle-22.15.35-768x417.png 768w, http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-05-alle-22.15.35-1024x556.png 1024w, http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-05-alle-22.15.35.png 1502w" sizes="(max-width: 623px) 100vw, 623px" />
</li>
<li style="text-align: justify;">
  A questo punto occorre definire cosa deve fare il vostro semplice servizio alla pressione del bottone DO. Compilate&nbsp;la ricetta come segue. Si tratta di una ricetta che vi permetterà di aggiungere una riga ad un foglio google chiamato Tombini ogni volta che farete pressione sul bottone con lo smartphone. Nel momento in cui farete pressione nel foglio Google saranno memorizzate queste informazioni su 3 colonne : Tempo , Latitudine , &nbsp;Longitudine.
</li>

<img class="wp-image-2405 aligncenter" src="http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-05-alle-22.26.42-1024x867.png" alt="Schermata 2016-02-05 alle 22.26.42" width="594" height="503" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-05-alle-22.26.42-300x254.png 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-05-alle-22.26.42-768x651.png 768w, http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-05-alle-22.26.42-1024x867.png 1024w" sizes="(max-width: 594px) 100vw, 594px" />

La ricetta (se non lo create voi) vi crea in automatico un foglio denominato Tombini in questa posizione su Google Drive.

<img class="size-large wp-image-2403 aligncenter" src="http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-05-alle-22.24.11-1024x219.png" alt="Schermata 2016-02-05 alle 22.24.11" width="660" height="141" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-05-alle-22.24.11-300x64.png 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-05-alle-22.24.11-768x164.png 768w, http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-05-alle-22.24.11-1024x219.png 1024w, http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-05-alle-22.24.11.png 1374w" sizes="(max-width: 660px) 100vw, 660px" />

Impostate il foglio in questo modo:

  * File->Impostazioni del foglio di lavoro->Impostazioni internazionali = Stati Uniti
  * Nella prima riga inserite queste tre parole: Tempo || Lat || Lon
  * Pubblicate il foglio sul web in formato CSV per rendere i dati disponibili per altre applicazioni dal menu File->Pubblica sul web->Foglio 1 -> Formato CSV. Otterrete un link pubblico per accedere ai dati in formato CSV.<img class="wp-image-2406 aligncenter" src="http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-05-alle-22.31.55-1024x703.png" alt="Schermata 2016-02-05 alle 22.31.55" width="449" height="308" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-05-alle-22.31.55-300x206.png 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-05-alle-22.31.55-768x527.png 768w, http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-05-alle-22.31.55-1024x703.png 1024w, http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-05-alle-22.31.55.png 1084w" sizes="(max-width: 449px) 100vw, 449px" />

Fatto!

<p style="text-align: justify;">
  <img class="alignleft size-medium wp-image-2409" src="http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/IMG_2978-169x300.png" alt="IMG_2978" width="169" height="300" />A questo punto potete andare in giro per la vostra città premendo sullo smartphone il bottone che avete creato nel momento in cui sarete proprio sopra un tombino. Il servizio da voi creato memorizzerà tramite lo smartphone la vostra posizione e quindi quella del tombino.
</p>

<p style="text-align: justify;">
  Al termine della vostra campagna avrete la lista delle posizioni geografiche di tutti i tombini come quella che vedete qui sotto. Questi dati sono informazioni digitali che possono essere mappati su mappe digitali con servizi come <a href="https://umap.openstreetmap.fr/it/">UMAP</a>&nbsp;o addirittura importati come dati aperti su <a href="https://www.openstreetmap.org" target="_blank">Openstreetmap</a> in modo da essere riusabili da tutti. Ai dati potrete accedere facilmente&nbsp;tramite il link al file CSV che voi avete pubblicato sul WEB all&#8217;inizio (UMAP permette di importare dati da un link CSV esterno <a href="http://www.startupcalabria.com/umap-crea-e-condividi-le-tue-mappe-open-in-10-minuti/" target="_blank">leggi qui</a>; per importare dati su Openstreetmap leggere queste&nbsp;<a href="http://wiki.openstreetmap.org/wiki/IT:Import/Guidelines" target="_blank">linee guida</a>).
</p>

<p style="text-align: justify;">
  <strong>Sto proponendo a voi di andare in giro a mappare i vostri tombini? Beh anche. Ricordatevi che i dati aperti sono generabili da chiunque. </strong>
</p>

<p style="text-align: justify;">
  <strong><img class="alignleft size-medium wp-image-2421" src="http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-06-alle-10.14.57-300x259.png" alt="Schermata 2016-02-06 alle 10.14.57" width="300" height="259" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-06-alle-10.14.57-300x259.png 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-06-alle-10.14.57-768x664.png 768w, http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-06-alle-10.14.57.png 826w" sizes="(max-width: 300px) 100vw, 300px" />Ma sto anche suggerendo un metodo GRATUITO, per cui NON E&#8217; NECESSARIO SVILUPPARE SOFTWARE e molto SEMPLICE da spiegare, per chiunque voglia digitalizzare la posizione geografica di qualcosa in città.&nbsp;</strong>
</p>

<p style="text-align: justify;">
  Immaginate un manutentore di un tombino che dopo aver fatto la sua attività di manutenzione lo mappa semplicemente premendo un pulsante. Immaginate una squadra della protezione civile che a valle di un controllo preme un pulsante e mappa un tombino. Lo stesso principio si può ovviamente applicare per qualunque altro oggetto o situazione in città&#8230;solo altre due idee applicabili in Italia:
</p>

<li style="text-align: justify;">
  qualche giorno fa suggerivo che la <a href="http://www.phlcrimemapper.com/" target="_blank">polizia di Philadelphia mappa</a> dove avvengono crimini su mappa pubbblica
</li>
<li style="text-align: justify;">
  ci sono squadre di dipendenti regionali che registrano la posizione di insetti nocivi alle piante da frutto come il <a href="http://iltirreno.gelocal.it/prato/cronaca/2014/07/12/news/tarlo-asiatico-a-prato-il-terzo-caso-in-italia-1.9583486" target="_blank">tarlo asiatico</a>.
</li>

Ed ora sta a voi!

<img class="size-medium wp-image-2423 aligncenter" src="http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-06-alle-10.16.18-300x215.png" alt="Schermata 2016-02-06 alle 10.16.18" width="300" height="215" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-06-alle-10.16.18-300x215.png 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-06-alle-10.16.18-1024x735.png 1024w" sizes="(max-width: 300px) 100vw, 300px" />