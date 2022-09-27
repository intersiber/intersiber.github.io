---
id: 806
title: '28.000 MongoDB Veritabanı Sunucusu Hacklendi'
date: '2017-01-12T00:12:23+03:00'
author: 'Hakan Torun'
layout: post
guid: 'http://www.intersiber.com/?p=806'
permalink: /28000-mongodb-veritabani-sunucusu-hacklendi/
post_views_count:
    - '938'
image: /wp-content/uploads/2017/01/mongodb-ransomware.png
categories:
    - İnceleme
    - 'Ne Nasıl?'
    - 'Öne Çıkan'
    - 'Veri Sızıntıları'
tags:
    - db
    - fidye
    - hack
    - hacklendi
    - mongo
    - mongodb
    - ransomware
    - virüsü
    - zaafiyet
---

![](http://www.intersiber.com/wp-content/uploads/2017/01/mongodb-logo.png)

Ransomware korsanlarının en son kurbanı MongoDB kullanıcıları oldu. Kısaca hedef sistemin verilerinin şifrelenmesi veya uzak bir sunucuya yedeğinin alınarak hedef sistemden silinmesinin ardından, fidye karşılığında verilerin geri iade edileceğini iddia eden zararlı yazılım ve saldırı türlerine ransomware deniliyor.

Veri tabanı yönetim sistemleri arasında, NoSQL kavramının en büyük oyuncularından MongoDB kullanıcılarının TB mertebesindeki verileri hedef alındı ve 28.000 MongoDB veritabanı bu saldırıdan etkilendi. Korsanlar, verileri kendi erişimlerine açık uzak sunuculara aktardı ve hedef sistemlerde bir veritabanı kaydı vasıtasıyla notlar bırakarak bitcoin olarak ödeme yapılmasını, ardından kullanıcının kendi sunucu ip adresini bildirmesini istiyor.

![](http://www.intersiber.com/wp-content/uploads/2017/01/mongodb-ransomware.jpg)

Yirmiye yakın şirketin bitcoin ile fidyecilere ödeme yaptığı belirtiliyor ancak ödeme yapılması durumunda bile verilerin kurtarılamadığı senaryolar mevcut.

**Nasıl gerçekleşti?**

MongoDB 2.6 sürümüyle birlikte, varsayılan yapılandırma dosyasında 127.0.0.1 ip adresine cevap verecek şekilde konfigüre edilmişti. Ancak 2.6 sürümünden önceki sürümlerde varsayılan yapılandırma yerel bağlantıların haricinde uzaktan erişime de izin veriyor. 2.6 sürümünden önceki sürümlerde yine varsayılan yapılandırma olarak kimlik doğrulama da gerekli değil ve varsayılan yapılandırma yetkilendirilmemiş kullanıcıların erişimine olanak sağlıyor.

2.6 öncesi kurulumlarda varsayılan port olarak 27017 kullanılıyor ve basit araçlarla port taraması yapılarak dahi, savunmasız olma ihtimali olan mongodb sunucuları listelenebiliyor. Ne yazık ki bu zafiyet yeni keşfedilmedi. 2015 yılında 30.000 savunmasız MongoDB kurulumunun tespit edildiği rapor edilmişti.

**Ne yapılmalı?**

Henüz bu zafiyetin kurbanı olmamış MongoDB kurulumlarının güncellenmesi ve yapılandırma dosyalarının gözden geçirilmesi gerekiyor. Nitekim, bu zafiyet MongoDB’nin yapısal veya yazılımsal bir zafiyetinden çok bir yapılandırma zafiyeti olarak kabul görüyor.