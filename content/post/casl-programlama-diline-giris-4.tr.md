+++
author = "Mehmet Akif Çakar"
categories = ["Programlama"]
date = "2003-10-07"
description = "CASL Programlama Diline Giriş Serisi 4"
linktitle = "CASL Programlama Diline Giriş 4"
title = "CASL Programlama Diline Giriş 4"
slug = "casl-programlama-diline-giris-4"
type = "post"
+++

## Fonksiyon Tipleri – 2
3- Hazır Fonksiyonları : Casl’ın programcıları tarafından önceden hazırlamış fonfsiyonlar bu gruba girer. ArcSin, Lenght, Right gibi onlarca fonksiyon casl kütüphanelerinde mevcuttur. Lazım olduklarında Casl’ın help dosyasında tümü sıralanmış bir biçimde mevcut.
Örnek :
```
Function tiklanirsa() as Numeric;
tiklanirsa=Day();
End;
```
Burada hazir fonksiyonlardan Day() fonksiyonunu kullandık. Day fonksiyonu geçerli olan günü döndürür.
4- Özyinelemeli Fonksiyon : Yine bilinen fonksiyon tiplerinden faktörüyel, üs alma gibi matematiksel işlemlerde üstüne yoktur. Oyunlarda şahsen yapay zeka kontrolü, yön bulma teknikleri, tanımlamalarda kullanımlarında üzerine tanımam. Fonksiyon içerisine yazdığımız kontrolün yanına fanksiyonun adını yazmamız gerekli. Fakat parametrelere dikkat sonsuz döngüye girebilir!.

5- Çağırımlı Basit fonksiyonlar. Ufak işlemleri yaptırmak için yazdığımız fonksiyonlar. Çağırım şekilleri (Call fonksiyon_adi(parametre));

6- Zamanlı fonksiyonlar ilk işlediğim olay fonksiyonunda buna örnek verdiğim için bunu hızlıca geçiyorum.