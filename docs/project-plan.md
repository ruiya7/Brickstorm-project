# Understanding Software and Symbolic AI: A Beginner's Learning Kit

## Team
- **Team name:** BrickStorm
- **Course:** Foundations of CS & AI, 2026
- **Selected module:** [Symbolic AI and Symbolic AI]

| Member | Role / Responsibility | GitHub username | Student ID |
|--------|-----------------------|-----------------|------------|
| Rashid Rawa | Content Lead | @ruiya7 | 1820262007 |
| Batbaatar Undrakhjargal | Submission and Logs | @una987 | 1820262173 |
| Myagmarsuren Batbileg | CEO | @Monark8599 | 1820262216 |
| Turmunkh Binderiya | Video Lead | @emilysmbb | 1820262220 |
| Alsheryani Alia | Visual Design Lead | @aliaashe | 1820262010 |
| Ochirsukh Bilguun | Coordinator | @Ryo-404 | 1820262182 |

## Purpose
This project teaches **[Software and Symbolic AI]** to beginners. We produce three
connected resources built from one shared Markdown source:
1. **Study Guide**: independent learning with explanations, examples, and exercises
2. **PPT Slides**: visual explanations of the key ideas
3. **Video Tutorials**: short, focused walkthroughs and demonstrations

## Target learners
First-year students with no prior AI background.
After using these materials, learners can explain propositional logic and
evaluate simple logical statements.

## Learning Goals

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

## Scope Boundaries

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

## Planned Learning Resources and Mini Lecture

These are our initial plans. We will revise them as we research, test, and receive feedback.

### Shared Markdown content

**Organization.** The `content/` folder holds one numbered Markdown file per topic, matching the 13 topics in our README:

| Part | Files |
| --- | --- |
| A. Software | `files` |
| B. Algorithms and data structures | `files` |
| C. Symbolic AI | `files` |
| D. Review | `files` |

**One template for every file:**

1. **Learning objectives:** 2-3 "explain" or "do" statements.
2. **Key terms:** each defined once, in plain language, when it first appears.
3. **Explanation:** short sections that move from concrete to formal.
4. **Worked example:** one solved case with labeled steps, so slides and videos can show it one step at a time.
5. **Try it:** a 2-5 minute activity, with the answer given below it.
6. **Common mistakes:** errors beginners typically make. These also become wrong answer options in the test bank.
7. **References:** course slides, textbooks and open sources, each cited.

**Stable section IDs.** Every section has an ID, for example `OS-01 Processes` or `PL-08 Modus ponens`. The study guide, test bank, slides and video scripts all cite these IDs, so when we correct the Markdown we can find every place that needs the same correction.

**Running examples (so the topics connect):**
- **Student records:** tables, SQL queries, sorting and searching (Topics 4-6).
- **Campus map:** a graph of buildings, used first for BFS in Topic 6 and again for route search in Topic 11.
- **Pneumonia rule:** *IF the patient has a fever AND a cough AND difficulty breathing THEN the patient may have pneumonia.* It appears in Topics 7, 8, 9 and 10, so learners watch one idea grow. It is a teaching example, not medical advice.

**Scope (to confirm with the teacher):**
- **Detailed:** Topics 5, 6, 8, 10 and 11.
- **Medium:** Topics 1, 4, 7 and 9.
- **Brief introduction:** Topics 2, 3 and 12.
- **Review:** Topic 13.

### Study Guide and Test Bank

**Study Guide (`study-guide/`).** It follows the topic order. Each chapter has:
- a half-page summary of the concepts,
- a glossary,
- a "Can you explain it?" self-check list,
- 3-4 practice exercises, with answers in a separate section so learners try first.

The last chapter (Hands-on and Review) has mixed problems and a table comparing symbolic AI with learning-based approaches.

**How learners use it:** read the chapter → try the exercises → check the answers → work through the self-check list.

**Test Bank.** About five questions per topic (roughly 65 in total). Each question is tagged with its section ID and a type: recall, application or interpretation. Question types:
- multiple choice, with wrong options taken from the Common mistakes lists (for example, confusing "if p then q" with "if q then p"),
- trace-the-steps questions (Round Robin scheduling, sorting, BFS, forward chaining),
- short SQL queries,
- truth-table completion,
- "Which conclusion follows from these rules?",
- short answers (for example, "Name one limitation of symbolic AI and give an example").

