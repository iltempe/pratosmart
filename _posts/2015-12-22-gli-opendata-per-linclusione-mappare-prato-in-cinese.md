---
id: 2317
title: 'Gli opendata per l&#8217;inclusione: mappare Prato in cinese'
date: 2015-12-22T12:14:38+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=2317
permalink: /gli-opendata-per-linclusione-mappare-prato-in-cinese/
dsq_thread_id:
  - 4424882922
categories:
  - Hackers
  - Opendata
tags:
  - cinese
  - openstreetmap
  - osm
  - prato
---
<p style="text-align: justify;">
  E&#8217; circa un anno che ho avviato all&#8217;interno della piattaforma <strong><a href="https://www.facebook.com/groups/1561722390780986/" target="_blank">M&#8217;Appare Prato</a>,</strong> un <a href="http://www.slideshare.net/pratosmart/mappare-prato-anche-in-cinese" target="_blank">progetto</a> di creazione di <em>opendata</em> a servizio della mia città per supportare i cinesi che come sapete a Prato rappresentano una realtà importante della città. Il progetto consente di essere applicato da subito a qualunque altra lingua per altre città.
</p>

<p style="text-align: justify;">
  Ho scoperto, parlando con chi opera per l&#8217;inclusione, che esiste un problema di orientamento delle persone che arrivano a Prato dalla Cina. Ma sono anche convinto che, nel prossimo futuro, &#8220;tradurre la città&#8221; sarà una risorsa per la città stessa, in termini per esempio di turismo ma anche di commercio.
</p>

<p style="text-align: justify;">
  Alla base di tutto c&#8217;è l&#8217;idea di usare <a href="http://www.openstreetmap.org/" target="_blank">Openstreetmap</a> come grande piattaforma di partecipazione su cui riversare la traduzione dei nomi dei luoghi in lingua cinese, iniziando da quelli più importanti per i cittadini cinesi stessi (ufficio immigrazione, la questura, uffici postali etc&#8230;). Questo come punto di partenza non solo per creare servizi in lingua, ma anche per avere un repository cittadino di informazioni a cui accedere per il riuso.
</p>

