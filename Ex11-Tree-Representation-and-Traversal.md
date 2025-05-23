# Ex11 Tree Representation and Traversal
## DATE:
## AIM:
To write a C function to perform post order traversal of a binary tree.

## Algorithm
1. 
2. 
3. 
4.  
5.   

## Program:
```
/*
Program to perform post order traversal of a binary tree.
Developed by: Shree Lekha.S
RegisterNumber: 212223110052
*/

struct node
{
int value;
struct node*left_child, *right_child;
};*/
void display_postorder(struct node*root_node){ if(root_node)
{
display_postorder(root_node->left_child); display_postorder(root_node->right_child); printf("%d\n",root_node->value);
}
}


*/
```

## Output:
![image](https://github.com/user-attachments/assets/5795cabb-9ad4-48ad-a118-e9951ddb8fd7)



## Result:
Thus, the function to perform post order traversal of a binary tree is implemented successfully
