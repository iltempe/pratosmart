---
id: 1379
title: Stampa 3D per bischeri – Fase 7
date: 2014-10-18T20:04:12+00:00
author: Matteo
layout: post
guid: http://pratosmart.teo-soft.com/?p=1379
permalink: /stampa-3d-per-bischeri-fase-7/
dsq_thread_id:
  - 3131027506
categories:
  - Una Stampante 3D per Prato
tags:
  - pratosmart
  - stampa 3d
  - steel
---
<p style="text-align: justify;">
  Salve carissimi che seguite la mia rubrica di stampa 3D. Stasera vi presento il montaggio preliminare dell&#8217;elettronica della stampante 3d.
</p>

<p style="text-align: justify;">
  Indovinate chi c&#8217;è a controllare tutto il circuito elettronico? Si proprio lui! <a title="Perchè con Arduino cambieremo il mondo" href="http://pratosmart.teo-soft.com/perche-con-arduino-cambieremo-il-mondo/" target="_blank">Arduino</a>!
</p>

<p style="text-align: justify;">
  Per provare la stampante 3D conviene prima cablare tutto il circuito in modo &#8220;prototipale&#8221; prima di passare i fili in modo definitivo. In questo modo se ci fosse qualcosa da sistemare dopo la prima accensione ancora i fili non sono stati fissati in modo definitivo. Nel nostro caso il secondo estrusore non è presente (anche se la stampante è predisposta per averne uno) quindi non consideratelo.
</p>

<p style="text-align: justify;">
  Per capire come va montata vi rimando alle mie foto e a questo schema di principio. <a href="http://reprap.org/wiki/Prusa_i3_Rework_Electronics_and_wiring/it" target="_blank">Qui</a> trovate anche una sezione di Wikipedia interamente dedicata all&#8217;argomento dove c&#8217;è il dettaglio delle connessioni.
</p>

<p style="text-align: justify;">
  Siamo quasi pronti per accendere&#8230;tenetevi forte!
</p>

&nbsp;

