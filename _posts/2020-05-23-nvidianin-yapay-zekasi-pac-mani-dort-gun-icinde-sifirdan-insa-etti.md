---
id: 7428
title: 'NVIDIA&#8217;nın Yapay Zekası Pac-Man&#8217;ı Dört Gün İçinde Sıfırdan İnşa Etti'
date: '2020-05-23T15:00:00+03:00'
author: 'Beyza Bayrakdar'
layout: post
guid: 'https://intersiber.com/?p=7428'
permalink: /nvidianin-yapay-zekasi-pac-mani-dort-gun-icinde-sifirdan-insa-etti/
post_views_count:
    - '74'
image: /wp-content/uploads/2020/05/nvidianin-yapay-zekasi-pac-mani-dort-gun-icinde-sifirdan-insa-etti.jpg
categories:
    - Oyun
tags:
    - nvidia
    - pacman
    - 'yapay zeka'
---

**Pac-Man** 22 Mayıs 1980’de oyun salonlarında çıkış yaptığında, tasarlanması, kodlanması ve tamamlanması için harcanan zamanın **17** ay sürdüğünün kaydını tuttu. 40 yıl sonra, **NVIDIA** yeni **GameGAN AI**‘ını başka bir **AI** oyununu izlemeye dayalı olarak oyunu sıfırdan oluşturacak şekilde eğitmesi için sadece dört günün yeterli olacağını açıkladı.

Dublajlı **GameGAN** üretken bir ağdır. Genel olarak GAN’lar jeneratör ve ayırımcı olmak üzere iki sinir ağını eşleştirerek çalışır. **Jeneratör**, büyük bir örnek veri kümesi üzerinde eğitilir ve daha sonra jeneratöre gördüklerine göre bir görüntü üretmesi talimatı verilir. **Ayrımcı ise** daha sonra ikisinin birbirine ne kadar yakın olduğunu belirlemek için oluşturulan görüntüyü örnek veri kümesiyle karşılaştırır. Bu ağlar arasında geçiş yaparak, **AI** yavaş yavaş daha gerçekçi görüntüler yaratır.

<figure class="wp-block-image size-large">![](https://intersiber.com/wp-content/uploads/2020/05/pacman-1600x897.jpg)</figure>Bu projede **üretken ağ**, oyunun **50.000** oyun oturumu kullanılarak eğitildi. Ardından üretken ağa statik duvarlardan ve noktalardan hayaletlere, **Pac-Man**‘ın kendisi ve etkileşimlerini yöneten kurallara kadar bir bütün olarak yeniden yaratması söylendi. Tüm süreç **GP100**‘lerin dörtlüsü üzerinde gerçekleşti. Ancak **GameGAN**, temel kod veya oyunun motoruna erişim sağlamadı. **GameGAN**, oyun oynarken ağabeyinizin omzuna bakarak kuralları öğrenmeye benzer şekilde, **Pac-Man**‘ı sadece başka bir AI’ın ekran hareketini izleyerek oluşturdu.

<figure class="wp-block-embed-youtube wp-block-embed is-type-video is-provider-youtube wp-embed-aspect-16-9 wp-has-aspect-ratio"><div class="wp-block-embed__wrapper"><span class="embed-youtube" style="text-align:center; display: block;"><iframe allowfullscreen="true" class="youtube-player" height="360" src="https://www.youtube.com/embed/BYt6r8z6pUY?version=3&rel=1&fs=1&autohide=2&showsearch=0&showinfo=1&iv_load_policy=1&wmode=transparent" style="border:0;" width="640"></iframe></span></div></figure>**NVIDIA**‘nın simülasyon teknolojisi başkan yardımcısı **Rev Lebaredian**, “Son yıllarda oyun oynayabilen ve bu oyunlarda ajan olan birçok yapay zeka yaratıldı. Ama bu aslında oyunun kendisini kara bir kutu olarak yeniden üretebilen ilk **GAN**.” dedi.

NVIDIA Toronto araştırma laboratuvarının direktörü **Sanja Fidler** gelişen teknoloji ile ilgili “Sonunda, sadece videoları izleyerek ve ajanların bir ortamda eylemde bulunduğunu görerek sürüş kurallarını, fizik yasalarını taklit etmeyi öğrenebilecek bir yapay zekaya sahip olabiliriz. **GameGAN** buna doğru ilk adım.” açıklamasını yaptı.

NVIDIA’nın **GameGAN Pac-Man** oyunu bu yaz sonunda **çevrimiçi** olarak piyasaya çıktığında hem insanların hem de **CPU**‘ların oynayabileceği tamamen işlevsel bir oyun olacak.