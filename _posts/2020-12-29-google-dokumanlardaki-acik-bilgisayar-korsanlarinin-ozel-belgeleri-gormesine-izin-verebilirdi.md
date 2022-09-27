---
id: 10204
title: 'Google Dökümanlar’daki Açık, Bilgisayar Korsanlarının Özel Belgeleri Görmesine İzin Verebilirdi'
date: '2020-12-29T18:47:33+03:00'
author: 'Ahmet Can Bilici'
layout: post
guid: 'https://intersiber.com/?p=10204'
permalink: /google-dokumanlardaki-acik-bilgisayar-korsanlarinin-ozel-belgeleri-gormesine-izin-verebilirdi/
post_views_count:
    - '20'
image: /wp-content/uploads/2020/12/google-dokumanlar-acigi-bilgisayar-korsanlarinin-ozel-bilgileri-gormesine-izin-verebilirdi.jpg
categories:
    - Güvenlik
tags:
    - google
    - 'google dökümanlar'
---

Google, bir siber korsan tarafından, hassas Google Dökümanlar belgelerinin ekran görüntülerini çalmak için kullanılabilecek, geri bildirim aracındaki bir hatayı düzeltti.

Google Dökümanlar açığı, birkaç ay önce güvenlik araştırmacısı Sheeram KL tarafından keşfedildi ve Google’ın Güvenlik Açığı Ödül Programı kapsamında, 3133,7 dolar verildi.

## Açık ‘geri bildirim gönderme aracı’ üzerinden geldi

Google Dökümanlar dahil olmak üzere birçok Google hizmeti, kullanıcıların geri bildirim göndermesine ve belli problemleri çözmesine izin vermek adına bir ekran görüntüsü eklemeyi sağlayan “Geri Bildirim Gönder” ve “Dökümanların iyileştirilmesine yardımcı ol” seçeneğine sahipti.

Ancak, feedback.googleusercontent.com adresinden gelen bir pop up içeriğinin, farklı domainlere bir iframe ile eklenmesi ile bu özelliğin bir açığı söz konusu oldu.

<figure class="wp-block-image size-large">![](https://intersiber.com/wp-content/uploads/2020/12/google-dokumanlar-geri-bildirim-guvenlik-acigi.jpg)</figure>Bu durum, Google Dökümanlar penceresinin bir ekran görüntüsü eklendiğinde, görüntünün işlenmesinin her pikselin RGB değerlerinin ana alan adına (google.com) iletilmesi gerektiği ve sonrasında yeniden yönlendirdiği anlamına geliyor. Sonuç olarak bu RGB değerleri görüntüyü oluşturuyor ve Base64 kodlanmış bir şekilde geri döndürüyor.

Sheeram, bu mesajların feedback.googleusercontent.com’a aktarılma biçiminde bir hata tespit etti. Güvenlik açığı, Google Dökümanlar alanındaki X-Frame-Options içeriğinin eksikliğinden kaynaklanıyor ve bu da mesajın hedef kaynağını değiştirmeyi ve sayfa ile içerdiği kaynak iletişiminden yararlanmayı olası kılıyor.

<figure class="wp-block-embed-youtube wp-block-embed is-type-video is-provider-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio"><div class="wp-block-embed__wrapper"><span class="embed-youtube" style="text-align:center; display: block;"><iframe allowfullscreen="true" class="youtube-player" height="360" src="https://www.youtube.com/embed/isM-BXj4_80?version=3&rel=1&fs=1&autohide=2&showsearch=0&showinfo=1&iv_load_policy=1&wmode=transparent" style="border:0;" width="640"></iframe></span></div></figure>Açık, “geri bildirim gönder” gibi bir butona tıklama olarak, kullanıcı etkileşimi gerektirse de, yüklenen ekran görüntüsünün URL’ini yakalamak ve kötü amaçlı olarak kullanmak mümkündü.