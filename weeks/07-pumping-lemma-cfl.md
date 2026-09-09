# Week 7 — Pumping Lemma for Context-Free Languages

> Syllabus (TR): *İçerikten bağımsız diller için şişirme lemması*

**Previous:** [Week 6](06-pushdown-automata.md) · **Next:** [Week 8](08-turing-machines.md)

## Goals
- State the CFL pumping lemma and use it to prove a language is not context-free.
- Contrast it with the regular pumping lemma — why five pieces instead of three.

## Key concepts
- **CFL pumping lemma:** if `A` is context-free, there is `p` such that every `s ∈ A`, `|s| ≥ p`, splits as `s = uvxyz` with (1) `uvⁱxyⁱz ∈ A` for all `i ≥ 0`, (2) `|vy| > 0`, (3) `|vxy| ≤ p`.
- Why five pieces: the proof uses a **repeated variable on a root-to-leaf path** in the parse tree, which pumps two substrings at once.
- `p = b^(|V|+1)` where `b` is the max right-hand-side length — from the parse-tree height argument.
- Classic non-CFLs: `{aⁿbⁿcⁿ}`, `{ww}`, `{aⁱbʲcᵏ | i ≤ j ≤ k}`.
- CFLs are closed under ∪, ∘, *, and intersection **with a regular language** — but not under ∩ or complement.

## Reading

- [Sipser — Ch. 2.3 (non-context-free languages)](../resources/books/sipser-introduction-to-the-theory-of-computation-3e.pdf#page=149)

## Practice
- [ ] Prove `{aⁿbⁿcⁿ}` is not context-free, covering every case of the split
- [ ] Show CFLs are not closed under intersection with a counterexample
- [ ] Sipser exercises 2.31-2.42

## Checklist
- [ ] Lecture attended
- [ ] Textbook section read
- [ ] Exercises done
- [ ] Notes written below

---

Your own notes for this week go in `terms/<your-term>/notes/week-07.md`, not here.
This file is the shared plan — improve it if the course changes, but keep it general.
