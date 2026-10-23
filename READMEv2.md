# Software & Algorithms · Symbolic AI

![Course](https://img.shields.io/badge/course-Chapters%203%20%26%204%20·%20CS%20Foundations-01696F)
![Type](https://img.shields.io/badge/type-study%20notes-informational)
![Format](https://img.shields.io/badge/format-GitHub%20Flavored%20Markdown-blue)

> An informational overview of software, operating systems, programming languages, software engineering, databases, algorithms, data structures (Chapter 3), and Symbolic AI (Chapter 4) — expanded from the two course slide decks.
>
> **Companion deck:** [software-and-symbolic-ai-course-deck.pptx](./software-and-symbolic-ai-course-deck.pptx) — the full 39-slide presentation version of these notes, including appendix slides with the architecture, semantic-network, ontology, frame/script, expert-system, and search diagrams, plus the original figures from the source deck embedded in a labeled source appendix.

---

## Table of Contents

- [Part I — Software & Algorithms (Chap 3)](#part-i--software--algorithms-chap-3)
  - [Software Overview](#1-software-overview)
  - [Operating Systems](#2-operating-systems)
  - [Programming Languages](#3-programming-languages)
  - [Software Engineering](#4-software-engineering)
  - [Databases](#5-databases)
  - [Algorithms](#6-algorithms)
  - [Data Structures](#7-data-structures)
  - [Complexity Reference](#8-complexity-reference)
  - [Choosing a Data Structure](#9-choosing-a-data-structure)
- [Part II — Symbolic AI (Chap 4)](#part-ii--symbolic-ai-chap-4)
  - [What is Symbolic AI](#10-what-is-symbolic-ai)
  - [Propositional Logic](#11-propositional-logic)
  - [Predicate Logic](#12-predicate-logic)
  - [Knowledge Representation](#13-knowledge-representation)
  - [Rule-Based & Expert Systems](#14-rule-based--expert-systems)
  - [Planning & Problem Solving](#15-planning--problem-solving)
  - [NLP in Symbolic AI](#16-nlp-in-symbolic-ai)
- [Hands-On: Rules vs. ML](#17-hands-on-exact-rules-vs-text-classification)
- [Sample Learning Materials](#18-sample-learning-materials)
- [Self-Check](#19-self-check)
- [Sources](#sources)

---

# Part I — Software & Algorithms (Chap 3)

## 1. Software Overview

### System vs. Application Software

| | System software | Application software |
|---|---|---|
| **Purpose** | Manages the computer itself; platform for other software | Solves end-user problems |
| **Examples** | Operating systems (Windows, Linux, macOS, Android), device drivers, utilities, translators (compilers, interpreters, assemblers) | Word processors, browsers, games, WeChat (Weixin), mobile apps |
| **Serves** | The machine and other programs | The end user |

**Key distinction:** system software serves the machine and other programs; application software serves the end user.

---

## 2. Operating Systems

### Evolution

| Stage | Era | Description |
|---|---|---|
| 1 | Batch systems | Jobs submitted in batches; no user interaction |
| 2 | Time-sharing | Many users and tasks share one CPU |
| 3 | Personal computers | GUI-driven OSes: Windows, macOS |
| 4 | Mobile & embedded | Android, iOS; phones and devices |
| 5 | Modern era | Virtualization, containers, cloud, multi-core |

### Process Management

- A **program** is a passive file on disk; a **process** is a running instance of it, with its own memory space and state.
- States include New, Ready, Running, Waiting, Terminated — with transitions such as Running → Ready, Waiting → Ready, Running → Waiting, and Running → Terminated (the states form a graph, not a single fixed pipeline).
- The scheduler decides which process gets the CPU; **context switching** creates the illusion of parallelism.

### Memory Management

- Each process gets an isolated **virtual address space**, translated to physical RAM by the OS (paging).
- **Virtual memory** is this per-process address translation and isolation; pages may additionally be **backed by disk**, letting a process exceed physical RAM.
- The OS protects processes from one another and handles fragmentation and allocation.

---

## 3. Programming Languages

### Evolution

```
Machine language → Assembly → Procedural → Object-oriented → Scripting/dynamic → Modern paradigms
(raw binary)      (MOV, ADD)  (C, Pascal)   (C++, Java)      (Python, JS)      (functional & declarative styles)
```

### Categories

| Category | Description | Examples |
|---|---|---|
| Low-level | Machine/hardware-oriented | Machine code, assembly |
| High-level procedural | Step-by-step instructions | C, Pascal |
| Object-oriented | Data + behavior bundled in objects | Java, C++, Python |
| Functional | Computation as function evaluation | Haskell, Lisp |
| Scripting | Glue code and automation | Python, Bash, JavaScript |
| Query | Data retrieval | SQL |

### Features to Compare

- **Compiled vs. interpreted** — ahead-of-time compilation translates the program to machine code before running (C, C++); interpreters execute the program, often step by step. Many languages mix strategies — Java compiles to bytecode that is interpreted/JIT-compiled, and Python compiles to bytecode internally — so "compiled = fast, interpreted = slow" is a rule of thumb, not a guarantee.
- **Static vs. dynamic typing** — types checked before the program runs (Java) vs. at runtime (Python).
- Other axes: paradigm support (paradigms coexist — Python supports procedural, OO, and functional styles), performance, portability, ecosystem.

---

## 4. Software Engineering

### Development Process Models

| Model | Idea | Trade-off |
|---|---|---|
| Waterfall | Linear phases: requirements → design → implementation → testing → deployment → maintenance | Simple, documented; inflexible to late change |
| Agile / iterative | Short cycles (sprints), frequent feedback, working software each iteration | Dominant modern approach |
| Spiral | Repeated risk-driven cycles with explicit risk analysis | Best when risk drives decisions |
| Others | Prototyping, RAD, V-model (testing planned per phase) | Situational |

### Modularity

- Break the system into independent modules (functions, classes, services) with clear interfaces.
- **Cohesion** — how strongly a module's parts belong together → want **high**.
- **Coupling** — how dependent modules are on each other → want **low**.

### Quality Assurance

- **Verification** — "did we build it right?" (reviews, static analysis)
- **Validation** — "did we build the right thing?" (testing against requirements)
- Test levels: **unit → integration → system → acceptance**
- Approaches: black-box, white-box, regression

---

## 5. Databases

### Database Models

- **Hierarchical** — tree structure; each child record has exactly one parent; one-to-many data ([Wikipedia — Database model](https://en.wikipedia.org/wiki/Database_model)).
- **Network** — extends hierarchical; a record can have multiple parents; many-to-many relationships ([Wikipedia — Database model](https://en.wikipedia.org/wiki/Database_model)).
- **Relational** — organizes data in tables of rows and columns, with relationships expressed as values shared between tables ([Wikipedia — Database model](https://en.wikipedia.org/wiki/Database_model)).
- Others: object-oriented, NoSQL (document, key-value, graph).

### Relational Databases — Key Terms

| Term | Meaning |
|---|---|
| Relation / tuple / attribute | Table / row / column; domain = allowed values for an attribute |
| Primary key (PK) | Uniquely identifies every row; must be unique and not-null ([Microsoft Learn](https://learn.microsoft.com/en-us/sql/relational-databases/tables/primary-and-foreign-key-constraints?view=sql-server-ver17)) |
| Foreign key (FK) | References a primary or unique key in another (or the same) table; enforces referential integrity ([Microsoft Learn](https://learn.microsoft.com/en-us/sql/relational-databases/tables/primary-and-foreign-key-constraints?view=sql-server-ver17)) |

**PK vs. FK:** a PK identifies rows within its own table; an FK links tables together. A column can be a PK in one table and an FK in another.

### SQL Essentials

```sql
-- Query: columns, filtering, sorting
SELECT name, email
FROM   students
WHERE  gpa >= 3.0
ORDER BY name ASC;

-- Joining tables via PK-FK pair
SELECT o.order_id, c.name
FROM   orders o
JOIN   customers c ON c.customer_id = o.customer_id;
```

Processing order: `FROM` → `WHERE` → `GROUP BY`/`HAVING` → `SELECT` → `ORDER BY` ([PostgreSQL docs](https://www.postgresql.org/docs/current/sql-select.html), [SQLite docs](https://sqlite.org/lang_select.html)).

---

## 6. Algorithms

### Features

An algorithm must be **well-defined** (unambiguous steps), **finite** (terminates), **effective** (each step doable), with well-defined **inputs and outputs**.

### Representation

Natural language, flowcharts, pseudocode, or code. Example — binary search (requires a **sorted** array; note the floor in the midpoint calculation so it works on any range, including two elements):

```
FUNCTION BinarySearch(A, target)
    low ← 0;  high ← length(A) − 1
    WHILE low ≤ high
        mid ← low + floor((high − low) / 2)
        IF A[mid] = target THEN RETURN mid
        ELSE IF A[mid] < target THEN low ← mid + 1
        ELSE high ← mid − 1
    RETURN NOT_FOUND
```

### Basic Algorithms

| Algorithm | Idea | Complexity |
|---|---|---|
| Linear search | Check items one by one | O(n) |
| Binary search | Halve a sorted range each step | O(log n) |
| Bubble sort | Swap adjacent out-of-order pairs | O(n²) |
| Selection sort | Repeatedly select the smallest remaining | O(n²) |
| Insertion sort | Insert each item into a sorted prefix | O(n²); fast on nearly-sorted data |
| Merge sort | Divide, sort halves, merge | O(n log n) |
| Quicksort | Partition around a pivot | O(n log n) avg, O(n²) worst |

(Complexities are standard results; see [Interview Cake — Big-O cheat sheet](https://www.interviewcake.com/big-o-cheat-sheet).)

### Iteration vs. Recursion

| | Iteration | Recursion |
|---|---|---|
| Mechanism | Loops (`for` / `while`) | Function calls itself; needs a **base case** |
| Memory | Loop state only, no extra frames (e.g. a simple factorial loop) | New stack frame per call |
| Best for | Simple repetition | Self-similar problems (trees, divide & conquer) |

Every recursion can be rewritten as iteration; deep recursion risks **stack overflow**. Example — n! iteratively:

```
f ← 1
FOR i ← 1 TO n
    f ← f × i
RETURN f
```

and recursively:

```
FUNCTION Fact(n)
    IF n ≤ 1 THEN RETURN 1
    ELSE RETURN n × Fact(n − 1)
```

---

## 7. Data Structures

| Structure | Description |
|---|---|
| Array | Contiguous block; O(1) index access; middle insert/delete O(n) |
| Record | Fixed named fields, mixed types (like a row or struct) |
| Linked list | Nodes chained by pointers; insert/delete O(1) only with the needed links in hand (e.g. the predecessor node for a singly linked list); no random access |
| Stack | LIFO — push/pop/peek, all O(1); undo, call stacks, expression evaluation |
| Queue | FIFO — enqueue/dequeue O(1); scheduling, breadth-first traversal |
| Tree | Hierarchical nodes with parent-child links; one root |
| Binary tree | Each node has at most two children |
| Binary search tree (BST) | Ordering property: left < node < right; operations cost O(h) where h = height — logarithmic when balanced, linear when skewed |
| Graph | Vertices + edges (directed/undirected, weighted or not); trees are a special case |

---

## 8. Complexity Reference

Average case; conditions matter:

| Structure | Access | Search | Insert | Delete | Notes |
|---|---|---|---|---|---|
| Array | O(1) | O(n) | O(n) | O(n) | Insert/delete shift elements |
| Linked list | O(n) | O(n) | O(1)* | O(1)* | only with the needed links in hand (e.g. the predecessor) |
| Stack | O(n) | O(n) | O(1) | O(1) | push/pop at the top only |
| Queue | O(n) | O(n) | O(1) | O(1) | enqueue rear, dequeue front |
| BST | — | O(h)* | O(h)* | O(h)* | *h = height; logarithmic when balanced, linear if skewed |
| Balanced BST (AVL, red-black) | — | O(log n) | O(log n) | O(log n) | self-balancing |

(Reference: [Interview Cake](https://www.interviewcake.com/big-o-cheat-sheet), [FaangPrep](https://faangprep.com/dsa/big-o-cheat-sheet/), [Gera Tools](https://geratools.com/data-structure-complexity-reference).)

---

## 9. Choosing a Data Structure

| Need | Use |
|---|---|
| Fast index-based access | Array |
| Frequent insert/remove at known positions | Linked list |
| LIFO undo / backtracking | Stack |
| Fair first-come-first-served | Queue |
| Ordered data, fast search & insert | Balanced BST |
| Hierarchical data | Tree |
| Arbitrary many-to-many relationships | Graph |

---

# Part II — Symbolic AI (Chap 4)

## 10. What is Symbolic AI

**Symbolic AI** (also called GOFAI — Good Old-Fashioned AI) focuses on high-level symbolic reasoning and the manipulation of symbols to simulate human intelligence. It relies on **explicit rules and logic** to represent knowledge and make decisions — in contrast to machine learning, which learns patterns from data.

- **Typical architecture:** a **knowledge base** (human-input facts and rules) plus an **inference engine** that derives answers to questions.
- **Example rule:** `IF patient has fever AND patient has cough AND patient has difficulty breathing THEN patient may have pneumonia.`
- **Landscape:** Symbolic AI is a branch inside Artificial Intelligence, distinct from the Machine Learning → Deep Learning lineage.
- **Applications:** Siri and digital assistants, medical diagnosis systems, autonomous cars, computer vision systems.
- **Benefits:** interpretability (decisions traceable to rules), knowledge representation, flexibility.
- **Limitations:** incomplete knowledge, scalability, difficulty with uncertain or ambiguous information, limited ability to learn and adapt.

---

## 11. Propositional Logic

- A **proposition** is a declarative sentence that is either true or false, not both. Examples: "The sky is blue." · "It is raining." · "2 + 2 = 4."
- Boolean operators combine propositions: **AND** (∧), **OR** (∨), **NOT** (¬).

**Truth table for AND, OR, NOT:**

| p | q | p ∧ q | p ∨ q | ¬ p | ¬ q |
|---|---|---|---|---|---|
| T | T | T | T | F | F |
| T | F | F | T | F | T |
| F | T | F | T | T | F |
| F | F | F | F | T | T |

**Implication & biconditional:**

- `p → q` — "if p, then q" — p is the **antecedent** (premise), q is the **consequent** (conclusion). True in every case except a true premise with a false conclusion.
- `p ↔ q` — "p if and only if q" — asserts p and q have the same truth value.

| p | q | p → q | p ↔ q |
|---|---|---|---|
| T | T | T | T |
| T | F | F | F |
| F | T | T | F |
| F | F | T | T |

**Logical equivalences** — statements with the same truth value in all circumstances:

- **De Morgan's Laws:** `¬(p ∧ q) ≡ ¬p ∨ ¬q` and `¬(p ∨ q) ≡ ¬p ∧ ¬q`
- **Double negation:** `¬(¬p) ≡ p`

**Inference rules** — principles for deriving new conclusions:

- **Modus Ponens:** from `p → q` and `p`, infer `q`
- **Modus Tollens:** from `p → q` and `¬q`, infer `¬p`

In AI, propositional logic provides a formal language for representing and manipulating knowledge in a way that enables **automated reasoning**.

---

## 12. Predicate Logic

- A **predicate** is a function that returns a truth value when applied to one or more variables — e.g. `Even(x)`.
- **Universal quantifier** `∀` — the predicate holds for every element of the domain: `∀x(Cat(x) → Mammal(x))`
- **Existential quantifier** `∃` — the predicate holds for at least one element: `∃x(Prime(x) ∧ x < 10)`

**Formalizing natural language:** identify the predicates → introduce variables → apply quantifiers → formulate the logical expression. Example: "Some birds can fly" becomes `∃y(Bird(y) ∧ CanFly(y))`.

**Rules of inference:**

| Rule | From | To |
|---|---|---|
| Universal Instantiation | `∀x(P(x) → Q(x))` | `P(a) → Q(a)` |
| Existential Instantiation | `∃x(P(x) ∧ Q(x))` | `P(c) ∧ Q(c)` — the witness must be a **fresh name** |
| Universal Generalization | `P(a) → Q(a)` | `∀x(P(x) → Q(x))` — valid only when `a` is an **arbitrary object**, not a specific example |
| Existential Generalization | `P(c) ∧ Q(c)` | `∃x(P(x) ∧ Q(x))` — from one established instance |
| Universal Modus Ponens | `∀x(P(x) → Q(x))` and `P(a)` | `Q(a)` |
| Universal Modus Tollens | `∀x(P(x) → Q(x))` and `¬Q(a)` | `¬P(a)` |

The restrictions matter: generalizing from a particular observed object is invalid — that is exactly what the course slides prompt you to notice about these four rules. (See the [UT Austin CS311H lecture notes on quantifiers](https://www.cs.utexas.edu/~isil/cs311h-2018/lecture3-6up.pdf) for the arbitrary-object and fresh-name conditions.)

---

## 13. Knowledge Representation

Knowledge representation structures information so programs can use it to solve complex tasks, reason, and make decisions.

### Types of Knowledge

| Type | Description |
|---|---|
| Declarative | Facts about objects |
| Heuristic | Rules of thumb |
| Meta | Knowledge about knowledge |
| Procedural | Rules and procedures |
| Structural | Relationships between objects and concepts |

### Representation Approaches

- **Logic-based** — propositional logic and first-order logic: "All humans are mortal" = `∀x(Human(x) → Mortal(x))`
- **Semantic networks** — nodes (concepts) and labeled links (relationships), e.g. `Cat — is-a → Mammal — is-a → Animal`
- **Frames** — data structures for stereotypical situations with slots and values; **scripts** — sequences of frames for typical activities
- **Production rules** — if-then statements: "If the patient has fever and cough, then consider a respiratory infection"
- **Ontologies** — formal, hierarchical frameworks of concepts and relationships (e.g. medical specialty trees)

**Applications:** medical diagnosis, natural language understanding, robotics, expert systems.

---

## 14. Rule-Based & Expert Systems

### Rule-Based (Production) Systems

- Operate with **condition-action ("if-then") rules**.
- Core components: **knowledge base** (the rules), **inference engine** (applies them), **working memory** (current facts); plus rule engineering tools and an **explanation system**.
- Everyday example: a thermostat that triggers heating at set thresholds.

### Expert Systems

- Emulate human experts using knowledge representation + inference engine + user interface.
- **Knowledge engineers** encode expert knowledge into the knowledge base; users query and receive advice with explanations.
- Classic applications: medical diagnosis, configuration, troubleshooting.

---

## 15. Planning & Problem Solving

- **Planning:** determining actions that transform an **initial state** into a **goal state**.
- **Problem solving:** computational methods and algorithms via **searching**, **reasoning**, and **evaluating** — e.g. the farmer, wolf, goat & cabbage river-crossing puzzle as a state-space search.

### Search Strategies

| Family | Algorithms | Idea |
|---|---|---|
| Uninformed (blind) | Breadth-First (BFS), Depth-First (DFS), Uniform-Cost | No heuristic estimates of distance or cost to the goal — only the problem definition (start state, actions, goal test) ([Cornell CS4700](https://www.cs.cornell.edu/courses/cs4700/2018fa/lectures/pdf/CS4700-03-Search_uninformed_v11.pdf)); BFS explores level by level, DFS follows one branch deeply first |
| Informed (heuristic) | A*, Greedy Best-First | Domain knowledge / heuristics guide the search efficiently |
| Adversarial | Minimax, Alpha-Beta Pruning | Game playing with opposing agents; pruning skips hopeless branches |
| Local | Hill Climbing, Simulated Annealing | Move iteratively to neighboring solutions; optimization without full path planning |

---

## 16. NLP in Symbolic AI

NLP is the subfield of AI focused on the interaction between computers and human language. In Symbolic AI, it uses **formal rules, logic, and symbolic representations** to process natural language.

- **Syntax** — formal grammars (context-free, phrase-structure) define the rules for valid sentences: "The cat chased the mouse."
- **Semantics** — meaning represented via formal logic, semantic networks, or ontologies.
- **Rule-based systems** perform part-of-speech tagging, syntactic parsing, and information extraction (e.g. labeling "the" as a determiner, "fox" as a noun).
- **Sentiment analysis** — rule-based patterns spot sentiment words ("good", "excellent" vs. "bad", "poor").
- **Question answering** — logical inference over knowledge graphs; e.g. medical ontologies of diseases, symptoms, and treatments.
- **Information retrieval** — encode domain knowledge (e.g. legal case law) in structured form, then match queries by inference.

---

## 17. Hands-On: Exact Rules vs. Text Classification

The course slides compare two block-programming implementations of the same four voice commands (fan on / fan off, lamp on / lamp off):

- **Rule-based, exact matching** — rules compare the answer to exact strings: `IF answer = "Fan on" OR "Fan on please" THEN turn the fan on` (same pattern for the other three commands). Brittle — "please turn the fan on" fails to match.
- **Machine learning, text classification** — a trained classifier assigns a label: `IF recognise-text(answer, label) = fan_on THEN turn the fan on` with labels `fan_on`, `fan_off`, `lamp_on`, `lamp_off`. Handles paraphrases, but must be trained and can mislabel.

This is the Symbolic AI vs. ML distinction made concrete.

---

## 18. Sample Learning Materials

From the course slides:

- **UNIX** — software example
- **Weixin (WeChat)** — software example
- **BFs** — algorithms example (the abbreviation is not expanded in the slides)
- YouTube videos and ChatGPT Q&As as supplementary study aids

---

## 19. Self-Check

<details>
<summary>Q1. What is the difference between a program and a process?</summary>

A program is a passive executable file; a process is a running instance of it with its own memory and state.
</details>

<details>
<summary>Q2. How do the hierarchical, network, and relational database models differ structurally?</summary>

Hierarchical: tree — each child has exactly one parent (one-to-many). Network: children may have multiple parents (many-to-many). Relational: data in tables linked by primary/foreign keys.
</details>

<details>
<summary>Q3. Why does binary search require a sorted array?</summary>

The halving step depends on knowing which half can contain the target; without order, half the candidates can't be discarded.
</details>

<details>
<summary>Q4. A linked list has O(1) insertion. What's the catch?</summary>

Only if you already hold the needed links (e.g. the predecessor node); finding that position is O(n).
</details>

<details>
<summary>Q5. Difference between primary key and foreign key?</summary>

A PK uniquely identifies rows in its own table (unique, not-null); an FK references a primary or unique key in another (or the same) table and enforces referential integrity.
</details>

<details>
<summary>Q6. When can a binary search tree take O(n) to search?</summary>

When it is unbalanced/skewed (e.g. inserting sorted data) it degenerates into a linked-list shape. Self-balancing variants (AVL, red-black) keep it O(log n).
</details>

<details>
<summary>Q7. What distinguishes Symbolic AI from machine learning?</summary>

Symbolic AI reasons over explicitly encoded rules and logic (knowledge base + inference engine); machine learning derives patterns from data. Symbolic systems are interpretable but struggle with uncertainty and learning from new data.
</details>

<details>
<summary>Q8. What do Modus Ponens and Modus Tollens let you infer?</summary>

Modus Ponens: from p → q and p, infer q. Modus Tollens: from p → q and ¬q, infer ¬p.
</details>

<details>
<summary>Q9. BFS vs. DFS — how do they traverse a search tree?</summary>

BFS explores level by level (breadth-first); DFS follows one branch to full depth before backtracking.
</details>

---

## Sources

- [Wikipedia — Database model](https://en.wikipedia.org/wiki/Database_model)
- [Microsoft Learn — Primary and foreign key constraints](https://learn.microsoft.com/en-us/sql/relational-databases/tables/primary-and-foreign-key-constraints?view=sql-server-ver17)
- [PostgreSQL SELECT documentation](https://www.postgresql.org/docs/current/sql-select.html)
- [SQLite SELECT documentation](https://sqlite.org/lang_select.html)
- [Interview Cake — Big-O cheat sheet](https://www.interviewcake.com/big-o-cheat-sheet)
- [FaangPrep — Big-O cheat sheet](https://faangprep.com/dsa/big-o-cheat-sheet/)
- [Gera Tools — Data structure complexity reference](https://geratools.com/data-structure-complexity-reference)
- [UT Austin CS311H lecture notes — predicates and quantifiers](https://www.cs.utexas.edu/~isil/cs311h-2018/lecture3-6up.pdf)
- [Cornell CS4700 lecture notes — uninformed search](https://www.cs.cornell.edu/courses/cs4700/2018fa/lectures/pdf/CS4700-03-Search_uninformed_v11.pdf)
- Course slide decks: `chap3-Software-and-Algorithms.pptx`, `chap4-Symbolic-AI-1.pptx` (content from Part II and the Chap 3 outline)

