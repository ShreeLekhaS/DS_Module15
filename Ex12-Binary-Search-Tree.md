# Ex12 Binary Search Tree
## DATE:
## AIM:
To write a C function to insert the elements in the binary search tree

## Algorithm

1.Start the program.

2.Define the insert function that takes a pointer to a node and a key to insert.

3.If the current node is NULL, create a new node, assign the key, set left and right children to NULL, and return the new node.

4.Otherwise, compare the key with the current node’s key.

5.If the key is less than or equal to the current node’s key, recursively insert it into the left subtree.

6.Else, recursively insert it into the right subtree, then return the current node.  

## Program:
```
/*
Program to insert the elements in the binary search tree
Developed by: Shree Lekha.S
RegisterNumber: 212223110052
*/

struct node { 
int key; 
struct node *left, *right; 
};*/ 
struct node* insert(struct node* node, int key) 
{ 
if(node==NULL) 
{ 
struct node* node=(struct node*)malloc(sizeof(struct node)); 
node->key=key; 
node->left=NULL; 
node->right=NULL; 
return node; 
} 
else 
{ 
struct node* cur; 
if(key<=node->key) 
{ 
cur=insert(node->left,key); 
node->left=cur; 
} 
  
else 
{ 
cur=insert(node->right,key); 
node->right=cur; 
} 
return node; 
} 
 
} 
```

## Output:
![image](https://github.com/user-attachments/assets/a959cccb-79cd-4c3b-a248-c7f5854d4ff2)


## Result:
Thus, the C function to insert the elements in the binary search tree is implemented successfully.
