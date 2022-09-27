---
id: 6337
title: 'Jio’daki Güvenlik Açığı, Koronavirüs Semptom Sonuçlarını Açığa Çıkardı'
date: '2020-05-03T17:00:20+03:00'
author: 'Ahmet Can Bilici'
layout: post
guid: 'https://intersiber.com/?p=6337'
permalink: /jiodaki-guvenlik-acigi-koronavirus-semptom-sonuclarini-aciga-cikardi/
post_views_count:
    - '27'
image: /wp-content/uploads/2020/05/jio-daki-guvenlik-acigi-koronavirus-semptom-sonuclarini-aciga-cikardi.png
categories:
    - Güvenlik
tags:
    - facebook
    - jio
    - koronavirüs
---

**Koronavirüs** salgınının başlangıcından bu yana hükümetler ve özel şirketler, virüs **semptomlarının** tanımlanması sürecini kolaylaştırmak için çeşitli uygulamalar ve web siteleri geliştirdiler.

Hindistan’ın en büyük mobil ağı olan **Jio**, ülke çapında **koronavirüs** ciddi bir şekilde yayılırken, insanların kendi kendine semptom testi yapabilmesi için bir uygulama başlatmıştı. **Semptom** **denetleyicisi** isimli uygulama, herkesin koronavirüs ile enfekte olup olmadığını öğrenebileceği bir yapı olarak, telefonlardan ya da Jio web sitesinden kontrol edilebiliyor.

Ancak veritabanındaki bir **güvenlik** **açığı**, semptom denetleyicisinin barındırdığı sonuçların, şifresiz bir şekilde herkes tarafından öğrenilebilmesine yol açtı.

Açık, kodlarda bu şekilde görünüyor:

<figure class="wp-block-image size-large">![](https://intersiber.com/wp-content/uploads/2020/05/jio-koronavirus-test-guvenlik-acigi.png)</figure>Güvenlik araştırmacısı Anurag Sen tarafından 1 Mayıs’ta tespit edilen açık öğrenildikten sonra, veritabanı çevrimdışı duruma getirildi. Ancak veritabanına kimlerin erişip erişmediği bilinmiyor.

**Jio** sözcüsü Tushar Pania, hemen harekete geçildiğini ifade ederek “Sunucu, herhangi bir **COVID**–**19** belirtisi olup olmadığını görmek için kendi kendini kontrol eden kişilerin bilgilerini içeriyordu” dedi.

17 Nisan’dan itibaren girilen bilgileri içeren veritabanı, milyonlarca kişinin kayıtlarını içeriyordu. Bunun yanı sıra veritabanında test olan insanların akrabaları, yaşları, cinsiyetleri gibi bilgiler de yer alıyordu. Bazı kayıtlarda ise kesin konum bilgisinin yer aldığı aktarıldı.

Hindistanlı telekom devi **Jio**, geçtiğimiz günlerde **Facebook** tarafından 5,7 milyar dolar **yatırım** almıştı. Şirket, konuyla ilgili gelen sorularla ilgili ek bir açıklama yapmazken, aboneler de bilgilendirilmedi.