# DSA — DEMO PAPERS (3 papers, exam format: 50 marks · 2 hrs)

Format cloned from RAI MJ-2025 (316U43C303): Q1 any-two ×5 · Q2 any-one ×10 (with a/b/c sub-parts) · Q3 any-one ×10 · Q4/Q5 mixed sub-parts.

---

# =================== DEMO PAPER 1 ===================

**Q1. Attempt any two:** *(2×5=10)*
(i) What is a pointer in C? Write a C function `swap(int *a, int *b)` and show a sample call.
(ii) What is recursion? Write a recursive C function for factorial; state how the stack supports it.
(iii) Define ADT. Explain how the Stack ADT can be implemented using both an array and a linked list.

**Q2. Attempt any one:** *(10)*
(i) a) Differentiate singly vs doubly linked list. (2)
   b) Time complexity of insertion at beginning vs end of SLL. (2)
   c) Write steps + C code for inserting a node at the beginning and at the end of an SLL. (6)
(ii) a) What is a circular queue? Explain the drawback of a linear queue that it solves. (4)
   b) Write C code for enqueue/dequeue in a circular queue (array-based). (6)

**Q3. Attempt any one:** *(10)*
(i) a) Binary tree vs BST. (2)
   b) Construct a BST: 45, 25, 65, 15, 35, 55, 75, 30. Show the tree; write its inorder traversal. (5)
   c) Applications of BST. (2)
   d) Delete a leaf node and a node with two children from a BST — explain with example. (3)... (adjust: marks to fit 10)
(ii) a) What is a graph? Adjacency matrix vs adjacency list — when is each preferred? (4)
   b) Explain DFS on a graph of 6 vertices with diagram; write its algorithm. (6)

**Q4. Attempt the following:** *(5+5=10)*
(a) Write the algorithm for **infix → postfix conversion** using a stack. Convert: `(a + b * c) / (d − e)` showing every stack step.
(b) Evaluate the postfix expression `6 2 3 + − 3 8 2 / + *` using a stack; show stack states.

**Q5. Attempt any two:** *(2×5=10)*
(i) Linear search vs binary search — algorithm + C function for binary search; compare time & space complexity.
(ii) Sort {38, 12, 45, 7, 29} by **bubble sort** — show every pass.
(iii) Explain Big-O, Big-Θ, Big-Ω with an example of each; how do they bound a function?

---KEY (Demo 1)---
Q3(i)(b): inorder = 15 25 30 35 45 55 65 75 (sorted — always check).
Q4(a): postfix = a b c * + d e − /.
Q4(b): [6] → [6,2] → [6,2,3] → '+' → [6,5] → '−' → [1] → [1,3] → [1,3,8] → [1,3,8,2] → '/' → [1,3,4] → '+' → [1,7] → '×' → [7]. Answer = 7. (verified by code)
Q5(ii): passes → {12,38,7,29,45} → {12,7,29,38,45} → {7,12,29,38,45} (4 passes max, early exit pass 3 if flag used... show all).

---

# =================== DEMO PAPER 2 ===================

**Q1. Attempt any two:** *(2×5=10)*
(i) Array vs structure vs union in C — with a small code example of each.
(ii) Need of data structures; classify (linear/non-linear, static/dynamic) with one real-life example each.
(iii) Write a C program: read 10 integers into an array; print max and min using pointer arithmetic (no [] operator).

**Q2. Attempt any one:** *(10)*
(i) a) Stack operations (push/pop/peek) with overflow & underflow conditions. (3)
   b) Array implementation of stack in C (push, pop functions). (4)
   c) Application: how a stack reverses a string. (3)
(ii) a) Queue ADT and its operations. (3)
   b) Applications of queues (any four — job sequencing queue from syllabus). (3)
   c) Deque — types and one use. (4)

**Q3. Attempt any one:** *(10)*
(i) Given inorder: DBEAFCG and preorder: ABDECFG — construct the binary tree showing all intermediate steps; write its postorder. (COMP ND25 clone — the hottest tree question right now.)
(ii) a) DFS vs BFS: data structure used, completeness, use cases. (4)
   b) Run BFS on: A–B, A–C, B–D, B–E, C–F, E–F starting at A; write visit order. (3)
   c) One application each of DFS and BFS. (3)

