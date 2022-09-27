---
id: 887
title: 'WPA2 Wi-Fi Ağları Üzerinde Krack Zafiyeti'
date: '2017-10-25T22:26:07+03:00'
author: 'Hakan Torun'
layout: post
guid: 'https://www.intersiber.com/?p=887'
permalink: /wpa2-wifi-aglari-uzerinde-krack-zafiyeti/
post_views_count:
    - '722'
image: /wp-content/uploads/2017/10/wifi-network.jpg
categories:
    - Genel
    - Güvenlik
    - 'Ne Nasıl?'
    - 'Öne Çıkan'
tags:
    - ağları
    - atağı
    - atak
    - krack
    - 'krack atağı nasıl'
    - 'krack zafiyeti'
    - network
    - wi-fi
    - wifi
    - wpa2
    - 'wpa2 ağlar'
    - 'wpa2 wifi ağlar'
---

![](https://www.intersiber.com/wp-content/uploads/2017/10/krack-attack.png)

KRACK zafiyeti ile WPA2 protokolünü kullanan wi-fi ağlarının artık güvenli olmadığı ortaya çıktı. Bugüne kadar WPA2(Wi-Fi Protected Access II) ile wi-fi ağlarının güvenli olduğu düşünülüyordu. Ancak araştırmacılar KRACK(Key Reinstallation Attacks) zafiyeti ile bir wi-fi ağının parolasının bilinmeden dahi ağ trafiğinin izlenebileceğini ortaya çıkardı. Bu ilgili wi-fi ağının kapsama alanında olan bir saldırganın ağ trafiğini izleyebileceği anlamına geliyor.

Krack zafiyeti protokol düzeyinde bir zafiyet ve wpa2 implementasyonunu geçerli biçimde uygulamış tüm wi-fi ağları; cihaz, platform veya marka farketmeksizin tehlikede. Wi-fi destekli herhangi bir ağınız, cihazınız varsa ağ trafiğiniz izleniyor olabilir.

Krack zafiyeti ile ilgili wi-fi ağının parolası ele geçirilemiyor. Krack ile amaçlanan ağ parolasının ele geçirilmesi değil, ağ parolasının kullanılmasına gerek kalmadan ağ trafiğinin izlenmesi. Ağ trafiğinin izlenmesi sonucunda wi-fi ağınız ile kullandığınız kredi kartı bilgileriniz, finans uygulamalarınızın parolaları ve herhangi bir web/mobil uygulama parolanız saldırganların eline geçebilir. Parolalarınızın çalınması haricinde erişmeye çalıştığınız içeriğe zararlı kod enjekte edilmesi, sisteminize ulaşılması da mümkün hale geliyor.

HTTPS üzerinden akan trafik krack zafiyetinden etkilenmiyor. Yine de %100 güvenli olduğunu söylemek mümkün değil. Krack zafiyetinden korunmak için tüm trafiği VPN üzerinden geçirmek yine alınabilecek önlemler arasında. Bunların haricinde son kullanıcılar, üreticilerin güncelleme/yamalarını beklemek durumunda. Araştırmacılar tarafından, bir wi-fi ağının krack zafiyetinden etkilenip etkilenmediğinin kontrolü için yayınlanmış bir betik [şu adreste](https://github.com/vanhoefm/krackattacks-test-ap-ft) mevcut. Betik bir wi-fi ağının dinlenmesini değil, yalnızca krack zafiyetinden etkilenip etkilenmediğinin tespitini sağlıyor.

Krack zafiyeti ile ilgili yayınlanan web sitesi : <https://www.krackattacks.com/>

Güvenlik araştırmacısı Mathy Vanhoef tarafından yayınlanan ilgili paper : <https://papers.mathyvanhoef.com/ccs2017.pdf>