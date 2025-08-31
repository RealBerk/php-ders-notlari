> Yayınlanma Tarihi : 01.09.2025
# Diziler / Arrays


Diziler değişkenden farklı olarak birden fazla değeri gruplandırarak taşıma işlemi yapan elemanlardır. Diziler'de kullanabileceğimiz 3 yöntem bulunmakta ve bu yöntemler aşağıdaki gibidir;

------------------
- ```php
  $dizi1 = array();
  ```

- ```php
  $dizi2[]="";
  ```

- ```php
  $dizi3 = ["HTML","CSS","PHP"];
  ```
------------------
# Kullanım / Usage
------------------


| Yöntem   | Kullanım                                |
| -------- | --------------------------------------- |
| Yöntem 1 |    $ornek = array("HTML","PHP","CSS");  |
| Yöntem 2 |     $dizi2[0]="deneme";                 |
| Yöntem 3 |     $dizi3 = ["HTML","CSS","PHP"];      |

------------------
# Diziye özel sayı yada numara atama (Assigning a special number or number to a sequence)
------------------
```php

$ornek2 = array("html"=>"HTML","css"=>"CSS","php"=>"PHP");
echo "Merhaba ".$ornek2['php'];

```

* "özel index değerimiz" => "atama yapılacak değer"
> Bu şekilde özel olarak index değeri atayabiliriz dizemizdeki elemanlara.
