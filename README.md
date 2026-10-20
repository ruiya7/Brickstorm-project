# Understanding Software and Symbolic AI: A Beginner's Learning Kit

## Team
- **Team name:** [https]
- **Course:** Foundations of CS & AI, 2026
- **Selected module:** [Symbolic AI and Symbolic AI]

| Member | Role / Responsibility | GitHub username | Student ID |
|--------|-----------------------|-----------------|------------|
| Rashid Rawa | Content Lead | @ruiya7 | 1820262007 |
| Batbaatar Undrakhjargal | Submission and Logs | @una987 | 1820262173 |
| Myagmarsuren Batbileg | Repository and Submission Lead | @Monark8599 | 1820262216 |
| Turmunkh Binderya | Video Lead | @emilysmbb | 1820262220 |
| Alsheryani Alia | Visual Design Lead | @aliaashe | 1820262010 |
| Ochirsukh Bilguun | Coordinator | @Ryo-404 | 1820262182 |

## Purpose
This project teaches **[Software and Symbolic AI]** to beginners. We produce three
connected resources built from one shared Markdown source:
1. **Study Guide**: independent learning with explanations, examples, and exercises
2. **PPT Slides**: visual explanations of the key ideas
3. **Video Tutorials**: short, focused walkthroughs and demonstrations

## Intended learners
[First-year students with no prior AI background.
After using these materials, learners can explain propositional logic and
evaluate simple logical statements.]

## Learning objectives

By the end of this project, learners should be able to:

1. Distinguish system software from application software and describe what an operating system does.
2. Explain how programming languages, software engineering practices, and databases support software development.
3. Describe basic algorithms (searching, sorting, recursion) and common data structures.
4. Explain what Symbolic AI is and how it represents knowledge using logic, facts, and rules.
5. Explain how rule-based systems and search algorithms reach conclusions or solve problems.
6. Identify real-world applications, advantages, and limitations of Symbolic AI.

## Repository structure
| Folder / file | What you'll find |
|---------------|------------------|
| `content/` | Shared Markdown content, which all three resources are based on |
| `assets/` | Images, diagrams, and example files |
| `study-guide/` | Study guide files |
| `slides/` | PPT slides |
| `video/` | Scripts, storyboards, and links to videos |
| `project-management/` | Project plan, task list, project log, meeting summaries |

**Where to start:** read `content/01-[...].md`, then see the study guide.

## Topics

| # | Topic |
|---|-------|
| 1 | Software Overview and Operating Systems |
| 2 | Programming Languages |
| 3 | Software Engineering |
| 4 | Databases and SQL |
| 5 | Algorithms |
| 6 | Data Structures |
| 7 | Introduction to Symbolic AI |
| 8 | Logic and Reasoning |
| 9 | Knowledge Representation |
| 10 | Rule-Based and Expert Systems |
| 11 | Planning and Search |
| 12 | Symbolic NLP |
| 13 | Hands-on and Review |

**Remaining**
- [ ] Review and verify Markdown content
- [ ] Produce study guide, slides, and videos
- [ ] Test activities and collect feedback
- [ ] Rehearse the live mini lecture

## AI use
Significant AI use is recorded in

# Module Content Outline: Software and Symbolic AI

**Module:**

## 1. The storyline: why these two chapters form one resource

The module answers one question in three steps:

> **How do computers run programs, how do those programs solve problems, and how can software be made to reason with explicit knowledge?**

| Part | Question | Chapters |
| --- | --- | --- |
| **A. Software** | What is software, and how is it run, written, built and stored? | Chap 3 |
| **B. Algorithms and data structures** | How do programs solve problems efficiently? | Chap 3 |
| **C. Symbolic AI** | How can software reason using logic, knowledge, rules and search? | Chap 4 |
| **D. Integration** | How do the pieces combine in one working system? | Both |


### Cross-chapter connections

