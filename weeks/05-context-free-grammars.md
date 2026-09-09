# Week 5 — Context-Free Languages and Grammars

> Syllabus (TR): *İçerikten bağımsız diller ve gramerler*

**Previous:** [Week 4](04-pumping-lemma-regular.md) · **Next:** [Week 6](06-pushdown-automata.md)

## Goals
- Write a CFG for a given language and derive strings from it.
- Detect and remove ambiguity; convert a CFG to Chomsky normal form.

## Key concepts
- CFG as `(V, Σ, R, S)`; derivation, parse tree, leftmost derivation.
- Ambiguity: two distinct parse trees for one string; inherently ambiguous languages.
- **Chomsky normal form**: every rule `A → BC` or `A → a` (plus `S → ε`). Needed for the CYK parser and the CFL pumping lemma proof.
- CFG → CNF procedure: add new start, remove ε-rules, remove unit rules, break up long rules.
- Every regular language is context-free (build a CFG from a DFA).

## Reading

- [Sipser — Ch. 2.1 (context-free grammars)](../resources/books/sipser-introduction-to-the-theory-of-computation-3e.pdf#page=126)

## Practice
- [ ] Convert a grammar to CNF, all four steps by hand
- [ ] Write a CFG for `{aⁱbʲcᵏ | i = j or j = k}` and explain why it is ambiguous
- [ ] Sipser exercises 2.1-2.17

## Checklist
- [ ] Lecture attended
- [ ] Textbook section read
- [ ] Exercises done
- [ ] Notes written below

## My notes

<!-- Lecture: what was actually covered. -->

<!-- Proofs worked out by hand. -->

<!-- Questions to ask the instructor. -->

<!-- Exam-worthy: definitions, theorem statements, proof templates. -->
