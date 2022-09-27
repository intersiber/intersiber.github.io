---
id: 835
title: 'HP Dizüstü Bilgisayar Modellerinde Yerleşik Keylogger Bulundu'
date: '2017-05-12T00:34:52+03:00'
author: 'Hakan Torun'
layout: post
guid: 'https://www.intersiber.com/?p=835'
permalink: /hp-dizustu-bilgisayar-modellerinde-yerlesik-keylogger-bulundu/
post_views_count:
    - '918'
image: /wp-content/uploads/2017/05/keyboard-black-notebook-input-163130.jpeg
categories:
    - Genel
    - Güvenlik
    - İnceleme
    - 'Ne Nasıl?'
    - 'Öne Çıkan'
tags:
    - elitebook
    - hp
    - keylogger
    - mictray
    - probook
    - 'ses kartı'
---

HP marka bir bilgisayara sahip misiniz? Cevabınız evetse, sorununuz bilgisayarınızın kronik ısınmasından öte olabilir.

İsviçre merkezli güvenlik şirketi Modzero, HP marka dizüstü bilgisayarlarda yerleşik olarak bulunan bir keylogger keşfetti. Keylogger, özetle bilgisayar giriş arabirimleri üzerinden gelen her türlü giriş (klavye tuşları gibi) bilgisini kaydeden ve bu bilgileri kaydederek, üçüncü şahıslara raporlayan araçların genel ismidir. Yani bilgisayarınızda bir keylogger aracı bulunuyorsa kullanıcı bilgileriniz, parolalarınız, kredi kartı bilgileriniz farkında olmadan üçüncü şahısların eline geçiyor olabilir.

HP bilgisayarlar, Conexant tarafından geliştirilen ses çiplerini kullanıyor. Conexant High Definition isimli ses sürücüsü bilgisayarın ses kartı ile olan iletişimini sağlıyor.

HP, bilgisayar modeline bağlı olarak bazı ortam tuşlarına erişim sağlamak için yine bu sürücüyü kullanıyor.

Araştırmacılar, HP tarafından ortam tuşlarına erişmek için yazılan kodun zayıf bir şekilde uygulandığını, özel tuşların yanı sıra tüm klavye tuşlarının kayıt altına alındığını ve okunabilir bir dosyada sakladığını ortaya çıkardı.

C:\\Users\\Public\\MicTray.log konumundaki günlük dosyasının, kullanıcının tüm tuş hareketlerini kaydettiği ve dolayısıyla çok sayıda hassas bilgiyi içerdiği ortaya çıktı.

Kullanıcının bilgisayarına fiziksel erişimi bulunan veya ilgili dizine erişebilecek bir zararlı yazılımla kullanıcının hesap bilgileri, parolaları gibi hassas bilgilerini barındıran bu günlük dosyası büyük tehlike arz ediyor.

Araştırma raporuna göre, HP Elitebook 800 serisi, Hp ProBook 600 ve 400 serileri ve bazı PClerin bu açıktan etkilenmiş durumda.

Araştırmacılar, Conexant donanım ve sürücülerini kullanan diğer markaların da aynı açıktan etkilenmiş olabileceğini belirtti.

**Ne yapılmalı?**

- C:\\Windows\\System32\\MicTray.exe
- C:\\Windows\\System32\\MicTray64.exe

Bilgisayarınızda bu iki çalıştırılabilir dosya bulunuyorsa, ilgili keylogger bilgisayarınızda barınıyor demektir. Ses sürücüsüne bağlı olarak, klavye girişlerinin engellenmesi için bulunan çalıştırılabilir dosyanın silinmesi gerekiyor. Ancak bu durumda ses tuşlarınızın gerektiği gibi çalışmayabileceğini hatırlatalım.

Bilgisayarınızdan dosyanın silinmesi durumunda dahi, yedekleme süresine bağlı olarak geçmişe yönelik klavye giriş loglarının elde edilebileceğini unutmamakta fayda var.