---
layout: default
title: Simple data structure implementations in C++
---

# {{ page.title }}

Each data structure shown will have a gist on GitHub.

Table of contents:

* <a href="#singly_linked_list">Singly linked list</a>
* <a href="#doubly_linked_list">Doubly linked list</a>
* <a href="#circularly_linked_list">Circularly linked list</a>
* <a href="#stack">Stack</a>
* <a href="#queue">Queue</a>

<a id="singly_linked_list"/>

## Singly linked list

A **linked list** is made up of **nodes**. Each node stores an **element** and a **pointer** to another node. The first node is called the **head** and the last node is called the **tail** which has a null pointer. This data structure can be scattered over memory; it does not have to be stored consecutively.

For linked list $$L$$, we may use the following notation:
* `L.head` the pointer for the head of the list and
* `L.tail`, the pointer for the tail of the list.

For node $$N$$ we may use the following notation:
* `N.data`, the element;
* `N.next`, the pointer to the next node in the list (or `NULL` if at the tail).

<script src="https://gist.github.com/benapier/0e7d1cebe2801d387609e20ec594646a.js"></script>

<a id="doubly_linked_list"/>

## Doubly linked list

**Doubly linked list** are an extension of what we have just defined (singly linked lists); a node in a **doubly** linked list stores two references:
* a pointer to the next node in the list and
* a pointer to the previous node in the list.

<script src="https://gist.github.com/benapier/590b5b808907cb8a4d2265562b197dfc.js"></script>

<a id="circularly_linked_list"/>

## Circularly linked list

**Circularly linked lists** are also an extension of singly linked lists. Nodes are defined the same as in singly linked list, that is, each node has a next pointer and a previous pointer and the data it is holding; however, there is no beginning or end, such that where normally the last element in a singly linked list would point to `NULL`, instead, it points to the first node in the list. As there is no beginning or end, we mark a node on the list as the **cursor** which is the starting node when we traverse the list.

<script src="https://gist.github.com/benapier/aa200b937771991f147c9f183f3c6783.js"></script>

<a id="stack"/>

## Stack

A **stack** is a collection of objects that are inserted and removed according to the **last-in-first-out** (LIFO) principle.
    
Objects can be inserted to the stack at any time, but only the most recently inserted objected can be removed at any time. Or more formally, a stack must have the methods
 
* `push(e)`, insert element `e` at the top of the stack and
* `pop()`, remove and return the top element of the stack.

Other miscellaneous methods are
* `size`, return the number of elements in the stack;
* `IsEmpty`, return boolean values indicating whether or not the stack is empty (though this seems to be pointless giving that it is equivalent to `size == 0`; and
* `top`, return the top element of the stack without removing it.

<script src="https://gist.github.com/benapier/b27ed3aec99538f2dfe2cb61dd53efb0.js"></script>

<a id="queue"/>

## Queue

A **queue** is a collection of objects that are inserted and removed according to the **first-in-first-out** (FIFO) principle. Element access and deletion are restricted to the first element in the sequence, called the \textbf{front} of the queue. Element insertion is restricted to the end of the sequence, which is called the \textbf{rear} of the queue.

A queue supports the methods

* `enqueue(e)`, insert element `e` at the rear of the queue;
* `dequeue()`, remove and return from the queue the element at the front;
and possibly
* `size`;
* `isEmpty`, although this is equivalent to `size == 0`; and
* `front`.

<script src="https://gist.github.com/benapier/54de9745bcdf5428883e553eedb78032.js"></script>
