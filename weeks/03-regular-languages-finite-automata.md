# Week 3 — Regular Languages and Finite Automata

> Syllabus (TR): *Düzenli Diller, Sonlu Otomatlar*

**Previous:** [Week 2](02-mathematical-preliminaries.md) · **Next:** [Week 4](04-pumping-lemma-regular.md)

## Goals
- Build a DFA or NFA for a given language and state its formal 5-tuple.
- Convert NFA → DFA by subset construction; convert regex ↔ finite automaton.
- Apply closure properties (union, concatenation, star, intersection, complement).

## Key concepts
- DFA as `(Q, Σ, δ, q₀, F)`; the language recognized, `L(M)`.
- NFA `(Q, Σ, δ, q₀, F)` with `δ: Q × Σ_ε → P(Q)`; nondeterminism as parallel guessing.
- **Subset construction**: every NFA has an equivalent DFA — worst case `2ⁿ` states.
- Regular expressions; Kleene's theorem: regex ≡ NFA ≡ DFA.
- GNFA and the state-elimination method (DFA → regex).
- Closure under ∪, ∘, *, ∩, complement — proved by construction on automata.

## Reading

- [Sipser — Ch. 1.1 (finite automata)](../resources/books/sipser-introduction-to-the-theory-of-computation-3e.pdf#page=55)
- [Sipser — Ch. 1.2 (nondeterminism)](../resources/books/sipser-introduction-to-the-theory-of-computation-3e.pdf#page=71)
- [Sipser — Ch. 1.3 (regular expressions)](../resources/books/sipser-introduction-to-the-theory-of-computation-3e.pdf#page=87)

## Practice
- [ ] Subset construction on a 3-state NFA by hand
- [ ] State elimination to get a regex from a DFA
- [ ] Sipser exercises 1.1-1.21

## Checklist
- [ ] Lecture attended
- [ ] Textbook section read
- [ ] Exercises done
- [ ] Notes written below

---

Your own notes for this week go in `terms/<your-term>/notes/week-03.md`, not here.
This file is the shared plan — improve it if the course changes, but keep it general.
