# Week 4 — Pumping Lemma for Regular Languages

> Syllabus (TR): *Düzenli diller için şişirme lemması*

**Previous:** [Week 3](03-regular-languages-finite-automata.md) · **Next:** [Week 5](05-context-free-grammars.md)

## Goals
- State the pumping lemma exactly and use it to prove a language is not regular.
- Recognize when the pumping lemma will not work and use closure properties instead.

## Key concepts
- **Pumping lemma:** if `A` is regular, there is a pumping length `p` such that every `s ∈ A` with `|s| ≥ p` can be split `s = xyz` with (1) `xyⁱz ∈ A` for all `i ≥ 0`, (2) `|y| > 0`, (3) `|xy| ≤ p`.
- It is a **necessary, not sufficient** condition — pumping does not prove regularity.
- The proof is an adversary game: they pick `p`, you pick `s`; they split, you pick `i`.
- Condition (3) `|xy| ≤ p` is what makes most proofs work — it forces `y` into the first `p` symbols.
- Classic non-regular languages: `{0ⁿ1ⁿ}`, `{ww}`, `{0ⁿ | n prime}`, balanced parentheses.
- Alternative route: closure properties (if `A ∩ regular` were regular but is known not to be).

## Reading

- [Sipser — Ch. 1.4 (nonregular languages)](../resources/books/sipser-introduction-to-the-theory-of-computation-3e.pdf#page=101)

## Practice
- [ ] Prove 3 languages non-regular, each with a different choice of `s`
- [ ] Find a non-regular language that *does* satisfy the pumping condition
- [ ] Sipser exercises 1.29-1.55

## Checklist
- [ ] Lecture attended
- [ ] Textbook section read
- [ ] Exercises done
- [ ] Notes written below

---

Your own notes for this week go in `terms/<your-term>/notes/week-04.md`, not here.
This file is the shared plan — improve it if the course changes, but keep it general.
