---
id: 1434
title: Come farsi mandare una mail da una schedino elettronico grande quanto una carta di credito
date: 2014-11-08T11:27:38+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=1434
permalink: /come-farsi-mandare-una-mail-da-una-schedino-elettronico-grande-quanto-una-carta-di-credito/
dsq_thread_id:
  - 3204257555
categories:
  - Hackers
  - Internet Nelle Cose
  - Laboratorio
tags:
  - internet of things
  - iot
  - nodejs
  - nodered
  - pratopioggia
---
<p style="text-align: justify;">
  <a href="http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/Schermata-2014-11-07-alle-20.26.42.jpg"><img class="alignleft  wp-image-1437" src="http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/Schermata-2014-11-07-alle-20.26.42-1024x513.jpg" alt="Schermata 2014-11-07 alle 20.26.42" width="419" height="210" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/Schermata-2014-11-07-alle-20.26.42-300x150.jpg 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/Schermata-2014-11-07-alle-20.26.42-1024x513.jpg 1024w, http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/Schermata-2014-11-07-alle-20.26.42-150x75.jpg 150w" sizes="(max-width: 419px) 100vw, 419px" /></a>Oggi due parole su come si fa a creare in poco tempo un sistemino per farsi inviare una mail all&#8217;avvenire di un particolare evento (come l&#8217;invio di un tweet taggato <a title="Piove. Anche a #Prato piove. Cerchiamo almeno di usare #twitter" href="http://pratosmart.teo-soft.com/piove-anche-prato-piove-cerchiamo-almeno-di-usare-twitter/" target="_blank">#pratopioggia</a>) da una scheda <a title="Un signor computer da 35 euro : ecco a voi Raspberry Pi" href="http://pratosmart.teo-soft.com/un-signor-computer-da-35-euro-ecco-voi-raspberry-pi/" target="_blank">Raspberry</a> come quelle che vi ho presentato qui nella mia rubrica dell&#8217;internet of things.
</p>

<p style="text-align: justify;">
  Il concetto è molto semplice ed sviluppabile in tanti altri modi: qui l&#8217;idea di base è come sia possibile creare un sistema che prendendo in ingresso un evento (come un tweet) può creare un dato in internet (come una mail).
</p>

<p style="text-align: justify;">
  Cosa va fatto?
</p>

<li style="text-align: justify;">
  Configurate il Raspberry come descritto <a title="Come si fa il primo setup di un Raspberry B+" href="http://pratosmart.teo-soft.com/come-si-fa-il-primo-setup-di-un-raspberry-b/" target="_blank">qui</a>
</li>
<li style="text-align: justify;">
  Connettete la scheda in rete con un normalissimo cavo ethernet al vostro router di casa e accendetela
</li>
<li style="text-align: justify;">
  Connettetevi con un normale computer alla scheda con una connessione sicura (SSH) come descritto <a href="http://www.raspberrypi.org/documentation/remote-access/ssh/" target="_blank">qui</a>
</li>
<li style="text-align: justify;">
  Installate sulla scheda il framework NODE.JS con i seguenti comandi
</li>

    wget http://node-arm.herokuapp.com/node_latest_armhf.deb
    sudo dpkg -i node_latest_armhf.deb

<p style="text-align: justify;">
  5. Installate il framework <a href="http://nodered.org/" target="_blank">Node Red</a> sulla scheda come descritto <a href="https://learn.adafruit.com/raspberry-pi-hosting-node-red/setting-up-node-red" target="_blank">qui</a>
</p>

<p style="text-align: justify;">
  Ora siete in grado di connettervi all&#8217;ambiente che avete sulla scheda via browser digitando <span class="pln">http</span><span class="pun">:</span><span class="com">//INDIRIZZO_IP_DEL_RASPBERRY:1880 oppure <span class="pln">http</span><span class="pun">:</span><span class="com">//INDIRIZZO_IP_DEL_RASPBERRY:1880/admin (in base a come avete installato il framework)</span></span>
</p>

<p style="text-align: justify;">
  A questo punto spostate e configurate 3 nodi come nella figura sotto
</p>

<li style="text-align: justify;">
  Uno per accedere a Twitter e cercare tutti i tweet taggati #<a title="Piove. Anche a #Prato piove. Cerchiamo almeno di usare #twitter" href="http://pratosmart.teo-soft.com/piove-anche-prato-piove-cerchiamo-almeno-di-usare-twitter/" target="_blank">pratopioggia</a>
</li>
<li style="text-align: justify;">
  Uno per inviare una mail
</li>
<li style="text-align: justify;">
  Uno per debug di quello che viene letto dalla vostra applicazione.
</li>

<p style="text-align: justify;">
  Fate Click su Deploy e&#8230;Il gioco è fatto! Twittare per credere!
</p>

<img class="aligncenter size-large wp-image-1435" src="http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/Schermata-2014-11-07-alle-22.26.57-1024x489.png" alt="Schermata 2014-11-07 alle 22.26.57" width="656" height="313" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/Schermata-2014-11-07-alle-22.26.57-300x143.png 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/Schermata-2014-11-07-alle-22.26.57-1024x489.png 1024w" sizes="(max-width: 656px) 100vw, 656px" />

[<img class="wp-image-1436 aligncenter" src="http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/Schermata-2014-11-07-alle-22.21.49-1024x358.jpg" alt="Schermata 2014-11-07 alle 22.21.49" width="493" height="172" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/Schermata-2014-11-07-alle-22.21.49-300x105.jpg 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/Schermata-2014-11-07-alle-22.21.49-1024x358.jpg 1024w" sizes="(max-width: 493px) 100vw, 493px" />](http://pratosmart.teo-soft.com/wp-content/uploads/2014/11/Schermata-2014-11-07-alle-22.21.49.jpg)