---
id: 1154
title: 'Sudo Komutu ve Detaylı Sudo Kullanımı'
date: '2019-01-18T14:42:44+03:00'
author: 'Ogun Baysal'
layout: post
guid: 'https://intersiber.com/?p=1154'
permalink: /sudo-komutu-ve-detayli-sudo-kullanimi/
td_post_theme_settings:
    - 'a:1:{s:16:"td_post_template";s:17:"single_template_5";}'
ampforwp_custom_content_editor:
    - ''
ampforwp_custom_content_editor_checkbox:
    - null
ampforwp-amp-on-off:
    - default
post_views_count:
    - '2093'
use_ampforwp_page_builder:
    - 'yes'
ampforwp_page_builder_enable:
    - 'yes'
amp-page-builder:
    - '{"rows":[],"totalrows":"1","totalmodules":"1","settingdata":{"front_class":"","front_css":""}}'
image: /wp-content/uploads/2019/01/sudo.png
categories:
    - Linux
    - 'Ne Nasıl?'
tags:
    - 'sudo arkaplanda çalıştırma'
    - 'sudo başka kullanıcı olarak çalıştırma'
    - 'sudo dosya düzenleme'
    - 'sudo grubu'
    - 'sudo grubuna kullanıcı ekleme'
    - 'sudo kullanıcı ekleme'
    - 'sudo kullanımı'
    - 'sudo nedir'
    - 'sudo parola süresini uzatma'
---

Yeni linux kullanıcıları genellikle sudo komutununu sadece ‘Permission Denied’ hatası alınan yerlerde hatayı düzeltmek amaçlı kullanırlar. Fakat sudo bundan daha fazla işleve sahip.

### **Sudo Nedir ?**

Sudo ile yaygın bir yanılgı, yalnızca sıradan bir kullanıcıya kök izinlerini sağlamak için kullanılmasıdır. Ama aslında, bu komut, varsayılan olarak root olan bir kullanıcı tarafından komut çalıştırmanıza izin verir.

### ![](https://intersiber.com/wp-content/uploads/2019/01/Screenshot-from-2019-01-18-14-01-51.png)

### **Kullanıcıya Sudo Kullanımı Yetkisi Nasıl Verilir ?** 

Ubuntu kullanıcıları genellikle girilen sudo komutunu çalıştırabilirler. Bunun nedeni, ubuntu kurulumu sırasında varsayılan bir kullanıcı oluşturulması ve ubuntudaki varsayılan kullanıcılara her zaman sudo izni verilmiş olmasıdır.

Sudo komutuna normal bir durumda sadece birkaç kişi erişebilmeli ve sistem yöneticisi olmalıdırlar. Diğer kullanıcılara sadece kendilerinin ihtiyacı olan yetkiler verilmelidir

Kullanıcılara Sudo izinleri vermek için, bunları Sudo grubuna eklemeniz yeterlidir. Bir kullanıcı oluştururken, aşağıdaki komutu kullanın:

`$sudo useradd -m -G sudo`

Yukarıdaki komut bir kullanıcı yaratacak ve kullanıcıyı Sudo grubuna ekleyecektir. Kullanıcı zaten varsa, aşağıdaki komutu kullanarak kullanıcıyı Sudo grubuna ekleyebilirsiniz:

`$sudo usermod -a -G sudo`

### **Sudo Komutuyla İlgili Küçük Bir Hile**

Eğer terminale uzun bir kod yazdıysanız ve ‘Permission Denied’ hatası aldıysanız aşağıda vereceğim kod ile kodu tekrar yazmaktan kurtulabilirsiniz.

`$sudo !!`

Bu kod, bunu yazmadan önce çalıştırılan son komutu direkt olarak sudo ile çaşıştırır.

### **Sudo ile Root Kullanıcısına Nasıl Geçilir ?**

Su komutu bir kullanıcı hesabından diğerine geçmek için kullanılır. Su komutunu kendi üzerinde çalıştırmak superuser hesabına geçer. Bu nedenle, Sudo kullanarak süper kullanıcı hesabına geçmek için aşağıdaki komutu çalıştırmanız yeterlidir:

`$sudo su`

### **Sudo Komutunu Arkaplanda Nasıl Çalıştırırım ?** 

Arka planda süper kullanıcı ayrıcalıkları gerektiren bir komut çalıştırmak isterseniz, burada gösterildiği gibi Sudo komutunu -b parametresi ile çalıştırın:

`$sudo -b`

Çalıştırılan komut kullanıcı etkileşimi gerektiriyorsa, bunun işe yaramayacağını unutmayın.

Arka planda bir komut çalıştırmanın alternatif bir yolu, sonuna aşağıdaki gibi bir ve işareti eklemek:

`$sudo &`

### **Sudo Ayrıcalıklarını Kullanarak Dosyaları Nasıl Düzenleriz ?**

Süper kullanıcı ayrıcalıklarını kullanarak bir dosyayı düzenlemenin yolu, Sudo kullanarak aşağıdaki gibi GNU nano gibi bir editör çalıştırmaktır:

`$sudo nano`

Alternatif olarak, aşağıdaki sözdizimini kullanabilirsiniz:

`$sudo -e`

### **Sudo Kullanarak Bir Komut Nasıl Başka Bir Kullanıcı Olarak Çalıştırılır ?** 

Sudo komutu bir komutu başka bir kullanıcı olarak çalıştırmak için kullanılabilir. Örneğin, “john” kullanıcısı olarak giriş yaptıysanız ve komutu “terry” olarak çalıştırmak istiyorsanız, Sudo komutunu aşağıdaki şekilde çalıştırırsınız:

`sudo-u terry`

### **Sudo Kimlik Bilgileri Nasıl Doğrulanır ?** 

Sudo kullanarak bir komut çalıştırdığınızda, şifreniz istenir. Daha sonra bir süre, Sudo kullanarak şifrenizi girmeden diğer komutları çalıştırabilirsiniz. Bu süreyi uzatmak istiyorsanız, aşağıdaki komutu çalıştırın:

`$sudo -v`