**Q4. Attempt the following:** *(5+5=10)*
(a) Insert into an initially empty BST: 10, 4, 3, 5, 11, 12, 14, 8, 1 (ND21 clone). Draw final tree; write preorder & postorder.
(b) Write C code for a binary tree node and an inorder traversal function (recursive).

**Q5. Attempt any two:** *(2×5=10)*
(i) Insertion sort — algorithm + trace on {12, 45, 7, 38, 29}; why is it preferred for nearly-sorted data?
(ii) Selection sort — algorithm + complexity (all cases); why fewest writes?
(iii) Solve the recurrence T(n) = 2T(n/2) + n by the recursion-tree method; state the final complexity.

---KEY (Demo 2)---
Q3(i): tree root A; B (left) with D,E; C with F,G; postorder = DEB F G C A → "DEBF GCA": D E B F G C A.
Q3(ii)(b): BFS order A B C D E F.
Q5(iii): levels sum n per level, log n levels → O(n log n).

---

# =================== DEMO PAPER 3 — PREDICTED DEC-2026 MOCK ===================

**Q1. Attempt any two:** *(2×5=10)*
(i) What is an array? C function: array + size → sum of elements (MJ25 exact family).
(ii) What is a structure? Design a 'Robot' struct (id, name, battery%) + function to display (MJ25 Book-style rotation).
(iii) What is an ADT? One example implemented two ways (MJ25's third short).

**Q2. Attempt any one:** *(10)*
(i) SLL family (MJ25 Q2 rotation): a) SLL vs DLL (2) b) insert-at-head vs insert-at-tail complexity (2) c) steps + C code insert head & tail (6).
(ii) Stack family (rotation pair): a) stack-based string reverse (3) b) push/pop time complexity — why O(1) (2) c) memory management & stack overflow (3) d) what to do when an array queue becomes full → circular (2).

**Q3. Attempt any one:** *(10)*
(i) BST family (MJ25 Q3 rotation): a) binary tree vs BST (2) b) node struct in C (2) c) inorder pseudocode + significance (4) d) two applications (2).
(ii) Graph family: a) directed vs undirected with examples (3) b) DFS working on a graph (3) c) DFS vs BFS compare (3) d) one DFS application (1).

**Q4. Attempt the following:** *(5+5=10)*
(a) Sorting scenario: when is insertion sort better than bubble/selection — justify (MJ25 asked exactly this "synthesise a scenario" skill).
(b) C function for linear search on an int array + its best/worst/average complexity.

**Q5. Attempt any two:** *(2×5=10)*
(i) Worst/average/best case analysis — determine all three for linear & binary search (MJ25 skill).
(ii) What is a recurrence relation and why does it matter? Solve T(n) = T(n−1) + c and T(n) = 2T(n/2) + n by substitution/recursion-tree. (MJ25 Q5 rotation.)
(iii) Trace binary search for 29 in {7, 12, 29, 38, 45, 51, 77} — show low/mid/high each step; count comparisons vs linear search.

---HOW BUILT / SELF-SCORE---
The MJ25 RAI paper's DNA: Q1 = C-basics + ADT (same pool all three shorts); Q2 = SLL or stack-queue; Q3 = BST or graph; Q4/Q5 = searching/sorting/complexity with "analyse/justify" verbs. Demo 3 keeps every slot inside those pools, rotating items per the validated rotation rule. The COMP ND25 tree-from-traversals question is added in Demo 2 as high-probability new entry — it's in your syllabus (traversals) and appeared in the sister branch's latest paper.
Skip-list (not your syllabus, ignore if seen elsewhere): hashing/AVL/MST/Dijkstra/heaps/set-map.
Rubric: C code compiles-in-head (semicolon-level care), complexity stated with reasoning ("each element shifted once → O(n)"), diagrams for trees/graphs. 45+ ready; 38–44 solid; <38 → rewrite the C functions from Demo 1–2 until fluent.
