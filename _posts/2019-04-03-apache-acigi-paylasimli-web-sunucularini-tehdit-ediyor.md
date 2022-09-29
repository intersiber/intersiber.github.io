---
id: 1171
title: 'Apache Açığı Paylaşımlı Web Sunucularını Tehdit Ediyor'
date: '2019-04-03T14:17:37+03:00'
author: 'Hakan Torun'
layout: post
guid: 'https://intersiber.com/?p=1171'
permalink: /apache-acigi-paylasimli-web-sunucularini-tehdit-ediyor/
ampforwp_custom_content_editor:
    - ''
ampforwp_custom_content_editor_checkbox:
    - null
ampforwp-amp-on-off:
    - default
post_views_count:
    - '255'
image: images/apache-http-web-server-sunucu.png
categories:
    - Güvenlik
    - 'Öne Çıkan'
tags:
    - apache
    - 'apache açığı'
    - CVE-2019-0211
    - httpd
    - 'web server'
    - 'web sunucusu'
---

Açık kaynak kodlu ve internet’in bel kemiği diyebileceğimiz oranda çok kullanılan, Dünya’nın en popüler web sunucularından biri olan Apache üzerinde yeni bir açık keşfedildi.

Apache vakfı ve OpenSSL projesinin kurucu üyelerinden Mark J Cox, Apache üzerinde yeni keşfedilen önemli bir açık hakkında, twitter üzerinden kullanıcıları uyardı.

CVE-2019-0211 kodlu güvenlik açığı, Ambionics Security firmasında güvenlik mühendisi olarak çalışan Charles Fol tarafından keşfedildi. Açık, Apache HTTP sunucusu 2.4.17 ile 2.4.38 sürüm kodları arasında kalan sürümleri etkiliyor. Açık sayesinde hedef sunucu üzerinde düşük yetkili kullanıcılar, root yetkisiyle kod çalıştırabiliyor.

Apache tarafından yayınlanan yeni sürüm ile, 2.4.39 sürümünde bu hata yamalandı.

Keşfedilen bu açıkla ilgili henüz bir PoC yayınlanmadı ancak araştırmacılar bu hatanın nasıl istismar edilebileceği ile ilgili bir blog yazısı [yayınladı](https://cfreal.github.io/carpe-diem-cve-2019-0211-apache-local-root.html).

Bu açık sebebiyle paylaşımlı web sunucuları büyük risk altında. Mark J Cox, kötü niyetli müşterilerin veya bir web sitesinde PHP veya CGI betiklerini çalıştırma yeteneğine sahip bir saldırganın, web sunucusu üzerinde root erişimi sağlamak için bu kusurdan faydalanabileceğini ve paylaşımlı web sunucularındaki diğer hesap sahiplerinin hizmetleri üzerinde yetki sağlayabileceğini belirtti.

Apache Web sunucusu üzerindeki bu açık sebebiyle, web barındırma hizmetleri veren şirketler, kendi sunucuları üzerinde web hizmeti veren kuruluşlar ve web sitesi yöneticilerinin Apache’nin yayınladığı son güncellemeyle sürüm yükseltmeleri önemle tavsiye edilir.