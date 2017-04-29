---
id: 2215
title: Suonare un megafono con i dati aperti di rischio idrogeologico
date: 2015-10-20T14:18:13+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=2215
permalink: /suonare-un-megafono-con-i-dati-aperti-di-rischio-idrogeologico/
dsq_thread_id:
  - 4242285856
categories:
  - Blog
  - Hackers
  - Internet Nelle Cose
  - Laboratorio
  - Makers
tags:
  - emergenzeprato
  - iot
  - opendata
  - prato
---
<p style="text-align: justify;">
  <a href="http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/IMG_2329.jpg"><img class=" wp-image-2218 alignright" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/IMG_2329-1024x768.jpg" alt="IMG_2329" width="472" height="354" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/IMG_2329-300x225.jpg 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/IMG_2329-1024x768.jpg 1024w" sizes="(max-width: 472px) 100vw, 472px" /></a>Devo dire la verità. Questa idea me l&#8217;ha infilata in testa una persona che lavora alla protezione civile di Prato quando un anno fa parlai di Twitter come possibile strumento per inviare aggiornamenti delle allerte via web. Questa persona mi disse &#8220;non sottovaluti la potenza del megafono, ingegnere, dove si arriva con quello Twitter non arriva&#8221;. Da nativo digitale quale sono in quella situazione non diedi la giusta importanza a quelle parole. Poi ci ho ripensato su ed effettivamente poi ho compreso: se tu devi dare un&#8217;allarme o un&#8217;allerta o anche solo comunicare un possibile rischio devi fare si comunicazione online, ma devi farla anche e soprattutto sul posto. Ecco perchè il megafono è ancora molto sponsorizzato dalla protezione civile, perchè permette di allertare chi è intorno a noi (anche se non ha internet).
</p>

<p style="text-align: justify;">
  Detto questo mi sono chiesto: e perchè non unire la rapidità del web e dei dati sul rischio idrogeologico con la possibilità di far suonare una sirena o un megafono non appena si dichiara stato di rischio online?
</p>

Con <a href="https://iltempe.github.io/Emergenzeprato/" target="_blank">emergenzeprato</a> questo è stato piuttosto semplice da realizzare per due motivi:

  * I dati di rischio idrogeologico sono online e vengono aggiornati tutti i giorni
<li style="text-align: justify;">
  I dati sono gestiti da un server host, ma ogni funzione di emergenzeprato è programmata da una schedina Raspberry B come <a href="http://www.amazon.it/Raspberry-Pi-Model-Plus-512MB/dp/B00LPESRUK/ref=sr_1_2?ie=UTF8&qid=1445341544&sr=8-2&keywords=raspberry+pi+b" target="_blank">questa</a>. Cosa è raspberry? Leggete <a href="http://pratosmart.teo-soft.com/un-signor-computer-da-35-euro-ecco-voi-raspberry-pi/" target="_blank">qui</a>. In parole povere è un computerino che vi consente di eseguire alcuni programmi ed, essendo connesso ad internet, vi consente di creare oggetti costantemente connessi. Nel nostro caso la useremo per dimostrare come un megafono può essere connesso ad internet per inviare l&#8217;allerta in città. Tutti i dati prima di essere inviati sul server sono scaricati sulla schedina che conosce quindi lo stato del rischio del giorno.
</li>

<p style="text-align: justify;">
  <a href="http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/sound.jpg"><img class="alignleft wp-image-2216" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/sound-1024x709.jpg" alt="sound" width="574" height="397" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/sound-300x208.jpg 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/sound-1024x709.jpg 1024w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/10/sound.jpg 1491w" sizes="(max-width: 574px) 100vw, 574px" /></a>Ho simulato il megafono connettendo alla scheda un piccolo altoparlante portatile di <a href="http://www.amazon.it/gp/product/B00OJ43RIK?psc=1&redirect=true&ref_=oh_aui_detailpage_o00_s00" target="_blank">questo tipo</a>. Ovviamente con un megafono con un ingresso audio come <a href="http://www.amazon.it/MEGAFONO-FUNZIONE-MICROFONO-TRASPORTO-TRASFORMATORE/dp/B00N3MLB8C/ref=sr_1_1?s=electronics&ie=UTF8&qid=1445341856&sr=1-1&keywords=megafono+ingresso" target="_blank">questo</a> si può ottenere lo stesso effetto, è sufficiente avere un qualunque dispositivo con un ingresso audio da connettere alla scheda raspberry con un cavetto jack, come schematicamente riportato in figura.
</p>

A questo punto per eseguire la prima configurazione dell&#8217;audio del raspberry eseguite questo comando un connessione SSH

    amixer cset numid=3 1

&nbsp;

Su raspberry eseguire un file audio è a questo punto roba da un&#8217;istruzione:

<pre class=" language-bash"><code class=" language-bash">omxplayer example&lt;span class="token punctuation">.&lt;/span>mp3</code></pre>

&nbsp;

<p style="text-align: justify;">
  Quindi se adesso volete capire come inserire tutto questo in un&#8217;applicazione, tenete presente che emergenzeprato ha un file getting.php che consente di leggere i dati periodicamente memorizzati da quanto pubblicato online. Eseguendo periodicamente il file <a href="https://github.com/iltempe/Emergenzeprato/blob/master/alert_risk.php" target="_blank">alert_risk.php</a> di emergenzeprato ogni giorno che un rischio verrà rilevato, la vostra sirena connessa ad internet suonerà (il suono è configurabile con un file audio a vostra scelta). Ricordatevi di cancellare il file alarm.txt una volta che volete riprogrammare l&#8217;allarme (il sistema è fatto in modo che l&#8217;allarme suoni una volta sola non appena si rileva un rischio).
</p>

La logica con cui inviare l&#8217;allarme può essere modificata ma il concetto è e resta uno solo: gli opendata per animare un oggetto connesso ad internet, di grande utilità in caso di allerta.