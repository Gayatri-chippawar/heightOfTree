# 🌳 Height of a Binary Tree (Java)

## 📌 Overview

This project demonstrates how to calculate the **height of a Binary Tree** using **recursion in Java**.

The height of a binary tree is the **number of levels (or the longest path from the root node to a leaf node)**.

This concept is widely used in **tree-based algorithms, AVL trees, heaps, and many coding interview problems**.

---

# 🌿 Binary Tree Example

The tree used in this program:

```
        1
       / \
      2   3
     / \  / \
    4  5 6   7
```

---

# 📏 Height of the Tree

The **height of a tree** is defined as:

```
Height = max(height(left subtree), height(right subtree)) + 1
```

For the above tree:

```
Height = 3
```

Because the longest path is:

```
1 → 2 → 4
```

or

```
1 → 3 → 7
```

---

# ⚙️ Algorithm

The program calculates the height using **recursion**.

### Steps:

1️⃣ If the root is `null`, return `0`
2️⃣ Recursively calculate height of the **left subtree**
3️⃣ Recursively calculate height of the **right subtree**
4️⃣ Return the **maximum height + 1**

---

# 💻 Java Implementation

```java
public static int height(Node root){
    if(root == null){
        return 0;
    }

    int Lh = height(root.left);
    int Rh = height(root.right);

    return Math.max(Lh,Rh) + 1;
}
```

---

# ▶️ Program Output

```
3
```

---

# ⏱ Time and Space Complexity

| Complexity       | Value                  |
| ---------------- | ---------------------- |
| Time Complexity  | O(n)                   |
| Space Complexity | O(h) (recursion stack) |

Where:

* **n** = number of nodes
* **h** = height of the tree

---

# 🧠 Concepts Used

* 🌳 Binary Trees
* 🔁 Recursion
* 📏 Tree Height Calculation
* ⚡ Divide and Conquer

---

# 🎯 Learning Outcome

After completing this program you will understand:

✔ How binary trees are structured
✔ How recursion works with trees
✔ How to calculate tree height efficiently
✔ Basic tree algorithm design

These concepts are important for **DSA interviews and competitive programming**.

---

