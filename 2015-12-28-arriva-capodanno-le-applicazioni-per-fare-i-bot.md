---
id: 2373
title: 'Arriva Capodanno: le applicazioni per fare i &#8220;BOT&#8221;'
date: 2015-12-28T11:47:01+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=2373
permalink: /arriva-capodanno-le-applicazioni-per-fare-i-bot/
dsq_thread_id:
  - 4440203519
categories:
  - Blog
tags:
  - app
  - bot
  - opendata
  - web
---
<p style="text-align: justify;">
  Mi permetto di giocare con le parole oggi ed indicarvi le migliori app sperimentate dal sottoscritto per creare dei &#8220;BOT di Capodanno&#8221; (leggi come RO-BOT). Il BOT, chi mi segue lo sa, non è altro che un meccanismo software che emula un umano nell&#8217;usare una applicazione inserendo dati, pubblicando informazioni e rispondendo a richieste ben definite. Chi vi parla è convinto (nonostante tante cose che si sentono dire in ogni angolo del web) che creare ROBOT sia un&#8217;ottima soluzione per sviluppare servizi (pubblici o privati) perchè consente di usare piattaforme esistenti che chiunque può utilizzare per altri scopi ed avere all&#8217;interno anche il servizio integrato.
</p>

> <p style="text-align: justify;">
>   Per esempio: usare Telegram per chattare con gli amici ma allo stesso tempo <strong>all&#8217;interno della stessa applicazione</strong> avere una chat che mi notifica le previsioni del tempo del giorno dopo&#8230;chiaro no? Significa che esiste una tecnologia che vi consente di NON sviluppare una APP specifica per quella esigenza (almeno fino a quando il vostro servizio si basa su un semplice invio e ricezione informazioni)!
> </p>

<p style="text-align: justify;">
  Ok, vediamo adesso le applicazioni più significative con cui potete sviluppare un BOT in modo che a capodanno possiate sbizzarrirvi. Tutte richiedono un minimo di programmazione, ma automatizzare alcune semplici azioni senza programmare è possibile anche tramite servizi web come <a href="https://ifttt.com/">IFTT</a> o la sua alternativa Opensource <a href="https://bip.io/">Bipio</a>.
</p>

#### <a href="https://telegram.org/" target="_blank">Telegram</a>

<p style="text-align: justify;">
  Sicuramente la più nota applicazione per fare i BOT. Ormai anche in Italia è presente una community interessata al tema. Cito tra tutti il caso della Protezione Civile di Firenze che riusa il BOT <a href="http://pratosmart.teo-soft.com/emergenzeprato-cresce-telegram-per-sapere-il-meteo-a-prato/" target="_blank">EmergenzePrato</a> e quanto fatto da <a href="http://www.piersoft.it/?p=626" target="_blank">Francesco Piersoft Paolicelli</a>. La piattaforma Telegram è costituita da una applicazione per smartphone gratuitamente scaricabile. Se avete dimestichezza con lo sviluppo per applicazioni web troverete non complesso sviluppare un BOT che tramite una chat vi comunichi informazioni o risponda a precisi comandi. Le API per accedere al server telegram sono aperte e liberamente usabili a patto che prima si registri il nome del BOT e ti venga rilasciato un token (codice alfanumerico) da usare all&#8217;interno del vostro codice. Oltre ad EmergenzePrato per ricevere informazioni sul meteo e rischio idrogeologico esempi significativi che ho visto in questi giorni il <a href="http://giovanni.pirrotta.it/blog/2015/10/28/protezione-civile-palermo-telegram-bot/" target="_blank">bot che comunica le aree di accoglienza della Protezione Civile di Palermo</a>, il bot per sapere gli <a href="https://telegram.me/pugliaeventsbot" target="_blank">eventi in Puglia</a>, il <a href="https://telegram.me/soldipubblicigovitbot" target="_blank">bot per sapere le spese del tuo comune</a>, il <a href="http://trentinocorrierealpi.gelocal.it/trento/cronaca/2015/12/23/news/app-per-viaggiare-gratis-in-busa-1.12663928?ref=hftrtnec-5&refresh_ce" target="_blank">bot per gestire un sistema di car pooling</a> . Telegram è ottimo non solo per inviare contenuti ma anche per raccogliere informazioni dagli utenti non solo testo ma anche foto, video e posizione geografica. Alcune indicazioni per iniziare a realizzare per creare un BOT Telegram sono <a href="http://pratosmart.teo-soft.com/come-fare-una-mappa-di-segnalazioni-usando-telegram/" target="_blank">qui</a>. L&#8217;introduzione per gli sviluppatori è <a href="https://core.telegram.org/bots" target="_blank">qui</a>.
</p>

<h4 style="text-align: justify;">
  <a href="https://twitter.com/?lang=it" target="_blank">Twitter</a>
</h4>

