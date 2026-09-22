# Exams

Past papers sit in this folder as `<year>-<type>.pdf`. Below: the pattern analysis,
then the midterm and final preparation checklists.

Built by reading every past paper in this folder. The midterm
structure has not changed in five years.

## Midterm — the recurring five-question shape

| Q | Points | Task | Week |
|---|--------|------|------|
| P1 | 20 | **Construct a DFA** — two languages | [3](../weeks/03-regular-languages-finite-automata.md) |
| P2 | 20 | **Construct an NFA** — two languages, *minimum states* | [3](../weeks/03-regular-languages-finite-automata.md) |
| P3 | 15-25 | **Prove a language is not regular** — pumping lemma | [4](../weeks/04-pumping-lemma-regular.md) |
| P4 | 20-30 | **Give a CFG _and_ a PDA** for one language | [5](../weeks/05-context-free-grammars.md), [6](../weeks/06-pushdown-automata.md) |
| P5 | 10-20 | **Prove a language is not context-free** — CFL pumping lemma | [7](../weeks/07-pumping-lemma-cfl.md) |

Verified across 2020, 2022, 2023 and 2024. The 2020 paper swapped P5 for a Turing
machine variant equivalence proof (`HopTM`), so week 9 is not entirely safe to skip.

**The scoring rule on P2 matters:** *"Use as few states as you can. Fewest gets full
point, every extra state halves your point."* A correct NFA with one extra state
scores 50%. Practice minimizing, not just constructing.

## Actual questions asked

| Year | P1 DFA | P2 NFA | P3 not regular | P4 CFG + PDA | P5 not CF |
|------|--------|--------|----------------|--------------|-----------|
| 2020 | no `00` or `11`; 1s in groups of 2 or 4 | every 3rd position is 1; `1*(001+)*` | `{aᵏbᵐcⁿ : k+m+n=100}`, `{0ᵐ1ⁿ : m≠n}`, `{1ᵏy : y has ≤ k 1s}` | odd length, first=middle=last; `{aᵐbⁿ : m ≤ n ≤ 3m}`; `{aᵐbⁿ : m divides n}` | *(TM variant `HopTM` instead)* |
| 2022 | starts/ends same symbol, ≤ two 1s; #a not a multiple of 3 | last three symbols equal; starts/ends given, exactly two `a`, no repeats | `{aᵐbⁿ : n divides m}` | `{aᵏbᵐcⁿ : k+n=m}` | `{0ᵐ1ⁿ0ᵐ1ⁿ}` |
| 2023 | `10` before `011`; even #0s and ends `00`/`11` | no `aa`/`bb`/`cc`; ≥ one 1 and last three have one or two 0s | `{wwᴿy}` | *(see paper)* | *(see paper)* |
| 2024 | even #0s and ≤ two 1s; binary number divisible by 5 | last two symbols equal; `a`/`t` alternate ignoring `c`/`g` | `{0ᵏ1ᵐ0ⁿ : k>m>n>0}` | `{aᵏbᵐcⁿ : k ≥ m+n}` | `{0ᵐ1ⁿ0ᵏ : k=mn}` |

Recurring tricks worth drilling:
- **Divisibility / counting mod k** as DFA states (`#a mod 3`, binary value mod 5).
- **"Last k symbols"** languages — trivial as an NFA, exponential as a DFA. This is
  the point of the minimum-state scoring rule.
- **Linear constraints on `aᵏbᵐcⁿ`** for the CFG+PDA question — `k+n=m`, `k ≥ m+n`,
  `m ≤ n ≤ 3m` are all variations of the same stack-counting idea.
- **Nonlinear constraints** (`m divides n`, `k = mn`) are the not-context-free ones.

## Final

Only one past final is available (2019, then coded CSE 436). Assume it is
comprehensive and weighted toward weeks 8-14: Turing machines, decidability,
undecidability, reducibility, NP-completeness.

## The archive

| File | Year | Type | Has solutions |
|------|------|------|---------------|
| [2019-midterm-solutions.pdf](./2019-midterm-solutions.pdf) | 2019 | Midterm | yes |
| [2019-final.pdf](./2019-final.pdf) | 2019 | Final | no |
| [2020-midterm.pdf](./2020-midterm.pdf) | 2020 | Midterm | no |
| [2020-makeup.pdf](./2020-makeup.pdf) | 2020 | Make-up | no |
| [2022-midterm.pdf](./2022-midterm.pdf) | 2022 | Midterm | no |
| [2023-midterm-solutions.pdf](./2023-midterm-solutions.pdf) | 2023 | Midterm | yes (handwritten) |
| [2024-midterm.pdf](./2024-midterm.pdf) | 2024 | Midterm | no |

Collected from previous cohorts; original authors unknown. Treat the handwritten
2023 solutions as one student's answers, not an official key.

## Midterm — 40%

**Date:** TBD · **Duration:** 90 minutes (every past paper) · **Scope:** weeks 1-7

The question shape has been identical for five years. See the pattern analysis above.


| Q | Points | Task |
|---|--------|------|
| P1 | 20 | Construct a DFA (two languages) |
| P2 | 20 | Construct an NFA — **minimum states, extra states halve your score** |
| P3 | 15-25 | Prove a language is not regular |
| P4 | 20-30 | Give a CFG **and** a PDA for one language |
| P5 | 10-20 | Prove a language is not context-free |

### Preparation

- [ ] Work [2024-midterm.pdf](./2024-midterm.pdf) under timed conditions (90 min)
- [ ] Work [2022-midterm.pdf](./2022-midterm.pdf) under timed conditions
- [ ] Work [2020-midterm.pdf](./2020-midterm.pdf) under timed conditions
- [ ] Check answers against [2023-midterm-solutions.pdf](./2023-midterm-solutions.pdf) and [2019-midterm-solutions.pdf](./2019-midterm-solutions.pdf)
- [ ] Drill NFA state minimization — this is where points are lost cheaply
- [ ] Write out the regular pumping lemma and the CFL pumping lemma from memory
- [ ] Review the `aᵏbᵐcⁿ` linear-constraint CFG/PDA family
- [ ] Read [2020-makeup.pdf](./2020-makeup.pdf) — the make-up paper's TM question

### My notes

<!-- What I got wrong in practice, and why. -->

## Final — 60%

**Date:** TBD · **Scope:** comprehensive, weighted toward weeks 8-14

Only one past final is available: [2019-final.pdf](./2019-final.pdf) (coded
CSE 436 that year). Plan for Turing machines, decidability, undecidability,
reducibility and NP-completeness on top of the whole midterm scope.

### Preparation

- [ ] Work [2019-final.pdf](./2019-final.pdf)
- [ ] Redo the midterm papers — the first half of the course is still examinable
- [ ] Reproduce the `A_TM` diagonalization proof from memory
- [ ] Do three reductions from `A_TM` without looking
- [ ] Do the 3SAT → CLIQUE reduction in full
- [ ] Draw the full class hierarchy: regular ⊂ CFL ⊂ P ⊆ NP ⊆ PSPACE ⊂ decidable ⊂ recognizable
- [ ] State the pumping lemmas, Rice's theorem, Savitch's theorem, Cook-Levin

### My notes
