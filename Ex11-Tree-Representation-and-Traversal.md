# Ex11 Tree Representation and Traversal

## AIM:
To write a C function to perform post order traversal of a binary tree.

## Algorithm
1.Start
2.Define a function display_postorder() that takes a pointer to the root node of the tree.
3.Check if the current node (root_node) is not null.
4.Recursively call display_postorder() for the left child of the current node.
5.Recursively call display_postorder() for the right child of the current node.
6.After visiting both children, print the value of the current node.
7.End

## Program:
```
/*
Program to perform post order traversal of a binary tree.
Developed by: Kamali E
RegisterNumber:  212222110015
*/

/*
struct node
{
    int value;
    struct node *left_child, *right_child;
};
*/

void display_postorder(struct node *root_node)
{
    // write your code here
    if (!root_node)
    {
        return;
    }
    display_postorder(root_node->left_child);
    display_postorder(root_node->right_child);
    printf("%d\n", root_node->value);
}
```

## Output:

<img width="950" height="531" alt="image" src="https://github.com/user-attachments/assets/91fec81f-e3ff-4937-8593-46be20618660" />


## Result:
Thus, the function to perform post order traversal of a binary tree is implemented successfully
