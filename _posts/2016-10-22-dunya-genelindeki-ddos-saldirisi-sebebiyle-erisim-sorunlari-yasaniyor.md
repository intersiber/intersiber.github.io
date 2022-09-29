---
id: 715
title: 'Dünya Genelindeki DDOS Saldırısı Sebebiyle Erişim Sorunları Yaşanıyor'
date: '2016-10-22T12:18:57+03:00'
author: 'Hakan Torun'
layout: post
guid: 'http://www.intersiber.com/?p=715'
permalink: /dunya-genelindeki-ddos-saldirisi-sebebiyle-erisim-sorunlari-yasaniyor/
post_views_count:
    - '1437'
image: images/network.jpg
categories:
    - Genel
    - Güvenlik
    - 'Ne Nasıl?'
    - 'Öne Çıkan'
tags:
    - ddos
    - dyndns
    - 'erişim problemi'
    - netflix
    - reddit
    - saldırı
    - sorun
    - spotify
    - twitter
---

21 Ekim’de başlayan DDOS saldırıları sonucunda aralarında Reddit, Twitter, Spotify, Amazon ve Netflix’in de bulunduğu bir çok servise erişim kısmen veya tamamen durdu. Saldırıyla ilgili henüz resmi bir kanaldan açıklama gelmedi. Saldırı hedefi olarak seçilense bizzat uygulama sunucuları değil dns sunucuları oldu. DNS sunucularında ağırlıklı olarak etkilenense DynDns sunucuları oldu. DNS hizmetinde önemli bir yere sahip olan DynDns yaptığı açıklamada özellikle Amerika Birleşik Devletlerinin doğu eyaletlerinin ciddi bir şekilde saldırıdan etkilendiğini, sorunun giderilmesi için çalıştıklarını iletti. DynDns ABD doğu kıyılarının etkilendiğini açıklasa da, dünya’nın bir çok bölgesinden ilgili hizmetlere erişim sağlanamadığı rapor edildi.

![iot-devices](http://www.intersiber.comimages/iot-devices.jpg)

Yapılan DDOS saldırılarında, standart şifreyle kullanıma sunulan IOT cihazların botnet olarak kullanıldığı neredeyse kesinleşti. Yaklaşık bir ay önce 1.5 milyon kameranın hacklendiği ve bu cihazların bir botnet haline getirildiği belirlenmişti. Bu saldırının da bu ve benzeri botnetler aracılığıyla gerçekleştirildiğini söylemek mümkün. IOT cihazların hemen her eve girdiği bir dönemde böyle bir saldırı ile yeni bir güvenlik zafiyeti de gündeme gelmiş oldu. Güvenlik zafiyetinin Twitter, Spotify gibi hizmetlerde veya ilgili hizmetlerin veri merkezlerinden kaynaklanmadığını belirtmekte fayda var.

**Peki saldırı nasıl gerçekleşti?**

Dünya devleri standart tek bir sunucu üzerinden hizmet vermezler. Esasında kullanım oranı belli bir düzeye gelmiş hiçbir hizmet (uygulama, web sitesi, hizmet vs.) tek bir sunucu ile hizmet ver-e-mez. Ya yatay bir genişleme izleyerek sunucu sayısını ve bilgi işlem gücünü arttırır ya da dikey bir genişleme izleyerek bulut çözümlerine yönelirler. Tek veya kısıtlı bir kaynaktan gerçekleşen, ilgili servisi hizmet dışı bırakmaya yönelik bir DOS saldırısı veya dağıtık bir şekilde farklı lokasyon ve geniş kaynak imkanlarıyla gerçekleştirilen DDOS saldırısı ile özellikle farklı lokasyonlarda ve ileri düzeydeki veri merkezlerinde barındırılan servisleri hizmet dışı bırakmak -neredeyse- imkansızdır.

Saldırıyı kimin düzenlediği henüz net değil. Ancak doğrudan uygulama sunucularını hedef alarak hizmet dışı bırakamayacaklarını bilen saldırganlar, doğrudan uygulama sunucuları yerine DNS sunucularını hedef aldılar.

![dns_nasil](http://www.intersiber.comimages/dns_nasil.jpg)

Bu sayede kullanıcılar ilgili DNS sunucusularından DNS çözümlemesini alamadığı için dolaylı yoldan ilgili servise ulaşamadılar. DNS sunucuları aynı anda çok fazla sayıda sorguya cevap verebilecek kapasitede olmasına rağmen yapılan saldırı dünyanın farklı bölgelerinden ve çok fazla sayıda istemciden gerçekleştiği için hizmet dışı kaldı.

**Neler yapılmalı?**

Zafiyetin standart şifreyle kullanıma sunulan IOT cihazlar olduğu neredeyse kesinleşti. Yani evinizdeki kombinin siz farkında olmadan bu saldırıya katılmış olma ihtimali var. Zafiyet son kullanıcı kaynaklı değil IOT cihaz üreticeleri kaynaklı olsa da, mobil uygulamalar gibi içerisinde size farkettirmeden bu tarz saldırı ağlarına katılabilecek zararlı yazılımlar olabileceğini unutmamak gerek.