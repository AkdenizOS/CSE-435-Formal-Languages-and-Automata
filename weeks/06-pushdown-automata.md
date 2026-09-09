# Week 6 — Pushdown Automata

> Syllabus (TR): *Aşağı ittirme otomatları*

**Previous:** [Week 5](05-context-free-grammars.md) · **Next:** [Week 7](07-pumping-lemma-cfl.md)

## Goals
- Build a PDA for a given CFL and trace its computation.
- Explain the CFG ↔ PDA equivalence in both directions.

## Key concepts
- PDA `(Q, Σ, Γ, δ, q₀, F)` = NFA + a stack; `δ: Q × Σ_ε × Γ_ε → P(Q × Γ_ε)`.
- The stack is what buys you unbounded counting — this is exactly what a DFA lacked in week 4.
- **CFG ≡ PDA**: convert a grammar to a PDA that simulates leftmost derivations; convert a PDA to a grammar via `A_pq` variables.
- Nondeterministic PDAs are strictly stronger than deterministic ones (unlike finite automata).
- DCFL and why real parsers care (LR parsing).

## Reading

- [Sipser — Ch. 2.2 (pushdown automata)](../resources/books/sipser-introduction-to-the-theory-of-computation-3e.pdf#page=135)
- [Sipser — Ch. 2.4 (deterministic context-free languages)](../resources/books/sipser-introduction-to-the-theory-of-computation-3e.pdf#page=154)

## Practice
- [ ] PDA for `{0ⁿ1ⁿ}` and for `{ww^R}`, with full transition traces
- [ ] Convert a small CFG to a PDA
- [ ] Sipser exercises 2.18-2.30

## Checklist
- [ ] Lecture attended
- [ ] Textbook section read
- [ ] Exercises done
- [ ] Notes written below

---

Your own notes for this week go in `terms/<your-term>/notes/week-06.md`, not here.
This file is the shared plan — improve it if the course changes, but keep it general.
