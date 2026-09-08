data structures





queue: FIFO

stack: LIFO

push
pop




struct

.

*

->


typedef struct node
{
  int number;
  struct node *next;
}
node;


array yerine linked list kullanmanın dezavantajı daha fazla hafıza kullanmaktır. Storage yanı sıra bir de birer pointer saklamak gerekiyor.
Linked list'e indeksleme yoluyla erişemeyiz.

Günümüzde bellek eskiye nazaran daha ucuz.


node *n = malloc(sizeof(node));
(*n).number = 1;

n->number = 1;
n->next = NULL;

list = n;


node *n = malloc(sizeof(node));
n->number = 2;
n->next = list;

list = n;

komut satırı argümanlarını terminalden almak için for döngüsünde i'yi 1 den başlatırız çünkü 0. indeks programın çalıştırma komutudur.



ptr







