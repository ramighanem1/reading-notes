# linked lists

A linked list is a linear data structure used for storing collections of elements. It consists of a sequence of nodes, where each node contains both a data element and a reference to the next node in the sequence.

The first node in the list is called the head, while the last node is called the tail, and the reference in the tail is typically null to indicate the end of the list.


## linked lists types

* singly linked lists : 
where each node only has a reference to the next node.

* doubly linked lists : 
where each node has references to both the next and previous nodes.

* circular linked lists : 
where the tail node has a reference to the head node.

## linked lists operations

* Accessing an element: O(n)

    Because linked lists do not have direct access to their elements like arrays, you must traverse the list from the beginning to access a particular element. The worst-case time complexity for this operation is O(n), where n is the number of elements in the list.

* Insertion at the head: O(1)

    To insert a new element at the beginning of a linked list, you simply create a new node and point it to the current head node. This operation takes constant time O(1) because it does not depend on the size of the list.

* Insertion at the tail: O(1) with a tail pointer, O(n) without

    If you have a tail pointer that points to the last node of the list, inserting a new node at the end of the list can be done in constant time O(1) by simply updating the tail pointer. However, if you do not have a tail pointer and must traverse the list to find the last node, this operation takes O(n) time in the worst case.

* Insertion at a specific position: O(n)

    To insert a new node at a specific position in the list, you must first traverse the list to find the node at the desired position, which takes O(n) time in the worst case. Once you have found the node, inserting the new node takes constant time O(1).

* Deletion at the head: O(1)

    To delete the first element of a linked list, you simply update the head pointer to point to the next node. This operation takes constant time O(1) because it does not depend on the size of the list.

* Deletion at the tail: O(n) with a tail pointer, O(n^2) without

    If you have a tail pointer that points to the last node of the list, deleting the last node can be done in linear time O(n) by updating the tail pointer to point to the second-to-last node. However, if you do not have a tail pointer and must traverse the list to find the last node, this operation takes O(n^2) time in the worst case because you must first find the last node and then iterate over the list again to update the pointer of the second-to-last node.

* Deletion at a specific position: O(n)

    To delete a node at a specific position in the list, you must first traverse the list to find the node at the desired position, which takes O(n) time in the worst case. Once you have found the node, deleting it takes constant time O(1).
