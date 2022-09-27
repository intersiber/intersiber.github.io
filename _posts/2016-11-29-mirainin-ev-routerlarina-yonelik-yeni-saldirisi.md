---
id: 757
title: 'Mirai&#8217;nin Ev Routerlarına Yönelik Yeni Saldırısı'
date: '2016-11-29T14:54:13+03:00'
author: 'Hakan Torun'
layout: post
guid: 'http://www.intersiber.com/?p=757'
permalink: /mirainin-ev-routerlarina-yonelik-yeni-saldirisi/
post_views_count:
    - '553'
image: /wp-content/uploads/2016/11/14-1280.jpg
categories:
    - Güvenlik
    - Linux
    - 'Öne Çıkan'
tags:
    - adsl
    - almanya
    - botnet
    - deutschland
    - dsl
    - linux
    - mirai
    - router
---

Dün Almanya’daki çok sayıda DSL kullanıcısı routerları ile ilgili sorun yaşadıklarını ve internet bağlantı hızlarının çok yavaş olduğunu rapor etmeye başladı. Sorun yaşayan DSL kullanıcılarının bir hayli fazla olması ve teknik incelemeler sonucunda bazı bulgular elde edilebildi.

DSL kullanıcılarının router arayüzlerine uzaktan bağlantı sağlamasına olanak sağlayan uzaktan yönetim protokolünün istismar edildiği belirlendi.

![tr069-request-mirai](http://www.intersiber.com/wp-content/uploads/2016/11/tr069-request-mirai.png)

Bu istek, DSL CPE yapılandırma yöntemlerinin TR-064 spesifikasyonunda açıklanmaktadır.  
Özetle linux tabanlı router üzerindeki açıktan faydalanan zararlı yazılım, wget aracı ile 1 isimli çalıştırılabilir dosyayı http://l.ocalhost\[.\]host adresinden /tmp dizinine indirip çalıştırmak üzere yapılandırılmış. l.ocalhost.host hostunun ip adresi ise gün içerisinde sürekli değişti.

İlgili çalışıtırılabilir dosya, kendisini çalıştırdıktan sonra;  
– Dosya sisteminden kendisini siliyor ve sadece bellek üzerinde çalışmaya devam ediyor  
– iptables ile 7547 portunu kapatıyor  
– TCP 7547 portunu kullanan diğer cihazları tara ve infekte ediyor

Ancak ilgili zararlı yazılım kendisini /tmp dizinine kaydetmekte ve kalıcı dosya sistemine kendisini yazamamakta. Dolayısıyla router yeniden başlatıldığında hayatına devam edememektedir.