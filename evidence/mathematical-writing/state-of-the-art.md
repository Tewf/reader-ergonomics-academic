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
| Upper bound (advice) | Halmos 1970, Krantz 2017, Tao 2026a, Tao 2026b, Ramdas 2026 | Expert advice | none; the guides agree |
| Lower bound (advice) | Ilmavirta 2015 | Q/A thread | none; one answer postpones proofs in long papers and holds that circularity is easy to check |
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
| Upper bound (any intervention) | Hodds 2014 | Randomised, self-explanation training of the reader, not of the text | d = 0.95 in the lab; replicated in a lecture hall (107 students, not checked) |
| Upper bound (text format) | Fuller 2014 | Randomised, Leron-style structured versus linear proof | better at identifying a good summary |
| Lower bound (text format) | Fuller 2014 | The same study | somewhat worse on justifications, transfer and examples, mostly not significant |
| Lower bound (text format) | Roy 2017b | Randomised, e-Proof versus textbook, N = 49 (not checked) | no immediate gain; worse retention after two weeks |
| Lower bound (text format) | Lew 2020 | Randomised, generic versus traditional proof | no difference |

The largest measured gain found here comes from teaching the reader to self-explain, not from changing the proof's format.

No study found tests Lamport's numbered format, as distinct from Leron's, on readers.

## Q5. Explicit dependencies between results

| | Holder | Method | Measured how |
|---|---|---|---|
| Upper bound | mathlib 2020 | Every dependency of every result checked by a proof assistant | machine check |
| Upper bound | leanblueprint (Massot 2026), used for PFR | Each statement declares the labels it uses; a graph is drawn and coloured | completion of the graph; about 40 projects list it |
| Upper bound (tool) | Uskuplu 2026 | Dependency graph drawn from LaTeX, no formalisation | none: no user study |
| Upper bound (argument) | Tao 2026c | Reasoned example: unused facts burden the reader's memory | none; design argument |
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

## Most adopted versus best evidence

The two records are defined in the [method](../README.md#method).

The two records are held by different practices.

| Question | Most adopted | Best evidence |
|---|---|---|
| Abstract and theorem styles | amsart rules, enforced by AMS 2017, EMS 2026, LMS 2021 | none; rules of form, untested |
| Where the main results go | introduction states them (21 of 22 openings; every guide) | none; no experiment |
| Layout of a proof | linear paragraphs | Fuller 2014, a trade-off |
| Dependencies | a list of labels in blueprints (about 40 projects) | none for human readers |
| Raising comprehension | not adopted: self-explanation training | Hodds 2014, d = 0.95 (Experiment 1) |
