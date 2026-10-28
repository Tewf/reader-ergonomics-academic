# State of the art: who holds the record on each sub-question

Two kinds of result are kept apart.

- **Upper bound**: what has been achieved, the best measured gain or the most complete description.
- **Lower bound**: a limit, a negative result, or a finding that something did not work.

## Q1. The order and kinds of sections

| | Holder | Method | Measured how |
|---|---|---|---|
| Upper bound | Kuteeva & McGrath 2015 | Move analysis of 22 pure-mathematics articles from 5 authors, with interviews | counts of headings and moves per article |
| Upper bound | Graves 2013 | Macrostructure analysis of 30 pure and applied articles | presence or absence of IMRD sections |
| Lower bound | Kuteeva & McGrath 2015 | The same corpus | no single prototype: notation, background and endings vary widely |

Caveat: both corpora are small, and the 22 articles come from only five authors in four fields.

## Q2. Where the main results go

| | Holder | Method | Measured how |
|---|---|---|---|
| Upper bound (descriptive) | Kuteeva & McGrath 2015 | Corpus count | 21 of 22 openings announce the principal findings |
| Upper bound (advice) | Halmos 1970, Krantz 2017, Tao intro | Expert advice | none; the guides agree |
| Lower bound | none found | | no experiment varies the position of the main theorem and measures readers |

## Q3. How a single proof is laid out

| | Holder | Method | Measured how |
|---|---|---|---|
| Upper bound (format) | Lamport 2012 | 20 years of practice with numbered hierarchical proofs, plus a machine-checked appendix | anecdotes of errors found; no reader test |
| Upper bound (format) | Dijkstra 2000, Gries & Schneider 1993 | Calculational proofs with a hint per step | none; design argument |
| Lower bound | Lamport 1995 | Report of reactions | skeptical checkers liked the format, skimmers did not |
| Lower bound | Lamport 2012 | Report of one referee | the long structured proofs were found tedious |

## Q4. Does the layout change comprehension?

| | Holder | Design | Result |
|---|---|---|---|
| Upper bound (any intervention) | Hodds 2014 | Randomised, self-explanation training of the reader, not of the text | d = 0.95 in the lab; replicated in a lecture hall with 107 students |
| Upper bound (text format) | Fuller 2014 | Randomised, Leron-style structured versus linear proof | better at identifying a good summary |
| Lower bound (text format) | Fuller 2014 | The same study | somewhat worse on justifications, transfer and examples, mostly not significant |
| Lower bound (text format) | Roy 2017b | Randomised, e-Proof versus textbook, N = 49 | no immediate gain; worse retention after two weeks |
| Lower bound (text format) | Lew 2020 | Randomised, generic versus traditional proof | no difference |

The largest measured gain comes from teaching the reader to self-explain, not from changing the proof's format.

No study found tests Lamport's numbered format, as distinct from Leron's, on readers.

## Q5. Explicit dependencies between results

| | Holder | Method | Measured how |
|---|---|---|---|
| Upper bound | mathlib 2020 | Every dependency of every result checked by a proof assistant | machine check |
| Upper bound | leanblueprint, used for PFR | Each statement declares the labels it uses; a graph is drawn and coloured | completion of the graph |
| Lower bound | Tao 2023 | Case report | the written proof had omitted hypotheses that only formalisation exposed |
| Lower bound | none found | | no study of whether a dependency graph helps a human reader |

## How comprehension is measured today

| Instrument | Source | What it gives |
|---|---|---|
| Seven-dimension test | Mejia-Ramos 2012 | a score per local and holistic dimension |
| Validated multiple-choice tests | Mejia-Ramos 2017 | short reliable tests for named proofs |
| Comparative judgement of summaries | Davies 2020 | a reliable holistic score without a rubric |
| Eye tracking | Inglis & Alcock 2012 | dwell time on formulae versus words; look-backs between lines |
| Delayed post-test | Roy 2017b | retention after two weeks, where e-Proofs lost |
