# Ex17 AVL Tree – Rotation
## DATE: 01/05/2025
## AIM:
To write a C function to perform right rotation in an AVL Tree.

## Algorithm
1.Start

2.Set y to the left child of x.

3.Set the left child of x to be the right child of y.

4.Set the right child of y to be x.

5.Update the height of x and y.

6.Return y as the new root after rotation.

7.End  

## Program:
```
/*
Program to perform right rotation in AVL Tree
Developed by: PRADEEP V
RegisterNumber: 212223240119
*/
typedef struct node 
{ 
int data; 
struct node *left,*right; 
int ht; 
}node; 
node *insert(node *,int); 
//node *Delete(node *,int); 
void preorder(node *); 
//void inorder(node *); 
int height( node *); 
node *rotateright(node *); 
node *rotateleft(node *); 
node *RR(node *); 
node *LL(node *); 
node *LR(node *); 
node *RL(node *); 
*/ 
node * rotateright(node *x) 
{ 
node *y; 
y=x->left; 
x->left=y->right; 
y->right=x; 
  
  
x->ht=height(x); 
y->ht=height(y); 
return(y); 
}

```

## Output:

![437471539-41f3635a-e8fa-4a9b-8e4b-dd45c55afc27](https://github.com/user-attachments/assets/a1056e28-dd91-4ab0-8586-654668adc4f8)


## Result:
Thus, the function to perform right rotation in an AVL Tree is implemented successfully.
