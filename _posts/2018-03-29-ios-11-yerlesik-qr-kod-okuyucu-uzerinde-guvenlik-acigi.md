---
id: 1048
title: 'iOS 11 Yerleşik QR Kod Okuyucu Üzerinde Güvenlik Açığı'
date: '2018-03-29T01:21:51+03:00'
author: 'Hakan Torun'
layout: post
guid: 'https://intersiber.com/?p=1048'
permalink: /ios-11-yerlesik-qr-kod-okuyucu-uzerinde-guvenlik-acigi/
ampforwp_custom_content_editor:
    - ''
ampforwp_custom_content_editor_checkbox:
    - null
ampforwp-amp-on-off:
    - default
post_views_count:
    - '287'
image: images/iphone-ios-11-qr.jpg
categories:
    - Apple
    - 'Öne Çıkan'
tags:
    - 'ios 11'
    - 'ios 11 güvenlik açığı'
    - 'kamera açık'
    - 'kamera qr kod'
    - 'qr kod okuyucu açığı'
---

Apple iOS 11 işletim sistemi üzerinde yeni bir güvenlik açığı keşfedildi. iOS 11 yerleşik kamera uygulaması üzerinde bulunan QR kod okuyucu üzerinde keşfedilen açık sayesinde, kullanıcıların bilgisi olmadan zararlı bağlantılara yönlendirilmesi mümkün hale geliyor.

Açık iOS 11 işletim sistemine sahip, iPhone, iPad ve iPod Touch cihazları etkiliyor ve yerleşik QR kod okuyucu sayesinde kullanıcıları saldırılara karşı savunmasız hale getiriyor.

Apple iOS 11 ile birlikte, yerleşik kamera uygulaması üzerinden QR kodların okunmasını mümkün kılmıştı. Bu sayede kullanıcıların, herhangi bir üçüncü parti uygulamaya ihtiyaç duymadan QR kodları okuması mümkün hale gelmişti.

iOS 11’e sahip Apple cihazları kamera uygulaması ile kadraja giren alanda herhangi bir URL’e sahip QR kod tespit ettiği anda, web tarayıcı üzerinden ilgili url’e bağlanmak için izin istiyor. Fakat güvenlik araştırmacısı Roman Mueller tarafından [keşfedilen güvenlik açığı](https://infosec.rm-it.de/2018/03/24/ios-camera-qr-code-url-parser-bug/) gösterdi ki, iOS 11 yerleşik QR kod okuyucusu, QR kodlar üzerindeki url’i tespit etme konusunda pek başarılı değil.

Mueller’e göre iOS 11’in yerleşik QR kod okuyucusu bağlantıları ayıklamada çok başarısız. Öyle ki, saldırganlar tarafından QR kod vasıtasıyla bağlantılar çok rahat bir şekilde manipüle edilebiliyor.

![](images/ios11-built-in-qr-code-camera-fail.jpg)

Bu QR kod’un içerdiği bilgi

*https://xxx\\@facebook.com:443@infosec.rm-it.de/*

![](images/ios-11-camera-qr-kod-acik.jpg)

iOS 11′ sahip bir cihazın kamera uygulaması ile görüntülediğiniz zaman algıladığı QR kod sonucunda web tarayıcı ile facebook.com’a bağlanmak istiyor. Kullanıcıdan onay aldığında ise bağlandığı adres infosec.rm-it.de oluyor, bingo!

Roman Mueller’in belirttiğine göre açık Apple’a 23.12.2017 tarihinde rapor edilmiş fakat 24.03.2018 tarihinde Mueller tarafından yayınlanan blog gönderisi itibariyle açık hala varlığını koruyor.

QR kodlar her ne kadar gündelik hayatta kolaylıklar sağlasa da, kullanıcıların dikkatli olmasında fayda var. Kullanıcıların QR kod vasıtasıyla bağlandığı adreslerde, url’e özellikle dikkat etmelerini öneriyoruz.

*Görseller ve kaynak: https://infosec.rm-it.de/2018/03/24/ios-camera-qr-code-url-parser-bug/*