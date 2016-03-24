---
id: 1536
title: Le fermate degli autobus di Prato su OpenStreetMap
date: 2014-12-04T21:01:18+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=1536
permalink: /le-fermate-degli-autobus-di-prato-su-openstreetmap/
dsq_thread_id:
  - 3291009695
categories:
  - Blog
  - Hackers
  - Opendata
tags:
  - autobus
  - bus stop
  - opendata
---
[<img class="alignleft  wp-image-1538" src="http://pratosmart.teo-soft.com/wp-content/uploads/2014/12/Disegno-senza-titolo.jpg" alt="Disegno senza titolo" width="617" height="462" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2014/12/Disegno-senza-titolo-300x225.jpg 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2014/12/Disegno-senza-titolo.jpg 960w" sizes="(max-width: 617px) 100vw, 617px" />](http://pratosmart.teo-soft.com/wp-content/uploads/2014/12/Disegno-senza-titolo.jpg)Prima di iniziare il mio approfondimento su <a title="Il “catasto 2.0″ si chiama OpenStreetMap" href="http://pratosmart.teo-soft.com/il-catasto-2-0-si-chiama-openstreetmap/" target="_blank">OpenStreetMap</a> le fermate dei bus mappate a Prato erano poche centinaia, con una mappatura aggiornata a qualche anno fa.

In realtà andando a verificare le fermate rilasciate come dati aperti sul portare degli opendata della regione Toscana (<a href="http://open.toscana.it/" target="_blank">OpenToscana</a>) si trova <a href="http://dati.toscana.it/dataset/8bb8f8fe-fe7d-41d0-90dc-49f2456180d1/resource/f42cbd9e-be0c-4bab-af32-1fee4160796a/download/c.a.p.0111201431122014googletransit.zip" target="_blank">questo</a> archivio di fermate di bus tutte taggate con un identificativo e georeferenziate in città.

Mi sono chiesto: perchè allora non inserirle come punti dentro OpenStreetMap? Adesso ogni fermata mappata dai dati della regione Toscana ha:

  * Identificativo (campo Ref)
  * Nome
  * Compagnia di Trasporti

<p style="text-align: justify;">
  Oltre ad un <a href="http://wiki.openstreetmap.org/wiki/IT:Import/Guidelines" target="_blank">import</a> (e ad una validazione) con il software <a href="https://josm.openstreetmap.de/" target="_blank">JOSM</a> dei dati non esistenti, ho fatto un&#8217;azione manuale di inserimento dati sulle zone dove i dati della Regione si sovrapponevano con quelli esistenti in modo (dove era necessario) da fare merge delle informazioni. L&#8217;operazione ha richiesto un lavoro accurato perchè in questi casi si deve stare molto attenti a non danneggiare i dati esistenti.
</p>

<p style="text-align: justify;">
  Ovviamente anche le informazioni della Regione potrebbero non essere precisissime e quindi chiunque (previa verifica) può correggere i dati di OSM modificandoli e se vuole segnalando l&#8217;aggiornamento degli opendata <a href="http://open.toscana.it/" target="_blank">qui</a>.
</p>

<p style="text-align: justify;">
  Delle vecchie fermate mappate ne restano ad oggi alcune che sono da verificare tramite ispezione in loco oppure grazie alla conoscenza di chi abita vicino. Sono rintracciabili <a href="http://overpass-turbo.eu/map.html?Q=%2F*%0AThis%20has%20been%20generated%20by%20the%20overpass-turbo%20wizard.%0AThe%20original%20search%20was%3A%0A%E2%80%9C%22Bus%20Stop%22%20and%20note%3DTBD%E2%80%9D%0A*%2F%0A%5Bout%3Ajson%5D%5Btimeout%3A25%5D%3B%0A%2F%2F%20gather%20results%0A(%0A%20%20%2F%2F%20query%20part%20for%3A%20%E2%80%9C%22Bus%20Stop%22%20and%20note%3DTBD%E2%80%9D%0A%20%20node%5B%22highway%22%3D%22bus_stop%22%5D%5B%22note%22%3D%22TBD%22%5D(43.81396800431211%2C10.943756103515625%2C43.982933852960805%2C11.269569396972656)%3B%0A)%3B%0A%2F%2F%20print%20results%0Aout%20body%3B%0A%3E%3B%0Aout%20skel%20qt%3B" target="_blank">qui</a> : nelle note trovate una stringa &#8220;TBD&#8221;, quindi chi può si dia da fare, grazie.
</p>

<p style="text-align: justify;">
  PS Un grazie a <a href="http://de.straba.us/" target="_blank">Napo</a>, che mi ha supportato inizialmente dandomi qualche dritta con cui affrontare l&#8217;impresa.
</p>