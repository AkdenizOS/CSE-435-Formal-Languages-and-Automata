# Week 10 — Decidability

> Syllabus (TR): *Karar verilebilirlik*

**Previous:** [Week 9](09-turing-machine-variants.md) · **Next:** [Week 11](11-undecidability.md)

## Goals
- Prove that a given language about automata is decidable by constructing a decider.
- Know the standard decidable problems and how each decider works.

## Key concepts
- Encoding objects as strings: `⟨M⟩`, `⟨M, w⟩`, `⟨G⟩`.
- Decidable: `A_DFA`, `A_NFA`, `A_REX`, `E_DFA`, `EQ_DFA`, `A_CFG`, `E_CFG`.
- `A_DFA = {⟨B,w⟩ | B is a DFA that accepts w}` — decidable by simulation.
- `EQ_DFA` — decidable via the symmetric difference and `E_DFA`.
- `A_CFG` — decidable by converting to CNF and trying all derivations of length `2|w|−1`.
- **Every context-free language is decidable** — the chain regular ⊂ CFL ⊂ decidable ⊂ recognizable.

## Reading

- [Sipser — Ch. 4.1 (decidable languages)](../resources/books/sipser-introduction-to-the-theory-of-computation-3e.pdf#page=218)

## Practice
- [ ] Write the decider for `EQ_DFA` in full
- [ ] Sipser exercises 4.1-4.10

## Checklist
- [ ] Lecture attended
- [ ] Textbook section read
- [ ] Exercises done
- [ ] Notes written below

---

Your own notes for this week go in `terms/<your-term>/notes/week-10.md`, not here.
This file is the shared plan — improve it if the course changes, but keep it general.
