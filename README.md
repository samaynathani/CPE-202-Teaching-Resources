# 🐍 Data Structures (CPE 202) Resources, Advice, & Hints
A markdown sheet with stuff to help my students succeed in Data Structures! by [🦕samay nathani](https://github.com/samaynathani)  

## 👋 Office Hours
MTW, 8:30 pm - 9:30 pm PDT (Zoom link on Canvas)
  
## 📖 Textbook   
[Textbook](https://runestone.academy/runestone/books/published/pythonds/index.html) - this is super helpful! The textbook contains a lot of working code for labs. If you ever get stuck or forget how a data structure works, this is how to get back on track. Feel free to check your lab code against the book or use it for hints since labs are for learning.

## ❔ FAQS  
**Q:** *How are assignments graded/ how did I get this score?*  
**A:** We use unit-tests to check all functions for correct output. If you would like to see which tests failed or feedback from the test cases, please send me (the TA) an email with the name of the assignment and your Github ID.    

**Q:** *How do I get better scores on assignments?*  
**A:** When writing tests, make sure to test assignment REQUIREMENTS listed in the spec, and NOT just the code you have written (code coverage). Getting 100% coverage itself is not enough to guarantee an A on an assignment.  

**Q:** *How do I write better test cases?*  
**A:** Be sure to write tests for edge-cases (empty strings, empty arrays, None objects, negative numbers, zeros, repeated values in arrays, etc). Be sure to test different states of classes & data structures you implement (empty, full, contains items but not at capacity, exception handling, etc).      

**Q:** *How should I prepare for the miderm?*  
**A:** Be able to write any function from any lab, know all time complexities (worst, best, average), understand how to draw and step through different data structures, know postfix and prefix notation.    

**Q:** *I'm stuck on a problem, how should I proceed?*  
**A:** 1. Re-read the instructions  
2. Draw the data structure and manually walk through a few sample cases for the problem/ function  
3. convert the above logic to pseudo-code  
4. convert the pseudo-code to Python code  
5. Test and use the debugger if you  run into errors  
6. repeat steps 3-5 until your function works  
7. If you are still stuck, the textbook contains a lot of helpful tips, explanations, and sample code for functions. Good luck!  

## 😄 Topic Hints
### Recursion
1. Always have a base-case, recursive call, and way to bring each recursive call closer to the base-case
2. If you are missing any of those things, you might get stuck in an infinite loop
3. You can put the recursive portion of your code into a helper function to improve simplicity and handle invalid inputs/ edge cases in the caller-function  

### Stacks
1. For array-based implementations, think about the relationship between the number of items it contains and how to access the topmost element.
2. For linked-list implementations, adding and removing from the head is the same as the "top".
3. Time complexities - push / pop - O(1), size - O(1), pop all / push all - O(n).

### Queues
1. For array-based implementations, think about the relationship between the front, rear, and how you can use the capacity to wrap-around.
2. For linked-list implementations, think about the front and rear node lists as 2 stacks.  
3. **Important!** for linked-list implementations, dequeue must be O(1) in the AVERAGE case. Our worst case is O(n) (a loop is okay for the worst case).
4. Time complexities - push / pop - O(1), size - O(1), pop all / push all - O(n).

### Double-Linked List
1. The sentinel node marks both the front and end of the list. If the sentinal node points to itself, the list is empty. 
2. The sentinel node contains no (significant) value.
3. This list must be ordered. You can use the less-than (<) operator for comparing values. 
4. Time complexities - insert / remove / find / index - O(n), size - O(1).  

### Binary Search Trees
1. If the root of the tree is None (i.e. ```if self.root is None```), then the tree is empty.
2. Binary search trees are always organized by the keys stored in their nodes. All keys in child nodes of node.left are < node.key, and all keys in child nodes of node.right are > node.key
3. Recursion is usually the preferred method of traversing through a binary search tree. In some cases, loops may be more intuitive, so feel free to experiment with both. 
  * Helper functions are super useful for recursive implementations. Separate the base case (hint: #1) and the recursive steps into 2 separate functions. 
  * When using recursion, each node can be treated as a subtree. i.e. A node itself is a subtree, with node.left and node.right being separate subtrees.
4. In-order, pre-order, and post-order traversals have almost identical implementations. The only difference is where the node's data is appended to the list. 
5. Time complexities - insert / find / min / max - avg: O(log n) | worst: O(n), order traversals - O(n).  


If you have any questions, [📧email me!](mailto:snathani@calpoly.edu)
