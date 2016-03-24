---
id: 2428
title: Inviare note ai mappatori Openstreetmap passeggiando in città
date: 2016-02-14T09:38:12+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=2428
permalink: /inviare-note-ai-mappatori-openstreetmap-passeggiando-in-citta/
dsq_thread_id:
  - 4577992358
categories:
  - Blog
  - Hackers
  - Laboratorio
  - Opendata
tags:
  - iot
  - map
  - opendata
  - openstreetmap
---
<p style="text-align: justify;">
  Oggi un semplicissimo tutorial su <a href="https://www.openstreetmap.org" target="_blank">Openstreetmap</a> che non prevede conoscenze particolari di programmazione. Tra le varie funzionalità che questa mappa mette a disposizione di tutti c&#8217;è la possibilità (secondo me sottovalutata) di scrivere delle note in un punto della mappa per fornire indicazioni a chi deve modificare la mappa stessa. Quindi annotare su Openstreetmap è un modo per contribuire a tenere aggiornate le mappe della propria città (e non solo della propria). E&#8217; possibile creare queste note anche senza essere iscritti a Openstreetmap, per cui la funzione si presta molto bene nel caso abbiate un gruppo di mappatori in città sempre attivi a cui volete affidare dei compiti indicando sulla mappa qualcosa da mappare facendo un aggiornamento. Il mappatore che troverà questa nota avrà le indicazioni per aggiornare la mappa.  Ma anche se siete un mappatore che passaggia in città e volete annotare su Openstreetmap un compito da svolgere a casa con calma la cosa fa a caso vostro. Per ogni indicazione su cosa si può scrivere nelle note e come usarle rimando al <a href="http://wiki.openstreetmap.org/wiki/IT:Notes" target="_blank">wiki di Openstreetmap</a>.
</p>

<p style="text-align: justify;">
  Anzichè annotare qualcosa su Openstreetmap dalla mappa stessa tramite browser supponiamo di essere in giro per la  nostra città e di voler notificare qualcosa da appuntare direttamente su mappa. Quello che scrivo di seguito è un metodo che si può implementare in vari modi (c&#8217;è chi lo ha fatto anche con <a href="https://telegram.me/OSMNotesBot" target="_blank">Telegram</a>). Io vi presento un modo semplice di farlo predispondendo una ricetta su DO di <a href="https://ifttt.com" target="_blank">IFTTT</a> che ho scoperto essere un&#8217;ottima soluzione per automatizzare azioni da smartphone, è usabile da tutti perchè non richiede programmazione. Per questa ricetta useremo <a href="https://ifttt.com/products/do/note" target="_blank">DO Note</a> che consente di inviare testo ad un&#8217;applicazione tramite la semplice pressione di un pulsante. In particolare per questa ricetta dovete abilitare il canale <a href="https://ifttt.com/maker" target="_blank">Maker</a> che vi consente di associare alla pressione di un pulsante un&#8217;azione per un servizio web o oggetti connessi ad internet. Dobbiamo fare in modo che quindi nel momento in cui si scrive una nota con DO e premiamo il pulsante questa nota venga annotata su openstreetmap con la nostra posizione rilvata con smartphone in quel preciso istante. Come si fa? Create una ricetta con IFTTT del tipo <strong>DO->Maker</strong> fatta cosi
</p>

<p style="text-align: justify;">
  <img class="size-large wp-image-2432 aligncenter" src="http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-13-alle-23.11.07-1024x718.png" alt="Schermata 2016-02-13 alle 23.11.07" width="660" height="463" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-13-alle-23.11.07-300x210.png 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-13-alle-23.11.07-768x539.png 768w, http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-13-alle-23.11.07-1024x718.png 1024w" sizes="(max-width: 660px) 100vw, 660px" />
</p>

<p style="text-align: justify;">
  Salvate la ricetta su smartphone ed adesso siete pronti per annotare su Openstreetmap scrivete le vostre notazioni per i mappatori e premete il pulsante!
</p>

<p style="text-align: justify;">
  <img class="alignleft size-full wp-image-2435" src="http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Add_a_note_screenshot.png" alt="Add_a_note_screenshot" width="213" height="75" />Le note saranno trasferite direttamente sulla mappa Openstreetmap (visibili a tutti) e potranno essere risolte e prese in carico da chi opera sulla piattaforma di mappatura basterà andare su Openstreetmap e selezionare il livello note per vederle!
</p>

<p style="text-align: justify;">
  <img class="wp-image-2434 alignleft" src="http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/IMG_3009-576x1024.jpg" alt="IMG_3009" width="291" height="517" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/IMG_3009-169x300.jpg 169w, http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/IMG_3009-576x1024.jpg 576w" sizes="(max-width: 291px) 100vw, 291px" />
</p>

<p style="text-align: justify;">
  <img class="wp-image-2433 alignright" src="http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/image2-576x1024.png" alt="image2" width="289" height="514" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/image2-576x1024.png 576w, http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/image2.png 750w" sizes="(max-width: 289px) 100vw, 289px" /><img class="size-medium wp-image-2431 alignleft" src="http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-13-alle-23.08.43-300x227.png" alt="Schermata 2016-02-13 alle 23.08.43" width="300" height="227" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-13-alle-23.08.43-300x227.png 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-13-alle-23.08.43-768x581.png 768w, http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-13-alle-23.08.43-1024x775.png 1024w, http://pratosmart.teo-soft.com/wp-content/uploads/2016/02/Schermata-2016-02-13-alle-23.08.43.png 1412w" sizes="(max-width: 300px) 100vw, 300px" />
</p>