---
id: 2177
title: Meteo e Rischio Idrogeologico su Google Calendar
date: 2015-10-02T13:49:33+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=2177
permalink: /meteo-e-rischio-idrogeologico-su-google-calendar/
dsq_thread_id:
  - 4186697607
switch_like_status:
  - 1
sharing_disabled:
  - 1
categories:
  - Hackers
  - Laboratorio
  - Opendata
tags:
  - emergenzeprato
  - google calendar
  - opendata
  - prato
---
<a href="https://www.google.com/calendar" target="_blank">Google Calendar</a> non ha bisogno di molte presentazioni. E&#8217; un servizio che Google vi mette a disposizione che vi consente di gestire un calendario eventi in modalità completamente cloud computing.

Senza fare troppa pubblicità perchè Google non ne ha bisogno, di questo servizio mi hanno però attirato queste particolari caratteristiche:

  * Possibilità di gestire più calendari (divisi per argomento)
  * Possibilità di aggiungere calendari su smartphone da cloud
  * Possibilità di condividere calendari e/o di renderli pubblici (cosi che siano anche indicizzabili da Google stesso)
  * Possibilità di integrare un Google Calendar in un sito internet
  * Possibilità di agire sui calendari tramite apposite API registrando una applicazione web in Google (esattamente come si fa per tuittare in modo programmatico qualcosa su Twitter).

<p style="text-align: justify;">
  L&#8217;altra sera guardavo tra i calendari disponibili quello di Google Meteo che vi da un&#8217;indicazione (sommaria) del meteo del giorno sopra il vostro Google Calendar e mi son chiesto: <strong>ma perchè non lo si può fare con gli opendata relativi a meteo e/o rischio che quotidianamente vengono elaborati dalla regione Toscana</strong>? D&#8217;altronde il bollettino meteo di aggiornamento di un territorio lo possiamo vedere come un &#8220;evento da segnare in un calendario&#8221;. Magari in un calendar pubblico che tutti possono vedere ed eventualmente integrare su siti web.
</p>

<p style="text-align: justify;">
  Per chi volesse provarci ecco come si fa. Occorre un account Gmail come prerequisito e un po&#8217; di voglia di &#8220;smanettare&#8221;.
</p>

<li style="text-align: justify;">
  Create un Google Calendar. Io ne ho fatto uno chiamato emergenzeprato. Impostatelo come pubblico.
</li>

[<img class="wp-image-2179 aligncenter" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/2-1024x316.jpg" alt="2" width="702" height="216" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/2-1024x316.jpg 1024w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/2.jpg 1294w" sizes="(max-width: 702px) 100vw, 702px" />](http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/2.jpg)<img class="wp-image-2182 aligncenter" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/1.jpg" alt="1" width="491" height="159" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/1-300x97.jpg 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/1.jpg 614w" sizes="(max-width: 491px) 100vw, 491px" />

<li style="text-align: justify;">
  Registrate una web app Google <a href="https://console.developers.google.com" target="_blank">qui</a>. Vi serve per dare accesso alla vostra applicazione al calendario che avete creato. Segnatevi dell&#8217;applicazione che avete creato i codici riportati in figura e scaricate il file JSON dal menu in alto. Se non avete mai fatto una web app google seguite <a href="https://developers.google.com/google-apps/calendar/quickstart/php" target="_blank">questa guida ufficiale</a> (step 1).
</li>

[<img class="wp-image-2181 aligncenter" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/4.jpg" alt="4" width="648" height="315" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/4-300x146.jpg 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/4.jpg 976w" sizes="(max-width: 648px) 100vw, 648px" />](http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/4.jpg)

<li style="text-align: justify;">
  Scaricate le API ufficiali di Google su Github <a href="https://github.com/google/google-api-php-client/tree/master/src/Google" target="_blank">qui</a>. (si anche Google sta su Github).
</li>
<li style="text-align: justify;">
  A questo punto usate <a href="https://github.com/iltempe/Emergenzeprato/tree/master/GoogleCalendar" target="_blank">la mia applicazione GoogleCalendar</a> che ho creato in <a href="https://iltempe.github.io/Emergenzeprato/" target="_blank">Emergenzeprato</a> per capire come agire. Copiate nella folder della applicazione il JSON che avete scaricato.
</li>
<li style="text-align: justify;">
  Per inserire i vostri dati anzichè quelli di emergenzeprato dovrete agire all&#8217;interno di calendar.php.
</li>
<li style="text-align: justify;">
  Usando con un cron il file calendar.php pubblicherete gli eventi sul calendario. (la prima volta che lo usate dovrete autorizzare la vostra applicazione a publicare).
</li>

Se avete altri dubbi potete far riferimento alla <a href="https://developers.google.com/google-apps/calendar/v3/reference/events/insert" target="_blank">documentazione ufficiale di Google</a>.

**[<img class="alignleft wp-image-2190" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/Schermata-2015-10-02-alle-20.10.44-725x1024.png" alt="Schermata 2015-10-02 alle 20.10.44" width="327" height="462" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/Schermata-2015-10-02-alle-20.10.44-725x1024.png 725w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/Schermata-2015-10-02-alle-20.10.44.png 1200w" sizes="(max-width: 327px) 100vw, 327px" />](http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/Schermata-2015-10-02-alle-20.10.44.png)Ma la cosa più interessante è che adesso potete iscrivervi al calendario in quanto pubblico senza alcun problema di account!**

**Ogni dispositivo mobile o no vi permette infatti di aggiungere calendari da LINK. **

**Per iscrivervi al calendario di emergenzeprato usate il link qui sotto**

[**https://www.google.com/calendar/ical/pratopioggia%40gmail.com/public/basic.ics**](https://www.google.com/calendar/ical/pratopioggia%40gmail.com/public/basic.ics)

&nbsp;

That&#8217;s all, amici. Ora sta a voi trovare altre applicazioni su questo usando opendata (pensate ai bollettini della protezione civile, gli eventi pubblici, incidenti etc etc&#8230;)  Spero sia tutto un minimo utile, alla prossima. Qui sotto il calendario di Emergenzeprato

&nbsp;

&nbsp;

&nbsp;

&nbsp;

&nbsp;



&nbsp;

&nbsp;