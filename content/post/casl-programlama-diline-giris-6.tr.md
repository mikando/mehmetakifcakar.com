+++
author = "Mehmet Akif Çakar"
categories = ["Programlama"]
date = "2003-10-09"
description = "CASL Programlama Diline Giriş Serisi 6"
linktitle = "CASL Programlama Diline Giriş 6"
title = "CASL Programlama Diline Giriş 6"
slug = "casl-programlama-diline-giris-6"
type = "post"
+++

## Obje Kontrolü

1- Görsel Objeler : Burada görsel objelerin kullanumı için kullanılan komutlar hakkında bilgi vereceğim.

a- Get fonksiyonu : Get fonksiyonu objenin değerini almada kullanırız mesela bir etiketin yazısını almak için ``` (Get label1,string_degeri;) ``` yazmak yeterlidir.

b- Hide – Show Fonksiyonları : Nesneleri gizleme veya göstermek için kullanılırlar. ``` (Hide obje_adi;) ``` şeklinde yazılır.

c- Move Fonksiyonu : Objeyi taşımak için kullanılır. ``` (Move obje_adi,x_pozisyonu,y_pozisyonu;) ``` Şeklinde yazılır.

d- Put Fonksiyonu : Objeye değer atamada kullanılır. TextBox’a veri girmede kullanılabilir. ``` (Put obje_adi,deger;) ``` Şeklinde yazılır.

2- Grafikler : Grafik çizdirmede kullanılan fonksiyonlar.

a- Draw Fonksiyonu : Draw fonksiyonunda çember,dikdörtgen veya çizgi çizdirebiliriz. ``` (Draw nesne_adi,tipi,x_noktasi,y_noktasi;) ``` buradaki tip Rectangle,Circle yada Line ‘dan biri olmalıdır.

b- Set Fonksiyonu : Draw fonksiyonuyla çizdirdiğimiz nesneyi taşımada kullanılabilir. çizdirirken verdiğimiz ismi kullanmalıyız. ``` (Set nesne_adi,x_pozisyon,y_pozisyon;) ```

c- Clear Fonksiyonu : Temizlemede kullanılır. ``` (Clear nesne_adi,tipi,x_noktasi,y_noktasi;) ```

d- Fill Fonksiyonu : Draw fonksiyonu gibi kullanılır. Çizilen nesneyi doldurmaya yarar.