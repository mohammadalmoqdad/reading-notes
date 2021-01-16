# Tree 

##### Important phrases:

* **Node** - A node is the individual item/data that makes up the data structure
* **Root** - The root is the first/top Node in the tree
* **Left Child** - The node that is positioned to the left of a root or node
* **Right Child** - The node that is positioned to the right of a root or node
* **Edge** - The edge in a tree is the link between a parent and child node
* **Leaf** - A leaf is a node that does not contain any children
* **Height** - The height of a tree is determined by the number of edges from the root to the bottommost node


- **In Depth First  Search** :
* We are going through the nodes until reaching the last node then their is tree methodolgies to go through:
  1. Pre-order: `root >> left >> right`
  2. In-order: `left >> root >> right`
  3. Post-order: `left >> right >> root`

* The biggest difference between each of the traversals is when you are looking at the root node.


- In the **Breadth First** :
* We are going through each level of the nodess strting from the root until the bottommost one and stsring from the lesf to the right nodes

* Depth First is an application of the *Stack* While the Breadth While the Breadth First is an application of the *Queue* 

* we  asume that the trees that we are dealling with here are *Binary Trees*
 

 ### Binary Search Trees :
* A **Binary Search Tree (BST)** is a type of tree that does have some structure attached to it. In a BST, nodes are organized in a manner where all values that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right

* Searching a BST can be done quickly, because all you do is compare the node you are searching for against the root of the tree or sub-tree. If the value is smaller, you only traverse the left side. If the value is larger, you only traverse the right side.

#### **The best way to approach a BST search is with a while loop.** 

* he Big O time complexity of a Binary Search Tree’s insertion and search operations is O(h), or O(height).


