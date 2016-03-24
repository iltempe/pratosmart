---
id: 683
title: 'L&#8217;analisi dei sentimenti tramite i social'
date: 2014-07-15T09:00:12+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=683
permalink: /lanalisi-dei-sentimenti-tramite-social/
dsq_thread_id:
  - 3027861466
categories:
  - Hackers
  - Laboratorio
  - Opendata
---
<p style="text-align: justify;">
  Una città che sa gestire le informazioni a disposizione è una città che sa capire cosa i suoi cittadini pensano e provano riguardo ad un certo argomento. E i cittadini oggi parlano, e parlano molto tramite i social network. Come ho detto da sempre, a cosa serve creare cultura dei social media se poi non sappiamo usare e gestire l&#8217;immensa mole di dati che si generano tramite questi?
</p>

<p style="text-align: justify;">
  Come potremmo pensare di analizzare ogni singolo parere espresso tramite un tweet rispetto ad un hashtag senza una gestione informatizzata delle informazioni? Non so se qualcuno di voi ha osservato la frequenza ad esempio con cui venivano generati i tweet con il tag <a title="La cronaca dei #mondiali2014 fatta da tutti noi su Twitter" href="http://pratosmart.teo-soft.com/la-cronaca-dei-mondiali2014-fatta-da-tutti-noi-su-twitter/" target="_blank">#Mondiali2014</a>. Sarebbe impensabile leggerseli tutti per capire quali sono stati i sentimenti delle persone generati da questo evento.
</p>

<p style="text-align: justify;">
  E quindi? &#8230; e quindi normalmente quello che fanno le grandi aziende (che fanno marketing sui social media) è l&#8217;analisi dei sentimenti tramite algoritmi che prelevano le informazioni dai social e la visualizzazione dei dati per prendere decisioni in merito ai loro prodotti/servizi. Per chi è dentro un po&#8217; la materia della informatica e della statistica non si tratta di niente di complesso. Tutto è basato sull&#8217;applicazione di metodi di ricerca di parole con accezione negativa o positiva dentro ogni elemento analizzato. Tramite questa analisi si associa un punteggio all&#8217;elemento testuale in analisi e si definisce se l&#8217;elemento è di carattere positivo o negativo. Se la mole di dati analizzata è ampia questo permette di fare valutazioni alquanto interessanti.
</p>

<p style="text-align: justify;">
  Sono qui a domandarmi e a domandarvi quindi perchè una città come Prato (la cui popolazione è così attiva sui social) non potrebbe effettuare questo tipo di analisi per definire il valore che i contenuti social hanno in città.
</p>

<p style="text-align: justify;">
  Questo è usare i nostri dati. Questo è comprendere cosa dice la gente dentro Facebook, Twitter&#8230;
</p>

<p style="text-align: justify;">
  Prendendo spunto dai principi illustrati <a href="http://www.slideshare.net/jeffreybreen/r-by-example-mining-twitter-for" target="_blank">qui</a> ho implementato un semplice algoritmo (creato in <a href="http://www.r-project.org/" target="_blank">linguaggio R</a>) per fare un&#8217;analisi dei sentimenti su tweet in lingua inglese contenenti la parola #arduino e #innovation.
</p>

<p style="text-align: justify;">
  Non poteva inoltre mancare un esempio fatto per la nostra città: e così ecco i sentimenti legati a 500 tweet emessi in zona Prato.
</p>

<p style="text-align: justify;">
  I tweet che hanno ottenuto score pari a 0 sono tweet &#8220;neutrali&#8221;, quelli con punteggio positivo hanno un&#8217;accezione positiva, quelli con punteggio negativo hanno un&#8217;accezione negativa. Su questo tema ho intenzione di perfezionare il mio algoritmo, chiunque abbia dei suggerimenti si faccia vivo, vi aspetto qui. E ricordate: una città che vuol far valere i suoi dati non li regala a Facebook o Twitter, ma li usa.
</p>

<!-- Flickr Photostream by Miro Mannino -->

<div id="flickrGal3" class="justified-gallery" >
  <a href="https://www.flickr.com/photos/125814874@N05/14678762653/in/set-72157645286450678/lightbox" target="_blank" title="I sentimenti a Prato in 500 tweets"><img alt="I sentimenti a Prato in 500 tweets" src="https://farm4.static.flickr.com/3876/14678762653_78e75b21fc_m.jpg" data-safe-src="https://farm4.static.flickr.com/3876/14678762653_78e75b21fc_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/14468826989/in/set-72157645286450678/lightbox" target="_blank" title="feelings of #arduino in 500 tweets"><img alt="feelings of #arduino in 500 tweets" src="https://farm6.static.flickr.com/5521/14468826989_6f9c8a7317_m.jpg" data-safe-src="https://farm6.static.flickr.com/5521/14468826989_6f9c8a7317_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/14645145124/in/set-72157645286450678/lightbox" target="_blank" title="Sentiment Analysis of #Innovation"><img alt="Sentiment Analysis of #Innovation" src="https://farm4.static.flickr.com/3888/14645145124_3003f526a1_m.jpg" data-safe-src="https://farm4.static.flickr.com/3888/14645145124_3003f526a1_m.jpg" /></a>
</div>

&nbsp;