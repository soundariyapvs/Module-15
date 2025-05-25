# Ex. No: 15C - Expression Tree with Inorder and Postorder Traversal

## AIM:
To write a Python program to build the given expression tree and print the inorder and postorder traversals.

---

## ALGORITHM:

1. **Start the program.**
2. Import the required modules (`build` and `Node` from `binarytree`).
3. Define a list `x` representing the expression tree in pre-order fashion (with `None` for missing nodes).
4. Use the `build()` function to generate the binary tree.
5. Print the **inorder** and **postorder** traversal of the tree.
6. **End the program.**

---

## PROGRAM:

```
from binarytree import build
x=['*',4,'-',5,'+',2,7]
bt=build(x)
print(bt.inorder)
print(bt.postorder)
```

## OUTPUT
![Screenshot 2025-05-19 123131](https://github.com/user-attachments/assets/dcdfb89c-8590-43d7-8ca3-e08088df446c)

## RESULT
Thus a Python program to build the given expression tree and print the inorder and postorder traversals has been successfully implemented.

