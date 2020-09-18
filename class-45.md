# Trees

A tree is a hierarchical data structure consisting of a node (potentially) with children. The children are trees unto themselves, that is, nodes with (potential) children. For this reason the tree is referred to as a recursive data structure.

![](https://s3-us-west-2.amazonaws.com/forge-production.galvanize.com/releases/4395/Data%20Modeling%20%26%20Classes/images/ternary-and-quaternary-tree.gif)

- A tree would be great for.... Making a family tree.

## Binary Trees 

A tree whose elements have at most 2 children is called a binary tree. Since each element in a binary tree can have only 2 children, we typically name them the left and right child.

![](https://www.geeksforgeeks.org/wp-content/uploads/binary-tree-to-DLL.png)

A Binary Tree node contains following parts.
1. Data
2. Pointer to left child
3. Pointer to right child

## Binary Search Trees

Binary Search Tree is a node-based binary tree data structure which has the following properties:

- The left subtree of a node contains only nodes with keys lesser than the node’s key.
- The right subtree of a node contains only nodes with keys greater than the node’s key.
- The left and right subtree each must also be a binary search tree.

![](https://media.geeksforgeeks.org/wp-content/uploads/BSTSearch.png)

A binary search tree can be used to implement a simple sorting algorithm, also can serve as priority queues
