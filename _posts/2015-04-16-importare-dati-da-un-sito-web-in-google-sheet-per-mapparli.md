---
id: 1897
title: Importare dati da un sito web in Google Sheet per mapparli
date: 2015-04-16T12:40:48+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=1897
permalink: /importare-dati-da-un-sito-web-in-google-sheet-per-mapparli/
dsq_thread_id:
  - 3686318211
categories:
  - Blog
  - Hackers
  - Laboratorio
tags:
  - comuni
  - dataviz
  - dati
  - google sheet
  - prato
  - web scraping
---
Ho ricevuto un paio di richieste la scorsa settimana per chiarire come poter velocemente formattare un set di dati presenti su un sito web in un <a href="https://docs.google.com/spreadsheets/u/0/" target="_blank">foglio Google Doc</a>.

<p style="text-align: justify;">
  Non starò qui a ribadire che Google Doc è a mio avviso un’ottima soluzione per elaborare documentazione in cloud, per cui importare e lavorare su dati in questo ambiente di lavoro consente di averli a disposizione (sempre e ovunque) anche tramite dispositivi mobile per consultarli, modificarli e presentarli. Non conosco ancora alternative valide a questo modo di elaborare documentazione in cloud computing.
</p>

<p style="text-align: justify;">
  Facciamo quindi un esercizio molto semplice. Supponiamo che abbiate necessità di lavorare su un set di dati presenti in un sito web per creare una vostra semplice applicazione basata su una mappa. Ovviamente attenzione a ciò che ri-pubblicate online: con google sheet avete modo di pubblicare i dati (elaborati o no) ma occhio alla licenza dei dati che avete importato, deve essere consentito il riuso!
</p>

Supponiamo di voler importare da <a href="https://www.wikipedia.org/" target="_blank">Wikipedia </a>una lista dei comuni della Toscana più popolosi che si trovano in forma tabellare <a href="https://it.wikipedia.org/wiki/Toscana" target="_blank">qui</a>, in modo da poterli mappare e far vedere dove si trova il comune di Prato e il suo numero di abitanti. Non saranno dati aggiornati, ma per quello che dobbiamo fare non serve. Come fare?.

****Importare i dati****

Aprite un foglio Google e nella cella in alto a sinistra (la A1) inserite la formula:

_=importHtml(&#8220;https://it.wikipedia.org/wiki/Toscana&#8221;, &#8220;table&#8221;, 12)_

dove _ImportHtml_ consente di importare dati dalla pagina Wikipedia <a href="https://it.wikipedia.org/wiki/Toscana" target="_blank">https://it.wikipedia.org/wiki/Toscana</a>. il parametro “table”, 12  consente di importare la dodicesima tabella presente nel sito.

Ecco il risultato che dopo qualche secondo si ottiene:



&nbsp;

I dati importati non sono modificabili in quanto linkati dinamicamente alla tabella wikipedia. Per cui se cambia quella tabella i dati saranno aggiornati automaticamente.

<p style="text-align: justify;">
  <strong><strong> </strong></strong>Se volete realizzare una mappa di questi dati ci sono molte alternative: la più rapida è quella di usare sempre la suite Google Doc in particolare potete usare una <a href="http://tables.googlelabs.com/" target="_blank">Google Fusion Table</a> che è uno strumento non basato su mappe libere, ma se lo scopo è avere una mappa in poco tempo per visualizzare un po’ di dati e non avete come missione quello di produrre dati aperti va benissimo.
</p>

****Mappare i dati****

<p style="text-align: justify;">
   Aprite quindi una Google Fusion Table quando create la tabella vi verrà chiesto da dove importare i dati, selezionate l’opzione Google Spreadsheet e specificate lo sheet dove avete importato i vostri dati. Specificate che nella prima riga è presente un’intestazione. Nell’importing dei dati in modo automatico lo strumento riconosce che ci sono dei nomi di città e le localizza su Google Maps associandoci i dati relativi al comune che sono stati trovati nel foglio. Potete divertirvi ad editare un po’ la mappa cambiando i colori, i marker e qualche altra opzione.
</p>

**** ****



Avete appena mostrato a partire dai dati e tramite una mappa che Prato è il secondo comune della Toscana per abitanti 😉