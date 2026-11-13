# ANSWER KEY — 03 · Data Structures & Algorithms

Covers every "possible question" in 03_Data_Structures_Algorithms.md. "(verified by code)" = executed programmatically.

---

## MODULE 1 — Intro + C + ADT

**1. Array sum function** *(MJ25 exact)*:
```c
int sum(int a[], int n) {
    int s = 0;
    for (int i = 0; i < n; i++) s += a[i];
    return s;
}
```
Array = contiguous, same-type, fixed-size elements, O(1) index access via base + i×sizeof.

**2. Book struct** *(MJ25 exact)*:
```c
struct Book {
    char title[50], author[50];
    int pages; float price;
};
void printBook(struct Book b) {
    printf("%s by %s, %d pages, Rs %.2f\n", b.title, b.author, b.pages, b.price);
}
```

**3. Union**: members share one memory block; size = largest member; only one member valid at a time. Array = many same-type; struct = many mixed-type (each own memory); union = mixed overlapping.

**4. Pointers**: `int *p = &x;` *p dereferences. `NODE *n = (NODE*)malloc(sizeof(NODE));` — cast void*, size of struct not pointer.

**5. Recursion**: base case + recursive case; each call gets a stack frame (params, locals, return address) → depth = number of pending calls; no base case → stack overflow.
```c
long fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
```

**6. ADT** *(MJ25 exact)*: logical spec (operations + behaviour) separated from implementation. Stack ADT: push/pop/peek/isEmpty — implement with array OR linked list; user code unchanged. Significance: abstraction, encapsulation, implementation freedom.

**7. Need & types**: organise data for the operations you need (fast search / fast insert / hierarchy). Linear (array, list, stack, queue) vs non-linear (tree, graph); static (array) vs dynamic (linked list). Real-life: music playlist (list), browser history (stack), printer queue (queue), org chart (tree), metro map (graph).

## MODULE 2 — Stack, Queue, Linked List

**1. Stack ADT**: LIFO; push/pop/peek; array impl: top index, overflow when top == MAX−1, underflow when top == −1. Memory: contiguous; overflow when full (array) or heap exhausted (linked).

