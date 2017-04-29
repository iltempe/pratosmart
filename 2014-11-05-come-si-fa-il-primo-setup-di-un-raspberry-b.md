---
id: 1426
title: Come si fa il primo setup di un Raspberry B+
date: 2014-11-05T21:05:45+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=1426
permalink: /come-si-fa-il-primo-setup-di-un-raspberry-b/
dsq_thread_id:
  - 3195605657
categories:
  - Internet Nelle Cose
tags:
  - iot
  - micro sd
  - raspberry
---
[<img class="alignleft size-medium wp-image-1428" src="http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/IMG_2511-300x225.jpg" alt="IMG_2511" width="300" height="225" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/IMG_2511-300x225.jpg 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/IMG_2511-1024x768.jpg 1024w" sizes="(max-width: 300px) 100vw, 300px" />](http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/IMG_2511.jpg)Stasera vi riporto in semplici passaggi ed in lingua italiana come si fa a fare il primo setup della scheda <a title="Un signor computer da 35 euro : ecco a voi Raspberry Pi" href="http://pratosmart.teo-soft.com/un-signor-computer-da-35-euro-ecco-voi-raspberry-pi/" target="_blank">Raspberry</a> , piattaforma alla base del mio Internet Nelle Cose.

Ho scelto di comprare la scheda assieme ad un case molto carino ed una micro SD Card da formattare e preparare &#8220;ad hoc&#8221;.

Come si procede? Semplice.

  1. Munirsi di un computer con possibilità di leggere la Micro SD
  2. Fari clic [<span class="goog-text-highlight">Downloads</span>](http://www.raspberrypi.org/downloads/)<span class="goog-text-highlight"> per accedere alla pagina di downloads dei sistemi operativi disponibili per la scheda.</span>
  3. Fare clic su `Download ZIP` sotto &#8216;NOOBS (offline e installazione di rete)&#8217;, e selezionare una cartella in cui salvarlo. Estrarre i file dal .zip.

**Preparare la scheda SD**

  1. Visita il [sito web di SD Association](http://www.sdcard.org/)  e scarica [SD Formatter 4.0](https://www.sdcard.org/downloads/formatter_4/) per Windows o Mac.
  2. Seguire le istruzioni per installare il software.
  3. Inserire la scheda SD nel lettore del computer o della scheda SD del computer portatile e prendere nota della lettera di unità assegnata
  4. In SD Formatter, selezionare la lettera di unità per la scheda SD e formattarla.

**Copiare i file relativi al sistema NOOBS**

  1. Una volta che la scheda SD è stata formattata, trascinare tutti i file dalla cartella NOOBS dentro la root della scheda SD.
  2. I file necessari saranno quindi copiati nella scheda SD.
  3. Quando questo processo è finito, rimuovere la scheda SD e inserirla nel Raspberry Pi.

**Prima Accensione [<img class="alignleft size-medium wp-image-1431" src="http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/IMG_2518-300x225.jpg" alt="IMG_2518" width="300" height="225" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/IMG_2518-300x225.jpg 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/IMG_2518-1024x768.jpg 1024w" sizes="(max-width: 300px) 100vw, 300px" />](http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/IMG_2518.jpg)**

  1. Collegare i cavi USB di una tastiera, un mouse e un monitor (potete usare un HDMI di un televisore LCD).
  2. Ora collegare il cavo di alimentazione al Pi.
  3. Il vostro Raspberry Pi si avvierà e apparirà una finestra con un elenco di diversi sistemi operativi che è possibile installare. Consiglio di scegliere  Raspbian e fare clic su `Installa` .
  4. Raspbian sarà quindi installato.
  5. Quando il processo di installazione è stato completato, il menu di configurazione Raspberry Pi (raspi-config) verrà caricato. Qui è possibile impostare l&#8217;ora e la data per la propria regione e fare un setup di una scheda con fotocamera Raspberry Pi, o addirittura creare gli utenti. È possibile uscire da questo menu utilizzando Tab sulla tastiera per spostarsi `su Fine` .

**Adesso avete un piccolo oggetto intelligente tra le vostre mani&#8230;un piccolo grande computer tutto da connettere e far parlare! E allora&#8230;si parte!**

NOTA BENE

Il default login for Raspbian è `pi` con password `raspberry`.

Per caricare l&#8217;interfaccia grafica digita `startx`.

[fonte <a href="http://www.raspberrypi.org/help/noobs-setup/" target="_blank">sito ufficiale Raspberry</a>]

&nbsp;