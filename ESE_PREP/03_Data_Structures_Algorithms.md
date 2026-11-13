# 03 · Data Structures and Algorithms (316U43C303) — ESE Question Bank

50 marks · 2 hrs · Q1 any-two ×5 · Q2 any-one ×10 (or both ×5+5) · Q3 any-one ×10 · Q4/Q5 mixed

Real RAI paper: May–Jun 2025. Sister papers: COMP ND25, EXTC ND25, COMP 2021 ×2 (same SVU scheme).

---

## CHEAT SHEET — what repeats

| # | Recurring item | Evidence |
|---|----------------|----------|
| 1 | **Array/structure C code + ADT theory** | RAI MJ25 Q1 (array sum function, Book struct, ADT example) |
| 2 | **Singly linked list: insert at beginning/end, complexity, vs array/doubly** | RAI MJ25 Q2, 2021 papers |
| 3 | **Stack: push/pop complexity, memory, stack overflow + application (string reverse / infix→postfix)** | RAI MJ25 Q2, DS ND21 Q2, DS MJ21 Q2 |
| 4 | **BST: vs binary tree, node in C, insert, inorder traversal, applications** | RAI MJ25 Q3, DS ND21, EXTC ND25 |
| 5 | **Graph: DFS vs BFS, directed/undirected, representation, application** | RAI MJ25 Q3, DS ND21 Q3, DS MJ21 Q3 |
| 6 | **Searching: linear vs binary + C code + space complexity comparison** | RAI MJ25 Q5, DS MJ21 |
| 7 | **Sorting: bubble/insertion/selection passes + when insertion is best** | RAI MJ25 Q5, EXTC ND25 Q1 (bubble passes {92,85,57,26}) |
| 8 | **Big-O/Θ/Ω, worst/avg/best, recurrence relations** | RAI MJ25 Q5 |
| 9 | **Build tree from traversals (inorder+preorder→postorder)** | DS ND25 COMP Q3 |
| 10 | Queue: types (circular), drawback of linear array queue, applications | EXTC ND25, DS MJ21 Q1B |

⚠️ NOT in your syllabus (appeared in COMP/EXTC sister papers — skip unless you have spare time): **hashing/hash tables/probing, AVL rotations, MST (Prim/Kruskal), Dijkstra, heaps, B-trees, Z-transforms**. The RAI MJ25 paper stayed 100% inside the RAI syllabus, and RAI's COs say nothing about hashing/AVL/graphs-shortest-path. Your Module 3 self-learning mentions shortest-path finding — so know *the idea* of BFS being used for shortest path, but the heavy algorithms are lower priority.

---

## MODULE 1 — Introduction + C revision + ADT

### Possible questions
1. What is an array in C? Write a C function: array + size → return sum of elements. *(asked MJ25)*
2. What is a structure? Design a 'Book' struct (title, author, pages) + function to print details. *(asked MJ25)*
3. What is a union? Array vs structure vs union (short).
4. Pointers: declaring, dereferencing; pointer to struct; malloc node creation code (2021 paper MCQ: `ptr = (NODE*)malloc(sizeof(NODE));`).
5. Recursion vs iteration; recursive functions in C (factorial), how stack supports recursion *(2021 short)*.
6. **ADT**: definition, significance, example (List/Stack/Queue as ADT) + how one ADT maps to different implementations *(asked MJ25)*.
7. Need of data structure; types (linear/non-linear, static/dynamic); real-life examples.

### Notes to remember
- ADT = logical contract (operations + behaviour) separate from implementation. Stack ADT can be array-based or linked-list-based.
- struct vs union: union members share memory; size = largest member.
- malloc returns void*, cast to (NODE*); sizeof(NODE) not sizeof(NODE*).

## MODULE 2 — Linear: Stack, Queue, Linked List

### Possible questions
1. **Stack ADT**: operations, array representation, overflow/underflow conditions. *(MJ25: memory management in stack + overflow implications)*
2. **Infix → postfix conversion** algorithm + trace A*(B+C)−D/E or (a+b^c*d)/(a+b+c) *(DS ND21 Q2, DS MJ21 Q2 — the classic 10-marker; RAI syllabus explicitly lists it)*.
3. Evaluate postfix with stack: e.g. 6 3 2 + * 4 2 / + 5 − *(EXTC ND25)*.
4. Stack application: reverse a string, undo-redo (two stacks), expression evaluation, recursion *(MJ25 + MJ21 MCQ)*.
5. **Queue ADT**: operations, array representation; drawback of linear queue (false overflow) → circular queue fixes it; circular conditions front=(rear+1)%MAX *(EXTC ND25, DS MJ21 Q1B)*.
6. Types of queue: circular, deque (double-ended), priority — short notes.
7. Applications of queues: job sequencing (syllabus-named), printer spooling, CPU scheduling, BFS *(MJ21 Q1B(G))*.
8. **SLL**: node representation (struct with data+next), insert at beginning/end — steps + C code, complexity O(1) at head vs O(n) at tail *(MJ25 Q2 full 10-marker)*.
9. Linked list vs array (memory, access time, insertion cost); SLL vs DLL; types: circular, doubly, circular-doubly.
10. Traversal/search in SLL; deletion from SLL (know the 3 cases: head, middle, tail).
11. Polynomial representation/addition using SLL *(DS ND21 Q2 — algorithm + example)*.

