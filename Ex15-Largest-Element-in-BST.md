# Ex 15(E) Largest Element in BST
## DATE:
## AIM:
To Write a c program to find the largest value in a Binary Search Tree.

## Algorithm

1.Start the program and define a node structure with data and pointers to left and right children.

2.Create a function createnode to allocate memory, initialize the node with a key, and set children to NULL.

3.Build the binary search tree by creating nodes and linking them to form the correct structure.

4.Define an inorder function to recursively traverse the tree in-order and print each node’s value.

5.Define a largest function to find and print the maximum value by moving to the rightmost node.

6.In main, construct the tree, call inorder to display nodes, then call largest to show the largest element, and finally end the program.


## Program:
```
/*
Program to find and display the priority of the operator in the given Postfix expression
Developed by: Shree Lekha.S
RegisterNumber: 212223110052 
*/

#include <stdio.h>
#include <stdlib.h>
struct node
{
int info;
struct node *left, *right;
};
struct node *createnode(int key)
{
struct node*newnode = (struct node*)malloc(sizeof(struct node));
newnode->info = key;
newnode->left = NULL;
newnode->right = NULL;
return(newnode);
}
void inorder(struct node *root)
{
if(root != NULL)
{
inorder(root->left);
 printf(" %d ",root->info);
inorder(root->right);
}
}
void largest(struct node *root)
{
while (root != NULL && root->right != NULL)
{
root = root->right;
}
printf("\nLargest value is %d", root->info);
}
 
int main()
{
/* Creating first Tree. */
struct node *newnode = createnode(25);
 newnode->left = createnode(17);
 newnode->right = createnode(35);
newnode->left->left = createnode(13);
 newnode->left->right = createnode(19);
 newnode->right->left = createnode(27);
 newnode->right->right =createnode(55);

printf("Inorder traversal of tree 1 :");
inorder(newnode);
largest(newnode);
return 0;
}
```

## Output:
![image](https://github.com/user-attachments/assets/a5553ce6-a3b0-4198-be77-881580206f21)


## Result:
Thus, the C program to find the largest value in a Binary Search Tree is implemented successfully.
