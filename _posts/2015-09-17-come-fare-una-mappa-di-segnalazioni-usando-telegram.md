---
id: 2148
title: Come fare una mappa di segnalazioni usando Telegram
date: 2015-09-17T11:02:12+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=2148
permalink: /come-fare-una-mappa-di-segnalazioni-usando-telegram/
dsq_thread_id:
  - 4137571549
categories:
  - Blog
  - Hackers
  - Laboratorio
  - Opendata
tags:
  - emergenzeprato
  - prato
  - social
  - telegram
---
<p style="text-align: justify;">
  Chi come me sperimenta col digitale si sarà sicuramente imbattuto in una di quelle applicazioni per segnalare tramite telefono un&#8217;informazione &#8220;georiferita&#8221; ossia associata ad un punto su una mappa.
</p>

<p style="text-align: justify;">
  Ho sempre avuto il pallino però di trovare un &#8220;prodotto&#8221; che consenta di fare questo indipendentemente da cosa si vuol segnalare in modo da aumentare il riuso del concetto di segnalazione: che tu stia segnalando una buca per strada, la presenza di un animale pericoloso, un sottopasso allagato o un bel paesaggio da visitare poco cambia tecnicamente. Tutte queste applicazioni infatti danno modo di associare un dato ad un punto nello spazio e lo inviano ad un server che normalmente ne consente l&#8217;utilizzo su una mappa.
</p>

<p style="text-align: justify;">
  <a href="https://telegram.org/" target="_blank">Telegram</a> pare fare a caso nostro in questo senso perchè è sempre possibile inviare attraverso la sua chat la propria posizione geografica (mica poco!) in modo tale che sia ricevuta.
</p>

<p style="text-align: justify;">
  <strong>Ho creato un esperimento per spiegare come MAPPARE le segnalazioni inviate ad un robot Telegram</strong>.
</p>

<p style="text-align: justify;">
  <a href="http://pratosmart.teo-soft.com/wp-content/uploads/2015/09/Schermata-2015-09-17-alle-02.23.38.png"><br /> </a>Il suo funzionamento è dimostrato nella applicazione <a href="http://iltempe.github.io/Emergenzeprato/" target="_blank">emergenzeprato</a> ma chiunque può rifarselo <a href="https://github.com/iltempe/TelegramMap" target="_blank">tramite questo codice</a> che ho rilasciato su Github.
</p>

<p style="text-align: justify;">
  Come funziona? Semplice:
</p>

<li style="text-align: justify;">
  Create un Robot con Telegram: per creare un Bot, bisogna scrivere ad un Bot, chiamato <a href="https://telegram.me/botfather" target="_blank">@BotFather</a>.  Non appena inizierà la chat, questo ci avviserà dei comandi usabili. Il primo comando è proprio ciò che ci serve: <em>/newbot</em>. Dando questo comando @BotFather ci chiederà dapprima il nome del nostro Bot, e poi l’username con cui potremo farlo aggiungere a chi vogliamo (il nome dopo la @, per intenderci). Quest’ultimo dovrà necessariamente terminare con “Bot”. Nomi validi quindi sono ilmiobot, superbot, ecc…, sempre che non siano già stati scelti da altri utenti. Una volta finita la creazione del Bot, @BotFather ci risponderà con un token da usare nella nostra applicazione per &#8220;pilotare il robot&#8221;.
</li>
<li style="text-align: justify;">
  A questo punto dovremo configurare il robot per rispondere ai comandi ricevuti dall&#8217;utente. Per usare il robot in questo senso è possibile usare due metodi (o tramite aggiornamenti a tempo o tramite il server webhook di Telegram). Per fare questo potete riferirvi alla documentazione di Telegram <a href="https://core.telegram.org/bots/api" target="_blank">qui</a>.
</li>
<li style="text-align: justify;">
  Nel momento in cui avete configurato tutto, <strong>l&#8217;utente per inviare una segnalazione deve</strong>: <ol>
    <li style="text-align: justify;">
      <strong>Inviare la propria posizione</strong> in chat tramite la &#8220;molletta&#8221; dell&#8217;allegato a sinistra in basso nella chat.<img class="  wp-image-2151 aligncenter" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/09/Schermata-2015-09-17-alle-02.23.23-1024x293.png" alt="Schermata 2015-09-17 alle 02.23.23" width="616" height="176" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/09/Schermata-2015-09-17-alle-02.23.23-300x86.png 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/09/Schermata-2015-09-17-alle-02.23.23-1024x293.png 1024w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/09/Schermata-2015-09-17-alle-02.23.23.png 1592w" sizes="(max-width: 616px) 100vw, 616px" />
    </li>
    <li style="text-align: justify;">
      <strong>Scrivere cosa vuol segnalare</strong> non appena il robot richiede le informazioni. Teoricamente nella risposta si potrebbero inviare foto, video, link oltre che testo (attualmente il mio esempio gestisce solo testo).
    </li>
  </ol>
</li>

Fatto!

Tutti i dati sono a questo punto memorizzati in una database (trasformato poi in un file .CSV) e &#8220;mappabili&#8221; su una pagina web come ho fatto qui. Semplice no?<img class="  wp-image-2152 aligncenter" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/09/Schermata-2015-09-17-alle-02.23.38-1024x458.png" alt="Schermata 2015-09-17 alle 02.23.38" width="537" height="240" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/09/Schermata-2015-09-17-alle-02.23.38-300x134.png 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/09/Schermata-2015-09-17-alle-02.23.38-1024x458.png 1024w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/09/Schermata-2015-09-17-alle-02.23.38.png 1560w" sizes="(max-width: 537px) 100vw, 537px" />

<p style="text-align: justify;">
  Chi volesse provare ad usare il sistema può farlo con il robot di <a href="https://telegram.me/emergenzeprato_bot" target="_blank">EmergenzePrato</a> : t<strong>rattasi ovviamente di servizio sperimentale e puramente dimostrativo</strong>.
</p>

Buone Mappe a Tutti!

[<img class="  wp-image-2154 aligncenter" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/09/Schermata-2015-09-17-alle-02.25.59-1024x674.png" alt="Schermata 2015-09-17 alle 02.25.59" width="477" height="314" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/09/Schermata-2015-09-17-alle-02.25.59-300x198.png 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/09/Schermata-2015-09-17-alle-02.25.59-1024x674.png 1024w" sizes="(max-width: 477px) 100vw, 477px" />](http://pratosmart.teo-soft.com/wp-content/uploads/2015/09/Schermata-2015-09-17-alle-02.25.59.png)