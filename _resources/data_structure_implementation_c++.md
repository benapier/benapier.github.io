---
layout: default
title: Simple data structure implementations in C++
---

# {{ page.title }}

Each data structure shown will have a gist on GitHub.

## Singly linked list

A **linked list** is made up of **nodes** Each node stores an **element** and a **pointer** to another node. The first node is called the **head** and the last node is called the **tail** which has a null pointer. This data structure can be scattered over memory; it does not have to be stored consecutively.

For linked list $$L$$, we may use the following notation:
* `L.head` the pointer for the head of the list and
* `L.tail`, the pointer for the tail of the list.

For node $$N$$ we may use the following notation:
* `N.data`, the element;
* `N.next`, the pointer to the next node in the list (or `NULL` if at the tail).

<script src="https://gist.github.com/benapier/0e7d1cebe2801d387609e20ec594646a.js"></script>

## Doubly linked list

**Doubly linked list** are an extension of what we have just defined (singly linked lists); a node in a **doubly** linked list stores two references:
* a pointer to the next node in the list and
* a pointer to the previous node in the list.

<script src="https://gist.github.com/benapier/590b5b808907cb8a4d2265562b197dfc.js"></script>

## Stack

## Queue
