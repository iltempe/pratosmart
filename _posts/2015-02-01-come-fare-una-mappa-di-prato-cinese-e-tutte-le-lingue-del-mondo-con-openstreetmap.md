---
id: 1720
title: Come fare una mappa di Prato in cinese (e in tutte le lingue del mondo) con openstreetmap
date: 2015-02-01T18:56:45+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=1720
permalink: /come-fare-una-mappa-di-prato-cinese-e-tutte-le-lingue-del-mondo-con-openstreetmap/
dsq_thread_id:
  - 3475804299
categories:
  - Blog
  - Opendata
  - 'Prato&amp;Ilmondo'
tags:
  - cinese
  - openstreetmap
  - prato
---
<p style="text-align: justify;">
  Con l&#8217;associazione <a href="https://www.facebook.com/meltinpo?fref=ts" target="_blank">Meltin-PO</a>,  che a Prato opera costantemente per un&#8217;inclusione degli immigrati nella nostra città e nella nostra cultura, ieri abbiamo iniziato insieme un percorso per arricchire le mappe <a href="http://www.openstreetmap.org/" target="_blank">Openstreetmap</a> del nostro territorio assieme alle persone provenienti da paesi stranieri che vivono a Prato (in maggioranza cinesi). L&#8217;idea è di popolare Openstreetmap a Prato con dati in lingua cinese (e non solo) in modo da creare mappe fruibili per gli stranieri che vivono e vivranno nella nostra città, ma anche per turisti.
</p>

<p style="text-align: justify;">
  La presentazione che ho fatto (e che è stata tradotta in lingua cinese mentre presentavo grazie a dei ragazzi volontari che si sono offerti di farlo) è <a href="http://www.slideshare.net/pratosmart/mappare-prato-anche-in-cinese" target="_blank">questa</a>.
</p>

<p style="text-align: justify;">
  Di seguito riporto un tutorial di come si può creare una mappa della propria città in lingue diverse che possa servire per Prato ma anche per altre persone che in Italia che vogliano ripetere lo stesso nostro percorso.
</p>

<h3 style="text-align: justify;">
  INSERIRE IN OPENSTREETMAP DATI IN MULTILINGUA
</h3>

<p style="text-align: justify;">
  Meltin-PO organizzerà un gruppo di lavoro con persone di qualsiasi nazionalità che possano arricchire le Openstreetmap di Prato iniziando dai punti di interesse (ospedali, uffici pubblici&#8230;).
</p>

<li style="text-align: justify;">
  Iscrivetevi a <a href="www.openstreetmap.org" target="_blank">Openstreetmap</a>
</li>
<li style="text-align: justify;">
  Individuate il punto di interesse o l&#8217;edificio che vi interessa tradurre in lingua. Se non esiste sulla mappa aggiungetelo direttamente inserendo nel tag &#8220;name&#8221; il suo nome in lingua italiana.
</li>
<li style="text-align: justify;">
  Aggiungete il nome del posto con il tag name nella lingua in cui volete tradurre il punto mappato. Per il cinese abbiamo individuato &#8220;name:zh&#8221; per il nome in ideogrammi. Potete anche usare &#8220;name:zh_pinyin&#8221; per il nome in caratteri per i nomi in cinese con caratteri standard. Trovate tutti gli altri tag delle lingue utilizzabili <a href="http://wiki.openstreetmap.org/wiki/Multilingual_names" target="_blank">qui</a>.
</li>
<li style="text-align: justify;">
  Eseguite le operazioni 2 e 3 per ogni punto che volete mappare e l&#8217;operazione 3 per ogni lingua in cui volete tradurre il punto di interesse.
</li>

### CREARE UNA MAPPA MULTILINGUA

Una volta popolato Openstreetmap del vostro territorio con le informazioni che vi servono in lingue diverse potrete facilmente creare una mappa in doppia lingua (ad esempio italiano-cinese) oppure anche in più di due. Seguite questi semplici passaggi:

  1. Iscrivetevi a <a href="http://umap.openstreetmap.fr/it/" target="_blank">UMAP</a>
  2. Creare una nuova mappa
  3. Aggiungete un livello di dati inserendo nel campo URL della voce dati remoti questo link

http://overpass-api.de/api/interpreter?data=\[out:json][timeout:25];(node[&#8220;name:zh&#8221;\](43.79092385423621,10.938949584960938,43.97082781825965,11.239700317382812);way\[&#8220;name:zh&#8221;\](43.79092385423621,10.938949584960938,43.97082781825965,11.239700317382812);relation\[&#8220;name:zh&#8221;\](43.79092385423621,10.938949584960938,43.97082781825965,11.239700317382812););out body;>;out skel qt;

Questo link è un&#8217;interrogazione a Openstreetmap che consente di visualizzare tutti i luoghi mappati in lingua cinese della zona di Prato (sostituendo il campo &#8220;name:zh&#8221; con altri tag multilingua potrete fare livelli in altre lingue). Per creare una mappa di un&#8217;altra città dovrete creare il link corrispondente alla vostra città con <a href="http://overpass-turbo.eu/" target="_blank">Overpass turbo</a>.

Nel campo Popup Content Template potete inserire queste due chiavi

\*\*{name}\*\*
  
#{name:zh}

per visualizzare quando si clicca su un punto di interesse il nome del luogo in italiano (name) e la sua traduzione ad esempio in cinese (name:zh) e ulteriori traduzioni se volete aggiungere altre lingue e se avete inserito i dati in lingua dentro openstreetmap.

Fatto!

Ieri abbiamo visto come si mappa l&#8217;ospedale di Prato, i pompieri, la questura e il circolo sede dell&#8217;associazione. Ecco cosa è venuto fuori!
  


[Visualliza schermo intero](http://umap.openstreetmap.fr/it/map/mappare-prato-anche-in-cinese_27310)