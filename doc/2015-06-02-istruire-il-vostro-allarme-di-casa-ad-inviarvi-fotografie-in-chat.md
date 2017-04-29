---
id: 1951
title: Istruire il vostro allarme di casa ad inviarvi fotografie in chat
date: 2015-06-02T20:10:01+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=1951
permalink: /istruire-il-vostro-allarme-di-casa-ad-inviarvi-fotografie-in-chat/
dsq_thread_id:
  - 3815576601
categories:
  - Blog
  - Internet Nelle Cose
  - Laboratorio
tags:
  - chat
  - internet of everething
  - iot
  - raspberry
  - telegram
---
<p style="text-align: justify;">
  Dato il successo avuto dall&#8217;ultimo <a title="Chattare con il proprio frigorifero: Telegram & Raspberry" href="http://pratosmart.teo-soft.com/chattare-con-il-proprio-frigorifero-telegram-raspberry/" target="_blank">post</a> sui messaggi inviati dal frigorifero, oggi mi è venuta in mente un&#8217;altra applicazione che possiamo testare sulla piattaforma <a href="https://www.raspberrypi.org/" target="_blank">Raspberry</a> e <a href="https://telegram.org/" target="_blank">Telegram</a>. Immaginiamo di avere un sistema di allarme con una videocamera connessa. Immaginiamo di che il sistema di allarme sia basato (o collegato) ad una scheda Raspberry connessa alla rete internet di casa (<a href="http://www.projects.privateeyepi.com/home/home-alarm-system-project/installation/how-it-works" target="_blank">questo</a> è un esempio, ma ne esistono molti altri in rete).
</p>

&nbsp;

[<img class=" wp-image-1957  aligncenter" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/06/IMG_1298-e1433268499440.jpg" alt="" width="385" height="514" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/06/IMG_1298-e1433268499440-225x300.jpg 225w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/06/IMG_1298-e1433268499440-768x1024.jpg 768w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/06/IMG_1298-e1433268499440.jpg 960w" sizes="(max-width: 385px) 100vw, 385px" />](http://pratosmart.teo-soft.com/wp-content/uploads/2015/06/IMG_1298-e1433268499440.jpg)

Vediamo come possiamo fare per richiedere via chat su Telegram un&#8217;istantanea della porta di casa in un certo momento anche in nostra assenza.

  1. Configurate Raspberry per il primo uso come scritto <a title="Come si fa il primo setup di un Raspberry B+" href="http://pratosmart.teo-soft.com/come-si-fa-il-primo-setup-di-un-raspberry-b/" target="_blank">qui</a>
  2. Installate Telegram su Raspberry come scritto <a title="Chattare con il proprio frigorifero: Telegram & Raspberry" href="http://pratosmart.teo-soft.com/chattare-con-il-proprio-frigorifero-telegram-raspberry/" target="_blank">qui</a>
  3. Installate una webcam sul vostro Raspberry come scritto <a href="https://www.raspberrypi.org/documentation/usage/webcams/" target="_blank">qui</a> (io ho usato una normalissima webcam USB Logitech, ma Raspberry avrebbe la sua cam nativa)
  4. Create una cartella per memorizzare le foto scattate ed uno script per automatizzare gli scatti e memorizzarli  con questi comandi SSH:

<pre class=" language-bash"><code class=" language-bash">mkdir webcam</code></pre>

<pre>sudo nano /home/pi/camera/camera.sh</pre>

<pre class=" language-bash"><code class=" language-bash">&lt;span class="token important">#!/bin/bash&lt;/span> 
fswebcam &lt;span class="token operator">-&lt;/span>r &lt;span class="token operator">--&lt;/span>no&lt;span class="token operator">-&lt;/span>banner &lt;span class="token operator">/&lt;/span>home&lt;span class="token operator">/&lt;/span>pi&lt;span class="token operator">/&lt;/span>webcam&lt;span class="token operator">/photo&lt;/span>&lt;span class="token punctuation">.&lt;/span>jpg </code></pre>

<img class="  wp-image-1955 aligncenter" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/06/Schermata-2015-06-02-alle-18.55.54.png" alt="Schermata 2015-06-02 alle 18.55.54" width="541" height="181" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/06/Schermata-2015-06-02-alle-18.55.54-300x100.png 300w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/06/Schermata-2015-06-02-alle-18.55.54-1024x342.png 1024w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/06/Schermata-2015-06-02-alle-18.55.54-150x50.png 150w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/06/Schermata-2015-06-02-alle-18.55.54.png 1430w" sizes="(max-width: 541px) 100vw, 541px" />

Salvate lo script camera.sh e rendetelo accessibile con:

<pre>sudo chmod -R 0655 /home/pi/webcam/camera.sh</pre>

A questo punto dovete istruire i vostro allarme a rispondere ad una precisa richiesta in chat. Ipotizziamo che vogliate ricevere una foto dell&#8217;interno di casa alla parola &#8220;scatto&#8221;. Create uno script con questi comandi.

<pre>sudo nano /home/pi/tg/action.lua</pre>

<pre>function on_msg_receive (msg)
      if msg.out then
          return
      end
      if (msg.text=='ping') then
         send_msg (msg.from.print_name, 'pong', ok_cb, false)
      end
     if (msg.text=='scatto') then
     os.execute('/home/pi/webcam/camera.sh')
     send_photo (msg.from.print_name, '/home/pi/camera/photo.jpg', ok_cb, false)
  end
end   
function on_our_id (id) 
end   

function on_secret_chat_created (peer) 
end   

function on_user_update (user) 
end   

function on_chat_update (user) 
end   

function on_get_difference_end () 
end   

function on_binlog_replay_end () 
end</pre>

[<img class="alignleft  wp-image-1954" src="http://pratosmart.teo-soft.com/wp-content/uploads/2015/06/Schermata-2015-06-02-alle-18.46.23.png" alt="Schermata 2015-06-02 alle 18.46.23" width="399" height="430" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2015/06/Schermata-2015-06-02-alle-18.46.23-278x300.png 278w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/06/Schermata-2015-06-02-alle-18.46.23-949x1024.png 949w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/06/Schermata-2015-06-02-alle-18.46.23-139x150.png 139w, http://pratosmart.teo-soft.com/wp-content/uploads/2015/06/Schermata-2015-06-02-alle-18.46.23.png 1386w" sizes="(max-width: 399px) 100vw, 399px" />](http://pratosmart.teo-soft.com/wp-content/uploads/2015/06/Schermata-2015-06-02-alle-18.46.23.png)Salvate lo script action.lua e mandatelo in esecuzione con questi comandi

<pre>cd /home/pi/tg</pre>

<pre>bin/telegram-cli -k tg-server.pub -W -s action.lua</pre>

Fatto!

Ora potete divertirvi a sentire se il vostro allarme è ONLINE digitando semplicemente PING: lui risponderà PONG!

Se invece volete un istantanea di casa vostra digitate &#8220;scatto&#8221; ed ecco qua!

L&#8217;allarme chatta con voi!