<p style="text-align: justify;">
  Non scordiamoci che anche Twitter, la piattaforma più famosa di microblogging, consente la possibilità di creare BOT. Ho spiegato come si fa <a href="http://pratosmart.teo-soft.com/fatti-un-pratopioggia-tutto-tuo-e-chiamalo-hopratopioggiaancheio/" target="_blank">qui</a> e sul repository Emergenzeprato trovate un esempio di implementazione nella cartella <a href="https://github.com/iltempe/Emergenzeprato/tree/master/TwitterBot" target="_blank">TwitterBot</a>. Twitter è un social ideale per gli aggiornamenti periodici di un contenuto per cui per tutte le applicazioni che devono &#8220;postare molto spesso&#8221; si presta bene (esempio previsioni del tempo, ma anche aggiornamenti da un blog o da un repository di contenuti web). E&#8217; possibile poi creare sistemi che permettano di rispondere o rituittare tweet con un certo hashtag: se non si può o vuole programmare una buona applicazione che consente di creare semplici regole che si basano su hashtag monitoring è sicuramente <a href="https://ifttt.com/">IFTT</a> o la sua alternativa Opensource <a href="https://bip.io/">Bipio</a>.
</p>

<h4 style="text-align: justify;">
  <a href="https://support.google.com/calendar/?hl=it#topic=3417969" target="_blank">Google Calendar</a>
</h4>

<p style="text-align: justify;">
  Un BOT un po&#8217; più &#8220;a senso unico&#8221; in termini di comunicazione, ma sicuramente utile quando si deve creare automaticamente un calendario eventi oppure quando si devono postare informazioni in modo periodico. Interessante notare che con un &#8220;attrezzo Google Calendar&#8221; se il calendario che create è pubblico potrà aggiunto usato da ogni utente tra i calendari della sua agenda visualizzandolo quindi anche su dispositivi mobile. Sarete quindi in grado di far ricevere le notifiche eventi a chi vi segue solo facendo aggiungere un calendario a quelli esistenti. Un esempio di come si può usare Google Calendar è <a href="http://pratosmart.teo-soft.com/meteo-e-rischio-idrogeologico-su-google-calendar/" target="_blank">qui</a>.
</p>

<h4 style="text-align: justify;">
  <a href="https://groupme.com/" target="_blank">GroupMe</a>
</h4>

<p style="text-align: justify;">
  Nasce come sistema di messaggeria instantanea indicato per messaggerie di gruppo. Nativamente fornisce la possibilità di aggiungere al gruppo un utente BOT che dica a quel gruppo quello che sa. Ideale per chi vuol comunicare informazioni automaticamente ad una community già costituita. Interessante notare che tra i sistemi con cui è possibile ricevere comunicazioni esiste anche l&#8217;SMS se l&#8217;utente registra il suo numero telefonico all&#8217;interno del servizio. Un esempio di quanto da me sperimentato lo trovate <a href="https://github.com/iltempe/Emergenzeprato/tree/master/GroupMeBot" target="_blank">qui</a>.
</p>

<h4 style="text-align: justify;">
  <a href="https://slack.com/" target="_blank">Slack</a>
</h4>

<p style="text-align: justify;">
  <strong>Slack è una piattaforma per comunicazione interna ai gruppi di lavoro</strong>, per contribuire in mobilità (o a grandi distanze) a un progetto comune. In altre parole, se più persone lavorano su un progetto, è possibile discutere in tempo reale/differito delle sue differenti caratteristiche e/o obiettivi, in stanze  molto simili a quelle dell’indimenticato IRC, solo in modo più semplice e con la possibilità di cercare velocemente il materiale passato. Si integra perfettamente con Twitter, Hangouts, DropBox.  Anche Slack nativamente consente la possibilità di creare <a href="https://api.slack.com/bot-users" target="_blank">robot</a> che possano postare nel gruppo e nella stanza ai partecipanti contenuti provenienti ad esempio da fonti web che vengano monitorate tramite hashtag particolati. Un buon esempio di applicazione software da cui partire per capire come funziona un bot è <a href="https://github.com/gstjohn/GifBot" target="_blank">questo</a>.
</p>

<p style="text-align: justify;">
  Ne esistono sicuramente molte altre. Il concetto di base è che
</p>

> <p style="text-align: justify;">
>   se appurate che la applicazione vi consente di sviluppare un robot software sappiate che solitamente quel robot potrà usare la applicazione come la usate voi ma automatizzandone i comandi
> </p>

<p style="text-align: justify;">
  il che consente risparmio di risorse (come il tempo), facilità e rapidità nella comunicazione.  Ultima nota: ricordatevi che <strong>le applicazioni che consentono di creare robot devono permettere di svilupparlo non solo tecnicamente</strong> fornendovi l&#8217;interfaccia software (API) per poter usare il robot che volete sviluppare ma non devono vietare i BOT nei loro termini di utilizzo, cosa significa questo? Tecnicamente creare un robot con <a href="https://www.whatsapp.com/?l=it" target="_blank">WhastApp</a> sarebbe possibile se non che la stessa WhatsApp non vi autorizza a farlo nei suoi termini di servizio. Occhio quindi, consultare sempre i termini di uso prima di lavorare con una applicazione!
</p>

<p style="text-align: center;">
  <strong>Buon anno e buoni BOT (gli unici che sicuramente non sono pericolosi)!</strong>
</p>