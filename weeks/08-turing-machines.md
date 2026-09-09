# Week 8 — Turing Machines

> Syllabus (TR): *Turing makinaları*

**Previous:** [Week 7](07-pumping-lemma-cfl.md) · **Next:** [Week 9](09-turing-machine-variants.md)

## Goals
- Give the formal definition of a TM and trace its configurations.
- Distinguish decider from recognizer, decidable from Turing-recognizable.

## Key concepts
- TM `(Q, Σ, Γ, δ, q₀, q_accept, q_reject)`; infinite tape, read/write head, `δ: Q × Γ → Q × Γ × {L,R}`.
- Configuration `uqv`; yields relation; accepting/rejecting/looping computation.
- **Turing-recognizable** (recursively enumerable) = some TM accepts every string in the language, may loop otherwise.
- **Decidable** (recursive) = some TM halts on every input. Decidable ⊂ Turing-recognizable, strictly.
- Three levels of description: formal, implementation, high-level — exams accept high-level.

## Reading

- [Sipser — Ch. 3.1 (Turing machines)](../resources/books/sipser-introduction-to-the-theory-of-computation-3e.pdf#page=189)

## Practice
- [ ] Build a TM for `{0ⁿ1ⁿ}` at implementation level, and trace it on `0011`
- [ ] Sipser exercises 3.1-3.8

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
