+++
author = "Mehmet Akif Çakar"
categories = ["Programlama"]
date = "2006-09-25"
description = "Mixed Code Generator Modeli Hakkında"
linktitle = "Mixed Code Generator Modeli Hakkında"
title = "Mixed Code Generator Modeli Hakkında"
slug = "mixed-code-generator-modeli-hakkinda"
type = "post"
+++

## Mixed Code Generator Modeli Hakkında

Inline Code Expander Modeli’nin dez-âvantajlarını kapatmak için geliştirilen kod üretim modelidir. Bu modelde gömülü SQL uygulamaları açıklama satırları olarak girilir. Böylece programcının kodu direk derlemesi mümkün olmakdadır. Ayrıca oluşturulan kaynak kod, üreticinden geçen kodun kendisi olduğundan herhangi bir uyum sorunu da yaşanmamaktadır.
Örnek : Gömülü SQL (CSQL) Dili
```
int main(int argc, char *argv[])
{
 //SQL select * from users
 //SQL END
 return 0;
}
```
Örnek : C Dili

```
#include “db.h”
int main(int argc, char *argv[])
{
 //SQL select * from users
 DBHandle *db_handle = db_connect();
 DBQueryData *db_data = db_db_query(db_handle, “select * from users”);
 for(int record= 0; record< db_data->length;record++)
 {
 //Programcı için açıklama alanı
 }
 //SQL END
 return 0;
}
```

Örnek Model Şeması :

![Mixed Code Generator 1](/images/MixedCodeGenerator1.jpg)

Model Üretim Süreç Şeması :

![Mixed Code Generator 2](/images/MixedCodeGenerator2.jpg)