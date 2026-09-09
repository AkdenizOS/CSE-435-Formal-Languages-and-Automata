# Week 11 — Undecidability

> Syllabus (TR): *Karar verilemezlik*

**Previous:** [Week 10](10-decidability.md) · **Next:** [Week 12](12-reducibility.md)

## Goals
- Prove `A_TM` is undecidable by diagonalization.
- Explain why a language can be recognizable but not decidable.

## Key concepts
- **`A_TM = {⟨M,w⟩ | M is a TM that accepts w}` is undecidable** — the halting problem.
- Proof by **diagonalization**: assume a decider `H`, build `D` that does the opposite of `H(⟨M,⟨M⟩⟩)`, run `D` on `⟨D⟩` → contradiction.
- Countability: `Σ*` is countable, the set of languages is uncountable ⇒ some languages have no TM at all.
- **`A_TM` is Turing-recognizable but not decidable**; its complement is not even recognizable.
- `L` decidable ⟺ `L` and `L̄` are both Turing-recognizable — the co-recognizability theorem.

## Reading

- [Sipser — Ch. 4.2 (undecidability)](../resources/books/sipser-introduction-to-the-theory-of-computation-3e.pdf#page=225)

## Practice
- [ ] Reproduce the diagonalization for `A_TM` from memory
- [ ] Prove `\overline{A_TM}` is not Turing-recognizable
- [ ] Sipser exercises 4.11-4.28

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
