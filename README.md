# CSE 435 — Formal Languages and Automata

Akdeniz University, Faculty of Engineering, Computer Engineering (English)
Semester 7 · 3 credits · 6 ECTS · **Compulsory** · Language: English
Prerequisites: CSE 221, CSE 222

**Coordinator:** Prof. Dr. Melih Günay · **Instructor:** Dr. Öğr. Üyesi Murat Ak

## Grading

| Component | Count | Weight |
|-----------|-------|--------|
| Midterm | 1 | **40%** |
| Final | 1 | **60%** |

No assignments, no quizzes, no project. The whole grade is two exams, so past
papers are the most valuable material in this repository — see
[docs/exam-patterns.md](docs/exam-patterns.md).

## Weekly plan

| # | Topic | Note |
|---|-------|------|
| 1 | Course overview | [weeks/01](weeks/01-course-overview.md) |
| 2 | Mathematical preliminaries | [weeks/02](weeks/02-mathematical-preliminaries.md) |
| 3 | Regular languages, finite automata | [weeks/03](weeks/03-regular-languages-finite-automata.md) |
| 4 | Pumping lemma for regular languages | [weeks/04](weeks/04-pumping-lemma-regular.md) |
| 5 | Context-free grammars | [weeks/05](weeks/05-context-free-grammars.md) |
| 6 | Pushdown automata | [weeks/06](weeks/06-pushdown-automata.md) |
| 7 | Pumping lemma for CFLs | [weeks/07](weeks/07-pumping-lemma-cfl.md) |
| 8 | Turing machines | [weeks/08](weeks/08-turing-machines.md) |
| 9 | Variants of Turing machines | [weeks/09](weeks/09-turing-machine-variants.md) |
| 10 | Decidability | [weeks/10](weeks/10-decidability.md) |
| 11 | Undecidability | [weeks/11](weeks/11-undecidability.md) |
| 12 | Reducibility | [weeks/12](weeks/12-reducibility.md) |
| 13 | NP and NP-completeness | [weeks/13](weeks/13-np-completeness.md) |
| 14 | Advanced topics in complexity | [weeks/14](weeks/14-advanced-complexity.md) |

## Textbook

The syllabus cites **Hopcroft, Motwani & Ullman**, but this repository has
**Sipser, _Introduction to the Theory of Computation_ (3rd ed.)**, which follows
the weekly topic order almost chapter for chapter. Every reading link in the week
notes points at the exact Sipser page.

## Layout

```
docs/            Syllabus summary, exam pattern analysis, glossary
weeks/NN-*.md    One note per week: goals, concepts, reading, practice, my notes
exams/past/      Past exam papers, 2019-2024 (the archive)
exams/midterm/   My midterm preparation
exams/final/     My final preparation
resources/       Syllabus PDF, Sipser
```

## Who changes what

| File | Who edits it | When |
|------|-------------|------|
| `weeks/NN-*.md` | **anyone** | Only when the course itself changes — a new topic, a better reading, a correction. Never for personal notes. |
| `docs/*.md` | **anyone** | When you learn something durable: a new exam pattern, a better source. |
| `terms/<your-term>/notes/week-NN.md` | **only you** | Every week. This is your notebook. |
| `terms/<your-term>/` | **only you** | Your slides, labs, assignments, submissions. |
| `exams/past/<term>/` | **anyone** | When you get hold of a new paper. |

Two students in different years never touch the same file except to improve the
shared plan — which is the point.
