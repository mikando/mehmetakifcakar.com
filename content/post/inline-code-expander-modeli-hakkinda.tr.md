+++
author = "Mehmet Akif Çakar"
categories = ["Programlama"]
date = "2006-09-03"
description = "Inline Code Expander Modeli Hakkında"
linktitle = "Inline Code Expander Modeli Hakkında"
title = "Inline Code Expander Modeli Hakkında"
slug = "inline-code-expander-modeli-hakkinda"
type = "post"
+++

## Inline Code Expander Modeli Hakkında

Mevcut bir dilde yazılmış olan kaynak kodu hedef dile uygun hazırlanmış şablona göre işleyip sonuçlandıran kod üretim modelidir. Bu model daha çok C dili içinde gömülü SQL (ing. embeded SQL) için kulanılmıştır.
Örnek : Gömülü SQL ((SQLC) Dili)
```
int main(int argc, char *argv[])
{
 <SQL select * from users>
 return 0;
}
```
Şeklinde yazılmış bir gömülü SQL kodunu Inline Code Expander Modeli ile yazılmış bir kod üreticiden geçirildiğinde SQLC kodu aşağıda görüleceği gibi saf C koduna çevrilmektedir.

Çıktı: C Dili

```
#include “db.h”
int main(int argc, char *argv[])
{
 DBHandle *db_handle = db_connect();
 DBQueryData *db_data = db_db_query(db_handle, “select * from users”);
 for(int record= 0; record< db_data->length;record++)
 {
 //Programcı için açıklama alanı
 }
 return 0;
}
```
Örneğin şeması :


![CASL Editor](/images/InlineCodeExpander1.jpg)


Böylece bir programcıya veritabanı ile yapacağı işlemleri veya birkaç satırda yapabilme olanağı tanınmış olmaktatır. Bu modelin en büyük dez-âvantajı kaynak kodda SQLC kodları yer aldığından bu kodun derlenebilmesi için kod üreticiden geçmesi gereğidir. Ki kod üretiminden geçse de oluşturulan kod farklı bir dosya olduğundan gelişim sürecinde kaynakla çıktı arasında uyumun kaybolmasıdır.
Model Üretim Süreç Şeması :

![CASL Editor](/images/InlineCodeExpander2.jpg)