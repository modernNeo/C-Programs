# C++ Programs  
  
## Assignment Details  
  
#### Binary Search Trees
 
``` 
Design and implement an Abstract Data Type Polynomial that provides the following functionality:
 creates a polynomial
 takes a term and adds it to the polynomial (includes it into the polynomial)
 destroys a polynomial
 creates a zero polynomial
 determines if the polynomial is zero
 prints the polynomial
 evaluates the polynomial for a value for x (given that the polynomial is in x)
 gives the degree of the polynomial (the degree of a polynomial is the power of
the term with the highest degree)
 returns the coefficient of a term in the polynomial given a degree (an exponent)
 returns the sum of the polynomial plus another polynomial
About your implementation
 use a binary search tree: store the terms by degree in descending order
 store both the coefficient and the degree (exponent) of the term in the node of
the tree
 overload the + operator
 overload << for printing and >> for reading
 provide a copy constructor, destructor and overload the assignment operator for
the polynomial
 free up memory that is no longer needed
 you should not have any terms that have zero as the coefficient (thus you need
to decide on a representation for the zero polynomial)
 you should only store once (in a node) a term of degree k (i.e. you should not
have two nodes for two terms both of degree k)
 you should be able to delete any node from the tree when needed (you will need
this functionality when adding terms)
 You can make Term an Abstract Data Type as well.
 Do not use the STL.

```   
  
### Numbrix
 
``` 
The purpose of this assignment is to learn about backtracking and to have some fun playing...
For your assignment1 you are to write a program to solve the game Numbrix® created by Marilyn Vos Savant2 of the Parade Magazine. It is similar to Hidato except that in Numbrix® the moves are either horizontal or vertical, whereas Hidato allows for diagonal moves.

About the implementation
Read the data from a file and output to a file the grid with the answer. Your program should produce all the possible solutions (each solution to be written out to a different file). Below you are given the input file format as well as the output file format (and yes, we want to be able to test your program automatically).
You could ‘pretty print’ the solution to the puzzle on the console as well, i.e. you need to print the solution as a grid of numbers onto a file but you may also display onto the console the solution too. Please follow the instructions given as to how the numbers are to be printed onto the output file.
Your program should be able to handle not having the number 1 as one of the initial numbers on the grid. The grid can start with any number which is less than or equal to n × n.
You don’t need to implement a class. But, I suggest that if you have many functions, that you prevent polluting the global space by putting your functions into a C++ namespace.

```   
  
#### Polynomial Addition and Differentiation

``` 
In this assignment, you are to implement a C++ class to sort a bivariate polynomial1, to add two bivariate polynomials, and to differentiate the bivariate polynomial with respect to each of the variables.
You are required to implement the polynomial using a linked list of pointers to terms. Suppose that the variables of your polynomial are x and y.
• read a term and add it to the polynomial: you need to read the coefficient, the degree (exponent) of x and the degree of y.
For simplicity, assume that all three numbers are entered, e.g. if the numbers are 3 2 1 then you should build the term 3 ∙ 𝑥! ∙ 𝑦!
• sort the terms of the polynomial first on the degree in x and if two terms have equal degree in x, then sort on the degree in y.
Use merge sort. Do not allocate any more memory in the merge. Do not call the merge sort from the STL.
• print the polynomial
You might want to implement printing by overloading the operator <<
add two polynomials a and b. Use merging. You may overload the + operator if you wish. You should produce a new polynomial c which is the sum of the polynomial a and the polynomial b. The sum c should not have any terms with zero coefficients.
• differentiate the polynomial with respect to x
• differentiate the polynomial with respect to y
Pass the comparison function that is to be used in merge sort as a function object or functor. This will give your polynomial class the flexibility of sorting in ascending or descending order.

```   
  
#### SkipLists
 
``` 
Implement an ADT list using a skip list, specifically, using exactly two linked lists.
Do some “timings” to see what the cost of a search is, more precisely, compute the number of comparisons done for various searches and see how they compare with respect to     𝑛 where n
is the total number of elements (as discussed in class)? How many comparisons are done on average when searching? What is the worst case?

About the implementation
Use a two level list i.e. use two linked lists. Use templates for the C++ class. You can make the linked lists doubly linked but it suffices to make the linked lists ‘singly linked’.
You do not need to implement insert so that the structure of the skip list is correct at all times. The probabilitstic algorithm, presented in class, for inserting into a skip list of height log2n was indeed cool. However, it’s too much to ask of you in this assignment. So, you can assume that all the insertions are done first, and then, subsequently, the proper skip list is built. You may assume that no more insertions are done afterwards but only queries of searching. You do not need to implement deletions.
Do implement the ‘destructor’, ‘copy constructor’, and ‘overloaded assignment operator’ for your C++ class. However, you don’t need to worry about the ‘move constructor’ nor the ‘move assignment operator’.

``` 
