## E. Master Task List

**Module:** Software and Symbolic AI
**Last updated:** October 22, 2026
**Status values:** not started · in progress · under review · completed
**Members:** Rawa (content lead), Batbaatar (submission and logs), Ochirsukh (coordinator), Myagmarsuren (repository and submission lead), Turmunkh (video lead), Alia (visual design lead). **Lead** = the person who makes sure the task gets done.

> Statuses show our best current estimate. The team should correct them at the first meeting. Deadlines for Stages 2 and 3 are not fixed yet, so later tasks have no dates until we confirm them.

---

## Stage 1 (due October 24, 2026, 23:59 Beijing time)

### 1. Team setup and planning

| ID | Task | Expected result | Responsible | Internal deadline | Status | Depends on |
| --- | --- | --- | --- | --- | --- | --- |
| S1-01 | Hold a team meeting: confirm module (Software and Symbolic AI), team name, and which topics are detailed, medium or brief | Meeting summary saved in `project-management/` | Lead: Ochirsukh; all | Oct 22 | in progress | none |
| S1-02 | Check the GitHub repo: all six members can edit, and the teacher can open it | Repo link works; member list checked | Myagmarsuren | Oct 22 | in progress | none |
| S1-03 | Create the folders: `content/`, `assets/`, `study-guide/`, `slides/`, `video/`, `project-management/` | Folders visible in the repo | Myagmarsuren | Oct 22 | in progress | S1-02 |
| S1-04 | Each member writes 2-3 lines on their strengths and the skills they want to develop | Text ready for plan section A | Each member; lead: Ochirsukh | Oct 22 | not started | none |
| S1-05 | Send the teacher our questions: depth of OS and database topics, search depth, hands-on language, slide 18 logic rules, the mini lecture topic menu | Questions sent; answers written in the project log | Ochirsukh | Oct 22 | not started | none |
| S1-06 | Finish the plan document: sections A, B, C, D and this task list in one file in the format the teacher asks for | Plan file ready to submit | Lead: Ochirsukh; Batbaatar | Oct 23 | in progress | S1-01, S1-04 |

### 2. README and module outline

| ID | Task | Expected result | Responsible | Internal deadline | Status | Depends on |
| --- | --- | --- | --- | --- | --- | --- |
| S1-07 | Fix the README: team name, module name, learners and learning goals matching our module, "where to start" link, progress and remaining work, AI-use note | Finished `README.md` | Lead: Myagmarsuren; Rawa checks | Oct 23 | in progress | S1-01 |
| S1-08 | Check the outline against the lecture slides, open slides 27, 34, 37 and 50 to see the diagrams, and update the status labels | Corrected `content/outline.md` | Lead: Rawa; Batbaatar | Oct 23 | in progress | S1-05 |

### 3. Content: one fully developed topic

We develop **Topic 8, Logic and Reasoning**, in full, because it supports the mini lecture.

| ID | Task | Expected result | Responsible | Internal deadline | Status | Depends on |
| --- | --- | --- | --- | --- | --- | --- |
| S1-09 | Look up and verify definitions of propositions, truth tables, implication, modus ponens and modus tollens in reliable sources | List of checked claims with references | Rawa | Oct 22 | not started | none |
| S1-10 | Write `content/08-logic-and-reasoning.md`: objectives, key terms, explanation, worked example (the pneumonia rule), table, "Try it" activity with its answer, common mistakes, references | Complete topic file | Lead: Rawa; Turmunkh checks the truth tables | Oct 23 | not started | S1-09 |
| S1-11 | Make the truth-table image and the inference diagram, saved in `assets/` and linked by relative path | Images that show correctly in the Markdown | Alia | Oct 23 | not started | S1-10 (draft) |
| S1-12 | Peer review of Topic 8: check definitions, example, answer, that the activity can be done from the text, sources, and image links | Written review note: what was checked, found and fixed | Ochirsukh (reviewer, not the author) | Oct 24, 10:00 | not started | S1-10, S1-11 |
| S1-13 | Fix the problems found in the review | Corrected topic file; note of what changed | Rawa | Oct 24, 12:00 | not started | S1-12 |

### 4. Content: first drafts of other topics

Each draft has objectives, key terms, an explanation, one worked example, a "Try it" activity with its answer, and references. Anyone writing code must run it.

| ID | Task | Expected result | Responsible | Internal deadline | Status | Depends on |
| --- | --- | --- | --- | --- | --- | --- |
| S1-14 | Draft Topic 1: Software and Operating Systems (check the Round Robin example by hand) | `content/01-software-and-operating-systems.md` | Ochirsukh | Oct 23 | in progress | S1-05 |
| S1-15 | Draft Topic 4: Databases and SQL (run every SQL query in SQLite and confirm the results) | `content/04-databases-and-sql.md` | Myagmarsuren | Oct 23 | in progress | S1-05 |
| S1-16 | Draft Topic 5: Algorithms (run the search and sort code, recheck the traces) | `content/05-algorithms.md` | Turmunkh | Oct 23 | in progress | S1-05 |
| S1-17 | Draft Topic 6: Data Structures (run the code, including BFS) | `content/06-data-structures.md` | Batbaatar | Oct 23 | in progress | S1-05 |
| S1-18 | Draft Topic 7: Introduction to Symbolic AI (check the claim about Siri, self-driving cars and computer vision, and rewrite it correctly) | `content/07-intro-to-symbolic-ai.md` | Alia | Oct 23 | not started | S1-05 |
| S1-19 | Cross-check: each member reviews one teammate's draft and writes what they found | One review note per draft | Lead: Ochirsukh; all | Oct 24, 10:00 | not started | S1-14 to S1-18 |
| S1-20 | Fix the problems found in the cross-checks | Corrected files | Each author | Oct 24, 12:00 | not started | S1-19 |

