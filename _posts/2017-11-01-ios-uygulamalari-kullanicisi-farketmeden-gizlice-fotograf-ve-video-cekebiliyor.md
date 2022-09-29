---
id: 898
title: 'iOS Uygulamaları Kullanıcısı Farketmeden Gizlice Fotoğraf ve Video Çekebiliyor'
date: '2017-11-01T14:38:57+03:00'
author: 'Hakan Torun'
layout: post
guid: 'https://www.intersiber.com/?p=898'
permalink: /ios-uygulamalari-kullanicisi-farketmeden-gizlice-fotograf-ve-video-cekebiliyor/
post_views_count:
    - '624'
image: images/iphone-camera.jpg
categories:
    - Apple
    - 'Ne Nasıl?'
    - 'Öne Çıkan'
tags:
    - 'gizli fotoğraf'
    - ios
    - 'ios camera permission'
    - 'ios kamera gizliliği'
    - 'ios kamera izin'
    - iphone
    - 'kullanıcı mahremiyeti'
    - 'veri ihlali'
    - video
---

iOS uygulamaları, kullanıcısını bilgilendirmeksizin, ön ve arka kemeralar vasıtasıyla gizlice fotoğraf ve video çekebiliyor. Google mühendislerinden Felix Krause geliştirdiği bir demo uygulama ile birlikte konunun detaylarını blogunda paylaştı.

iOS uygulamalarında, uygulamanın kamera erişim iznini kullanıcıdan almadan kameraya erişip fotoğraf ve video çekebilmesi mümkün değil. Facebook, Twitter, Instagram gibi popüler uygulamalar dahil tüm iOS uygulamaları kamera erişimi için aldığı kullanıcı izni ile kamera erişimini sağlıyor.

Ancak kamera erişim iznini kullanıcıdan almış herhangi bir uygulama, kullanıcıyı bilgilendirmeksizin istediği zaman fotoğraf çekebilir ve video kaydedebilir hale geliyor. Tabi ki yapılabilecekler sadece bunlarla sınırlı değil. Kamera erişim iznine sahip herhangi bir uygulama;

- Ön ve arka kamera vasıtasıyla dilediği zaman fotoğraf ve video kaydedebilir, gerçek zamanlı video yayını yapabilir
- Fotoğraf ve videoları uzak bir sunucuya aktarabilir
- Yüz tanıma ve gerçek zamanlı duygu analizi yapabilir

Apple’ın bu konuda yapabileceği pek bir şey yok. Zira erişim izin altyapısı Apple tarafından tasarlanmış haliyle kullanışlı durumda. Fakat bu durum, art niyetli geliştiricilerin elinde bir tehdit haline geliyor. Felix Krause tarafından paylaşılan, bu durumun nasıl istismar edileceğini gösteren demo uygulamaya [github](https://github.com/KrauseFx/watch.user) üzerinden erişebilirsiniz. Yine araştırmacı tarafından yayınlanan video ile; esasında bir sosyal medya uygulaması gibi görünen uygulamanın saniyede bir görüntü almasını gösteriyor.

<div class="jetpack-video-wrapper"><span class="embed-youtube" style="text-align:center; display: block;"><iframe allowfullscreen="true" class="youtube-player" height="360" src="https://www.youtube.com/embed/GqWUaflPMh0?version=3&rel=1&fs=1&autohide=2&showsearch=0&showinfo=1&iv_load_policy=1&wmode=transparent" style="border:0;" width="640"></iframe></span></div>**Nasıl korunabilirsiniz?**

Bu tarz bir durumla karşı karşıya kalmamak için yapabilecekleriniz sınırlı sayıda olsa da var. Güvendiğiniz uygulamaları resmi uygulama marketleri haricinde kurmamalı, güvenmediğiniz uygulamalardan -özellikle kamera erişimine ihtiyaç duymamasına rağmen kamera erişimi isteyen uygulamalardan- olabildiğince uzak durmalı ve bu uygulamalarara gerekmediği durumlarda kamera erişim izni vermemelisiniz.

Yine de bu tam bir koruma sağlamayacaktır. Güvendiğiniz uygulamaların dahi, sizin izniniz olmadan fotoğraf ve/veya video kaydı yapmadığının garantisini maalesef kimse veremeyecektir.

Kesin bir çözüm olarak Mark Zuckerberg ve James Comey gibi kameralarınızın üzerini şeffaf olmayan bir bantla kapatabilirsiniz.