[<img class="wp-image-1380 aligncenter" src="http://pratosmart.teo-soft.com/wp-content/uploads/2014/10/1200px-Rampswire14.svg_.png" alt="1200px-Rampswire14.svg" width="601" height="850" srcset="http://pratosmart.teo-soft.com/wp-content/uploads/2014/10/1200px-Rampswire14.svg_-212x300.png 212w, http://pratosmart.teo-soft.com/wp-content/uploads/2014/10/1200px-Rampswire14.svg_-724x1024.png 724w, http://pratosmart.teo-soft.com/wp-content/uploads/2014/10/1200px-Rampswire14.svg_.png 1200w" sizes="(max-width: 601px) 100vw, 601px" />](http://pratosmart.teo-soft.com/wp-content/uploads/2014/10/1200px-Rampswire14.svg_.png)

&nbsp;

<!-- Flickr Photostream by Miro Mannino -->

<div id="flickrGal8" class="justified-gallery" >
  <a href="https://www.flickr.com/photos/125814874@N05/14981541499/in/set-72157647321268121/lightbox" target="_blank" title="KIT PRUSA I3 STEEL 3D PRINTER"><img alt="KIT PRUSA I3 STEEL 3D PRINTER" src="https://farm4.static.flickr.com/3860/14981541499_ebb4e40c55_m.jpg" data-safe-src="https://farm4.static.flickr.com/3860/14981541499_ebb4e40c55_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/14981704897/in/set-72157647321268121/lightbox" target="_blank" title="KIT PRUSA I3 STEEL 3D PRINTER"><img alt="KIT PRUSA I3 STEEL 3D PRINTER" src="https://farm4.static.flickr.com/3855/14981704897_a2e275c68c_m.jpg" data-safe-src="https://farm4.static.flickr.com/3855/14981704897_a2e275c68c_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15145242936/in/set-72157647321268121/lightbox" target="_blank" title="Il kit"><img alt="Il kit" src="https://farm4.static.flickr.com/3920/15145242936_000f8b36ce_m.jpg" data-safe-src="https://farm4.static.flickr.com/3920/15145242936_000f8b36ce_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/14981603310/in/set-72157647321268121/lightbox" target="_blank" title="Kit Plastiche"><img alt="Kit Plastiche" src="https://farm4.static.flickr.com/3857/14981603310_83e43d2a43_m.jpg" data-safe-src="https://farm4.static.flickr.com/3857/14981603310_83e43d2a43_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15165259911/in/set-72157647321268121/lightbox" target="_blank" title="Kit elettronica +  Kit LCD"><img alt="Kit elettronica +  Kit LCD" src="https://farm4.static.flickr.com/3887/15165259911_4c2d7bd9a9_m.jpg" data-safe-src="https://farm4.static.flickr.com/3887/15165259911_4c2d7bd9a9_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15168246085/in/set-72157647321268121/lightbox" target="_blank" title="Strutture Meccaniche"><img alt="Strutture Meccaniche" src="https://farm6.static.flickr.com/5568/15168246085_61c178b32a_m.jpg" data-safe-src="https://farm6.static.flickr.com/5568/15168246085_61c178b32a_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15168236355/in/set-72157647321268121/lightbox" target="_blank" title="Kit Minuteria"><img alt="Kit Minuteria" src="https://farm6.static.flickr.com/5574/15168236355_b1e0beeef9_m.jpg" data-safe-src="https://farm6.static.flickr.com/5574/15168236355_b1e0beeef9_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/14981651958/in/set-72157647321268121/lightbox" target="_blank" title="Kit Barre"><img alt="Kit Barre" src="https://farm6.static.flickr.com/5580/14981651958_cb01ee5304_m.jpg" data-safe-src="https://farm6.static.flickr.com/5580/14981651958_cb01ee5304_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15167837502/in/set-72157647321268121/lightbox" target="_blank" title="Kit di Trasmissione"><img alt="Kit di Trasmissione" src="https://farm6.static.flickr.com/5558/15167837502_4ea609c899_m.jpg" data-safe-src="https://farm6.static.flickr.com/5558/15167837502_4ea609c899_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15145183756/in/set-72157647321268121/lightbox" target="_blank" title="5 Motori"><img alt="5 Motori" src="https://farm6.static.flickr.com/5556/15145183756_a7fb9c479e_m.jpg" data-safe-src="https://farm6.static.flickr.com/5556/15145183756_a7fb9c479e_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/14981625298/in/set-72157647321268121/lightbox" target="_blank" title="Alimentatore"><img alt="Alimentatore" src="https://farm6.static.flickr.com/5571/14981625298_4cff08dc21_m.jpg" data-safe-src="https://farm6.static.flickr.com/5571/14981625298_4cff08dc21_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15167807302/in/set-72157647321268121/lightbox" target="_blank" title="Kit HEATBED MK2"><img alt="Kit HEATBED MK2" src="https://farm6.static.flickr.com/5596/15167807302_e1fd485ba3_m.jpg" data-safe-src="https://farm6.static.flickr.com/5596/15167807302_e1fd485ba3_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15167798042/in/set-72157647321268121/lightbox" target="_blank" title="Filamento PLA"><img alt="Filamento PLA" src="https://farm4.static.flickr.com/3900/15167798042_d3a0b93538_m.jpg" data-safe-src="https://farm4.static.flickr.com/3900/15167798042_d3a0b93538_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15168172615/in/set-72157647321268121/lightbox" target="_blank" title="Lacca"><img alt="Lacca" src="https://farm4.static.flickr.com/3855/15168172615_ec379d103c_m.jpg" data-safe-src="https://farm4.static.flickr.com/3855/15168172615_ec379d103c_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15168164985/in/set-72157647321268121/lightbox" target="_blank" title="Cavi di Alimentazione"><img alt="Cavi di Alimentazione" src="https://farm4.static.flickr.com/3854/15168164985_f6502d4dbe_m.jpg" data-safe-src="https://farm4.static.flickr.com/3854/15168164985_f6502d4dbe_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15145131146/in/set-72157647321268121/lightbox" target="_blank" title="Kit per Estrusore"><img alt="Kit per Estrusore" src="https://farm4.static.flickr.com/3893/15145131146_2a67c62829_m.jpg" data-safe-src="https://farm4.static.flickr.com/3893/15145131146_2a67c62829_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/14981576118/in/set-72157647321268121/lightbox" target="_blank" title="Relè"><img alt="Relè" src="https://farm4.static.flickr.com/3919/14981576118_be321d0485_m.jpg" data-safe-src="https://farm4.static.flickr.com/3919/14981576118_be321d0485_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15353736615/in/set-72157647321268121/lightbox" target="_blank" title="IMG_2253"><img alt="IMG_2253" src="https://farm4.static.flickr.com/3877/15353736615_c3f04a5ff7_m.jpg" data-safe-src="https://farm4.static.flickr.com/3877/15353736615_c3f04a5ff7_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15167013189/in/set-72157647321268121/lightbox" target="_blank" title="IMG_2321"><img alt="IMG_2321" src="https://farm4.static.flickr.com/3885/15167013189_9f2a8b683a_m.jpg" data-safe-src="https://farm4.static.flickr.com/3885/15167013189_9f2a8b683a_m.jpg" /></a><a href="https://www.flickr.com/photos/125814874@N05/15167012569/in/set-72157647321268121/lightbox" target="_blank" title="IMG_2319"><img alt="IMG_2319" src="https://farm4.static.flickr.com/3895/15167012569_46bfb8e8d1_m.jpg" data-safe-src="https://farm4.static.flickr.com/3895/15167012569_46bfb8e8d1_m.jpg" /></a>
</div>

&nbsp;