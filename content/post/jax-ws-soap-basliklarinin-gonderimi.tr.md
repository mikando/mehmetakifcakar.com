+++
author = "Mehmet Akif Çakar"
categories = ["Programlama"]
date = "2008-05-07"
description = "Jax-ws ile Soap Başlıklarının Gönderimi"
linktitle = "Jax-ws ile Soap Başlıklarının Gönderimi"
title = "Jax-ws ile Soap Başlıklarının Gönderimi"
slug = "jax-ws-soap-basliklarinin-gonderimi"
type = "post"
+++

JAX-WS RI 2.1.3 ile birlikte Web servislere [Soap başlıklarını](https://jax-ws.dev.java.net/guide/SOAP_headers.html) gönderirken kullanılabilecek pratik bir yöntemi paylaşmak istiyorum. wsimport aracı artık -XadditionalHeaders parametresi ile ürettiği istemci kodunda soap başlıklarını metot parametresi olarak üretebiliyor. Böylece WSBindingProvider sınıfını kullanmamıza gerek yok. Ant kullananlarsa wsimport görevine aynı şekilde XadditionalHeaders=true parametresini ekleyebilirler.