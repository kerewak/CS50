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



malloc -> memory allocation: bellek tahsisi için kullanılır. Bu belleğin ilk baytının adresini döndürecektir.

free -> malloc'un tam tersi, bir bellek bloğuyla işimiz bittiğinde onu serbest bırakabiliriz.

...


#include <stdlib.h>


Genel olarak for döngüsündeki koşulumuzun içinde bir fonksiyon çağırmak optimizasyon açısından iyi bir tasarım değil.



NULL bir pointer'dır, 0 numaralı adres. Bilgisayar belleğinin sol üst köşesini işaret eder diyebiliriz.


malloc kullandıktan sonra onu free yapmamız gereklidir


Valgrind programı: Kodu inceleyip çalışırken oluşan bellek hatalarını bulacağız.


Oscar the Grouch'a ithafen garbage.c kodu.


garbage values


heap overflow

stack overflow


buffer overflow

















