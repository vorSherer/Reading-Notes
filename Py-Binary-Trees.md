# Read 15 - Binary Trees and Binary Search Trees

#### 2020-07-24

## RESOURCES:
## Trees <br>
https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html <br>
<br>

### Binary Trees and Binary Search Trees <br>
High level explanation of the mechanics of Binary Trees and Binary Search Trees - what they are, how - generally - to traverse them, and which methodology and data structure to use to do so. <br>
#### Binary Trees - 
### Common Terminology:
- __Node__ - A node is the individual item/data that makes up the data structure
- __Root__ - The root is the first/top Node in the tree
- __Left Child__ - The node that is positioned to the left of a root or node
- __Right Child__ - The node that is positioned to the right of a root or node
- __Edge__ - The edge in a tree is the link between a parent and child node
- __Leaf__ - A leaf is a node that does not contain any children
- __Height__ - The height of a tree is determined by the number of edges from the root to the bottommost node <br>
### Traversal Methods
__Depth first__ traversal is where we prioritize going through the depth (height) of the tree first.
- *__Pre-order__: root >> left >> right* <br>
- *__In-order__: left >> root >> right* <br>
- *__Post-order__: left >> right >> root* <br>
These methods use a __Call Stack__ and __recursion__. <br>

__Breadth first__ traversal iterates through the tree by going through each level of the tree node-by-node.  Traditionally, breadth first traversal uses a __queue__ (instead of the call stack via recursion) to traverse the width/breadth of the tree. <br>
#### Adding a node
Because there are no structural rules for where nodes are "supposed to go" in a binary tree, it really doesn't matter where a new node gets placed. <br>
The __Big O time complexity for inserting a new node__ is __`O(n)`__. __Searching__ for a specific node will also be __`O(n)`__. Because of the lack of organizational structure in a Binary Tree, the worst case for most operations will involve traversing the entire tree. If we assume that a tree has __`n`__ nodes, then in the worst case we will have to look at __`n`__ items, hence the `O(n)` complexity. <br>
The __Big O space complexity for a node insertion using breadth first__ insertion will be __`O(w)`__, where __`w`__ is the largest width of the tree. <br>
#### Binary Search Trees -
In a __Binary Search Tree (BST)__, nodes are organized in a manner where all values that are *smaller than the root* are placed to the __*left*__, and all values that are *larger than the root* are placed to the __*right*__. <br>
The best way to approach a __BST__ search is with a __`while`__ loop. We cycle through the `while` loop until we hit a __leaf__, or until we reach a __match__ with what we’re searching for. <br>
The __Big O time complexity__ of a Binary Search Tree’s __*insertion*__ and __*search*__ operations is __`O(h)`__, or `O(height)`. In the worst case, we will have to search all the way down to a __leaf__, which will require searching through as many nodes as the tree is tall. In a __*balanced*__ (or "perfect") tree, the height of the tree is __`log(n)`__. In an __*unbalanced*__ tree, the worst case height of the tree is __`n`__. <br>
The __Big O space complexity__ of a BST __*search*__ would be __`O(1)`__. During a search, we are not allocating any additional space. <br>
