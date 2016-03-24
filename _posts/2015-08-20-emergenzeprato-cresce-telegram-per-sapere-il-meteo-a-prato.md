---
id: 2084
title: 'Emergenzeprato cresce: Telegram per sapere il meteo a Prato'
date: 2015-08-20T11:00:44+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=2084
permalink: /emergenzeprato-cresce-telegram-per-sapere-il-meteo-a-prato/
dsq_thread_id:
  - 4048561720
categories:
  - Hackers
  - Internet Nelle Cose
  - Opendata
tags:
  - emergenzeprato
  - iot
  - opendata
  - prato
  - telegram
---
<p style="text-align: justify;">
  Da un po&#8217; di tempo avevo intenzione di fare crescere il mio progetto <a href="http://pratosmart.teo-soft.com/emergenzeprato/" target="_blank">Emergenzeprato</a> con il concetto di Instant Messenger e di Internet of Things. Da oggi potete parlare infatti con Emergenzeprato se avete <a href="https://telegram.org/" target="_blank">Telegram</a> installato sul vostro telefono.
</p>

<p style="text-align: justify;">
  Ho già <a href="http://pratosmart.teo-soft.com/chattare-con-il-proprio-frigorifero-telegram-raspberry/" target="_blank">applicato Telegram</a>, ma qui ne faremo un uso un po&#8217; diverso ovvero lo useremo per parlare con un &#8220;<strong>robot emergenzeprato</strong>&#8221; (che altro non è che un software programmato in modo opportuno) per sapere le previsioni del tempo del giorno e quelle del giorno dopo (dati che emergenzeprato tuitta periodicamente anche su Twitter).
</p>

<img class="  wp-image-2097 aligncenter" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/08/Schermata-2015-08-21-alle-00.49.09-1024x564.png" alt="Schermata 2015-08-21 alle 00.49.09" width="682" height="376" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/08/Schermata-2015-08-21-alle-00.49.09-300x165.png 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/08/Schermata-2015-08-21-alle-00.49.09-1024x564.png 1024w" sizes="(max-width: 682px) 100vw, 682px" />

Come si fa ad usarlo? Semplice.

  1. Installate Telegram sul vostro smatphone o sul vostro computer (l&#8217;applicazione è multipiattaforma)
  2. Aggiungete l&#8217;utente <a href="https://telegram.me/emergenzeprato_bot" target="_blank">@emergenzeprato_bot</a> ai vostri contatti Telegram
  3. A questo punto vi comparirà una tastiera con dei pulsanti per invio dei comandi possibili. Per far apparire la tastiera con i pulsanti facilitati come in figura sotto (se avete già avviato una chat e la tastiera non fosse presente) digitate il comando **/start** oppure cancellate la chat e riapritene un&#8217;altra con emeregenzeprato_bot. Se preferite inviare i comandi con la tastiera a singoli caratteri iniziando a digitare / nella chat, Telegram vi suggerirà tutti i comandi disponibili da poter inviare al servizio. Ad oggi questi comandi sono: 
      * **_/meteo_ per ricevere il meteo (e il biometeo) del giorno**
      * **_/previsioni_ per ricevere il meteo (e il biometeo) del giorno dopo **
      * **_/rischi_ per ricevere l&#8217;elenco dei rischi metereologici del giorno legati a Prato**
  4. Riceverete le relative risposte nella conversazione entro 1 minuto circa

I dati sono quelli che Emergenzeprato tratta e sono dettagliati nella relativa pagina del progetto <a href="http://pratosmart.teo-soft.com/emergenzeprato/" target="_blank">qui</a>.

Così oggi abbiamo messo assieme: Opendata, Internet Of Things, Tecnologia Mobile, Messaggeria Istantanea e Informative Meteo Locali. Mica poco. No?

Per ogni suggerimento o segnalazione contattatemi!

<p style="text-align: justify;">
  <strong>PER GLI SMANETTONI:</strong> per chi volesse implementare una cosa analoga il <a href="https://github.com/TeoSoft80/Emergenzeprato" target="_blank">codice sorgente</a> aggiornato è su Github. Alla base c&#8217;è la costruzione di un <a href="https://telegram.org/blog/bot-revolution" target="_blank">robot telegram</a> su cui è stata sviluppata un&#8217; applicazione PHP a partire da <a href="https://github.com/Eleirbag89/TelegramBotPHP" target="_blank">questo</a> progetto. Attualmente il &#8220;robot&#8221; è installato su una scheda Raspberry Pi connessa in rete (costo dell&#8217;infrastruttura IT 35 euro). Non sono stati effettuati test intensivi di risposta ma attualmente il software è programmato per rispondere entro un minuto di tempo. Per ogni segnalazione sto qua.
</p>

<p style="text-align: justify;">
  <a href="http://pratosmart.teo-soft.com/wp-content/uploads/2015/08/IMG_2001.png"><img class="  wp-image-2106 aligncenter" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/08/IMG_2001-576x1024.png" alt="IMG_2001" width="337" height="599" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/08/IMG_2001-576x1024.png 576w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/08/IMG_2001.png 750w" sizes="(max-width: 337px) 100vw, 337px" /></a>
</p>