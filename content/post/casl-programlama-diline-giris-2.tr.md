+++
author = "Mehmet Akif Çakar"
categories = ["Programlama"]
date = "2003-10-04"
description = "CASL Programlama Diline Giriş Serisi 2"
linktitle = "CASL Programlama Diline Giriş 2"
title = "CASL Programlama Diline Giriş 2"
slug = "casl-programlama-diline-giris-2"
type = "post"
+++

## Genel Programlama Tanımı
1- Casl’da açıklamalar # işaretiyle başlar.
Örnek :
```
# Diziye iki katı değer atama
for i=1,i<10;
Array[i]=2*i;
next i;
```

2- Değişken isimlendirirken anlaşılır olmasına dikkat edin.
Örnek :
Arabanın fiyatı için kullanacağımız bir değişkene arabanin_fiyati demek doğru bir
kullanımdır. Af, afiy gibi değişken isimlendirmeleri yanlış bir kullanımdır. Küçük
programlarda bu pek fark etmesede büyük çaplı projelerde bu tip kullanımın yararını
epey göreceksiniz. Bu tip isimlendirmeleri fonksiyon yazarken veya obje tanımlarkende
kullanmak gayet yerinde olacaktır.

Veri Yapıları
Casl’da 4 çeşit veri yapısı vardır. Bunlar : Nümerik, String,
Byte ve Objedir.
Nümerik veri tipi 8 byte’lık yer kaplar. Uzun tam sayılar ondalıklı sayılar bu gruba
girer.
Casl’daki string veri tipinin C dilindekinden farkı NULL karakter içermemesidir.
Byte tipi 0-255 arası tam sayıları içeren veri tipidir. Genelde programlarda bu
tipi kullanacağız.
Obje tipi adındanda anlaşılacağı gibi Casl’daki Buton, Etiket,
Resim nesnelerini tanımlarken kullanılacak tiptir. Aynı zamanda dizilerde obje olarak
tanımlanır.
Programda kullanacağımız değerleri Variables bloğu,fonksiyon içi, satır arasında tanımlayabiliriz. Tanımlarken Obje ise tipi adı, diğer tiplerde ise yalnızca değişken_adı kullanılır. Tanımlarken değer atayabiliriz.(C’deki gibi)

Örnekler :

Variables;
Dizi_adi[3,5,4];

End;

Button tus_grubu[4];
End;

ad=borc_miktari[4+alacakli];
Gördüğünüz gibi tanımlamalar oldukça basit. Dikkatinizi çektiyse her satırın noktalı virgüle bittiğini görebilirsiniz.


Casl da programlamaya geçmeden önce kullanacağımız ekran üzerinde bilgi veriyim. Cep bilgisayarlarının ekranları arasında pixel olarak pek fark olmasada genelde 160×200 çözünürlük kullanılır. Casl’da ekran çözünürlüğünü 160×200 olarak kullanır ve pozisyon 0’dan başlar. Aşağıdaki resimi incelediğinizde konuyu daha iyi kavrayacaksınız.

![CASL Ekran](/images/casl_ekran.jpg)