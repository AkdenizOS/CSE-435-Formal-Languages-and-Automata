# Week 12 — Reducibility

> Syllabus (TR): *İndirgenebilirlik*

**Previous:** [Week 11](11-undecidability.md) · **Next:** [Week 13](13-np-completeness.md)

## Goals
- Prove undecidability by reduction from `A_TM` instead of by diagonalization.
- Use mapping reducibility and Rice's theorem.

## Key concepts
- **Reduction**: to show `B` undecidable, assume a decider for `B` and use it to decide `A_TM`.
- Undecidable by reduction: `HALT_TM`, `E_TM`, `EQ_TM`, `REGULAR_TM`.
- **Mapping reducibility** `A ≤_m B` via a computable `f` with `w ∈ A ⟺ f(w) ∈ B`.
- If `A ≤_m B` and `B` is decidable then `A` is decidable; contrapositive is the working tool.
- `A ≤_m B` ⟹ `Ā ≤_m B̄` — used to show non-recognizability.
- **Rice's theorem**: every nontrivial semantic property of TM languages is undecidable.
- Post Correspondence Problem as a non-TM undecidable problem.

## Reading

- [Sipser — Ch. 5.1 (undecidable problems from language theory)](../resources/books/sipser-introduction-to-the-theory-of-computation-3e.pdf#page=240)
- [Sipser — Ch. 5.2 (a simple undecidable problem — PCP)](../resources/books/sipser-introduction-to-the-theory-of-computation-3e.pdf#page=251)
- [Sipser — Ch. 5.3 (mapping reducibility)](../resources/books/sipser-introduction-to-the-theory-of-computation-3e.pdf#page=258)

## Practice
- [ ] Do 3 reductions from `A_TM`, writing the constructed machine explicitly
- [ ] Apply Rice's theorem and then prove the same result by hand reduction
- [ ] Sipser exercises 5.1-5.30

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
