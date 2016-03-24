---
id: 1933
title: 'Chattare con il proprio frigorifero: Telegram &#038; Raspberry'
date: 2015-05-29T11:17:30+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=1933
permalink: /chattare-con-il-proprio-frigorifero-telegram-raspberry/
dsq_thread_id:
  - 3803469634
categories:
  - Blog
  - Hackers
  - Internet Nelle Cose
  - Laboratorio
tags:
  - internet of everething
  - internet of things
  - iot
  - raspberry
---
<p style="text-align: justify;">
  <a href="https://telegram.org/" target="_blank">Telegram</a> è un servizio basato su cloud di messaggeria instantanea. A differenza di altre app come WhatsApp si tratta di una applicazione opensource che nasce con l&#8217;idea di essere anche una base per applicazioni più complesse.
</p>

<p style="text-align: justify;">
  Avevo in testa dai tempi di <a title="#HACKTOSCANA : ha vinto la LEGO ;-)" href="http://pratosmart.teo-soft.com/hacktoscana-ha-vinto-la-lego/" target="_blank">Hacktoscana</a> di provare ad usare un servizio del genere di comunicazione istantanea tra uomini e macchine (basato su opensource) ed oggi vi presento questo mio esperimento.
</p>

<p style="text-align: justify;">
  Partendo da <a href="https://geekytheory.com/tutorial-raspberry-pi-uso-de-telegram-con-python/" target="_blank">questo</a> post, ho provato ad installarlo su un computer di tipo <a title="Un signor computer da 35 euro : ecco a voi Raspberry Pi" href="http://pratosmart.teo-soft.com/un-signor-computer-da-35-euro-ecco-voi-raspberry-pi/" target="_blank">Raspberry</a> B+ per valutare come un oggetto dotato di sensori e una scheda Raspberry attraverso la rete possa inviare messaggi come fosse un normalissimo utente e quindi &#8220;parlare&#8221; con umani che abbiano l&#8217;applicazione installata su smartphone o su altro computer. In questo caso un frigorifero e Matteo usando lo stesso profilo parlano tra loro (o meglio il frigo parla a Matteo, farlo rispondere a domande è un po&#8217; più complesso).
</p>

<p style="text-align: justify;">
  Devo dire che il principio funziona&#8230; e funziona bene. D&#8217;altra parte il fatto che il software sia opensource e completamente disponibile in termini di sorgenti online aiuta e non poco. Considerate che ogni frase inviata dal nostro frigo simulato può essere associata ad una precisa condizione dei suoi sensori: è possibile quindi definire una precisa notifica in base a quale alimento manca in frigo.
</p>

<p style="text-align: justify;">
  <img class="  wp-image-1935 alignleft" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/05/IMG_1248.png" alt="IMG_1248" width="282" height="502" />Ho quindi rispolverato il mio Raspberry, come avevo <a title="Come si fa il primo setup di un Raspberry B+" href="http://pratosmart.teo-soft.com/come-si-fa-il-primo-setup-di-un-raspberry-b/" target="_blank">configurato</a> qua. E qualcuno ora mi dirà: &#8220;grazie, Matteo&#8230;ma che ci faccio con questo attrezzo?&#8221;  Immaginate ad esempio che questa scheda Raspberry sia installata dentro un elettrodomestico e che tramite un sensore (come <a href="http://wirelesstag.net/" target="_blank">questo</a> o <a href="http://www.shopnfc.it/it/" target="_blank">questi</a>) possa rilevare la presenza di latte fresco.  Considerate che a schede come Raspberry si possono connettere vari tipi di sensori. Ecco, quindi, cosa potreste vedere sul vostro smartphone nel caso il frigo rilevasse che nel frigo il latte è stato terminato.
</p>

Stessa cosa se la scheda monitorasse con una cam connessa cosa c&#8217;è e cosa manca e vi aggiornasse ogni giorno su cosa avete in fresco, potrebbe mandarvi immagini!

Per gli smanettoni che volessero provare a mettere in piedi la cosa i comandi per installare Telegram su Raspberry sono questi.

&nbsp;

**INSTALLAZIONE**

  1. Dopo esservi connessi via SSH alla scheda connessa in rete, installate le librerie necessarie 
    <pre>sudo apt-get install libreadline-dev libconfig-dev libssl-dev lua5.2 liblua5.2-dev libevent-dev make</pre>

  2. Clonare il repository del codice di Telegram su Raspberry 
    <pre>git clone --recursive https://github.com/vysheng/tg.git && cd tg</pre>

<pre>./configure</pre>

<pre>make</pre>

Tutto questo richiederà un po&#8217; di tempo ma al termine della procedura avrete installato la applicazione sulla scheda.

**UTILIZZO**

Digitate

<pre>cd tg</pre>

<pre>bin/telegram-cli -k tg-server.pub -W</pre>

Dopo aver impostato il numero di cellulare su cui ricevere il codice di sicurezza (con il +39 per l&#8217;Italia) potrete iniziare la chat simulando che il frigo rilevi assenza di cibo (ad esempio).

  1. Comandi per invio messaggi di testo dal &#8220;frigo&#8221; 
    <pre>msg Nome_Cognome messaggio dal frigo</pre>
    
    <pre></pre>

  2. Per inviare una foto dal &#8220;frigo&#8221; invece digitare (supponendo di avere la foto nella cartella tg/folder
  3. <pre>send_photo Nome_Cognome /folder/foto.jpg</pre>

Nel momento in cui siete connessi con Telegram ogni messaggio inviato al frigo verrà visualizzato nella shell SSH aperta e digitando

<div>
  <ol>
    <li>
      <pre>history Nome_Cognome</pre>
    </li>
  </ol>
  
  <p>
    Otterrete tutti i messaggi che vi siete scambiati tu e il tuo frigo!
  </p>
</div>

<div>
  <img class="  wp-image-1936 aligncenter" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/05/Schermata-2015-05-28-alle-22.47.55.png" alt="Schermata 2015-05-28 alle 22.47.55" width="1092" height="168" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/05/Schermata-2015-05-28-alle-22.47.55-300x46.png 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/05/Schermata-2015-05-28-alle-22.47.55-1024x157.png 1024w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/05/Schermata-2015-05-28-alle-22.47.55-150x23.png 150w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/05/Schermata-2015-05-28-alle-22.47.55.png 1966w" sizes="(max-width: 1092px) 100vw, 1092px" />
</div>

Adesso non scordatevi più di passare a prendere il latte!