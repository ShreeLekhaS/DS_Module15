# Ex 15(C) Expression Tree
## DATE:
## AIM:
To write a C function to construct an Expression Tree for the given Postfix Expression and display the output in the format of In-order ,Pre-order and Post-order traversal.

## Algorithm

1.Start the program.

2.Define the preOrder function to visit and print the current node, then recursively traverse the left and right subtrees.

3.Define the inOrder function to recursively traverse the left subtree, print the current node, then traverse the right subtree.

4.Define the postOrder function to recursively traverse the left and right subtrees, then print the current node.

5.In each function, check if the current node is not NULL before processing.

6.End the program after traversals.

 

## Program:
```
/*
Program to construct an Expression Tree for the given Postfix Expression and display the output in the format of In-order ,Pre-order and Post-order traversal.
Developed by: Shree Lekha.S
RegisterNumber: 212223110052
*/

struct n {
char d;
struct n*l;
struct n*r;
};*/
void preOrder(struct n*tree)
{
if(tree)
{
printf("%c",tree->d);
preOrder(tree->l);
preOrder(tree->r);
}
}
void inOrder(struct n*tree)
{
if(tree)
{
inOrder(tree->l);
printf("%c",tree->d);
inOrder(tree->r);
}
}
void postOrder(struct n*tree)
{
if(tree)
{
postOrder(tree->l);
postOrder(tree->r);
printf("%c",tree->d);
}
}

```

## Output:
![image](https://github.com/user-attachments/assets/9dcb2a9e-a45d-432d-9d59-ca1c977d6b59)


## Result:
Thus, the C program to display the Expression Tree in the format of In-order ,Pre-order and Post-order traversal.
