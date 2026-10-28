# Shape: structured proof

The shape of one [structured proof](../evidence/mathematical-writing/frame.md), with each [warrant](../evidence/mathematical-writing/frame.md) named. It has a one-line sketch first, then numbered steps in Lamport's hierarchical style, each with its own justification, at most three levels deep, with the results it uses named at the top.

## When to use it

- A proof longer than about ten lines, with cases, or with a chain of claims a referee will check one by one.
- A proof you are not yet sure of: writing it in steps is how Lamport 1995 and Tao 2023 report errors being found.
- Not for a short proof with one idea: keep a paragraph, as the last section below explains.
- Inside an article, this shape fills the proofs section of a [mathematical article](mathematical-article.md).

## How each part maps to the evidence

| Part | What it does | Evidence | Grade |
|---|---|---|---|
| Uses line | names the definitions and lemmas the proof depends on | leanblueprint, Tao organise, Tao 2023 | convention, untested for human readers |
| Sketch first | the holistic idea, where a reader may stop | Lamport 2012; structure helped summaries in Fuller 2014 | measured, one study (for the summary effect) |
| Numbered steps ⟨level⟩position | each claim with its own proof | Leron 1983, Lamport 1995, Lamport 2012 | convention, untested on readers |
| Every warrant named | spares the reader the search for implicit justifications | Inglis & Alcock 2012 (experts hunt for them), Hodds 2014 | supported with caveat |
| Citations only to visible steps | earlier siblings and ancestors' earlier siblings | Lamport 2012 | convention, untested |
| Q.E.D. step closing each level | says how the steps give the claim above | Lamport 1995 | convention, untested |
| 4 to 10 steps per level | the size Lamport finds easiest to read | Lamport 2012 | convention, untested |
| At most three levels | a deeper step is a lemma to state on its own | this repository; Lamport 2012 finds step names past level 4 hard to read | convention, untested; stricter than Lamport, who writes six levels |
| Calculation at the lowest level | a chain of relations with a hint per link | Dijkstra 2000, Gries & Schneider 1993, Lamport 2012 | convention, untested |
| Paragraph alternative | for short, single-idea proofs | Lamport 2012 (prose under about ten lines), Fuller 2014 (readers found structure jumpy) | supported with caveat |

The one randomised test of a structured layout, Fuller 2014, found a better grasp of the summary and slightly lower scores on justifications, transfer and examples; this shape adds named warrants to protect those.
Whether it succeeds is untested: [baseline](../evidence/mathematical-writing/baseline.md) gives the comparison.
Each key (Author Year) is listed in [references](../evidence/bibliography.md).

The LaTeX version is [proof.tex](proof.tex).

## The principles it applies

| Part | Principle |
|---|---|
| Sketch first, where a reader may stop | [overview first](../principles/document/overview-first.md) |
| Numbered steps, at most three levels | [shallow outline](../principles/document/shallow-outline.md) |
| Every warrant named; the Uses line | [define before use](../principles/document/define-before-use.md), [short reference distance](../principles/document/short-reference-distance.md) |
| A Q.E.D. step closing each level | [signal the structure](../principles/page/signal-the-structure.md) |

## The skeleton

**Theorem n.** One sentence with every hypothesis inside it.

Uses: Definition 2.1, Lemma 3.2.

**Proof sketch.** One line that gives the idea, for example: "Induct on $n$; the step reduces to Lemma 3.2."

- ⟨1⟩1. First claim.
  *Proof:* by Definition 2.1.
- ⟨1⟩2. Second claim.
  - ⟨2⟩1. First sub-claim. *Proof:* by ⟨1⟩1.
  - ⟨2⟩2. Q.E.D. *Proof:* by ⟨2⟩1 and Lemma 3.2.
- ⟨1⟩3. Q.E.D.
  *Proof:* by ⟨1⟩1 and ⟨1⟩2. $\square$

## The rules

1. The sketch comes first, so a reader who wants only the idea can stop there.
2. Each step is a claim, numbered ⟨level⟩position, followed by its own proof.
3. A step's proof names every step, hypothesis and earlier result it uses.
4. A step may cite only its earlier siblings and the earlier siblings of its ancestors.
5. Each level ends with a Q.E.D. step that says how the level's steps give the claim above.
6. Keep 4 to 10 steps per level; split a longer level into sub-steps, merge a shorter one.
7. Stop at three levels; a proof that needs a fourth has a lemma inside it, so state the lemma separately.
8. A sub-proof may open with its own one-line sketch.
9. The lowest level is a short paragraph or a calculation with a hint per link.
10. Assumptions are named in the step that makes them: "Assume: ... Prove: ..." or "Case: ...".

## A calculation as the lowest level

$a + 1$
$\quad \leq \quad$ { hypothesis 1 }
$b^2 - 3$
$\quad = \quad$ { definition of $c$ }
$c - 4$

## Worked example

**Theorem.** No rational number $r$ satisfies $r^2 = 2$.

**Proof sketch.** Write $r$ in lowest terms; both numerator and denominator turn out even.

- ⟨1⟩1. It suffices to assume integers $p, q$ with $q \neq 0$, $\gcd(p, q) = 1$ and $p^2 = 2q^2$, and derive a contradiction.
  *Proof:* every rational is $p/q$ in lowest terms, and $(p/q)^2 = 2$ exactly when $p^2 = 2q^2$.
- ⟨1⟩2. $p$ is even.
  *Proof:* $p^2 = 2q^2$ is even by ⟨1⟩1, and the square of an odd integer is odd.
- ⟨1⟩3. $q$ is even.
  - ⟨2⟩1. $p = 2k$ for some integer $k$. *Proof:* by ⟨1⟩2.
  - ⟨2⟩2. $q^2 = 2k^2$. *Proof:* substitute ⟨2⟩1 into $p^2 = 2q^2$ from ⟨1⟩1 and divide by 2.
  - ⟨2⟩3. Q.E.D. *Proof:* $q^2$ is even by ⟨2⟩2, so $q$ is even, as in ⟨1⟩2.
- ⟨1⟩4. Q.E.D.
  *Proof:* by ⟨1⟩2 and ⟨1⟩3, 2 divides both $p$ and $q$, which contradicts ⟨1⟩1. $\square$

## When a conventional paragraph proof is better

Keep a paragraph, still with a first sentence that gives the idea and each warrant named, when:

- the proof is under about ten lines, the size below which Lamport 2012 himself writes prose;
- it is one idea or one calculation, where numbering adds length and no structure;
- the readers are experts skimming for the idea, the readers Lamport 1995 reports the format did not please;
- the venue expects prose and the detailed version can be published alongside, as Lamport 1995 suggests;
- the steps would force the reader to jump back and forth, the cost readers reported in Fuller 2014.

Use the structured form when the proof is long, has cases, or will be checked line by line, by a referee or by the author.
