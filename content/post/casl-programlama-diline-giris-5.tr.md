+++
author = "Mehmet Akif Çakar"
categories = ["Programlama"]
date = "2003-10-08"
description = "CASL Programlama Diline Giriş Serisi 5"
linktitle = "CASL Programlama Diline Giriş 5"
title = "CASL Programlama Diline Giriş 5"
slug = "casl-programlama-diline-giris-5"
type = "post"
+++

## Döngüler, Kontroller Ve Operatörler

Döngüler : Burada döngülerin kullanımından bahsetmeyeceğim yalnızca
Casl’daki yazım şekillerini vereceğim.
For döngüsü :
Yazımı :
```
For i=0, i<=Kontrol_degeri;
dizi[i]=dizi[i]+2;
Next i+2;
```
Örnekte görüldüğü gibi yazım şekli

For baslangic_degeri,nereye_kadar;
```
#islemler
Next artis_miktari;

While döngüsü :
While uzunluk<20;
sayi=sayi2+1;
End_while;
```

Konroller: Burada en çok kullanılan if kontrolünü ve tiplerini göreceğiz.
If kontrolü :
```
If deger=20;
# işlemler
End_if;
Dallanmalı if kontrolü :
if deger=0;
#işlemler
{ Else_if deger2<>-1;
#işlemler
{ Else;
#işlemler
}End_if;
```

Operatörler :
Matemetiksel operatörler : C dilindeki operatörlerle aynıdır.
```
+ Toplama
– Çıkarma
/ Bölme
* Çarpma
% Mod
```
Mantıksal Operatörler : Pascal dilindeki operatörlerle aynı yazılıma sahiptirler.
```
= Eşittir
<> Eşit Değildir
< Küçüktür.
> Büyüktür
<= Küçük Eşit
> Büyük Eşit
And ve
Or veya
Not Değil
```