| Earlier idea (Part A or B) | Reappears in Part C as |
| --- | --- |
| Graphs, trees, BFS/DFS, queues and stacks | State-space search, uninformed search, parse trees, semantic networks and ontologies |
| Recursion and base cases | Logical inference chains, minimax, parsing nested sentences |
| Pseudocode and algorithm properties | Search algorithms (BFS, A*) and inference procedures |
| Relational databases and tables | Knowledge bases, knowledge graphs, facts and rules |
| SQL as a *declarative* language | Rules as declarative knowledge |
| Programming language syntax and compilers | Formal grammars for natural language |
| Software engineering: modularity, testing, maintenance | Expert systems: knowledge base vs inference engine, testing and maintaining rules |
| Process scheduling (queues) | Planning as choosing sequences of actions |


## 2. Target learners and prerequisites

**Target learners:** first-year or non-specialist students meeting these topics for the first time.

**Assumed:** basic computer use; everyday if-then reasoning; high-school algebra.
**Not assumed:** programming experience, formal logic notation, AI terminology.

**Internal prerequisites (learning order matters):**
- Part B (graphs, recursion, queues) before Part C search and inference.
- Part A databases (tables, declarative queries) helps with Part C knowledge representation.
- Propositional logic before predicate logic; logic before rule-based systems.


## 3. Intended learning outcomes

After using our materials, a beginner should be able to:

**Software and algorithms**
1. Distinguish system software from application software, and explain what an operating system does (processes, memory).
2. Compare programming language categories, including compilers and interpreters.
3. Describe common software development models and basic quality assurance.
4. Explain the relational model and write simple SQL queries.
5. State the properties of an algorithm, trace basic sorting and searching, and compare iteration with recursion.
6. Choose among arrays, linked lists, stacks, queues, trees and graphs for a simple task.

**Symbolic AI**
7. Explain what symbolic AI (GOFAI) is, with its strengths and limitations.
8. Translate simple statements into propositional and predicate logic, and apply basic inference rules.
9. Compare knowledge representation methods (logic, semantic networks, frames/scripts, rules, ontologies).
10. Trace a small rule-based/expert system.
11. Describe planning as search and compare search strategies.
12. Explain how symbolic methods process natural language, and where they fail.

**Integration**
13. Explain how symbolic AI depends on ideas from software and algorithms (using at least three of the connections above).

---

## 4. Learning sequence

# Part A: Software (Chap 3)

### Unit 1: Software overview and operating systems
- **Subtopics:** system vs application software; OS role; OS evolution; process management (states, scheduling, deadlock); memory management (paging, virtual memory); UNIX case study
- **Activities:** list running processes on your own computer and classify them; hand-trace Round Robin scheduling; research brief on UNIX
- **Status:** `Drafted` (`chap3-study-guide.md` §1.1-1.2), not yet `Checked`
- **Gaps:** diagrams needed (process states, paging); depth expected by the teacher unknown

### Unit 2: Programming languages
- **Subtopics:** evolution; categories (compiled vs interpreted; procedural, object-oriented, functional, declarative); common features
- **Activities:** same task in two styles; Python Tutor walkthrough
- **Status:** `Drafted` (§1.3), not yet `Checked`
- **Gaps:** "features" subtopic is brief; link the declarative paradigm to Part C rules

### Unit 3: Software engineering
- **Subtopics:** development phases; process models (waterfall, iterative, agile, spiral); modularity (cohesion, coupling); quality assurance (testing levels, review, version control)
- **Activities:** write unit tests for a small function; connect to our own GitHub workflow
- **Status:** `Drafted` (§1.4), not yet `Checked`
- **Gaps:** consider a short case example of a failed project

### Unit 4: Databases
- **Subtopics:** why databases; database models; relational model (tables, keys); SQL (SELECT, INSERT, JOIN, WHERE)
- **Activities:** run the student/enrollment queries (SQLBolt or SQLite)
- **Status:** `Drafted` (§1.5), not yet `Checked`
- **Gaps:** sample database file needed; decide whether to mention normalization (suggested: brief mention only)

