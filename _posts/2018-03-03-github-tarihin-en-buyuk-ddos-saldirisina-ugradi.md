---
id: 1012
title: 'Github Tarihin En Büyük DDOS Saldırısına Uğradı'
date: '2018-03-03T13:02:35+03:00'
author: 'Hakan Torun'
layout: post
guid: 'https://intersiber.com/?p=1012'
permalink: /github-tarihin-en-buyuk-ddos-saldirisina-ugradi/
ampforwp_custom_content_editor:
    - ''
ampforwp_custom_content_editor_checkbox:
    - null
ampforwp-amp-on-off:
    - default
post_views_count:
    - '210'
image: /wp-content/uploads/2018/03/github-ddos-saldiri.jpg
categories:
    - Genel
    - 'Öne Çıkan'
tags:
    - ddos
    - github
---

28 Şubat 2018 günü, GitHub’a DDOS saldırısı gerçekleştirildi. 1.35 Tbps rekor bir seviye ile yapılan saldırı tarihin en büyük DDOS saldırısı olarak kayıtlara geçti.

Saldırganlar, saldırı için herhangi bir botnet ağı kullanmadılar, saldırı için yalnızca yanlış yapılandırılmış Memcached sunucularını kullandılar.

![](https://intersiber.com/wp-content/uploads/2018/03/github-28-subat-ddos-memcrashed-memcached.png)

Popüler açık kaynaklı önbellekleme sistemi Memcached, yanlış yapılandırmaya sahip web sunucularını bir nevi botnet ağı haline getirdi. Geçen seneki [Mirai botnet](https://intersiber.com/mirainin-ev-routerlarina-yonelik-yeni-saldirisi/) saldırılarından sonra bu saldırı bir hayli diikkat çekti. [Github mühendislik blogunda](https://githubengineering.com/ddos-incident-report/) yapılan yayında, binlerce farklı uç noktadan binlerce farklı istek yapıldığını ve 1.35 Tbps zirve noktasıyla saniyede 126.9 milyon paketle saldırının gerçekleştirildiği açıklandı.

Memcached kullanan web sunucuları için sistem yöneticilerinin, doğru yapılandırma kullanmaları, 11211 portunu firewall ile korumaları ve UDP desteğine ihtiyaç duyulmuyorsa tamamen kapatmaları öneriliyor.