# Week 13 — NP and NP-Completeness

> Syllabus (TR): *NP, ve NP-Tamlık*

**Previous:** [Week 12](12-reducibility.md) · **Next:** [Week 14](14-advanced-complexity.md)

## Goals
- Define P, NP, and NP-completeness precisely.
- Prove a problem is NP-complete by polynomial-time reduction from a known NP-complete problem.

## Key concepts
- Big-O on TMs; `TIME(t(n))`; **P** = decidable in polynomial time on a deterministic TM.
- **NP** = verifiable in polynomial time ≡ decidable in polynomial time on a nondeterministic TM. The verifier definition is the one to use in proofs.
- **Polynomial-time reduction** `A ≤_p B`.
- **NP-complete** = in NP **and** every NP language reduces to it. Both halves must be shown.
- **Cook-Levin theorem**: SAT is NP-complete — the root of the whole reduction tree.
- Standard chain: SAT → 3SAT → CLIQUE / VERTEX-COVER / HAMPATH / SUBSET-SUM.
- P vs NP: `P ⊆ NP`; equality unknown.

## Reading

- [Sipser — Ch. 7.1 (measuring complexity)](../resources/books/sipser-introduction-to-the-theory-of-computation-3e.pdf#page=299)
- [Sipser — Ch. 7.2 (the class P)](../resources/books/sipser-introduction-to-the-theory-of-computation-3e.pdf#page=308)
- [Sipser — Ch. 7.3 (the class NP)](../resources/books/sipser-introduction-to-the-theory-of-computation-3e.pdf#page=316)
- [Sipser — Ch. 7.4 (NP-completeness)](../resources/books/sipser-introduction-to-the-theory-of-computation-3e.pdf#page=323)
- [Sipser — Ch. 7.5 (additional NP-complete problems)](../resources/books/sipser-introduction-to-the-theory-of-computation-3e.pdf#page=335)

## Practice
- [ ] Do the 3SAT → CLIQUE reduction in full, both directions of correctness
- [ ] Give a polynomial verifier for 3 different NP problems
- [ ] Sipser exercises 7.1-7.30

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
