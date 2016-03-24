---
id: 1215
title: La mappa OpenIncidenti è online
date: 2014-09-03T23:28:15+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=1215
permalink: /la-mappa-openincidenti-e-online/
dsq_thread_id:
  - 3027839137
categories:
  - Blog
  - Hackers
  - Opendata
tags:
  - crowdsourcing
  - opendata
  - openincidenti
---
<p style="text-align: justify;">
  Da quando ho dato vita all’iniziativa web <a href="www.pratociclabili.com" target="_blank">Prato Ciclabili</a>, molte volte mi sono posto il problema di effettuare delle ricerche sui dati degli incidenti stradali che coinvolgono ciclisti, incidenti che nella nostra zona sono purtroppo ancora numerosi.
</p>

<p style="text-align: justify;">
  <a href="http://pratosmart.teo-soft.com/wp-content/uploads/2014/09/Schermata-2014-09-04-alle-00.13.06.png"><img class="alignleft size-large wp-image-1216" src="http://pratosmart.teo-soft.com/wp-content/uploads/2014/09/Schermata-2014-09-04-alle-00.13.06-1024x386.png" alt="Schermata 2014-09-04 alle 00.13.06" width="656" height="247" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2014/09/Schermata-2014-09-04-alle-00.13.06-300x113.png 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2014/09/Schermata-2014-09-04-alle-00.13.06-1024x386.png 1024w" sizes="(max-width: 656px) 100vw, 656px" /></a>Purtroppo censire gli incidenti è cosa complessa se nessuno contribuisce a tenere aggiornati i dataset che li riguardano.
</p>

<p style="text-align: justify;">
  Si badi bene: non sto parlando di metodologie per segnalare un incidente, per questo esistono i mezzi di comunicazione ufficiali verso le forze dell’ordine. Parlo piuttosto di censire un incidente perché è da questo modo di censire che possiamo evidenziare ad esempio se esistono zone nelle nostre città particolarmente pericolose e di conseguenza attivare processi decisionali in merito alla sicurezza.
</p>

<p style="text-align: justify;">
  E’ quindi da una discussione su Facebook che ho avuto in questi giorni con <a href="http://about.me/flaviamarzano">Flavia Marzano</a> che chiedeva più pubblicazione di dati in merito a questi eventi, che ci è venuto in mente di lanciare una campagna nazionale in formato open data di crowdsourcing. Il nome del progetto è <b>#openincidenti</b> e si prefigge lo scopo tramite registrazione su mappa di rilevare in Italia le zone più a rischio per la sicurezza. Il contributo può essere di tutti e i dati sono rilasciati in licenza aperta. Unico vincolo: solo chi ha inserito un incidente può eliminare lo stesso incidente dalla mappa (funzione da usare se ritiene di aver fatto un errore nell’inserimento dati).
</p>

<p style="text-align: justify;">
  <a href="http://teo-soft.com/openincidenti" target="_blank"><strong>Clicca qui per visualizzare la mappa </strong></a>: è possibile registrare un incidente cliccando sulla mappa e inserendo pochi dati sulla quantità di mezzi di trasporto coinvolti. Viene richiesto un indirizzo mail di chi registra (unico dato personale) a cui viene inviato una password da usare per poter eliminare un incidente inserito. E’ inoltre possibile effettuare un download di tutti i dati attualmente come un database.
</p>

<p style="text-align: justify;">
  Come sempre accetto critiche, suggerimenti e idee.
</p>

<p style="text-align: justify;">
  ALCUNE NOTE TECNICHE DI RILASCIO
</p>

<p style="text-align: justify;">
  Questa volta la ricetta adottata è:
</p>

  * backend fatto in <a href="http://www.sqlite.org/" target="_blank">Sqlite</a> con metodi di gestione in PHP
  * frontend in HTML5, CSS e JS (Bootstrap Framework)
  * Ovviamente mappa basata su OSM

PS: Ringrazio tutta la community [spaghetti open data](http://www.spaghettiopendata.org/) che ogni tanto mi da’ qualche dritta per implementare le mie idee.