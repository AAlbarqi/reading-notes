# Linked Lists

A Linked List is a sequence of Nodes that are connected/linked to each other.

## Linked Lists Types:

1. Singly - Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list.

2. Doubly - Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node.

3. Circular 

![](https://cdn.spotle.ai/7262/large/6vrSoRNX24.png)


## Big O for searching in a linkedlist

- The Big O of time for Includes would be O(n). This is because, at its worse case, the node we are looking for will be the very last node in the linked list. n represents the number of nodes in the linked list.

- The Big O of space for Includes would be O(1). This is because there is no additional space being used than what is already given to us with the linked list input.

## Terms:

1. Linked List - A data structure that contains nodes that links/points to the next node in the list.

2. Singly - Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list.

3. Doubly - Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node.

4. Node - Nodes are the individual items/links that live in a linked list. Each node contains the data for each link.

5. Next - Each node contains a property called Next. This property contains the reference to the next node.

6. Head - The Head is a reference type of type Node to the first node in a linked list.

7. Current - The Current reference is a reference type of type Node that is currently being looked at. This node is traditionally used when traversing through a full linked list. When traversing, you typically reset the current to the head to guarantee you are starting from the beginning of the linked list.