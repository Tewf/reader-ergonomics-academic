# Shape: mathematical research article

The shape of a proof-centred mathematics article on the AMS `amsart` class: the field's Introduction-Results genre, the main theorem stated in section 1, milestones before details, and each proof naming what it uses.

## When to use it

- A research article whose contribution is theorems and their proofs, for a journal or arXiv.
- A thesis chapter with the same contribution; keep the institution's class for layout and take the section order from here.
- Not for an empirical study: the [research paper](research-paper.md) shape covers IMRaD.
- Not for a survey or a monograph, whose order follows the subject rather than one main theorem.
- Not literally for papers that fill a journal issue; Krantz 2017 says the scheme bends there.

## How each part maps to the evidence

| Part | What it does | Evidence | Grade |
|---|---|---|---|
| Class and theorem styles | `amsart`; plain, definition and remark styles from amsthm | AMS 2017, amscls, amsthm | convention, enforced by the publisher |
| Abstract before `\maketitle` | short, no citations; under 1920 characters for arXiv | AMS 2017, arXiv 2026 | convention, enforced |
| MSC 2020 code, keywords | at least one primary code; keywords optional | AMS 2017, MSC2020 | convention, enforced |
| Introduction, plain first paragraph | the result in words before any definition | Krantz 2017 | convention, untested |
| Main results in section 1 | self-contained one-sentence theorem, stated before its proof | Kuteeva 2015 (21 of 22 openings), Halmos 1970, Tao 2026a | measured, descriptive; convention for the effect |
| Relation to previous work | what is new, and an example showing a hypothesis is needed | Tao 2026a | convention, untested |
| Idea of the proof | the milestones and how they combine | Krantz 2017, Tao 2026b | convention, untested |
| Organisation paragraph | one sentence per section | Krantz 2017 | convention, untested |
| Preliminaries and notation | notation fixed once so statements stand alone | Kuteeva 2015 (17 of 22 have such a section), Knuth 1989 | measured, descriptive |
| Results before proofs | milestones stated, then the main theorem derived from them | Krantz 2017, Tao 2026b | convention, untested |
| Uses line in each proof | the results a proof depends on, so the dependency tree is explicit | Massot 2026, Tao 2026b, Tao 2023 | convention, untested for human readers |
| Proofs: sketch, then numbered steps | holistic summary first, then explicit warrants | Fuller 2014, Inglis 2012, Lamport 2012 | measured, one study; see [proof](proof.md) |
| Ending | optional remarks or open questions; the field has no fixed ending | Kuteeva 2015 (11 of 22 have no conclusion) | measured, descriptive |

Each key (Author Year) is listed in [references](../evidence/bibliography.md).
No part of this shape has been tested against the conventional article on reader outcomes; [baseline](../evidence/mathematical-writing/baseline.md) says how it would be.

## The principles it applies

