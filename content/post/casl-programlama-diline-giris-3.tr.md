+++
author = "Mehmet Akif Çakar"
categories = ["Programlama"]
date = "2003-10-06"
description = "CASL Programlama Diline Giriş Serisi 3"
linktitle = "CASL Programlama Diline Giriş 3"
title = "CASL Programlama Diline Giriş 3"
slug = "casl-programlama-diline-giris-3"
type = "post"
+++

## Fonksiyon Tipleri

Casl’da fonksiyonlar farklı olmasada fonksiyon mantığının yerleşmesi için fonksiyonları 6 grupta incelemede fayda görüyorum.
1- Olay Fonksiyonları : Bir olayı yerine getirmek için yazabileceğimiz fonksiyon tipidir. Periyodik olarak tekrarlamak istediğimiz işleri (Yazım şekliTimer fonkiyon_adı,milisaniye;) yada açılış kapanış olaylarında bu fonksiyon tipi kullanılır.

Örnek:
```
Function salisede_bir_defa;
#tekrarlanacak olay buraya yazılır
Timer salisede_bir_defa,100;
End;
```
Örnektede görüldüğü gibi işimize çok yarayacak bir fonksiyon yazılımı. Böylece salisede birkez kendini çağırır.

2-Normal Fonksiyonlar : Bildiğimiz parametreli değer döndüren fonksiyonlar bu gruba girer. Çoğu iş için kullanılabilirler genelde hesaplamalarda işimize yararlar.
Örnek :
```
Variables;
Numeric deger1;
Numeric deger2[2];
End;

Function hesapla(Numeric a, Numerib b[]);
a=a*2;
b[1]=b[1]*4;
End;

Funtion baslangic;
deger1=2;
deger2[1]=5;
hesapla(deger1,deger2);
End;
```

Bilinen basit bir hesaplama örneği burada başta global değişkenler tanınıp baslangic fonksiyonunda ilk değerleri atandı ve hesapla fonksiyonu çağırılarak hesaplama yapıldı. Değer döndüren fonksiyonlarda tek fark tipin belirtilmesi bunu da(Function fonsiyon_adi(parametreler) as Veri_Tipi;) döndürülecek değer fonksiyonun adına eşitlenir.