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



O(n) linked list'te öğe aramak (stack ve queue)

O(1) linked list'e öğe eklemek (stack)

O(n) linked list'e öğe eklemek (queue), sıralı şekilde öğe eklemek





trees



binary search trees

ikili aramaya ağacın kökü olan en tepesinden başlarız, bu linked list'teki list pointer'a çok benziyor.



typedef struct node
{
  int number;
  struct node *left;
  struct node *right;
}
node;



bool search(node *tree, int number)
{
  if (tree = NULL)
  { 
    return false;  
  }
  else if (number < tree->number)
  {
    return search(tree->left, number);
  }
  else if (number > tree->number)
  {
    return search(tree->right, number);
  }
  else
  {
    return true;
  }  
}


İkili arama algoritmasını uygulamazsak binary search tree bir linked array'e benzer.

O(log n) doğru algoritma kullanılmış binary search tree



dictionaries

in real life: word | definition
in computer science: key | value

key is what you look for something, value is what you find by that key.

name => number



hashing

geniş bir alandan daha basit bir alana indirgemek.


hash function


hash tables

teorik olarak amaç, sabit zaman O(1) ulaşmaktır.



node *table[26];


Albus -> |     | -> 0

Zacharias -> |     | -> 25

Arama yapmak O(n)

İyi bir hash function'u O(n/k) hala O(n) sayılır.


tries

retrieval'ın kısaltmasıdır,

fancier tree

Tries her node'u array olan bir tree'dir.

constant time, O(1)


typedef struct node
{
  char *number;
  struct node *children[26];
}
node;

node *trie;