| Part | Principle |
|---|---|
| Main theorem stated in section 1, in words before any definition | [overview first](https://github.com/Tewf/reader-ergonomics/blob/v1.13.0/principles/document/overview-first.md) |
| Idea of the proof before its details | [overview first](https://github.com/Tewf/reader-ergonomics/blob/v1.13.0/principles/document/overview-first.md) |
| Notation fixed once, in Preliminaries | [define before use](https://github.com/Tewf/reader-ergonomics/blob/v1.13.0/principles/document/define-before-use.md), [one place per fact](https://github.com/Tewf/reader-ergonomics/blob/v1.13.0/principles/collection/one-place-per-fact.md) |
| A Uses line in each proof; results ordered so each comes after what it uses | [short reference distance](https://github.com/Tewf/reader-ergonomics/blob/v1.13.0/principles/document/short-reference-distance.md) |
| Sections on at most three levels | [shallow outline](https://github.com/Tewf/reader-ergonomics/blob/v1.13.0/principles/document/shallow-outline.md) |

## Skeleton

Copy this into a new file, or start from the LaTeX version, [mathematical-article.tex](mathematical-article.tex).

````markdown
# A title that names the result

Author Name, Department, Institution, City, Country.

**Abstract.** One to three sentences: what is proved, under which hypotheses, and why it matters. No citations; the AMS proceedings checklist suggests at most about 150 words for a short paper and 300 for a long one, and arXiv accepts under 1920 characters.

**MSC 2020.** Primary 00-XX; Secondary 00-XX (replace by full codes from msc2020.org).

**Keywords.** first keyword, second keyword.

## 1. Introduction

State the main result in one or two plain sentences that a reader outside the subfield can follow.

### 1.1 Main results

**Theorem 1.1.** Let $X$ be an object of the kind studied here. If $X$ satisfies condition $(\ast)$, then $X$ has property $P$.

**Corollary 1.2.** A consequence of Theorem 1.1 that a reader in a neighbouring field would use.

If Theorem 1.1 is too technical for the introduction, state an informal version labelled "informal" and point to the precise statement.

### 1.2 Relation to previous work

Say what was known, one sentence per result, with citations [1].
Say what this paper adds.
Give an example showing that condition $(\ast)$ cannot be removed.

### 1.3 Idea of the proof

The proof has three steps.
Proposition 3.1 reduces Theorem 1.1 to a statement about a simpler object.
Lemma 3.2 proves that statement in a special case, and Lemma 3.3 extends it.
The new difficulty sits in Lemma 3.3.

### 1.4 Organisation

Section 2 fixes notation and recalls known results.
Section 3 states the milestones and derives Theorem 1.1 from them.
Section 4 proves the milestones.

## 2. Preliminaries and notation

Throughout, $X$ denotes an object of the kind studied here and $n \geq 1$ an integer.

**Definition 2.1.** An object $X$ satisfies *condition $(\ast)$* if it has the defining property.

**Theorem 2.2 (known, [2]).** Quote the known theorem exactly as it is used, with its source.

## 3. Results

**Proposition 3.1.** If Lemmas 3.2 and 3.3 hold, then every $X$ satisfying $(\ast)$ has property $P$.

**Lemma 3.2.** The special case of property $P$ holds.

**Lemma 3.3.** If the special case holds, then the general case holds.

*Proof of Theorem 1.1.*
Uses: Proposition 3.1, Lemmas 3.2 and 3.3.
Lemma 3.2 gives the special case, Lemma 3.3 extends it, and Proposition 3.1 concludes. $\square$

## 4. Proofs

*Proof of Proposition 3.1.*
Uses: Definition 2.1, Theorem 2.2.
A short argument stays a paragraph: say what is shown, then why, naming each result where it is used. $\square$

*Proof of Lemma 3.2.*
Uses: Definition 2.1, Theorem 2.2.

Sketch: one sentence that gives the idea, so a reader can stop here.

- ⟨1⟩1. First claim. *Proof:* by Definition 2.1.
- ⟨1⟩2. Second claim. *Proof:* by ⟨1⟩1 and Theorem 2.2.
- ⟨1⟩3. Q.E.D. *Proof:* by ⟨1⟩1 and ⟨1⟩2. $\square$

*Proof of Lemma 3.3.*
Uses: Lemma 3.2.

Sketch: one sentence that names the new difficulty and how it is overcome.

- ⟨1⟩1. Reduction to the special case. *Proof:* by Lemma 3.2.
- ⟨1⟩2. Q.E.D. *Proof:* by ⟨1⟩1. $\square$

The full proof shape, with deeper levels and when to keep a paragraph, is in [proof.md](proof.md).

## Acknowledgements

Funding and thanks.

## References

1. A. Author, *Title of the earlier result*, Journal **1** (2000), 1-10.
2. B. Author, *Title of the known theorem*, Publisher, City, 2010.
````

## Worked example

A classical theorem written to this shape, with its proof in the structured form of [proof.md](proof.md).

```markdown
# Every finite tournament has a Hamiltonian path

A worked example for this shape.

**Abstract.** Every tournament on $n \geq 1$ vertices has a directed path through all its vertices. The proof inserts
one vertex at a time.

**MSC 2020.** Primary 05C20; Secondary 05C38.

**Keywords.** tournament, Hamiltonian path, induction.

## 1. Introduction

In any round-robin contest with no draws, the players can be listed so that each one beat the next.

### 1.1 Main results

**Theorem 1.1.** Every tournament on $n \geq 1$ vertices has a Hamiltonian path.

### 1.2 Relation to previous work

Rédei proved this, and that the number of such paths is odd [1]; this note proves existence only. Completeness
cannot be dropped: on vertices $a, b, c$ with arcs $a \to b$ and $c \to b$ only, no path passes through all three.

### 1.3 Idea of the proof

Lemma 3.1 inserts a new vertex into any directed path; induction on $n$ then builds the whole path.

### 1.4 Organisation

Section 2 defines the terms, Section 3 states the lemma and derives the theorem, and Section 4 proves the lemma.

## 2. Preliminaries and notation

**Definition 2.1.** A *tournament* is a finite set $V$ of vertices with, for each pair of distinct vertices $u, v$,
exactly one of the arcs $u \to v$ and $v \to u$.

**Definition 2.2.** A *Hamiltonian path* is a list $v_1, \dots, v_n$ of all the vertices, each once, with
$v_i \to v_{i+1}$ for every $i < n$.

## 3. Results

**Lemma 3.1.** Let $v_1, \dots, v_k$ be a directed path in a tournament and $u$ a vertex not on it. Then $u$ can be
inserted into the path so that $v_1, \dots, v_k$ and $u$ form a directed path.

*Proof of Theorem 1.1.*
Uses: Lemma 3.1.
By induction on $n$: one vertex is a path. For $n \geq 2$, remove a vertex $u$; the rest is a tournament with a
Hamiltonian path, and Lemma 3.1 inserts $u$. $\square$

## 4. Proofs

*Proof of Lemma 3.1.*
Uses: Definition 2.1.

Sketch: put $u$ just before the first vertex it beats.

- ⟨1⟩1. If $u \to v_1$, then $u, v_1, \dots, v_k$ is a path.
- ⟨1⟩2. If $v_k \to u$, then $v_1, \dots, v_k, u$ is a path.
- ⟨1⟩3. Otherwise $v_1 \to u$ and $u \to v_k$. Let $j$ be the least index with $u \to v_j$; then $j \geq 2$,
  and $v_{j-1} \to u$, so $v_1, \dots, v_{j-1}, u, v_j, \dots, v_k$ is a path.
  *Proof:* $j$ exists since $u \to v_k$, and $j \neq 1$ since $v_1 \to u$; by the choice of $j$, $u \to v_{j-1}$
  fails, so $v_{j-1} \to u$ by Definition 2.1.
- ⟨1⟩4. Q.E.D. *Proof:* by Definition 2.1 either $u \to v_1$ or $v_1 \to u$, and either $v_k \to u$ or
  $u \to v_k$, so ⟨1⟩1 to ⟨1⟩3 cover every case. $\square$

## References

1. L. Rédei, *Ein kombinatorischer Satz*, Acta Litterarum ac Scientiarum Szeged **7** (1934), 39-43.
```
