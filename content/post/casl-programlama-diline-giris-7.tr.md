+++
author = "Mehmet Akif Çakar"
categories = ["Programlama"]
date = "2003-10-10"
description = "CASL Programlama Diline Giriş Serisi 7"
linktitle = "CASL Programlama Diline Giriş 7"
title = "CASL Programlama Diline Giriş 7"
slug = "casl-programlama-diline-giris-7"
type = "post"
+++

## Obje Kontrolü 2

3- Dosya Objeleri : Dosya objelerinin kullanımı Casl’da oldukça kolaydır.
a- Close Fonksiyonu : Dosya kapatmaya yarar. ``` (Close dosya_obje_adi;) ```
b- Delete Fonksiyonu : Dosya silmeye yarar. ``` (Delete dosya_obje_adi;) ```
c- Open Fonksiyonu : Dosya açmaya yarar. ``` (Open dosya_obje_adi,dosya_adi;) ```
d- Rename Fonksiyonu : Yeniden adlandırmaya yarar. ``` (Rename eski_dosya_adi,yeni_dosya_adi;) ```
e- Get Fonksiyonu : Dosyadan veri almada kullanılır ``` (Get dosya_obje_adi,atanacak_string_deger,sayisal_veri_uzunlugu;) ```
f- Put Fonksiyonu : Get gibi kullanılır dosyaya veri yazmaya yarar.
g- Insert Fonksiyonu : Put fonksiyonuna benzer yazılım şeklide aynıdır.
h- Seek_start Fonksiyonu : Put,get fonksiyonlarının kullanacağı pozisyonu belirlemede kullanılır. ``` (Seek_start dosya_obje_adi,sayisal_sira_nosu;) ```
i- Seek_here Fonksiyonu : Put, get fonksiyonları için sonraki adımı belirlemede kullanılır.
j- Seek_end Fonksiyonu : Atlamayı bitirir. Tüm seek fonksiyonlarının yazımı aynıdır.
4- Diğer Objeler : SeriPort, VeriTabanı ve Network objelerini bu grupta inceleyecektim fakat bu konular orta düzey olduklarından şimdiden işlemeyi uygun bulmuyorum. Bilgi için Casl’daki yardım dosyalarına bakabilirsiniz.