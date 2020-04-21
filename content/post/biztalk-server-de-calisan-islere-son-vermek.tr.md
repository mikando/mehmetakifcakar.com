+++
author = "Mehmet Akif Çakar"
categories = ["Programlama"]
date = "2009-03-15"
description = "Biztalk Server’de çalışan işlere son vermek"
linktitle = "Biztalk Server’de çalışan işlere son vermek"
title = "Biztalk Server’de çalışan işlere son vermek"
slug = "biztalk-server-de-calisan-islere-son-vermek"
type = "post"
+++

Bilindiği üzere Biztalk Server ile entegrasyon çözümlerinde düzenli olarak yapılması gereken bakım işlemlerinde atıl durumdaki çalışan(aslında çalışmayan) işlemlerin temizlenmesi gerekmektedir. Temizleme işlemine başlamadan önce unutulmaması gerekenler:

    * Receive Location Adaptörlerinin kontrolü (Bazı durumlarda durdurulmaları gerekebilir)
    * Adaptörün kullandığı IIS sunucusunun kontrolü (Adaptörle aynı durum söz konusu)
    * SQLServer Agent servisinin çalıştığından emin olun.(Biztalk sunucusu çoğu bakım işinde SQLServer Agent’i kullanır.)