**2. Infix→postfix** (the classic 10-marker, 2021×2): scan; operand → output; operator → pop while stack-top precedence ≥ incoming (^ > *,/ > +,−), then push; '(' push; ')' pop-to-'('.
Trace (a+b*c)/(d−e): output a → b → c; '+' < '*' hold... final **a b c * + d e − /** (verified).

**3. Postfix eval** (EXTC ND25): 6 3 2 + * 4 2 / + 5 − → 6·5 + 2 − 5 = **30−5+... trace: [6][6,3][6,3,2]+→[6,5]×→[30][30,4][30,4,2]/→[30,2]+→[32][32,5]−→27**. Answer 27. Second trace (6 2 3 + − 3 8 2 / + *) = **7** (verified by code).

**4. Stack applications**: string reverse, undo/redo (2 stacks), expression conversion/eval, recursion, browser back, parenthesis matching.

**5. Queue ADT & circular**: FIFO; linear array queue wastes cells after dequeues (false overflow) → circular with modulo: rear = (rear+1)%MAX; full: (rear+1)%MAX == front; empty: front == −1.

**6. Queue types**: circular, deque (input/output-restricted), priority (served by priority not order).

**7. Queue applications**: printer spooling, CPU scheduling/ready queue, keyboard buffer, BFS, call-center holding — job sequencing (syllabus-named): jobs wait in queue for a resource.

**8. SLL insert code** *(MJ25 10-marker)*:
```c
struct Node { int data; struct Node *next; };
// insert at beginning: O(1)
void insBeg(struct Node **head, int v) {
    struct Node *n = malloc(sizeof(struct Node));
    n->data = v; n->next = *head; *head = n;
}
// insert at end: O(n) without tail pointer
void insEnd(struct Node **head, int v) {
    struct Node *n = malloc(sizeof(struct Node)), *t = *head;
    n->data = v; n->next = NULL;
    if (!*head) { *head = n; return; }
    while (t->next) t = t->next;
    t->next = n;
}
```

**9. Array vs linked list**: contiguous vs scattered nodes; O(1) vs O(n) access; O(n) vs O(1) insert-at-head; no vs extra pointer memory. SLL (one direction) vs DLL (prev+next, 2× pointers, easier deletion). Circular: tail→head.

**10. SLL deletion 3 cases**: head (move head, free old), middle/tail (find predecessor, bypass, free).

**11. Polynomial via SLL**: node = (coeff, power, next); add: merge by descending power, add matching exponents.

## MODULE 3 — Trees & Graphs

**1. Terminology**: root, leaf, degree (children count), siblings, depth (root=0 or 1 per convention — MJ21 MCQ: nodes on longest root→leaf path), height.

**2. Full (0 or 2 children) vs complete (filled level-order) vs skewed (a list).

**3. Node + representations**:
```c
struct tnode { int data; struct tnode *left, *right; };
```
Array: node i → children 2i+1, 2i+2 (0-indexed).

**4. Traversals**: LNR / NLR / LRN.
Inorder pseudocode *(MJ25)*: `inorder(t): if t: inorder(t.left); visit(t); inorder(t.right)`.
**Rebuild from inorder+preorder** *(COMP ND25)*: preorder[0] = root; locate in inorder; left of it = left subtree, right = right; recurse. DBEAFCG + ABDECFG → root A; (DBE)(FCG); B: (D)(E); C: (F)(G) → postorder = **D E B F G C A** (verified).

**5. BST**: left < root < right; inorder = sorted. Insert 10,4,3,5,11,12,14,8,1 *(ND21)*: preorder = **10 4 3 1 5 8 11 12 14**, postorder = **1 3 8 5 4 14 12 11 10** (verified by code). Deletion: leaf → free; one child → splice; two children → replace with inorder successor (min of right subtree), delete successor. Applications: sorted insert+search, in-memory maps/sets, range queries.

**6. Graph definition & representations**: G = (V, E); directed (arcs one-way — Twitter follows) vs undirected (roads). Adjacency matrix: O(V²) space, O(1) edge check — dense. List: O(V+E) — sparse (2021 MCQ).

**7. DFS/BFS**: DFS = depth-first via stack/recursion; BFS = level-order via queue. DFS on 6-vertex graph: mark visited, push neighbours, pop-continue. DFS vs BFS: stack vs queue; DFS good for cycle/topological/path-existence; BFS for shortest path (unweighted), level order. Applications: DFS — cycle detection, topological sort; BFS — shortest path, web crawling. Both O(V+E) with lists.

**8. Graph types**: weighted/complete/cyclic/connected — one line each.

## MODULE 4 — Analysis

**1–2. Good algorithm**: correct + finite + efficient; time = # primitive ops vs input size; space = extra memory. Both matter (embedded/robotics: memory-constrained).

**3. Big-O/Θ/Ω** *(MJ25)*: O = upper bound (∃c: f ≤ c·g for n ≥ n₀); Ω = lower; Θ = both — tight. Example: linear search = O(n), Ω(1), Θ(n) overall (worst-case tight).

**4. Worst/avg/best**: linear: n / (n+1)/2 / 1; binary: log n / ~log n / 1. Determine by input arrangements: reversed (worst), random (avg), already-found-first (best).

**5. Recurrences** *(MJ25)*: T(n) = T(n−1)+c → O(n) (substitution unrolls to c·n). T(n) = 2T(n/2)+n → **O(n log n)** (recursion tree: n per level × log n levels).

**6. Master method** (self-learning): T(n) = aT(n/b)+f(n); compare f with n^(log_b a).

**7. Complexity table**: linear O(n); binary O(log n); bubble/insertion/selection O(n²); merge O(n log n).

**8. Asymptotic**: machine-independent growth comparison; constants dropped.

## MODULE 5 — Searching & Sorting

**1. Bubble passes {92,85,57,26}** *(EXTC ND25)*: P1: {85,57,26,92} P2: {57,26,85,92} P3: {26,57,85,92}. n−1 passes, n(n−1)/2 comparisons.

**2. Insertion sort & nearly-sorted scenario** *(MJ25)*: grow sorted prefix; each element shifts only past larger elements — nearly sorted → ~1 shift each → **O(n) best case, adaptive**; scenario: daily-updated leaderboard re-sorted each morning.

**3. Selection**: find min of unsorted tail, one swap per pass (n−1 swaps total — fewest writes; good when writes costly e.g. flash).

**4. C implementations**: 3 nested-loop sorts — standard; write each from memory.

**5. Complexity table**: bubble/selection O(n²) all cases; insertion O(n²)/avg O(n²)/best O(n); all space O(1), in-place.

**6. Stability**: equal elements keep order — bubble & insertion stable; selection NOT (long-distance swap).

**7–9. Searching** *(MJ25 family)*: linear C function + O(n), works unsorted; binary O(log n) needs sorted; trace 29 in {7,12,29,38,45,51,77}: mid 38 → left, mid 12 → right, mid 29 found — 3 comparisons (verified by code). Space: iterative O(1) both; recursive binary O(log n) stack.

---

## TRACE-CHECK TABLE (all verified by code)
postfix eval 27 (6 3 2 + * 4 2 / + 5 −) and 7 (6 2 3 + − 3 8 2 / + *) · infix (a+b*c)/(d−e) → a b c * + d e − / · rebuild postorder DEBFGCA · BST 9-node preorder/postorder above · bubble 3 passes · binsearch 3 comparisons
