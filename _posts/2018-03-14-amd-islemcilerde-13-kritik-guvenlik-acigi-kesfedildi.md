---
id: 1016
title: 'AMD İşlemcilerde 13 Kritik Güvenlik Açığı Keşfedildi'
date: '2018-03-14T13:02:36+03:00'
author: 'Hakan Torun'
layout: post
guid: 'https://intersiber.com/?p=1016'
permalink: /amd-islemcilerde-13-kritik-guvenlik-acigi-kesfedildi/
ampforwp_custom_content_editor:
    - ''
ampforwp_custom_content_editor_checkbox:
    - null
ampforwp-amp-on-off:
    - default
post_views_count:
    - '342'
image: /wp-content/uploads/2018/03/amd-flaws-2.jpg
categories:
    - Analiz
    - Genel
    - 'Öne Çıkan'
tags:
    - açık
    - amd
    - flaws
    - işlemci
    - zafiyet
---

Güvenlik araştırmacıları AMD’nin Ryzen ve EPYC işlemcilerinde [Meltdown ve Spectre](https://intersiber.com/meltdown-ve-spectre-islemci-zafiyetleri/) zafiyetlerine benzer ciddi güvenlik açıkları keşfetti. 13 farklı kritik açık sayesinde kullanıcıların hassas verilerinin ele geçirilmesi, kalıcı şekilde kötücül yazılımların yüklenebilmesi ve sistemler üzerinde tam yetki sağlanabilmesi gibi sonuçlar meydana gelebilir.

Tüm güvenlik açıkları AMD’nin genellikle aygıt, parola ve şifreleme anahtarları gibi hassas verilerin bulunduğu ve bilgisayarların başladığı zaman kötü amaçlı bir şeyler olup olmadığını kontrol eden mimarisinde bulunuyor.

Keşfedilen güvenlik açıkları Ryzenfall, Fallout, Chimera, Masterkey olmak üzere dört kategoriye ayrılmış durumda. Güvenlik açıkları AMD Ryzen, Ryzen Pro, Ryzen Mobile ve EPYC işlemcileri kullanan sunucular, iş istasyonları ve taşınabilir bilgisayarları etkiliyor.

İsrail merkezli güvenlik şirketi CTS-Labs araştırmacıları, henüz yamanmamış açıklar sayesinde AMD’nin Şifrelenmiş Güvenli Sanallaştırma teknolojisini aşmayı başardı. Bu sayede saldırganların Microsoft Windows Kimlik Bilgisi Güvencesini bypass edebileceği ortaya koyuldu.

Araştırmacılar ayrıca, Ryzen çipleri üzerinde üretici tarafından kötü niyetli kodların çalıştırılmasını sağlayabilecek iki arka kapı olduğunu iddia etti.

![](https://intersiber.com/wp-content/uploads/2018/03/amd-flaws.png)

**Ryzenfall**

Bu açık yalnızca AMD’nin Ryzen çiplerini etkiliyor. Bu sayede kötü amaçlı yazılım işlemcinin tamamen ele geçirilmesini sağlıyor. Bu sayede saldırgan şifreleme anahtarları ve kullanıcı parolaları da dahil olmak üzere tüm hassas verilere erişebilir.

Saldırganlar bu açık ile birlikte Windows Kimlik Güvencesini -Hassas verilerin normal şartlarda erişilemeyen, işletim sisteminin korunan bir bölümünde saklanmasını sağlayan özellik- aşabilirse, bir ağ içindeki diğer aygıtlara da saldırmak için kullanabilir.

![](https://intersiber.com/wp-content/uploads/2018/03/amd-ryzenfall.png)

**MasterKey**

Bir bilgisayar başlatıldığı zaman, güvenli önyükleme işleminden geçer. Bilgisayarda bir şeylerin kurcalanmadığını kontrol etmek ve sadece güvenli olarak bilinen yazılımların çalıştırılması için işlemci kullanılır.

EPYC ve RYzen işlemecilerdeki bu açık sayesinde ise, saldırganlar işlemcinin bu doğrulamaları yapmasını engelleyebilir. Dahası işlemciye kötü amaçlı yazılımların yüklenmesi ve başlangıçta hangi yazılımların çalıştırılmasına izin verileceğinin kontrolünün saldırganların eline geçmesini sağlayabilir.

![](https://intersiber.com/wp-content/uploads/2018/03/amd-masterkey.png)

**Fallout**

Araştırmacılar Ryzenfall gibi Fallout’un da saldırganların korumalı bellek alanlarına erişebilmesine olanak sağlayacağını söyledi. Ancak bu açık yalnızca AMD’nin EPYC güvenli işlemcisini kullanan cihazları etkilemekte. Açık sayesinde saldırganlar Windows Kimlik Güvencesi gibi izole bir alanda tutulan veriler olmak üzere bellek üzerinde korumalı alanlara erişebilir.

AMD’nin EPYC çiplerini kullanan işlemciler veri merkezleri ve bulut sunuculardada Dünya çapında kullanılmakta. Saldırganlar bu açık sayesinde ağda depolanan ve yayılan tüm kimlik bilgilerini çalabilirler. Yakın zamanda Microsoft Azure Bulut sunucularında EPYC işlemcilerin kullanılması yönünde AMD ile bir ortaklık yapmıştı.

**Chimera**

Bu güvenlik açığı AMD’nin Prozotory çipleri içinde arka kapı olarak bulunuyor ve Ryzen ve Ryzen Pro iş istasyonlarını etkiliyor. Araştırmacılara göre ağ trafiği, Wifi ve Bluetooth trafiği çipset üzerinden aktığı için, çip üzerinde man-in-the-middle saldırıları gerçekleştilebilir.

Yine çip üzerinden akan USB trafiğini dinleyerek, saldırganların bu sayede her şeyi görmesini sağlayan keyloggerlar üretebileceğini söyledi.

![](https://intersiber.com/wp-content/uploads/2018/03/amd-ryzen.jpg)

Araştırmacılar bu açıkları 21 farklı AMD işlemcisi üzerinde başarılı bir şekilde test etti ve 11 işlemcinin de bu sorunlara karşı savunmasız olduğuna inanıyorlar.

AMD şu anda bu kusurları araştırıyor fakat güvenlik şirketi Trail Of Bits’in kurucusu Dan Guido, AMD’nin belirtilen tüm açıklarının gerçek olduğunu doğruladı.

**Ne Yapılmalı?**

Intel ve işletim sistemi üreticileri [Meltdown ve Spectre](https://intersiber.com/meltdown-ve-spectre-islemci-zafiyetleri/) işlemci zafiyetlerini giderebilmek için hala çalışıyor. Zafiyetleri gidermek performans kayıplarına yol açmıştı. Yeni keşfedilen AMD işlemci açıkları benzer sorunlar yaratacak gibi görünüyor.

Son kullanıcılar olarak güvenlik yamalarının yayınlanmasını beklemekten başka şimdilik yapılabilecek pek bir şey maalesef yok. Yine de normal şartlar altında alınması gereken tüm güvenlik tedbirlerinin alınmasında fayda var.