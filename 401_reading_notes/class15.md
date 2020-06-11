# Tree


***common Terminology in trees***

 * Node - A node is the individual item/data that makes up the data structure
 * Splitting - dividing two node into two subnodes
 * Root - The root is the first/top Node in the tree
 * Left Child - The node that is positioned to the left of a root or node
 * Right Child - The node that is positioned to the right of a root or node
 * Edge - The edge in a tree is the link between a parent and child node
 * Leaf - A leaf is a node that does not contain any children
 * Height - The height of a tree is determined by the number of edges from  the root to the bottommost node

 ## How to traverse between nodes in a tree

 we can traversse through any tree in two ways:
 1. Depth first
 2. Breadth first


### Depth first
 the paths in depth trees are:
 1. per-order
 2. in-order
 3. post-order

its when we priotrize traversing through the depth and the common way traverse through a tree is to use ***recursion***.

#### pre-order

pre-order pesudo code

ALGORITHM preOrder(root)

  OUTPUT <-- root.value

  if root.left is not NULL
      preOrder(root.left)

  if root.right is not NULL
      preOrder(root.right)

it means that the root has to be looked at first. looking means that we have to output its value calling preOrder function for the first time will add the root to the call stack then it will print the value of root value
because that OUTPUT <-- root.value in the pesudo code then check for left node then call the function preOrder recursivly and left node now become the root and we print its value this operation continue until we reach the end of the tree which called leaf and keep adding to the call stack 



### Breadth First

its when we priotrize traversing in the same level of the tree node.
Breadth first traversal uses a queue (instead of the call stack via recursion) to traverse the width/breadth of the tree. Let’s break down the process. 






## Tree Types
There are different types of tree data structures. Some of them are

**Binary Tree**: each node can have two children. A perfect binary tree is a binary tree in which all interior nodes have two children and all leaves have the same depth or same level.The Big O time complexity for inserting a new node is O(n). Searching for a specific node will also be O(n)

**Binary search tree**: BST is a binary tree with certain properties such as left child of the given node contains value less than equal to the given node and right hand child contain node greater than the given node.
The Big O time complexity of a Binary Search Tree’s insertion and search operations is O(height) Big O space complexity of a BST search would be O(1) becuse we are not allocating any additional space. during the search

**Red-Black tree**: Another variant of binary tree it is a self balancing binary search tree. In this tree nodes are either colored red or black.

**Splay tree**: A splay tree is a self-adjusting binary search tree with the additional property that recently accessed elements are quick to access again. All normal operations on a binary search tree are combined with one basic operation, called splaying wich is just re arranging the tree so that the element is placed at the root of the tree.

**N-ary tree**: In this tree the limitation of the binary tree is removed. Here a node can have at most n children. Like binary tree it can be full,complete or perfect n-ary tree. N-ary is some time known as forest.

**Huffman Tree**: Huffman tree is a frequency sorted binary tree used in compressing data.

**Heap Structure** : Heap structure is another widely used tree structure with a specific ordering property. There are two types of heap - Min heap and Max heap. In a min heap the parent of a node must be smaller than the values of all its children. Similarly in max heap the parent always have greater value compared to all its children.