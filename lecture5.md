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













