# Döngüler / Loops
## For Loop / For Döngüsü
```php
<?php 
// Döngüler belirli bir koşula bağlı olarak bir kod satırını birden fazla kez tekrarlamak amacıyla kullanılır. 
$isimler = ["Ali","Mehmet","Şeref","Ela","Osman","Kerim","Pancar","Şeftali"]; 

// count : Bu method ile array içerisinde kaç adet değer olduğunu bulursunuz 
// count($isimler) 
// Count methodu 1.index'den saymaya başlar. 

// for içerisinde girilen değer yukarıdaki ile aynı ada sahip olamaz, olması durumunda yukarıdaki değişkeni yeni değişken olarak tanımlar ve içerisini değiştirir. 

// $i < 8 : i değişkeni 8'den küçük, 8'i dahil etmez 
// [< : küçük ,<= : küçük eşittir,> : büyük,>= : büyük eşitir] 
// $i++ : i değişkenini 1 arttır, sonra ekrana yazdırır. 
// ++$i : i değişkenini ekrana yazdırır sonra 1 arttırır. 
// [++ : 1 arttırır, -- : 1 azaltır] 

 for($i=0; $i<count($isimler); $i++){
    echo " ".$isimler[$i]." ";
} 
?> 
```

> Örnek 1
```php
<select> 
<?php 
for($i=1961; $i<2025; $i++) { 
    echo '<option>'.$i.'</option>'; 
} 
?> 
</select> 
```
----
## Foreach Döngüsü / Foreach loop
```php
<?php 

// foreach döngüsü sadece diziler için oluşturulmuş döngü türüdür. 
$dizi = ["Armut","Elma","Şeftali","Turp"]; 
print_r($dizi); // Dizinin tüm içeriğini yazdırır.

// foreach içerisine : $diziAdı as $elemanaAtanacakDeger şeklinde yazılmalıdır. Örnek Aşağıda bulunmakta 
foreach($dizi as $meyveler) { 
  echo $meyveler." "; // $dizi adlı dizinin içerisindeki her elemanı $meyveler değişkenine atar ve ekrana yazdırır. 
}


// for döngüsü ile dizilerde key olarak tanımlı değerleri almak mümkün değildir, ancak foreach ile bir dizide değişken key olarak tanımlı olsa dahi bunu çağırmak mümkündür. 
$dizi2 = array("Meyve"=>"Elma","Armut","Sebze"=>array("Pırasa","Turp"),"Yemek"); 


// for ile $dizi2'de olan Yemek elemanını alabiliriz yalnızca. 
// foreach ile $dizi2'de olan tüm elemanları (meyve,sebze) de dahil alabiliriz, çağırabiliriz. 
// Dizi'deki elemanların index değerini öğrenmek istiyorsak ve bunu foreachle yapmak istiyor isek; 
foreach($dizi2 as $anahtar=>$eleman) { 
   echo "Key : ".$anahtar." / Eleman : ".$eleman; 
} 
?> 
```
