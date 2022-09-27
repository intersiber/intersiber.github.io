---
id: 997
title: 'uTorrent Güvenlik Açığı İle Saldırganlar Bilgisayarınıza Uzaktan Erişebilir'
date: '2018-03-01T12:15:49+03:00'
author: 'Hakan Torun'
layout: post
guid: 'https://intersiber.com/?p=997'
permalink: /utorrent-guvenlik-acigi-ile-saldirganlar-bilgisayariniza-uzaktan-erisebilir/
post_views_count:
    - '907'
image: /wp-content/uploads/2018/03/uTorrent.jpg
categories:
    - Genel
    - Güvenlik
    - 'Öne Çıkan'
tags:
    - açık
    - utorrent
    - μTorrent
---

Dünyanın en popüler torrent istemcilerinden μTorrent üzerinde ciddi bir güvenlik açığı keşfedildi.

Google Project Zero ekibi, μTorrent Windows masaüstü ve yeni kullanıma sunulan μTorrent Web üzerinde bir uzaktan kod çalıştırma(RCE) açığı keşfetti. μTorrent ve μTorrent Web uygulamaları Windows işletim sistemini kullanan bilgisayarlarda arka planda çalışıyor ve 10000-19575 portlarını kullanıyor. μTorrent yerel olarak bir HTTP RPC sunucusunu başlatarak kullanıcıların web arayüzü üzerinden istemciye ulaşmasını ve torrentlerini yönetmelerine olanak sağlıyor. Project Zero ekibinden Tavis Ormandy, RPC sunucuları üzerinde yapılabilecek bir saldırıyla, saldırganların torrent istemcisinin kontrolünün ele geçirilebileceğini keşfetti.

Ormandy’ye göre, μTorrent uygulamaları kullanıcılarının bilgisayarında, kötü amaçlı kod çalıştırmak için kullanıcının ziyaret ettiği kötü niyetli bir web sitesi vasıtasıyla istismara açık durumda.

![](https://intersiber.com/wp-content/uploads/2018/03/utorrent-web-ui.png)

Keşfedilen açık sayesinde, saldırganlar klasik μTorrent ve μTorrent Web istemcilerini kullanan kullanıcıların bilgisayarlarında uzaktan zararlı kod çalıştırabiliyor. Geçtiğimiz günlerde Ormandy, Transmission Bittorrent istemcisi üzerinde de benzer bir güvenlik açığını duyurmuştu.

**Ne yapılmalı?**

μTorrent istemcilerini kullanıyorsanız, hemen güncelleme yapmalısınız. μTorrent açığın kapatıldığı yeni bir sürüm yayınlamış durumda. μTorrent Stable 3.5.3.44358, μTorrent Beta 3.5.3.44352 ve μTorrent Web 0.12.0.502 sürümler şu an için en güncel sürümler.