### 5. Records, logs and evidence

| ID | Task | Expected result | Responsible | Internal deadline | Status | Depends on |
| --- | --- | --- | --- | --- | --- | --- |
| S1-21 | Start and update the project log and meeting summaries as work happens | Dated entries in `project-management/` | Lead: Batbaatar | Oct 22, then every day | not started | none |
| S1-22 | Record all significant AI use: date, person, tool, purpose, important prompts and answers, how it was checked, what was changed, what was learned | Entries in the project log and each person's own personal log (personal logs go to the teacher through the submission page, not the public repo) | Each member; lead: Batbaatar | Oct 24, 12:00 | not started | ongoing |
| S1-23 | Each member commits their own work from their own account, with clear commit messages | Commit history that shows who did what | Each member; lead: Myagmarsuren | Oct 24, 10:00 | in progress | S1-10, S1-14 to S1-18 |
| S1-24 | Take readable screenshots: repo overview, commit history, two or three change views, and one review example | Image files with captions | Lead: Batbaatar; Myagmarsuren | Oct 24, 14:00 | not started | S1-23 |
| S1-25 | Write the table of individual contributions: member, files or sections, and evidence | Contribution table | Lead: Batbaatar; each member supplies their own row | Oct 24, 14:00 | not started | S1-23 |

### 6. Building and checking the submission

| ID | Task | Expected result | Responsible | Internal deadline | Status | Depends on |
| --- | --- | --- | --- | --- | --- | --- |
| S1-26 | Download a snapshot of the repo (README, `.md` files and assets) and note the date and latest commit ID | Snapshot folder | Myagmarsuren | Oct 24, 14:00 | not started | S1-13, S1-20 |
| S1-27 | Make a PDF of the rendered content: outline, status, topics, images, tables, questions and answers readable | `content` PDF | Lead: Alia; Myagmarsuren | Oct 24, 16:00 | not started | S1-13, S1-20 |
| S1-28 | Write the submission report: team and module, repo link, snapshot date and commit ID, content status, evidence, contributions, review result, AI-log pointers, next steps | Report in Word or PDF | Lead: Batbaatar | Oct 24, 16:00 | not started | S1-12, S1-24, S1-25 |
| S1-29 | Make `TeamName_Stage1_GitHub_Markdown_V1.zip`, unzip it in a different folder, and check that files open, images show and the structure is clear | Tested ZIP | Lead: Myagmarsuren; Ochirsukh checks | Oct 24, 18:00 | not started | S1-26, S1-27, S1-28 |
| S1-30 | The whole team goes through both quality checklists honestly and fixes gaps | Checklists completed; fixes done | Lead: Ochirsukh; all | Oct 24, 18:00 | not started | S1-29 |
| S1-31 | Submit the plan and the ZIP, and confirm that the uploads were received | Confirmation of both submissions | Lead: Myagmarsuren; Batbaatar | Oct 24, 20:00 | not started | S1-06, S1-30 |

---

## Later stages (deadlines to be added when confirmed)

These tasks are broader for now. We will split them into smaller tasks at the start of each stage.

| ID | Task | Expected result | Responsible | Internal deadline | Status | Depends on |
| --- | --- | --- | --- | --- | --- | --- |
| L-01 | Draft and verify the remaining topics: 2, 3, 9, 10, 11, 12 and 13 | One checked `.md` file per topic | Lead: Rawa; each member takes the topics agreed at the first meeting | TBD | not started | S1-31 |
| L-02 | Settle the accuracy questions: logic rules on slide 18, applications on slide 5, one set of names for inference rules, and run all code | Decisions recorded; corrections made in the Markdown | Rawa; Turmunkh | TBD | not started | S1-05 |
| L-03 | Build the study guide: per topic a summary, glossary, self-check list and 3-4 exercises, with answers in a separate part | Study guide files in `study-guide/` | Lead: Rawa; Alia (layout) | TBD | not started | L-01 |
| L-04 | Build the test bank: about 5 questions per topic, each tagged with its section ID and type, with explained answers | Test bank file | Lead: Turmunkh; each topic author writes the questions for their topic | TBD | not started | L-01 |
| L-05 | Make the slides: one template, then slides for each topic using the planned visuals | Slide deck in `slides/` | Lead: Alia; Batbaatar (content) | TBD | not started | L-01 |
| L-06 | Make the 6 video tutorials: scripts, recording, editing | Videos and scripts in `video/` | Lead: Turmunkh; Alia (visuals); Myagmarsuren (code demos) | TBD | not started | L-01, L-05 |
| L-07 | Prepare the mini lecture: confirm the question is on the topic menu, make the fact and rule cards, practise to 6-7 minutes | Lecture plan, cards, rehearsal notes | Lead: Rawa; Alia (cards); Ochirsukh (timing and practice) | TBD | not started | S1-05, L-03 |
| L-08 | Peer review every resource before it is submitted | Review notes | Lead: Ochirsukh; all | TBD | not started | L-03 to L-07 |
| L-09 | Collect teacher feedback and audience feedback, then revise and note what changed and where | Revision summary | Lead: Ochirsukh; all | TBD | not started | L-08 |
| L-10 | Keep the repo, README, task list and progress notes up to date | Current repo | Myagmarsuren | Every week | not started | none |
| L-11 | Keep the project log, meeting summaries and AI-use records up to date | Current logs | Batbaatar; all members for their own logs | Every week | not started | none |
| L-12 | Each member studies the course content outside our module, using other teams' materials and mini lectures | Short notes in each personal log | Each member | TBD | not started | none |
| L-13 | Package and submit each later stage, checking the files open and the evidence is readable | Submission confirmation | Lead: Myagmarsuren; Batbaatar | TBD | not started | L-03 to L-09 |

