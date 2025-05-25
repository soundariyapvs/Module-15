# Ex. No: 15A - Build a Binary Tree with INTEGER Values

## AIM:
To write a Python program to build a binary tree with a root, left, and right node using integer-point values.

---

## ALGORITHM:

1. **Start the program.**
2. **Import** the `Node` class from the `binarytree` module.
3. **Create a root node** using the `Node` class and assign a integer-point value.
4. **Create left and right child nodes** for the root with int values.
5. **Convert the tree** to a list and print the list of nodes.
6. **End the program.**

---

## PYTHON PROGRAM

```
from binarytree import Node
l=[]
for i in range(3):
    a=input()
    l.append(a)
root=Node(l[0])
root.left=Node(l[1])
root.right=Node(l[2])
print("List of nodes :",list(root))
```

## OUTPUT
![Screenshot 2025-05-19 121958](https://github.com/user-attachments/assets/1c0662ca-7f1c-45c7-ac69-552f8057bf1e)

## RESULT
Thus a Python program to build a binary tree with a root, left, and right node using integer-point values.
