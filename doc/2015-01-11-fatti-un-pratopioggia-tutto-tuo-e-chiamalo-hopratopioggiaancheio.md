---
id: 1642
title: 'Fatti un emergenzeprato tutto tuo: e chiamalo #hoemergenzepratoancheio'
date: 2015-01-11T22:54:55+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=1642
permalink: /fatti-un-pratopioggia-tutto-tuo-e-chiamalo-hopratopioggiaancheio/
dsq_thread_id:
  - 3411629618
categories:
  - Blog
  - Hackers
  - Opendata
tags:
  - emergenzahack
  - emergenzeprato
  - opendata
  - pratopioggia
---
<p style="text-align: justify;">
  A grandissima richiesta stasera un tutorial per creare un servizio analogo ad #emergenzeprato per la propria città.
</p>

<p style="text-align: justify;">
  Per chi se lo fosse perso è un servizio Twitter che consente di essere aggiornati su Prato e provincia su quanto accade in tema meteo ed inoltre di segnalare possibili disagi derivanti da maltempo tramite i social network. Il servizio è evoluto nel tempo per cui può darsi che quando leggerete il tutorial non sarà più aggiornato, ma il principio base resta quello: usare Twitter per aggregare fonti relative ad emergenze (opendata, segnalazioni dal basso e dall&#8217;alto).
</p>

<p style="text-align: justify;">
  Sotto una illustrazione delle fonti ad oggi gestite da questo servizio&#8230;non metto limiti a quanto fatto (tutto è migliorabile e perfettibile, ma oggi è così).
</p>

[<img class="aligncenter wp-image-1643" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/01/@pratopioggia.jpg" alt="@emergenzeprato" width="763" height="429" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/01/@pratopioggia-300x169.jpg 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/01/@pratopioggia.jpg 960w" sizes="(max-width: 763px) 100vw, 763px" />](http://pratosmart.teo-soft.com/wp-content/uploads/2015/01/@pratopioggia.jpg)

&nbsp;

&nbsp;

<p style="text-align: justify;">
  Cercherò di riassumere in semplici passaggi come creare un sistema simile per la propria città. Ribadisco che il sistema è pensato per il territorio pratese, per cui ciò che è riusabile è la tecnica, i metodi e l&#8217;idea in sè (che a Prato vedo che sta iniziando a funzionare e a coinvolgere le persone). Da notare che il servizio mischia i dati di fonti ufficiali (sottoforma di opendata) assieme a dati provenienti da canali social che già le persone hanno familiarità nell&#8217;utilizzo. Per i cittadini della Toscana sicuramente gli script sono riusabili in toto modificandoli per parsare i dati del luogo su cui si vuol creare il servizio.
</p>

<p style="text-align: justify;">
  Come si procede dunque?
</p>

<li style="text-align: justify;">
  Create l&#8217;account Twitter e un indirizzo mail associato (meglio se gmail).
</li>
<li style="text-align: justify;">
  Create una applicazione Twitter <a href="https://apps.twitter.com/" target="_blank">qui</a> e segnatevi i 4 codici di autorizzazioni OAUTH per il tweet dei dati.
</li>
<li style="text-align: justify;">
  Utilizzate i <a href="https://github.com/TeoSoft80/Pratopioggia-parse-and-tweet" target="_blank">miei script in PHP</a> per prelevare i dati che vi interessano da fonti online e che dovete necessariamente prelevare tramite uno script ad hoc perchè non potete prelevarli tramite un servizio automatico (come <a href="https://ifttt.com" target="_blank">iftt</a>). Questi script parsano (per quanto riguarda prato e provincia) le fonti del CFR Toscana, le temperature, il Lamma, il centro funzionale Toscana ed il Biometeo Toscana. E successivamente twittano i dati prelevati. Negli script che utilizzerete è necessario inserire i codici della app al passo 2. Ogni script può essere programmato per essere eseguito su un server tramite una <a href="http://it.wikipedia.org/wiki/Crontab" target="_blank">CronTab</a> in base ad ogni quanto volete tuittare i dati. Attenzione: non programmare gli script se non ce n&#8217;è bisogno e mai troppo spesso altrimenti rischi di fare solo spam su twitter!
</li>
<li style="text-align: justify;">
  Tra gli script troverete anche l&#8217;applicazione per creare il robot che comunica con la app Telegram.
</li>
<li style="text-align: justify;">
  Create un account IFTT con la mail del servizio che hai realizzato e crea tutte le ricette dei social che ti serve aggregare nel tuo servizio Twitter. Le mie sono <a href="https://ifttt.com/p/pratopioggia/shared" target="_blank">queste</a>. Ovviamente in tutti i social devi creare sensibilizzazione e attenzione al servizio perchè la gente impari ad usarlo (quindi non usare ricette troppo complesse).
</li>
<li style="text-align: justify;">
  <a href="https://www.slideshare.net/pratosmart/emergenzeprato?from_m_app=ios">Questa</a> è una presentazione del progetto e <a href="http://pratosmart.teo-soft.com/emergenzeprato/">questa</a> la<b> pagina web</b>
</li>

E adesso tocca a te! che aspetti?

Riusano questo progetto:

  * <a href="https://twitter.com/ProtCivComuneFi" target="_blank"><strong>Protezione Civile di Firenze</strong></a>