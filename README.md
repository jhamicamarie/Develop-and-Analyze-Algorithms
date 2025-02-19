Java Data Structures & Algorithms  

Overview  
This project contains Java implementations of fundamental data structures and algorithms, including:  
- Linked List (Floyd's Cycle Detection)  
- Queue (FIFO Implementation)  
- Stack (Balanced Parentheses)  
- Heap (Min/Max Heap Implementation)  
- Graph (Breadth-First & Depth-First Search)  
- Tree (Binary Search Tree Operations)  



How to Run the Code
Prerequisites  
Make sure you have Java installed. You can check by running:  
java -version  

Steps to Compile and Run  
1. Clone the repository  
git clone https://github.com/jhamicamarie/Develop-and-Analyze-Algorithms.git
cd Develop-and-Analyze-Algorithms  

2. Compile a Java file  
Example: Running the LinkedList implementation:  
javac LinkedListDemo.java  
java LinkedListDemo  



Algorithms Implemented  

1. Linked List

A Linked List is a data structure where elements (nodes) are connected using pointers. Each node contains:

Data (the value stored).
Pointer (Next) to the next node in the list.

Example Algorithm: Floyd’s Cycle Detection Algorithm (Tortoise and Hare)
This algorithm detects if a cycle exists in a linked list using two pointers.
 
Algorithm:  
- Use two pointers (slow and fast).  
- Move slow one step, fast two steps.  
- If they meet, a cycle exists.  
- If fast reaches null, no cycle is present.  

File: LinkedListDemo.java, Node.java

2. Stack

A Stack follows LIFO (Last-In-First-Out), meaning elements are added and removed from the top.

Example Algorithm: Balanced Parentheses Check
A stack can be used to check if parentheses in an expression are balanced (( ) { } [ ]).

Algorithm:  
- Push opening brackets onto the stack.  
- When encountering a closing bracket, check if it matches the top.  
- If the stack is empty at the end, the string is balanced.  

File: StackDemo.java  

3. Queue

A Queue follows FIFO (First-In-First-Out), meaning elements are added to the back and removed from the front.

Example Algorithm: Breadth-First Search (BFS)
BFS is used in graphs and trees to traverse level by level. It uses a queue to process nodes.

Operations Implemented:  
- enqueue() → Adds element to the queue.  
- dequeue() → Removes from the front.  
- peek() → Returns front element.  

File: QueueDemo.java  

4. Heap

A Heap is a complete binary tree where:
  A Min-Heap ensures that the smallest element is always at the root.
  A Max-Heap ensures that the largest element is always at the root.

Example Algorithm: Find K Smallest Elements

Algorithm:  
- Insert elements while maintaining heap property.  
- Extract min/max efficiently in O(log n) time.  

File: HeapDemo.java  

5. Graph

A graph is a data structure that consists of nodes (vertices) connected by edges.

Example Algorithm: Depth-First Search (DFS)
DFS explores as deep as possible before backtracking.
 
Algorithm:  
- BFS (Breadth-First Search): Uses Queue (FIFO)  
- DFS (Depth-First Search): Uses Stack (LIFO or Recursion)  

File: GraphDemo.java  

6. Trees

A Tree is a hierarchical data structure where:
  The root is the topmost node.
  Each node has zero or more child nodes.
  A Binary Tree has at most two children per node.
  A Binary Search Tree (BST) follows the rule:
  Left subtree contains values smaller than the parent.
  Right subtree contains values greater than the parent.

Example Algorithm: Finding the Lowest Common Ancestor (LCA) in a BST
The Lowest Common Ancestor (LCA) of two nodes in a BST is the deepest node that is an ancestor of both nodes.

Algorithm:  
- Insert values recursively.  
- Search efficiently in O(log n).  
- Perform Inorder, Preorder, and Postorder Traversal.  

File: TreesDemo.java, TreeNode.java



Example Usage  
To check if a string has balanced parentheses, run:  
java StackDemo "{[()]}"  
Expected Output:  
true  



License  
This project is open-source under the MIT License.
