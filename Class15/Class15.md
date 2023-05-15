# Trees 

A tree data structure is a hierarchical structure that is used to represent and organize data in a way that is easy to navigate and search. It is a collection of nodes that are connected by edges and has a hierarchical relationship between the nodes


# Trees data structure component

* Node: A component of a tree that contains values and references to other nodes.
* Root: The starting node of the tree.
* K: The maximum number of children any node can have in a k-ary tree. For binary trees, k = 2.
* Left: A reference to the left child node in a binary tree.
* Right: A reference to the right child node in a binary tree.
* Edge: The link between a parent and child node.
* Leaf: A node without any children.
* Height: The number of edges from the root to the furthest leaf.


# Traversals Trees
There are two categories of tree traversals:

### Depth-First Traversal: 

Prioritizes going through the depth (height) of the tree first. Three methods for depth-first traversal are:
* Pre-order: Root -> Left -> Right.
* In-order: Left -> Root -> Right.
* Post-order: Left -> Right -> Root.

### Breadth-First Traversal:

Iterates through the tree level by level, going node-by-node.


# Binary Trees and K-ary Trees

### Binary Trees:

Restrict the number of children per node to two (left and right child). There is no specific sorting order for nodes in a binary tree.
### K-ary Trees:

Nodes can have more than two children, and the tree is referred to as a k-ary tree. Traversing a k-ary tree is similar to breadth-first traversal, but instead of checking for left and right children, we check a list of children.

# Binary Search Trees (BST)

* Binary Search Trees: Organize nodes in a specific order. All values smaller than the root are placed to the left, and all values larger than the root are placed to the right.
* Searching in a BST: Comparisons are made against the root to determine whether to traverse the left or right side of the tree. This process continues until a leaf or a match is found.

# Big O Complexity
* Insertion and search operations in a binary search tree have a time complexity of O(h), where h is the height of the tree.
* In the worst case, the height of a balanced tree is log(n), while an unbalanced tree can have a height of n.
* The space complexity for a search in a binary search tree is O(1), as no additional space is allocated during the search.

