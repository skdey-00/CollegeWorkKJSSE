# DSA — RANKED SAMPLE PAPERS (3 papers, best → decent)

Format per RAI MJ-2025: Q1 any-two ×5 · Q2 any-one ×10 (sub-parts) · Q3 any-one ×10 · Q4/Q5 mixed. 50 marks · 2 hrs.

Evidence codes: [BOTH] = asked in MJ25 RAI + sister papers · [ROT] = slot rotation · [NEW] = never asked / overdue.

---

# ======== PAPER 1 — BEST PREDICTION ========

**Q1. Attempt any two:** *(2×5=10)*
(i) What is an array? Write a C function returning the sum of all elements of an int array. **[BOTH — MJ25 Q1(i) exact family]**
(ii) What is a structure? Define a Book struct (title, author, price) and write a C function to display it. **[BOTH — MJ25 Q1(ii) exact family]**
(iii) What is an ADT? Explain with one example. **[BOTH — MJ25 Q1(iii) exact]**

**Q2. Attempt any one:** *(10)*
(i) a) SLL vs DLL differences. (2) b) Complexity of insert at beginning vs end of SLL. (2) c) Steps + C code: insert node at beginning and at end of SLL. (6) **[BOTH — MJ25 Q2(i) near-exact]**
(ii) a) What is a stack? push/pop/peek with overflow & underflow. (3) b) Array stack in C: push & pop functions. (4) c) Reverse a string using stack. (3) **[BOTH — MJ25 Q2(ii) near-exact]**

**Q3. Attempt any one:** *(10)*
(i) a) Binary tree vs BST. (2) b) BST node in C. (2) c) Insert 45,25,65,15,35,55,75,30; write inorder. (4) d) Applications of BST. (2) **[BOTH — MJ25 Q3(i) family]**
(ii) a) Graph: directed vs undirected. (2) b) DFS on a 6-vertex graph — algorithm + diagram. (4) c) DFS vs BFS: structure used, use case. (2) d) One application of each. (2) **[BOTH — MJ25 Q3(ii) family]**

**Q4. Attempt the following:** *(5+5=10)*
(a) Scenario question: when is **insertion sort** preferable to bubble/selection? Justify with data condition + complexity reasoning. **[BOTH — MJ25 Q4 exact skill]**
(b) C function for **linear search** + best/worst/average complexity. **[BOTH — MJ25 Q4/Q5 family]**

**Q5. Attempt any two:** *(2×5=10)*
(i) Linear vs binary search — algorithm, C snippet, time & space complexity table. **[BOTH]**
(ii) Trace **binary search** for 29 in {7,12,29,38,45,51,77}; count comparisons vs linear. **[ROT]**
(iii) Explain Big-O, Θ, Ω with one example each. **[BOTH — MJ25 Q5 exact]**

---KEY P1---
Q3(i)(c): inorder = 15 25 30 35 45 55 65 75.
Q5(ii): mid=38→29<38 left; mid=12→29>12 right; mid=29 found. 3 comparisons vs 3rd position linear (3 comparisons best-case linear position).
Q5(iii): O upper, Θ tight, Ω lower; linear search: O(n)/Θ(n)/Ω(1).

---

# ======== PAPER 2 — GOOD PREDICTION ========

**Q1. Attempt any two:** *(2×5=10)*
(i) Pointer basics: & and * operators; swap(int*, int*) C function. **[ROT]**
(ii) Recursion: factorial in C; how the call stack supports recursion. **[ROT]**
(iii) Need of data structures + classification (linear/non-linear, static/dynamic). **[ROT]**

**Q2. Attempt any one:** *(10)*
(i) a) Circular queue: drawback of linear queue it fixes. (4) b) C code enqueue/dequeue circular. (6) **[ROT]**
(ii) a) Queue applications (any four). (3) b) Deque types + one use. (4) c) Priority queue concept. (3) **[ROT]**

**Q3. Attempt any one:** *(10)*
(i) Given **inorder DBEAFCG + preorder ABDECFG**, construct the binary tree step-by-step; write postorder. **[NEW — asked in COMP ND25 (sister branch, latest window); hottest tree question]**
(ii) a) BFS algorithm. (3) b) BFS on A–B, A–C, B–D, B–E, C–F, E–F from A: visit order. (3) c) DFS vs BFS completeness & memory. (4) **[ROT]**

