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

1. Linked List - Cycle Detection (Floyd’s Algorithm)  
Uses Floyd’s Cycle-Finding Algorithm to detect cycles in a linked list.  
Algorithm:  
- Use two pointers (slow and fast).  
- Move slow one step, fast two steps.  
- If they meet, a cycle exists.  
- If fast reaches null, no cycle is present.  

File: LinkedListDemo.java, Node.java

2. Stack - Balanced Parentheses (LIFO)  
Uses Stack Data Structure to check if parentheses are balanced.  
Algorithm:  
- Push opening brackets onto the stack.  
- When encountering a closing bracket, check if it matches the top.  
- If the stack is empty at the end, the string is balanced.  

File: StackDemo.java  

3. Queue - FIFO Implementation  
First-In-First-Out (FIFO) approach using Java’s Queue interface.  
Operations Implemented:  
- enqueue() → Adds element to the queue.  
- dequeue() → Removes from the front.  
- peek() → Returns front element.  

File: QueueDemo.java  

4. Heap - Min & Max Heap  
Uses Priority Queue (Min-Heap) and Max-Heap implementation.  
Algorithm:  
- Insert elements while maintaining heap property.  
- Extract min/max efficiently in O(log n) time.  

File: HeapDemo.java  

5. Graph - BFS & DFS Traversal  
Graph Representation: Uses Adjacency List  
Algorithm:  
- BFS (Breadth-First Search): Uses Queue (FIFO)  
- DFS (Depth-First Search): Uses Stack (LIFO or Recursion)  

File: GraphDemo.java  

6. Trees - Binary Search Tree (Operations)
Implements Insertion, Deletion, and Traversal for BST.  
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
