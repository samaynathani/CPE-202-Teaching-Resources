# CPE-202-Guide-to-Success
A markdown sheet with tips, tricks, and resources to succeed in Data Structures by [Samay Nathani](https://github.com/samaynathani)  
  
[Textbook](https://runestone.academy/runestone/books/published/pythonds/index.html) - this is super helpful! The textbook contains a lot of actual code for labs. If you ever get stuck/ forget how a data structure works, this is how to get back on track. Feel free to check your lab code against the book or use it for hints since labs are meant more for learning.  

## FAQS:  
**Q:** *How are assignments graded/ how did I get this score?*  
**A:** We use unit-tests to check all functions for correct output. If you would like to see which tests failed or feedback from the test cases, please send me (the TA) an email with the name of the assignment and your Github ID.    

**Q:** *How do I get better scores on assignments?*  
**A:** Make sure that your programs return the correct outputs every time. Be sure to write tests for edge-cases (empty strings, empty arrays, None objects, negative numbers, zeros, repeated values, ect)    

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

## Topic Hints:
### Recursion
1. Always have a base-case, recursive call, and way to bring each recursive call closer to the base-case
2. If you are missing any of those things, you might get stuck in an infinite loop
3. You can put the recursive portion of your code into a helper function to improve simplicity and handle invalid inputs/ edge cases in the caller-function  

### Stacks:
1. For array-based implementations, think about the relationship between the number of items it contains and how to access the topmost element.
2. For linked-list implementations, adding and removing from the head is the same as the "top".
3. Time complexities - push/ pop - O(1), size - O(1), pop all/ push all - O(n).


If you have any questions, [email me!](mailto:snathani@calpoly.edu)