### Notes to remember
- Infix→postfix: operands straight out; operators push/pop by precedence (^ > *,/ > +,−); '(' pushed, ')' pops to '('.
- Postfix eval: push operands; operator → pop 2, compute (second-popped OP first-popped), push back.
- Circular queue empty: front==rear==−1 (or front==−1); full: (rear+1)%MAX==front.
- SLL insert-at-head O(1); insert-after-known-node O(1); insert-at-tail O(n) without tail pointer.
- Job sequencing queue = applications list from syllabus unit 2.2 — pre-prepare this answer.

## MODULE 3 — Non-Linear: Trees & Graphs

### Possible questions
1. Tree terminology: root, leaf, depth/height *(MJ21 MCQ: depth = max nodes root→deepest leaf)*, degree, siblings.
2. Binary vs ternary vs n-ary; full vs complete vs skewed binary trees.
3. Binary tree node in C (struct with left/right pointers) *(MJ25)*; array vs LL representation (2i+1, 2i+2 children in array).
4. **Traversals**: give pseudocode for in-order *(asked MJ25)*; pre/post; all three on a given tree; **construct tree from inorder+preorder, write postorder** *(COMP ND25 Q3 with steps — very likely for RAI too)*.
5. **BST**: definition/property; insertion with example *(EXTC ND25)*; construct BST from sequence 10,4,3,5,11,12,14,8,1 *(DS ND21 short)*; search; deletion (3 cases: leaf, one child, two children — successor); inorder gives sorted order; applications ×2 *(MJ25)*.
6. **Graph**: definition, directed vs undirected with examples *(MJ25)*; representation: adjacency matrix vs list (sparse→list, 2021 MCQ); when each is preferred.
7. **DFS**: algorithm + working on a graph *(MJ25 asked "explain how DFS works"; ND21 asked full BFS algorithm)*; DFS vs BFS comparison (stack vs queue, use cases) *(MJ25)*; applications of DFS/BFS (1 each; BFS for shortest path in unweighted graphs — your self-learning).
8. Types of graphs: weighted, connected, complete, cyclic (short-theory bank).

### Notes to remember
- Inorder(LNR), Preorder(NLR), Postorder(LRN). For BST, inorder = ascending sort.
- Rebuild from inorder+preorder: preorder[0]=root → split inorder → recurse. (inorder+postorder also unique; pre+post is NOT unique for general binary trees.)
- DFS uses stack (or recursion); BFS uses queue. DFS: O(V+E) with adjacency list.
- Binary tree array rep: node i → children 2i+1, 2i+2 (0-indexed).

## MODULE 4 — Analysis of Algorithms

### Possible questions
1. Role of algorithms; what makes a good algorithm; parameters of efficiency.
2. **Time vs space complexity** — definitions + why both matter.
3. **Big-O, Big-Θ, Big-Ω**: definitions, how they relate (Θ = O ∩ Ω) *(MJ25: "relate to each other in bounding a function")*; formal definitions with constants.
4. **Worst / average / best case** — determine for a given algorithm (e.g. linear search: n / n/2-ish / 1) *(MJ25 asked how to determine)*.
5. **Recurrence relations**: what & why important *(MJ25)*; solve by substitution method and recursion-tree method (syllabus-named): T(n)=T(n−1)+c → O(n); T(n)=2T(n/2)+n → O(n log n).
6. Master method (self-learning — know statement + one example, may show as IA/lab not ESE).
7. Analyze complexity of: linear search O(n), binary search O(log n), bubble/insertion/selection O(n²), merge O(n log n).
8. Asymptotic analysis idea: machine-independent growth-rate comparison.

### Notes to remember
- O = upper bound, Ω = lower, Θ = tight. "f ∈ O(g) and f ∈ Ω(g) ⇒ f ∈ Θ(g)".
- Binary search needs sorted array. Recursion tree: draw levels, sum costs per level.
- Common chain: 1 < log n < n < n log n < n² < n³ < 2ⁿ.

## MODULE 5 — Searching & Sorting

### Possible questions
1. **Bubble sort with passes** on a small set, e.g. {92,85,57,26} ascending *(EXTC ND25)*; count passes/comparisons.
2. **Insertion sort**: working + why best for nearly-sorted data (adaptive, O(n) best case) — "synthesise a scenario where insertion beats bubble/selection" *(MJ25)*.
3. **Selection sort**: working, min-search per pass, #swaps = n−1.
4. C implementations of all three on arrays (syllabus says implementation using array).
5. **Complexity table** all three: bubble/selection O(n²) all cases; insertion O(n²) worst/avg, O(n) best; space O(1) all (in-place).
6. Stability of sorts (bubble & insertion stable, selection not — 2021 short note).
7. **Linear search**: C function on int array *(MJ25)*; O(n).
8. **Binary search**: algorithm, C code, O(log n), requires sorted input; trace on array.
9. **Space complexity of linear vs binary search** — both O(1) iterative; binary recursive O(log n) stack *(MJ25 asked exactly this)*.

### Notes to remember
- Bubble: adjacent swaps, largest bubbles to end each pass. Early-termination flag if no swap.
- Insertion: grow sorted prefix; shift larger elements right. Best case already sorted = n−1 comparisons.
- Selection: find min in unsorted part, single swap per pass — fewest writes.
- Linear search works on unsorted; binary only sorted. Space: iterative binary O(1).

---

## PRACTICE PRIORITY
(1) Infix→postfix + postfix evaluation, (2) BST construct/insert/delete + traversal rebuild, (3) SLL insert/delete C code, (4) DFS/BFS on a drawn graph, (5) bubble-sort passes, (6) complexity table + Big-O trio. Write actual C snippets while revising — MJ25 asked for C functions/code in 4 of 5 questions.