# Part B: Algorithms and data structures (Chap 3)

### Unit 5: Algorithms, sorting, searching, iteration and recursion
- **Subtopics:** algorithm properties; representation (pseudocode, flowcharts); Big-O (brief); linear and binary search; bubble, selection, insertion, merge sort; iteration vs recursion
- **Activities:** trace sorts by hand; count comparisons in binary search; factorial both ways
- **Status:** `Drafted` (§2.1-2.3), not yet `Checked`
- **Gaps:** confirm all code runs; flowchart diagram needed

### Unit 6: Data structures
- **Subtopics:** arrays, records, linked lists, stacks, queues, trees, binary trees (traversals), graphs (adjacency list, BFS, DFS)
- **Activities:** VisuAlgo exploration; run BFS on the campus map
- **Status:** `Drafted` (§2.4), not yet `Checked`
- **Gaps:** DFS code example not yet written; diagrams needed

# Part C: Symbolic AI (Chap 4)

### Unit 7: What is symbolic AI?
- **Subtopics:** definition and GOFAI; symbols and explicit rules; example IF-THEN rule; applications; benefits (interpretability, knowledge representation, flexibility); limitations (incomplete knowledge, scalability, uncertainty, no learning)
- **Activities:** discuss the diagnosis rule; classify real tools as rule-driven vs learning-driven
- **Status:** `Outline only`
- **Gaps:** the slides list Siri, autonomous cars and computer vision as symbolic AI applications; modern versions mostly use machine learning, so this claim must be **checked and qualified**. Also need a note on why symbolic AI declined and how it relates to machine learning.

### Unit 8: Propositional logic
- **Subtopics:** propositions; AND/OR/NOT; truth tables; equivalences (De Morgan, double negation); implication and biconditional; inference rules (modus ponens, modus tollens); role in AI
- **Activities:** truth table practice; Python truth-table generator; deduction puzzles
- **Status:** `Outline only`
- **Gaps:** modus ponens and modus tollens are named but **not defined or illustrated** on the slides; address confusing an implication with its converse

### Unit 9: Predicate (first-order) logic
- **Subtopics:** predicates; ∀ and ∃; formalizing English; connectives; instantiation and generalization; universal modus ponens/tollens
- **Activities:** translation exercises; Socrates-style syllogism; error-spotting
- **Status:** `Outline only`
- **Gaps and issues to verify:**
  - Slide 18 asks "Do you see anything strange for the above 4 rules?" without answering. The rules as written are **unsafe without conditions** (generalization is valid only for an arbitrary element; existential instantiation needs a fresh constant).
  - Slide 16's last example leaves `x` outside the quantifier's scope (intentional trap or error?).
  - Slide 19's `∀n(Even(n))` is false, so it could be a true/false question.
  - Existential instantiation/generalization appears twice (slides 17-18 and 20); needs one clean treatment.

### Unit 10: Knowledge representation
- **Subtopics:** what KR is; logic-based; semantic networks; frames and scripts; production rules; ontologies; applications
- **Activities:** draw a semantic network of the family example; build a frame and a script for a restaurant; compare which representation suits which problem; store the family facts in SQL tables and compare
- **Status:** `Outline only`
- **Gaps:** slide 27 has no extractable text (probably a diagram); frames/scripts and ontologies need our own worked examples

### Unit 11: Rule-based and expert systems
- **Subtopics:** condition-action rules; knowledge base; inference engine; user interface; how an expert system emulates an expert; software engineering view (modular design, testing and maintaining rules)
- **Activities:** hand-trace forward chaining; Python mini expert system for the diagnosis assistant
- **Status:** `Outline only`
- **Gaps:** slides do not explain forward vs backward chaining or conflict resolution; scope question for the teacher

