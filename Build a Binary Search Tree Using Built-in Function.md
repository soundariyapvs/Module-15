# Ex. No: 15B - Build a Binary Search Tree Using Built-in Function

## AIM:
To write a Python program to build a binary search tree using a built-in function.

---

## ALGORITHM:

1. **Start the program.**
2. Define `_build_bst_from_sorted_values(sorted_values)` to recursively build a binary search tree (BST) from a sorted list.
3. Define `left_subtree(l)` to print the left subtree of the BST.
4. Take user input for the number of elements and store the values in a list `a`.
5. Sort the list and pass it to `_build_bst_from_sorted_values()` to construct the BST.
6. Print the postorder traversal of the BST.
7. Call `left_subtree(l)` to print the left subtree.
8. Check whether the tree is a binary search tree using the `is_bst` property.
9. **End the program.**

---

## PROGRAM:

```
from binarytree import Node

def _build_bst_from_sorted_values(sorted_values):
    if len(sorted_values)==0:
        return None
    mid_index=len(sorted_values)//2
    root=Node(sorted_values[mid_index])
    root.left=_build_bst_from_sorted_values(sorted_values[:mid_index])
    root.right=_build_bst_from_sorted_values(sorted_values[mid_index+1:])
    return (root)
    
def subtree(l):
    print("Left Subtree :")
    for i in l[1].values:
        print(i,'-->',end='')
    return
        

a=[]
s=int(input())
for i in range(s):
    val=int(input())
    a.append(val)
x=sorted(a)
t=_build_bst_from_sorted_values(x)
print("Postorder :",t.postorder)
subtree(t)
print("\nIs this a Binary Search Tree? ",t.is_bst)
```

## OUTPUT
![Screenshot 2025-05-19 121146](https://github.com/user-attachments/assets/b10bbbf1-0bf0-4531-b75f-66a86e5bd121)
![Screenshot 2025-05-19 121152](https://github.com/user-attachments/assets/3e626d95-0469-4c26-a000-1e16bfe9a8d2)


## RESULT
Thus a Python program to build a binary search tree using a built-in function  has been successfully implemented.

