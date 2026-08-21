Programcı olarak yazacağımız kod, bundan böyle kısaca source code (kaynak kod) olarak adlandırılacaktır.
Bilgisayarların anladığı ise machine code (makine kodu).

Kaynak kodumuzu makine koduna çeviren özel programlar var.
Bu programlara compiler (derleyici) denir.

Kod kalitesini bu üç eksen üzerinden değerlendiriyoruz.

correctness, design, style.

Terminal -> CLI (Command Line Interface)
Bu, GUI (Grafic User Interface) ile tezattır.

VS Code üzerinde terminalde code hello.c yazarak sekmemizi oluşturuyoruz.
make hello yazarak programımızı derliyoruz.
make programı bizim için bir derleyicidir.

./hello ile programı çalıştırıyoruz.


terminalde ctrl + L, clear ile eşdeğerdir.


bool
char
double
float
int
long
string
...

if (x < y)
{
  printf("x is less than y\n");
}

if'ten sonra boşluk bırakılır stilistik açıdan.


if (x < y)
{
  printf("x is less than y\n");
}
else
{
  printf("x is not less than y\n");
}


C'de = karakteri, sağdan sola atama manasına gelirken, Scratch'te eşittir anlamına gelir.

Mevcut bir değişkeni güncellerken 'İnt' anahtar kelimesini belirtmemize gerek yoktur.

Syntactic sugar: kodlamada aynı şeyi yapmanın genellikle birçok yolu vardır.

counter = counter + 1
counter += 1;
counter++;

Değişken adlandırırken genelde int için 'i', char için 'c', string için 's'... olarak adlandırırlar.

Sıfırdan saymaya başlamak döngülerde.




