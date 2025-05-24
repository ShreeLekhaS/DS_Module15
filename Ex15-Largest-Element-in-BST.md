# Ex 15(E) Largest Element in BST
## DATE: 26.03.2025
## AIM:
To Write a c program to find the largest value in a Binary Search Tree.

## Algorithm

1.Start the program.

2.Define a function largest() that takes a pointer to a binary tree node as input.

3.Inside the function, check if the current node has a right child.

4.If it does, recursively call the largest() function on the right child to keep moving right.

5.If the current node has no right child, return its value as it is the largest in the binary search tree.

6.End the program.



## Program:
```
/*
Program to find and display the priority of the operator in the given Postfix expression
Developed by: Shree Lekha.S
RegisterNumber: 212223110052 
*/

#include<stdio.h>
int largest(struct btnode *t)
{
   if (t->r != NULL)
   {
       t2 = t;
       return(largest(t->r));
   }
   else   
       return(t->value);
}
```

## Output:
![image](https://github.com/user-attachments/assets/d58b7b30-4d57-45ed-8c6f-05377c22ad90)


## Result:
Thus, the C program to find the largest value in a Binary Search Tree is implemented successfully.
