hexadecimal, base-16

Bir sayının hexadecimal olduğunu belirtmek için gelenek gereği başına "0x" konulur. Bu karışıklıkları önler.

integer 4 bayttır, ızgarada 4 baytlık kare yani 4 kare kaplar.


& bellekteki bir veri parçasının adresini almak.

* ampersand'ın tersini yapar. Adrese götürür.


pointers

bir pointer bir değerin adresini içeren bir değişkendir.
pointers 8 baytlık yer kaplar.

string'i tanımlarken " " otomatik olarak sona \0 (NUL) karakterini ekler.

string diye bir şey yoktu, char * vardı.

char *s = "HI!";
printf("%s\n", s);

s pointer HI! stringindeki H'nin adresini tutuyor. printf'de *s yazmayıp s yazıyoruz çünkü %s böyle çalışır. *s yazarsak 'H' karakterini ekrana yazdırırdı.

