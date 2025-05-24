# Ex 3(D) Heap Tree
## DATE:
## AIM:
To write a C function to delete an element in a Heap Tree.

## Algorithm

1.Start the function deleteRoot with the array and the number to delete.

2.Loop through the array to find the index of the element equal to num.

3.Swap the found element with the last element in the heap.

4.Decrease the heap size by 1 to remove the last element.

5.Call heapify from the middle of the heap down to the root to restore the heap property.

6.End the function after rebalancing the heap.
## Program:
```
/*
Program to delete an element in a Heap Tree
Developed by: Shree Lekha.S
RegisterNumber: 212223110052
*/

voiddeleteRoot(int array[], int num)
{
int i; for(i=0;i<size;i++)
{
if(num==array[i])
{
break;
}
}
swap(&array[i],&array[size-1]); size-=1;
for(i=size/2-1;i>=0;i--)
{
heapify(array,size,i);
}
}  
```

## Output:
![image](https://github.com/user-attachments/assets/a182fab9-8ebd-4b1b-b77f-a85a2d34eac3)


## Result:
Thus, the function to delete an element in a Heap Tree is implemented successfully.
