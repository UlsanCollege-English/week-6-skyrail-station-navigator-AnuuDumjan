[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/mHMwxQwH)
# Weekly Coding #5: Skyrail Station Navigator

## Summary
Write 3–6 lines here.
This program works with a binary tree and a binary search tree (BST).
It implements tree traversals such as preorder, inorder, and postorder.
It also implements BST operations like searching for a value and inserting a value.

Example questions to answer:
- What does your program do?
- What tree tasks did you implement?
- What BST tasks did you implement?

---

## Approach
- Describe how you handled preorder traversal.
I visited the root first, then left subtree, then right subtree using recursion.
- Describe how you handled inorder traversal.
I visited left subtree, then root, then right subtree using recursion.
- Describe how you handled postorder traversal.
I visited left subtree, then right subtree, then root using recursion.
- Describe how you handled BST search.
I compared the target with the root and moved left or right recursively.
- Describe how you handled BST insert.
I inserted the value in the correct position based on BST rules and ignored duplicates.

---

## Complexity

### `preorder_values`
- **Time:**O(n)
- **Space:**O(n)
- **Why:**It visits every node once.

### `inorder_values`
- **Time:**O(n)
- **Space:**O(n)
- **Why:**It visits all nodes in the tree.

### `postorder_values`
- **Time:**O(n)
- **Space:**O(n)
- **Why:**Every node is visited once.

### `bst_contains`
- **Time:**O(n)
- **Space:**O(n)
- **Why:**It follows one path from root to leaf (height of tree).

### `bst_insert`
- **Time:**O(n)
- **Space:**O(n)
- **Why:** It inserts along one path in the tree.


---

## Edge-Case Checklist
- [x] Empty tree traversal returns `[]`
- [x] Single-node traversal works correctly
- [x] `bst_contains` returns `False` for an empty tree
- [x] `bst_contains` returns `False` when the target is missing
- [x] `bst_insert` creates a root when the tree is empty
- [x] `bst_insert` ignores duplicate values
- [x] I tested at least one deeper insert case

Add short notes here explaining what your code does for each case.

---

## Assistance & Sources
- **AI used? (Y/N):**Y
- **What AI helped with:**Understanding traversal and BST logic
- **Other sources used:**Class notes

---

## Test Results
Paste or summarize your `pytest -q` result here.
pytest -q