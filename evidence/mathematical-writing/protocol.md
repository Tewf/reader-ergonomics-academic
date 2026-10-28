# Protocol: how the pool of sources was built

This file records how the formal and grey sources of this review were searched, selected and scored, after Garousi 2019.

The method is a lighter multivocal literature review (see the [evidence README](../README.md)): the formal pool was built before the protocol existed, and the grey search was run to the protocol. Dates of every search: 2026-10-28.

## 1. Why grey literature (Garousi 2019, Table 4)

| # | Question | Answer for this topic |
|---|---|---|
| 1 | Is the subject complex and not solvable by the formal literature alone? | No: the comprehension question is bounded and academic |
| 2 | Is there a lack of volume or quality of evidence in the formal literature? | Yes: one randomised test of a structured proof, none of where the main theorem goes |
| 3 | Is contextual information important? | Yes: conventions differ between pure and applied mathematics and between journals |
| 4 | Is the goal to validate scientific outcomes with practical experience? | Yes: do the style guides' rules survive the comprehension studies? |
| 5 | Is the goal to challenge practice with research, or the reverse? | Yes: Fuller 2014 and Roy 2017b against the guides |
| 6 | Would a synthesis help both communities? | Yes |
| 7 | Is there a large volume of practitioner sources? | No: a few dozen guides, which repeat one another |

Five yes answers include grey literature. Garousi 2019 notes that bounded academic topics have little practitioner literature, which the last answer confirms, so the grey search is small.

## 2. Questions

Q1 to Q5 of frame.md: section order, place of the main results, layout of one proof, effect of layout on comprehension, explicit dependencies between lemmas.

## 3. Existing reviews (Garousi Guideline 2)

Four searches, run first, on the web; results are placed in review.md strand 0.

| Id | String | Found worth reading |
|---|---|---|
| E1 | systematic review proof comprehension OR proof reading, undergraduate | Stylianides 2024, Lessing 2025, Davies 2021 (cites a 2009 review, secondary) |
| E2 | proof and proving literature review handbook chapter | Stylianides 2017 |
| E3 | survey of proof assistants or interactive theorem provers, mathematicians' use | Tran Minh 2025 |
| E4 | review of research on mathematical writing | Teledahl 2024, Powell 2017 |

## 4. Formal search

The formal pool was built by a narrative search plus snowballing, not by screening the counts below. Backward and forward snowballing started from Leron 1983, Mejia-Ramos 2012 and Lamport 1995, through the works citing them.

OpenAlex was the planned counter (`title_and_abstract.search`). It refused every request on the day (the free daily budget was spent), so no OpenAlex count exists. The same strings were run once through the Semantic Scholar bulk search (`/graph/v1/paper/search/bulk`, field `total`):

| String | Total |
|---|---|
| "proof comprehension" | 60 |
| "structured proofs" | 477 |
| "genre analysis" "mathematics" "research articles" | 6 |
| "definition-theorem-proof" | 52 |
| "mathematical writing" | 508 |
| "proof reading" mathematics | 73 |
| "self-explanation" proof | 21 |
| "proof validation" | 144 |
| "mathematical exposition" | 308 |

These totals count full-text matches, so "structured proofs" and "mathematical writing" include much off-topic work.

## 5. Grey search

Producers chosen (Guideline 6): societies and publishers (AMS, LMS, EMS), mathematicians' blogs and essays, university handouts, a Q/A site, formalisation projects' documentation. Engine: a web search tool (results are personalised and change), plus the MathOverflow API for Q/A.

| Id | String (abridged) | Results listed | Included |
|---|---|---|---|
| G1 | how to write mathematics, AMS manual for authors | 20 | Lee 2005 |
| G2 | EMS or LMS journal style guide, structure | 20 | LMS 2021 |
| G3 | Tao advice on writing a paper | 9 | Tao 2026c, and the 3 Tao pages already cited |
| G4 | Gowers how to write mathematics, structure of a proof | 9 | none |
| G5 | MathOverflow long proof, lemmas, refereeing | 9 | Georgakopoulos 2023, Ramdas 2026 |
| G6 | leanblueprint, dependency graph | 9 | Massot 2026 (already cited) |
| G7 | EMS Press style guide | 10 | EMS 2026 |
| G8 | mathlib documentation style | 19 | Mathlib 2026 |
| G9 | proof-writing handouts, proof idea | 19 | Stanford 2023 |
| M1-M4 | MathOverflow API, four queries, top 10 by votes | 30 | Ilmavirta 2015, MathOverflow 2021 |
| S1 | One-level snowball from Tao's reading list (6 pages opened) | 6 | Cohn 2026 |

Excluded:

- 4 unreachable pages (Goss, Barwick, Milne, Tomforde)
- a blog post off the question (citation styles)
- the 2016 LMS guide (review process only)
- a thread that only points to Halmos, Krantz and Tao
- the 1943 AMS manual (not opened)
- a Gowers experiment whose results were not found
- mirrors and duplicates of sources already held

## 6. Stopping rule (Guideline 8)

Effort bounded: the top 10 results per string, nine web strings and four API queries fixed in advance, one level of snowball. Saturation was observed, not used as the rule: the last two included sources (Stanford 2023, EMS 2026) added no concept not already met, while Mathlib 2026 and Ilmavirta 2015 had each added one.

## 7. Selection

Include a source that answers Q1 to Q5 with a concrete layout rule or a measured fact, written by a mathematician or a body that publishes mathematics, and readable in full. Exclude pages that are unreachable, off the question, or copies of a source already held.

## 8. Quality of grey sources (Guideline 11, Table 7)

Twenty criteria scored 1, 0.5 or 0, in eight groups:

- authority 4, methodology 6, objectivity 4, date 1
- position among related sources 1, novelty 2, impact 1, outlet tier 1

Tier 1 scores 1 (books, publisher rules), tier 2 scores 0.5 (handouts, Q/A, repositories), tier 3 scores 0 (blogs). Impact is scored 0.5 when no count was taken.

Threshold 10 of 20: below it a source stays only as an example of practice. Scores are in sources.md.

## 9. Extraction and synthesis

Extracted per source: the rule or fact, its question, the stated limits. Synthesis is narrative by question, traceable through sources.md.

## 10. Limits

- One reviewer, no inter-rater agreement; scores are judgement calls near the threshold.
- Search engines personalise and change; the Tao pages show no date.
- OpenAlex counts are missing; the substitute counts are not comparable with them.
- Higham 2020 and Serre 2003 were not read, only described by secondary sources.
