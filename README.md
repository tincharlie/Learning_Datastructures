# Learning_Datastructures
> ## Queue
**Queue is an linear data structure where you can add element from one side and delete from another side as well.**
We have first in first out and last in last out.

Here adding element at the rear and removing front 

Add Element --> Enqueue --> append method 
Delete Element --> Dequeue --> pop method

`Two ways of implementation`
### 1. List 
In the list we can normally define and use the pop and append function 

### 2. Module
In this need to import the `queue or collection` package to make the queue.

> ## Linked List:
**It basisclly contains chain of nodes those nodes contains data field, link, reference.**

For example:
If we have 3 node, one node is connected to 2nd node and 2nd node is connected to 3rd node so here it store some reference of previous node.

   [D1| ]-->[D2| ]-->[D3| ]
[head      contains ref    tail]
    [N1       N2       N3]

Ref of Node2 is store in Node1
Ref of Node3 is store in Node2
Ref of Node1 is called head
End Node is called tail

### Type of Linked List:

`Singly`: Contains one reference
`Doubly`: Contains two reference
`Circular`: Contains reference in eg: 1-->2-->3-->1 it is called circular

> ### Singly Linked List: 
**Chain of node contain reference of next node**

     [17|5015]-->[36|5025 ]-->[50|5035]-->[80|None ]
[head    5010        5015        5025        5035    tail]
     [    N1          N2          N3          N4]
5015 nothing but a reference of next node.


> ### Doubly Linked List:
**Contains two reference in the chain of node.**

     [ None | 17 | 5015]<-->[ 5010 | 36 | 5025 ]<-->[ 5015 | 50 | 5035 ]<-->[ 5025 | 80 | None ]
[head        5010                   5015                     5025                    5035    tail]
         [N1                         N2                       N3                      N4]
5015 nothing but a reference of next node.
Here you can see the left ref and right ref.

> ### Circular Linked List:

Circular Singly
     [17|5015]-->[36|5025 ]-->[50|5035]-->[80|5010 ]
[head    5010        5015        5025        5035    tail]
         [N1          N2          N3          N4]
Here 5010 ref is in the last node so thats why its an circular list

Circular Doubly
     [ 5035 | 17 | 5015]<-->[ 5010 | 36 | 5025 ]<-->[ 5015 | 50 | 5035 ]<-->[ 5025 | 80 | 5010 ]
[head        5010                   5015                     5025                    5035    tail]
         [N1                         N2                       N3                      N4]

Here you can see right ref of 1st node is 5035 connect to last node ref. and right ref of last node is 5010 is the first node ref.
