# Reading 4

## Linked List

* A data structure that contains nodes that links/points to the next node in the list.

- A link list is a sequence of nodes
- Each node references the next node in the link

## There are two types of Linked Lists
- Node - Individual items/links that are housed in a linked list.  Each node will contain data pertaining to that nodes functionality.

* NEXT - Each node contains a property called next that references the next node.
* HEAD - Reference of type Node that points to the first node in a linked list
* CURRENT - Reference of type Node to the node that is currently being looked at.
* Traversing- When traversing a current variable at the Head must be created at the Head to ensure we are starting from the beginning of the Linked List.
- The best way to traverse a Linked List is through the use of a while() loop, which lets us check that the Next node in the list is not null.  When traversing  the current variable will tell us exactly where we are in the Linked List and help us to traverse forward.

- Singly - Refers to the number of references a node has and a singly linked list means that there is only one reference which points to the next node in the list.
- Doubly - There are two references within the node.  A doubly linked list means there will be a reference to both the 'Next' and 'Previous' node.
