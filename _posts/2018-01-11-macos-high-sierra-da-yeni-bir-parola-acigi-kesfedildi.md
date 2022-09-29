---
id: 936
title: 'MacOS High Sierra&#8217;da Yeni Bir Parola Açığı Keşfedildi'
date: '2018-01-11T14:53:38+03:00'
author: 'Hakan Torun'
layout: post
guid: 'https://www.intersiber.com/?p=936'
permalink: /macos-high-sierra-da-yeni-bir-parola-acigi-kesfedildi/
post_views_count:
    - '516'
image: images/macos-high-sierra-password-bug.png
categories:
    - Apple
    - Genel
    - 'Öne Çıkan'
tags:
    - 10.13.2
    - 'app store'
    - 'high sierra'
    - macos
    - 'parola açığı'
    - 'parola hatası'
    - 'sistem tercihleri'
---

MacOS işletim sisteminin High Sierra sürümünde, App Store sistem tercihlerini parola kullanmadan açabilen yeni bir zafiyet açığa çıkarıldı.

Bu yeni parola hatası MacOS işletim sistemin en son sürümü olan High Sierra sürümünde keşfedildi. Bu hata sayesinde herhangi biri Mac bilgisayarınızın App Store sistem tercihlerine parola kullanmadan veya rastgele bir parola ile erişebilir hale geliyor.

Bu güvenlik açığı daha önceki MacOS High Sierra 10.13.1 sürümündeki boş şifre girerek elde edilen *root* yetkisi kadar ciddi bir açık değil.

Bu hafta Open Radar’da bildirildiği üzere güvenlik açığı MacOS 10.13.2 sürümünü etkiliyor ve bu güvenlik açığının çalıştırılabilmesi için saldırganın yönetici seviyesindeki bir hesap ile oturum açılmış bir bilgisayara erişiminin olması gerekiyor. Saldırgan boş bir parola veya rastgele bir parola ile açıktan faydalanabiliyor.

Eğer MacOS High Sierra kurulu bir bilgisayarınız varsa, kontrol etmek için:

- Sisteminize giriş yapın
- Sistem Tercihleri (System Preferences) ve ardından App Store’a tıklayın
- Kilit ikonuna tıklayın
- Açılan login ekranında rastgele bir parola ile veya boş bırakarak deneyin
- Kilidi Aç’a tıklayın, bingo!

Başarılı olabildiyseniz, App Store ayarlarında tam yetki elde etmiş olacaksınız. Bu sayede, otomatik güncellemeleri iptal etme, uygulama güncellemeleri, güvenlik güncellemeleri ile ilgili tüm ayarları değiştirebilir hale geleceksiniz.

Apple’ın MacOS High Sierra 10.13.3 güncellemesi ile hatayı gidereceği düşünülüyor.