### Unit 12: Planning and problem solving (search)
- **Subtopics:** state space, actions, goal; uninformed search (BFS, DFS, uniform-cost); informed search (A*, greedy best-first, heuristics); adversarial search (minimax, alpha-beta); local search (hill climbing, simulated annealing)
- **Activities:** BFS vs DFS on the campus map (reusing Unit 6); route planning with a heuristic; tic-tac-toe minimax
- **Status:** `Outline only`
- **Gaps:** slides 34 and 37 appear to be diagrams with no text; slides give one-line descriptions only. Suggested depth: **detail for BFS, DFS and A\***, **brief introduction for the rest** (needs teacher confirmation).

### Unit 13: Symbolic natural language processing
- **Subtopics:** what NLP is; syntax (context-free grammars, parse trees); semantics (logic, semantic networks, ontologies); rule-based tagging, parsing and extraction; logic over language; applications (rule-based sentiment analysis, question answering, information retrieval)
- **Activities:** parse "The cat chased the mouse" by hand; write sentiment word rules and test them on short reviews; show where rules fail (sarcasm, negation, ambiguity)
- **Status:** `Outline only`
- **Gaps:** slides contain no actual grammar rules, so we must write a small grammar; the legal-retrieval example is generic and should be verified before reuse

# Part D: Integration

### Unit 14: Capstone and wrap-up
- **Subtopics:** how the parts combine; strengths and limits of symbolic approaches; comparison with learning-based approaches (briefly)
- **Activities:** a short coding lab combining a rule base (Unit 11) with a search or database component; reflective questions on the cross-chapter connections
- **Status:** `Outline only`
- **Gaps:** the "Hands on" slide (50) is **empty**, so the lab design is entirely ours; choose a language (suggest Python)

---

## 6. Planned question types (test bank)

- Multiple choice on definitions and concepts
- Trace-the-algorithm questions (scheduling, sorting, BFS, forward chaining)
- Write a short SQL query
- Translate English ↔ logic; truth tables
- Short explanation ("why does symbolic AI struggle with ambiguity?")
- Spot-the-error questions
- **Integration questions** ("how does BFS from Chap 3 appear in AI planning?")

**Status:** `Outline only` for the bank overall. Chap 3 check questions with answers exist in the study guide and can seed it.

## 7. Development status summary

| Part | Units | Status |
| --- | --- | --- |
| A. Software | 1-4 | `Drafted` (study guide), none `Checked` |
| B. Algorithms and data structures | 5-6 | `Drafted`, none `Checked` |
| C. Symbolic AI | 7-13 | `Outline only` |
| D. Integration | 14 | `Outline only` |
| Test bank | n/a | `Outline only` |

**Imbalance:** Chap 3 is drafted and Chap 4 is not, so the next writing effort should go to Part C.

## 8. Gaps and uncertainties

| Issue | Why it matters | Action |
| --- | --- | --- |
| Chap 3 slides are bullet points only, so expected depth is unknown | We may over- or under-teach OS and databases | Ask the teacher |
| Balance between Parts A/B and Part C | Chap 4 has more conceptual material; Chap 3 is broad | Agree a rough proportion as a team |
| Slides 27, 34, 37, 50 have no extractable text | May contain key diagrams or the lab | Open the original slides |
| Slide 18 question and unsafe generalization rules | Risk of teaching incorrect logic | Research, then check with the teacher |
| Modus ponens/tollens undefined | Core inference rules | Write worked examples |
| Applications claimed as symbolic AI (Siri, cars, vision) | May be outdated or misleading | Verify and qualify |
| Depth of search algorithms and chaining methods | Scope control | Ask the teacher |
| Part A and B content drafted but unchecked | Possible errors in code and traces | Second member reviews and runs all code |
| Cross-chapter connections are our own synthesis | Not in the slides; must be accurate | Review and confirm with the teacher |





