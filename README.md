Download Link: https://assignmentchef.com/product/solved-coen171-homework-3-functional-programming
<br>
In this assignment, you will write programs in ML and Scheme Use the Linux machines in the Engineering Computing Center for this project. The ML interpreter is sml (use setup smlnj) and the Scheme interpreter is guile.

<h1>1        Quicksort</h1>

Under /scratch/coen171/homework3, you will find an implementation in ML of <strong><em>quicksort</em></strong>, the sorting algorithm used previously. Translate the program to Scheme, keeping the same function names and parameters. Call this program sort.scm.

<strong>Goal:                   </strong>To introduce functional programming in strongly-typed and dynamically-typed languages.

<strong>Hints:                   </strong>You will need to use let* in Scheme to achieve the same effect as let in ML.

<h1>2        BinarySearchTrees</h1>

As in the first assignment, a <strong><em>binarysearchtree </em></strong>is either empty, or it consists of a node with two binary search trees as subtrees. Each node holds an integer. The elements in a binary search tree are arranged so that smaller elements appear in the left subtree of a node and larger elements appear in the right subtree. In <strong><em>both </em></strong>ML and Scheme, write a program to implement binary search trees. Call your programs tree.sml and tree.scm, respectively. Each program should have at least the following two functions:

<ul>

 <li>insert: given a binary search tree and an integer, inserts the integer into the tree, and returns the new tree; if the integer has already been inserted, then the tree is unchanged and the tree itself is returned</li>

 <li>member: given a binary search tree and an integer, returns true if the integer is found in the tree, and returns false otherwise (in Scheme, call this function member? to avoid clashing with the built-in function of the same name)</li>

</ul>

In this assignment, you <strong><em>maynot </em></strong>use assignment or iteration (i.e., any Scheme function whose name ends in an exclamation point such as set! or the ML assignment operator). Consequently, the insert function must return a tree. For the Scheme program, you will have to use lists to represent the tree, as Scheme does not support userdefined datatypes. However, since ML does support user-defined datatypes, you should define your own datatype to represent the tree.

<strong>Goal:                 </strong>To represent structures in languages with structured types and without structured types.

<strong>Hints: </strong>For the Scheme program, I found it easiest to represent a node as a list with three elements: the data, the left subtree, and the right subtree. Both the left and right subtrees would themselves be lists with three elements. The empty list is used to represent an empty subtree.