<p style="text-align: justify;">
  Per questa operazione di mappatura è stato necessario (ed è tutt&#8217;ora necessario) sensibilizzare. I pratesi e i cinesi devono capirne l&#8217;importanza. E&#8217; stato un anno in cui ho cercato di spiegare questo: non solo per avere una mappa in multi-lingua, ma anche per far capire il potenziale che ha Prato in termini di conoscenza che se trasformata in dato aperto costituisce un possibile valore.
</p>

<p style="text-align: justify;">
  Tradurre in cinese i nomi dei punti di interesse, delle piazze o delle attività commerciali non è cosa banale. Ho scoperto che alcuni luoghi di Prato sono conosciuti dai cinesi perchè li hanno ribattezzati con un nome completamente diverso dal nome italiano perchè li associano ad una loro percezione di quel posto. E&#8217; il motivo per cui alcune traduzioni puoi farle solo intervistando le persone di nazionalità cinese. Per i nomi delle strade invece si apprende che molte non hanno una vera e propria traduzione. Abbiamo iniziato quindi a mappare alcuni luoghi, organizzandoci con alcune persone che forniscono i dati (i luoghi con relativa traduzione del nome) e persone che mappano. <strong>Chiunque può contribuire</strong>.
</p>

<p style="text-align: justify;">
  <strong>Tutta la traduzione della città è basata sulla gestione di un tag Openstreetmap (<em>name) </em>degli oggetti mappati</strong>. Per aggiungere nomi di località in lingue diverse è possibile usare un suffisso a questo tag. Per indicare il nome in cinese di un luogo di Prato si usa <strong>name:zh</strong>, (mentre per il suo nome in inglese <tt>name:en)</tt>. Il nome di default deve essere quello nella lingua locale. I codici per le lingue sono quelli definiti dal codice alpha-2 dello <a href="http://www.loc.gov/standards/iso639-2/php/code_list.php" target="_blank">standard ISO 639-2</a>. Se si vuole indicare la traduzione in pinyin (cinese con caratteri leggibili da occidentali) va usato <strong>name:zh_pinyin</strong>.
</p>

<p style="text-align: justify;">
  Di seguito una breve procedura per inserire dati in cinese in Openstreetmap e per usarli. <strong>Chiunque può dare supporto alla causa</strong>.
</p>

<h3 style="text-align: justify;">
  Procedura per inserire dati su Openstreetmap in lingua cinese
</h3>

  1. Se non siete ancora utenti, iscrivetevi a <a href="http://www.openstreetmap.org" target="_blank">Openstreetmap</a>
  2. Individuate il punto di interesse o l’edificio che vi interessa tradurre in lingua. Se non esiste sulla mappa aggiungetelo direttamente inserendo nel tag _name_ il suo nome prima in lingua italiana.
  3. Aggiungete il nome del posto con il tag _name_ nella lingua in cui volete tradurre il punto mappato. Come detto sopra per il cinese va usato _name:zh_ per il nome in ideogrammi. Potete anche usare _name:zh_pinyin_ per il nome in cinese con caratteri standard.
  4. Se non volete o non potete mappare il luogo in Openstreetmap potete comunque reperire il nome del luogo, l&#8217;indirizzo e la sua traduzione e chiedere una mano al <a href="https://www.facebook.com/groups/1561722390780986/" target="_blank">gruppo dei mappatori su Facebook</a> affidandovi a loro.

<h3 style="text-align: justify;">
  Procedura per usare i dati di Openstreetmap in lingua cinese
</h3>

<p style="text-align: justify;">
  Tutti i dati di Openstreetmap mappati in una certa lingua possono essere visualizzati con tool di interrogazione Openstreetmap come OverpassTurbo. Con <a href="http://overpass-turbo.eu/s/dmW">questo link</a> ad esempio visualizzate i luoghi mappati in cinese di Prato ad oggi.  Scaricando il file dei dati in formato <strong>geoJson</strong> potete creare una mappa con le indicazioni che avete tradotto e che sono inserite all&#8217;interno di Openstreetmap. Per esempio archiviando gli attuali dati tradotti su github vedrete questa mappa.
</p>



Se poi avete confidenza con ambienti di lavoro come <a href="https://www.mapbox.com" target="_blank">Mapbox</a> potete divertirvi ad usare i dati per fare mappe come quella sotto.

Un paio di esempi di possibili mappe che si possono creare

  * Una mappa in doppia lingua creata da me con Mapbox è visibile [qui](https://api.mapbox.com/styles/v1/iltempe/ciih8iw2300c0brkmkmd5qhz8.html?title=true&access_token=pk.eyJ1IjoiaWx0ZW1wZSIsImEiOiJjaWloN3NwbHAwMDA5dnFtNjNuZTE5cjlnIn0.Iuvy3L21YoURJrQrly2oWA#14.09/43.8855/11.0839) con i luoghi mappati ad oggi.
  * Un mappa che mostra Prato con i luoghi in cinese via via che sono mappati la trovate <a href="https://api.mapbox.com/styles/v1/iltempe/cij1k30qk003icam59eo8iyft.html?title=true&access_token=pk.eyJ1IjoiaWx0ZW1wZSIsImEiOiJjaWloN3NwbHAwMDA5dnFtNjNuZTE5cjlnIn0.Iuvy3L21YoURJrQrly2oWA#14.244975988674852/43.88246470979311/11.08937891092097/0" target="_blank">qui</a>. (creata sempre con Mapbox)

[<img class="aligncenter size-medium" title="" src="http://pratosmart.teo-soft.com/wp-content/uploads/2016/01/img_1239.jpeg" alt="" width="583" height="360" />](http://pratosmart.teo-soft.com/wp-content/uploads/2016/01/img_1239.jpeg)

<h3 style="text-align: justify;">
  Altro Materiale
</h3>

<p style="text-align: justify;">
  <a href="http://www.slideshare.net/pratosmart/mappare-prato-anche-in-cinese" target="_blank">Qui</a> la mia presentazione fatta presso Meltin-PO. <a href="http://www.slideshare.net/pratosmart/note-openstreetmap-in-lingua-cinese?related=1" target="_blank">Qui</a> una presentazione in cinese su Openstreetmap. <a href="http://wiki.openstreetmap.org/wiki/WikiProject_China" target="_blank">Qui</a> il progetto wiki di mappatura della Cina. Altre indicazioni su come mappare in più lingue con Openstreetmap si trovano <a href="http://wiki.openstreetmap.org/wiki/Multilingual_names" target="_blank">qui</a>. <a href="http://wiki.openstreetmap.org/wiki/Zh-hant:Beginners%27_guide" target="_blank">Qui</a> il getting started di OSM in cinese.
</p>

<h3 style="text-align: justify;">
  Crediti
</h3>

<li style="text-align: justify;">
  Un ringraziamento va a <strong><a href="http://de.straba.us/" target="_blank">Maurizio Napolitano</a></strong> (in arte Napo) che è stato il primo a farmi capire che la mia città aveva questo tipo di opportunità.
</li>
<li style="text-align: justify;">
  Un grazie all&#8217;associazione <strong><a href="https://www.facebook.com/meltinpo" target="_blank">Meltin-Po</a></strong> che da tempo opera a Prato per l&#8217;inclusione e con cui abbiamo fatto <a href="http://pratosmart.teo-soft.com/come-fare-una-mappa-di-prato-cinese-e-tutte-le-lingue-del-mondo-con-openstreetmap/" target="_blank">un incontro di sensibilizzazione con la comunità cinese</a> e abbiamo spiegato come si mappano alcuni luoghi.
</li>
<li style="text-align: justify;">
  Un grazie per la raccolta dei dati va ai ragazzi attivissimi del <a href="http://www.centrointerazioni.it/" target="_blank">Centro Inter-Azioni</a> che operano nell&#8217;ambito del <a href="http://www.poloprato.unifi.it/it/ricerca/laboratori/progetto-prato/home.html" target="_blank">Progetto Prato</a> all&#8217;interno del <strong><a href="http://www.poloprato.unifi.it/it/home-polo.html?no_cache=1">Polo Universitario di Prato</a></strong>. In particolare grazie a <strong>Iacopo Benini</strong>, <strong>Ilaria Mundula</strong> e <strong>Yang Guang: </strong>con queste persone sono tutt&#8217;ora in stretto contatto per la mappatura continua di nuovi dati all&#8217;interno di Openstreetmap.
</li>
<li style="text-align: justify;">
  Grazie a chiunque vorrà contribuire a questo progetto cosi importante per la città.
</li>

<div id='gallery-1' class='gallery galleryid-2317 gallery-columns-3 gallery-size-thumbnail'>
  <figure class='gallery-item'> 
  
  <div class='gallery-icon landscape'>
    <a href='http://pratosmart.teo-soft.com/gli-opendata-per-linclusione-mappare-prato-in-cinese/1660742_319438808246778_1054773938652458649_n/'><img width="150" height="150" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/12/1660742_319438808246778_1054773938652458649_n-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="incontro da meltin-po" aria-describedby="gallery-1-2339" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-1-2339'> incontro da meltin-po </figcaption></figure><figure class='gallery-item'> 
  
  <div class='gallery-icon landscape'>
    <a href='http://pratosmart.teo-soft.com/gli-opendata-per-linclusione-mappare-prato-in-cinese/10953186_319438798246779_8682457695955999612_n-2/'><img width="150" height="150" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/12/10953186_319438798246779_8682457695955999612_n-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="incontro da meltin-po" aria-describedby="gallery-1-2345" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-1-2345'> incontro da meltin-po </figcaption></figure><figure class='gallery-item'> 
  
  <div class='gallery-icon portrait'>
    <a href='http://pratosmart.teo-soft.com/gli-opendata-per-linclusione-mappare-prato-in-cinese/10858448_319438828246776_2188011069374954310_n/'><img width="150" height="150" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/12/10858448_319438828246776_2188011069374954310_n-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="incontro da meltin-po" aria-describedby="gallery-1-2343" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-1-2343'> incontro da meltin-po </figcaption></figure><figure class='gallery-item'> 
  
  <div class='gallery-icon portrait'>
    <a href='http://pratosmart.teo-soft.com/gli-opendata-per-linclusione-mappare-prato-in-cinese/10342988_319438874913438_7320467679646356160_n/'><img width="150" height="150" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/12/10342988_319438874913438_7320467679646356160_n-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="incontro da meltin-po" aria-describedby="gallery-1-2342" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-1-2342'> incontro da meltin-po </figcaption></figure><figure class='gallery-item'> 
  
  <div class='gallery-icon landscape'>
    <a href='http://pratosmart.teo-soft.com/gli-opendata-per-linclusione-mappare-prato-in-cinese/1975115_319438788246780_4466341676256034410_n/'><img width="150" height="150" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/12/1975115_319438788246780_4466341676256034410_n-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="incontro da meltin-po" aria-describedby="gallery-1-2341" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-1-2341'> incontro da meltin-po </figcaption></figure><figure class='gallery-item'> 
  
  <div class='gallery-icon landscape'>
    <a href='http://pratosmart.teo-soft.com/gli-opendata-per-linclusione-mappare-prato-in-cinese/1969124_319438844913441_1384434076793234196_n/'><img width="150" height="150" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/12/1969124_319438844913441_1384434076793234196_n-150x150.jpg" class="attachment-thumbnail size-thumbnail" alt="incontro da meltin-po" aria-describedby="gallery-1-2340" /></a>
  </div><figcaption class='wp-caption-text gallery-caption' id='gallery-1-2340'> incontro da meltin-po </figcaption></figure>
</div>