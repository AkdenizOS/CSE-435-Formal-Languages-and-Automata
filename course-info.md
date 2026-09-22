# CSE 435 — Syllabus Summary

Source: [`resources/CSE435-syllabus.pdf`](resources/CSE435-syllabus.pdf) (official, Turkish).

| Field | Value |
|-------|-------|
| Code | CSE 435 |
| Title | Formal Languages and Automata |
| Semester | 7 |
| T+U | 3 · Credits 3 · ECTS 6 |
| Type | **Compulsory** (Zorunlu) |
| Language | English |
| Prerequisites | CSE 221 and CSE 222 |
| Coordinator | Prof. Dr. Melih Günay |
| Instructor | Dr. Öğr. Üyesi Murat Ak |

## Aim

Teach the fundamental concepts of formal languages, automata and computation
theory; enable students to analyze models of computation through regular
languages, context-free languages and Turing machines.

## Content

Alphabets, strings and languages; finite automata; regular expressions and regular
languages; the pumping lemma; context-free grammars and languages; normal forms;
pushdown automata; Turing machines; decidability and the limits of computability.

## Learning outcomes

- **Ö01** — Explains basic concepts of formal languages, alphabets, strings and models of computation.
- **Ö02** — Explains the relationship between regular languages, finite automata and regular expressions.
- **Ö03** — Constructs a suitable finite automaton, regular expression or context-free grammar for a given language.
- **Ö04** — Analyzes language properties using the pumping lemma, closure properties and normal forms.
- **Ö05** — Evaluates the theoretical limits of computation using Turing machines and decidability.
- **Ö06** — Distinguishes the classes P, NP and NP-complete; analyzes basic NP-completeness proofs using polynomial-time reduction.

## Content distribution

| Area | % |
|------|---|
| Mathematics and basic sciences | 40 |
| Engineering sciences | 40 |
| Field knowledge | 20 |

## Assessment

| Component | Count | Weight |
|-----------|-------|--------|
| Midterm | 1 | 40% |
| Final | 1 | 60% |

## Workload (ECTS 6 = 180 hours)

| Activity | Count | Hours | Total |
|----------|-------|-------|-------|
| Lectures | 14 | 3 | 42 |
| Outside-class study | 14 | 6 | 84 |
| Midterm prep | 1 | 24 | 24 |
| Final prep | 1 | 30 | 30 |
| **Total** | | | **180** |

Note the 6 hours/week of outside-class study — twice the lecture time, and the
highest of any course this semester.

## Weekly topics

1. Course information and rules, overview of topics
2. Mathematical preliminaries
3. Regular languages, finite automata
4. Pumping lemma for regular languages
5. Context-free languages and grammars
6. Pushdown automata
7. Pumping lemma for context-free languages
8. Turing machines
9. Variants of Turing machines
10. Decidability
11. Undecidability
12. Reducibility
13. NP and NP-completeness
14. Advanced topics in complexity

## References

- Hopcroft, Motwani & Ullman, *Introduction to Automata Theory, Languages, and Computation* (cited by the syllabus).
- Taught at the board; studied from the textbook.

This repository uses **Sipser, *Introduction to the Theory of Computation* (3rd ed.)**
instead — it matches the weekly topic order more closely. See
[Resource Map](#resource-map) below.

## Resource Map

### Textbook mismatch, and why Sipser is used

The syllabus cites Hopcroft-Motwani-Ullman. This repository has Sipser 3rd edition.
The weekly topics map onto Sipser almost one to one, so every reading link in the
week notes points at Sipser with an exact page.

| Week | Topic | Sipser |
|------|-------|--------|
| 1 | Course overview | Ch. 0.1 |
| 2 | Mathematical preliminaries | Ch. 0.2-0.4 |
| 3 | Regular languages, finite automata | Ch. 1.1-1.3 |
| 4 | Pumping lemma (regular) | Ch. 1.4 |
| 5 | Context-free grammars | Ch. 2.1 |
| 6 | Pushdown automata | Ch. 2.2, 2.4 |
| 7 | Pumping lemma (CFL) | Ch. 2.3 |
| 8 | Turing machines | Ch. 3.1 |
| 9 | Variants of TMs | Ch. 3.2-3.3 |
| 10 | Decidability | Ch. 4.1 |
| 11 | Undecidability | Ch. 4.2 |
| 12 | Reducibility | Ch. 5.1-5.3 |
| 13 | NP and NP-completeness | Ch. 7.1-7.5 |
| 14 | Advanced complexity | Ch. 8, 9 |

Sipser page offset: **printed page + 24 = PDF page** (verified on printed 36, 66, 126).
The week notes' `#page=` links already have this applied.

### Files

| File | Source |
|------|--------|
| `resources/CSE435-syllabus.pdf` | Official Akdeniz University syllabus |
| `resources/books/sipser-introduction-to-the-theory-of-computation-3e.pdf` | Sipser, 3rd ed., 482 pp. |
| `exams/*.pdf` | Seven past papers, 2019-2024 — see [exams/README.md](exams/README.md) |

### Not in this repository

- Hopcroft, Motwani & Ullman — the syllabus's cited textbook. Sipser covers the same
  material; get HMU only if the instructor's notation follows it.

## Glossary — Turkish ↔ English

The syllabus is Turkish, the course and exams are English.

| Turkish | English |
|---------|---------|
| biçimsel dil | formal language |
| alfabe / dizgi | alphabet / string |
| boş dizgi | empty string (ε) |
| sonlu otomat | finite automaton |
| belirlenimci / belirlenimci olmayan | deterministic / nondeterministic |
| düzenli dil | regular language |
| düzenli ifade | regular expression |
| şişirme lemması / pompala lemması | pumping lemma |
| kapanış özellikleri | closure properties |
| bağlamdan bağımsız dil (içerikten bağımsız) | context-free language |
| gramer / dilbilgisi | grammar |
| türetme | derivation |
| ayrıştırma ağacı | parse tree |
| belirsizlik | ambiguity |
| normal biçim | normal form |
| yığıt otomatı / aşağı ittirme otomatı | pushdown automaton |
| Turing makinesi | Turing machine |
| yapılandırma | configuration |
| tanınabilir | recognizable |
| karar verilebilirlik | decidability |
| karar verilemezlik | undecidability |
| indirgenebilirlik | reducibility |
| köşegenleştirme | diagonalization |
| durma problemi | halting problem |
| hesaplanabilirlik | computability |
| karmaşıklık | complexity |
| NP-tamlık | NP-completeness |
| polinom zamanda indirgeme | polynomial-time reduction |
| doğrulayıcı | verifier |
