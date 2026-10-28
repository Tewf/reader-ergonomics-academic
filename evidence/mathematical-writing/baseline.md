# Baseline: what the templates are compared against, and how

This file names the baseline article and proof a new shape is compared against, and how the comparison would be measured.

## The named baseline

**The conventional amsart article with paragraph proofs.**

| Part | Baseline form | Source |
|---|---|---|
| Class | `amsart`, current AMS article class, theorem styles plain, definition, remark | AMS 2017, amscls |
| Top matter | title, author, abstract before `\maketitle`, primary MSC 2020 code, optional keywords | AMS 2017, MSC2020 |
| Opening | introduction that announces the principal findings | Kuteeva & McGrath 2015 |
| Middle | optional background or notation section, then sections of definitions, lemmas, theorems and proofs | Kuteeva & McGrath 2015 |
| Proofs | linear prose inside `\begin{proof}...\end{proof}`, warrants often implicit | Inglis & Alcock 2012 |
| Ending | no fixed form: often QED, sometimes remarks or open questions | Kuteeva & McGrath 2015 |

The baseline is what a referee at an AMS journal expects, so any change must beat it, not merely differ from it.

## What is compared

| Arm | Article | Proofs |
|---|---|---|
| A, baseline | as above | linear paragraph proofs |
| B, template | `shapes/mathematical-article` | `shapes/proof`: sketch, then numbered steps at most three levels deep, each lemma listing what it uses |
| C, positive control | as A | as A, but readers first study self-explanation training (Hodds 2014) |

Arm C sets the bar: d = 0.95 is the largest gain among the studies found here, and it changes the reader, not the text.

## How a comparison is measured

1. **Materials**: the same theorem and the same mathematical content in arms A and B; only the layout differs.
2. **Assignment**: readers randomised between arms, as in Fuller 2014, Roy 2017b and Lew 2020.
3. **Comprehension test**: one item set per dimension of Mejia-Ramos 2012, built and checked for reliability by the method of Mejia-Ramos 2017.
4. **Per-dimension scores**: report local (terms, logical status, justifications) and holistic (idea, modules, transfer, examples) separately, because Fuller 2014 found a trade-off that a total score hides.
5. **Summary quality**: ask for a short summary and score it by comparative judgement (Davies 2020).
6. **Retention**: repeat the test after two weeks without warning, since Roy 2017b's loss appeared only then.
7. **Time**: record reading time and time to answer; a longer read that buys nothing is a cost.
8. **Eye tracking, where available**: dwell time on formulae versus words, and look-backs between consecutive lines (Inglis & Alcock 2012).
9. **Article level**: time to locate the main theorem, and accuracy in restating it after reading only the abstract and introduction; this measure is proposed here and untested.

## Sample size

- A two-sided test at alpha 0.05 with power 0.8 needs about 64 readers per arm to detect d = 0.5.
- Roy 2017b had 21 and 28 per arm (not checked against the paper), so effects smaller than about d = 0.8 could be missed.
- Undergraduates and research mathematicians are tested as separate groups, since every study found used undergraduates.

## Decision rule

- Arm B is adopted if it is not worse than arm A on any local dimension and better on at least one holistic dimension.
- Arm B is rejected if any local dimension drops significantly, the pattern Fuller 2014 warned of.
- If neither arm beats arm C, the cheaper intervention is reader training, and the templates' value is convenience for the writer.
