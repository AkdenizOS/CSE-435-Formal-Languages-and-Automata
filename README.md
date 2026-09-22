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
[exams/README.md](exams/README.md).

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
README.md        This page
course-info.md   Syllabus summary, resource map (Sipser page offsets), glossary
weeks/NN-*.md    One file per week: the shared plan on top, everyone's notes below
exams/           Past papers 2019-2024, pattern analysis, midterm and final prep
resources/       Syllabus PDF, books/
```

## Taking notes

Open the week, scroll to the bottom, write under your own heading:

```markdown
## Notes — <Name> (<term>)
### Lecture
### Worked out by hand
### Questions
### Exam-worthy
```

Add your heading below the existing ones and never edit someone else's section —
different sections merge in git without conflicts.

## Who changes what

| What | Who edits it | When |
|------|-------------|------|
| Top of `weeks/NN-*.md` (goals, reading, practice) | **anyone** | Only when the course itself changes — a new topic, a better reading, a correction. |
| `## Notes — <you>` in a week file | **only you** | Every week. |
| `course-info.md`, `exams/README.md` | **anyone** | When you learn something durable: a new exam pattern, a better source. |
| `assignments/<term>-<you>-*` | **only you** | Your assignments, projects, submissions, if the course has them. |
| `resources/<term>/` | **anyone in that term** | Slides and handouts the instructor issued that term. |
| `exams/` | **anyone** | When you get hold of a new paper — blank or answered. Put the writer's surname in the filename (`2025-final-answered-altungoz.pdf`). |
Two students in different years never touch the same file except to improve the
shared plan — which is the point.

## Terms

| Term | Instructor | Schedule | Midterm | Final | Notes |
|------|-----------|----------|---------|-------|-------|
| Fall 2026-2027 | Dr. Öğr. Üyesi Murat Ak | TBD | TBD | TBD | Efe — in every week file |
