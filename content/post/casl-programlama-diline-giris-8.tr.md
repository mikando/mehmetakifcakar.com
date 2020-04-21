+++
author = "Mehmet Akif Çakar"
categories = ["Programlama"]
date = "2003-10-11"
description = "CASL Programlama Diline Giriş Serisi 8"
linktitle = "CASL Programlama Diline Giriş 8"
title = "CASL Programlama Diline Giriş 8"
slug = "casl-programlama-diline-giris-8"
type = "post"
+++

## Casl’da Veritabanı Kullanımı

Casl’ın programcıları diğer bütün işlerde olduğu gibi veritabanı kullanımında da işimizi oldukça kolaylaştırılmış.

1- Veri tabanına bağlanma : Casl’da bağlanacağımız veri tabanını dbfile objesi olarak tanımlamamız gerekiyor.

Örnek :
```
dbfile veritabani;
field alan_adi;
field alan_adi2;
#veri tabanınındaki tüm alan adlarını belirtmemiz gerekiyor.
sync_pref merge;
data_sourche_name “Veri_tabani_adi“;
end;
```
Görüldüğü gibi bağlanmak kolay. Bu veritabanını değiştirmek istersek bunu bir fonksiyonla halledebiliriz şöyle.
```
function veri_tabanini_değiştir;
close veritabani;
veritabani.data_sourche_name = “Yeni_veritabani_adi“;
open veritabani;
end;
```
işin mantığınızı anladığınızı umuyorum. Yaptığımız veritabanını kapatıp adını değiştirip yeniden açtık. Güvenlikli veritabanına bağlanırken tek değişen komut veri tabanının isminin yanına kullanıcı adı ve parolayıda yazıyoruz
Şöyle :
```
dbfile veritabani;
field alan_adi;
field alan_adi2;
#veri tabanınındaki tüm alan adlarını belirtmemiz gerekiyor.
sync_pref merge;
data_sourche_name “DSN=Veri_tabani_adi;UID=Kullanici_adi;PWD=Parola;”;
end;
```
Bundan sonrasını kullandığımız veri tabanının komutlarını kullanarak yapabiliriz.