**Q4. Attempt the following:** *(5+5=10)*
(a) Insert into empty BST: 10,4,3,5,11,12,14,8,1; draw final tree; preorder + postorder. **[KT — ND21 clone]**
(b) C code: binary tree node struct + recursive inorder function. **[BOTH — MJ25 asked pseudocode]**

**Q5. Attempt any two:** *(2×5=10)*
(i) Bubble sort: trace {38,12,45,7,29} pass by pass; complexity all cases. **[BOTH-adjacent]**
(ii) Selection sort: algorithm + why fewest writes. **[ROT]**
(iii) Solve T(n) = 2T(n/2)+n by recursion tree; final complexity. **[ROT — MJ25 asked recurrence; this is the paired method]**

---KEY P2---
Q3(i): A root; B left (D,E under B), C right (F,G under C); postorder = D E B F G C A.
Q3(ii)(b): A B C D E F.
Q4(a): preorder = 10 4 3 1 5 8 11 12 14; postorder = 1 3 8 5 4 14 12 11 10. (verified by code)
Q4(b): struct tnode { int data; struct tnode *left, *right; }; void inorder(struct tnode* r){ if(r){ inorder(r->left); printf("%d ", r->data); inorder(r->right); } }
Q5(i): bubble passes {38,12,45,7,29}: P1→{12,38,7,29,45} P2→{12,7,29,38,45} P3→{7,12,29,38,45} (no swap in P4 → early exit). All cases O(n²), space O(1).
Q5(ii): selection: n−1 swaps total (one per pass); fewest writes among simple sorts.
Q5(iii): levels cost n each (root n, two halves n/2+n/2 = n, ...), log n levels → total n·log n → O(n log n).

---

# ======== PAPER 3 — DECENT PREDICTION ========

**Q1. Attempt any two:** *(2×5=10)*
(i) Array vs pointer arithmetic: print max/min of 10-int array using pointers only (no []). **[NEW]**
(ii) Structure vs union with code. **[NEW]**
(iii) Row-major vs column-major address calculation; element at A[4][5] in a 10×8 array (base 1000, 2 bytes). **[NEW — classic never asked in RAI]**

**Q2. Attempt any one:** *(10)*
(i) a) Stack applications: infix→postfix rules. (3) b) Convert (a+b*c)/(d−e) showing stack each step. (4) c) Evaluate the postfix by stack. (3) **[ROT — 2021-era asked infix/postfix; unasked in MJ25 → overdue]**
(ii) a) DLL: node struct in C. (3) b) Insert at head in DLL — steps + code. (4) c) DLL vs SLL deletion cost. (3) **[ROT]**

**Q3. Attempt any one:** *(10)*
(i) BST deletions: leaf, one child, two children — explain with example tree. **[NEW — MJ25 built & traversed but never deleted]**
(ii) Graph representations: adjacency matrix vs list with a 5-vertex example; when each preferred (sparse vs dense). **[NEW]**

**Q4. Attempt the following:** *(5+5=10)*
(a) Insertion sort trace on {12,45,7,38,29} + why preferred for nearly-sorted. **[ROT]**
(b) Radix OR bucket sort concept + when better than comparison sorts. **[NEW — in your college slides CH05; sister papers asked radix passes]**

**Q5. Attempt any two:** *(2×5=10)*
(i) Solve T(n) = T(n−1)+n by substitution; complexity. **[ROT]**
(ii) Amortized/intro-analysis OR space vs time trade-off with example (e.g., array vs SLL memory overhead). **[NEW]**
(iii) Evaluate postfix 6 2 3 + − 3 8 2 / + * by stack. **[ROT]**

---KEY P3---
Q1(iii): row-major: 1000 + (4·8+5)·2 = 1000+74 = 1074.
Q4(a): nearly-sorted → few shifts, O(n) best case.
Q5(iii): result 49 — trace carefully: 6, 2, 3, + → 5; − → 1; then 3 8 2 / → 4; + → 7; × → 7? recompute fully: stack [6], [6,2], [6,2,3], + → [6,5], − → [1], [1,3], [1,3,8], [1,3,8,2], / → [1,3,4], + → [1,7], × → [7]. Final 7 (verify sign of 6−5=1 ✓).

---HOW THESE WERE RANKED---
P1 = MJ25's exact slot content (the only RAI paper, so every P1 item is a direct family repeat of what their examiner asked in May). P2 = rotations confirmed by sister papers + the hot new entry (tree-from-traversals, asked COMP ND25). P3 = never-asked residual (address calc, unions, BST deletion, radix, postfix eval) — insurance. Skip-list still applies: no hashing/AVL/MST/Dijkstra/set-map.