Each answer explains why it is correct and names the section to reread. Learners study, take a low-stakes quiz, and use the tags to decide what to revisit.

### PPT Slides

Each slide carries one idea. Visuals add something the text does not, instead of repeating it.

| Topic area | Planned visuals |
| --- | --- |
| Software and OS | Layer diagram (hardware → OS → apps); process-state diagram; paging diagram |
| Languages and engineering | Compiler vs interpreter flow; waterfall vs agile timeline |
| Databases | Two linked tables, with the JOIN result highlighted |
| Algorithms | Sorting shown step by step; binary search halving a list |
| Data structures | Pictures of stack, queue, linked list, tree and graph |
| Logic | Truth tables filled in row by row; inference diagram (facts + rules → inference engine → conclusion) |
| Knowledge and rules | Semantic network (Cat → is-a → Mammal); frame with slots; pneumonia rule traced with animation |
| Search and language | BFS and DFS on the same tree with visit order numbered; parse tree for "The cat chased the mouse" |
| Every topic | A recap slide matching the study guide summary |

### Video Tutorials

Each video runs about 4-6 minutes. We chose topics where narration and a live demonstration help most, because the learner can pause and replay.

| # | Tutorial | What the demonstration shows |
| --- | --- | --- |
| 1 | Inside an operating system | Process states and Round Robin scheduling, animated |
| 2 | Your first SQL queries | Typing SELECT and JOIN queries on the student tables and reading the results |
| 3 | Sorting and searching step by step | Bubble sort and binary search traced live |
| 4 | Truth tables and modus ponens | Building a table, and why "false → anything" is true |
| 5 | Building a tiny rule-based system | Screen recording of a short Python program: facts and rules in, conclusion out |
| 6 | BFS vs DFS (optional) | Both searches animated on the campus map |

### Live Mini Lecture

**Question:** *How can a computer reach a conclusion from IF-THEN rules?* (Topics 8 and 10)

**Why it matters:** This is the core idea of symbolic AI: explicit knowledge plus a reasoning step, with no training data. It also connects the two halves of our module, because the reasoning is carried out by a program built from the algorithms and data structures we teach in Topics 5 and 6.

**Initial plan (about 6-7 minutes):**
1. **Hook:** show the pneumonia rule and ask, "If a patient has all three symptoms, what should the system say, and why?"
2. **Explain:** one diagram of facts, rules and the inference engine, then modus ponens in one sentence.
3. **Audience activity:** hand out fact cards and rule cards. Volunteers act as the inference engine and apply rules until no new facts appear, so the class sees forward chaining happen.
4. **Trap question:** "The system concludes pneumonia is *possible*. Does that mean the patient *has* pneumonia?" This separates valid reasoning from the mistake of affirming the consequent, and leads into the limits of symbolic AI.
5. **Quick check:** a two-question poll.

*To confirm:* whether this question is on the teacher's topic menu.

### How the resources support one another

- **Markdown is the source of truth.** The guide, test bank, slides and video scripts all draw from it and cite the same section IDs.
- **Slides** supply the shared visuals, which reappear in the videos and the lecture.
- **Videos** demonstrate what slides can only sketch, such as running a query or a rule-based program.
- **Study guide and test bank** let learners practice and self-check, and each item links back to a section, slide or video.
- **The mini lecture** is a small version of the whole project: one question, taught with a diagram, an activity and a check for understanding.

### Content accuracy checks before production

We will check these during the Markdown review so errors do not spread into all three resources:
- **Generalization rules (Symbolic AI slides 17-18):** universal generalization from a single instance is not valid without extra conditions. We will state this rather than copy the rule.
- **Applications (slide 5):** autonomous cars and computer vision are listed as symbolic AI applications, but both rely heavily on learning-based methods. We will check sources and qualify the claim.
- **Names of inference rules (slides 17 and 20):** the slides use different names. We will choose one convention before writing the glossary.
- **Software topics:** every code example and worked trace (scheduling, sorting, BFS) will be run or recalculated by a second team member.

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



